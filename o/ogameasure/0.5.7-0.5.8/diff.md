# Comparing `tmp/ogameasure-0.5.7.tar.gz` & `tmp/ogameasure-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogameasure-0.5.7.tar", last modified: Sat Dec 31 03:52:18 2022, max compression
+gzip compressed data, was "ogameasure-0.5.8.tar", last modified: Sat Dec 31 06:35:30 2022, max compression
```

## Comparing `ogameasure-0.5.7.tar` & `ogameasure-0.5.8.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.891307 ogameasure-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2022-12-31 03:52:18.891307 ogameasure-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-31 03:52:05.000000 ogameasure-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.883306 ogameasure-0.5.7/ogameasure/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.883306 ogameasure-0.5.7/ogameasure/communicator/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/communicator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/communicator/communicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/communicator/ethernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/communicator/gpib_prologix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/communicator/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/communicator/usb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.883306 ogameasure-0.5.7/ogameasure/device/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.887307 ogameasure-0.5.7/ogameasure/device/Agilent/
--rw-r--r--   0 runner    (1001) docker     (123)    22817 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Agilent/E4418.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Agilent/E8247.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Agilent/E8257.py
--rw-r--r--   0 runner    (1001) docker     (123)    38588 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Agilent/N9342.py
--rw-r--r--   0 runner    (1001) docker     (123)    37947 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Agilent/N9938.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Agilent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17718 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Agilent/agilent_11713.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.887307 ogameasure-0.5.7/ogameasure/device/Anritsu/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Anritsu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Anritsu/ma24126a.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Anritsu/ml2437a.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.887307 ogameasure-0.5.7/ogameasure/device/Canon/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Canon/M100_raspi.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Canon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.887307 ogameasure-0.5.7/ogameasure/device/Cosmotechs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Cosmotechs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9279 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Cosmotechs/sp100.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.887307 ogameasure-0.5.7/ogameasure/device/ELVA1/
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/ELVA1/GPDVC15.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/ELVA1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.887307 ogameasure-0.5.7/ogameasure/device/HEIDENHAIN/
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/HEIDENHAIN/ND287.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/HEIDENHAIN/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.887307 ogameasure-0.5.7/ogameasure/device/KIKUSUI/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/KIKUSUI/PMX18.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/KIKUSUI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.887307 ogameasure-0.5.7/ogameasure/device/Lakeshore/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Lakeshore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53861 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Lakeshore/model218.py
--rw-r--r--   0 runner    (1001) docker     (123)    53982 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Lakeshore/model218_usb.py
--rw-r--r--   0 runner    (1001) docker     (123)    57216 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Lakeshore/model331.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.887307 ogameasure-0.5.7/ogameasure/device/Pfeiffer/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Pfeiffer/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6156 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Pfeiffer/tpg261.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Pfeiffer/tpg261_lan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.891307 ogameasure-0.5.7/ogameasure/device/Phasematrix/
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Phasematrix/QuickSyn_FSW0000.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/Phasematrix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.891307 ogameasure-0.5.7/ogameasure/device/SCPI/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/SCPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22606 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/SCPI/scpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.891307 ogameasure-0.5.7/ogameasure/device/SENA/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/SENA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/SENA/adios.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.891307 ogameasure-0.5.7/ogameasure/device/TandD/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/TandD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/TandD/tr_73u.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/device/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.891307 ogameasure-0.5.7/ogameasure/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:05.000000 ogameasure-0.5.7/ogameasure/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 03:52:18.883306 ogameasure-0.5.7/ogameasure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2022-12-31 03:52:18.000000 ogameasure-0.5.7/ogameasure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2022-12-31 03:52:18.000000 ogameasure-0.5.7/ogameasure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-31 03:52:18.000000 ogameasure-0.5.7/ogameasure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-31 03:52:18.000000 ogameasure-0.5.7/ogameasure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-31 03:52:18.000000 ogameasure-0.5.7/ogameasure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-31 03:52:18.891307 ogameasure-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2022-12-31 03:52:05.000000 ogameasure-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.474091 ogameasure-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2022-12-31 06:35:30.474091 ogameasure-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-31 06:35:16.000000 ogameasure-0.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.458091 ogameasure-0.5.8/ogameasure/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.462091 ogameasure-0.5.8/ogameasure/communicator/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/communicator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/communicator/communicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/communicator/ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/communicator/gpib_prologix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/communicator/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/communicator/usb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.462091 ogameasure-0.5.8/ogameasure/device/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.466091 ogameasure-0.5.8/ogameasure/device/Agilent/
+-rw-r--r--   0 runner    (1001) docker     (123)    22817 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Agilent/E4418.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Agilent/E8247.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Agilent/E8257.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38588 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Agilent/N9342.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37947 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Agilent/N9938.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Agilent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17718 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Agilent/agilent_11713.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.466091 ogameasure-0.5.8/ogameasure/device/Anritsu/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Anritsu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Anritsu/ma24126a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Anritsu/ml2437a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.466091 ogameasure-0.5.8/ogameasure/device/Canon/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Canon/M100_raspi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Canon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.466091 ogameasure-0.5.8/ogameasure/device/Cosmotechs/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Cosmotechs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9279 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Cosmotechs/sp100.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.466091 ogameasure-0.5.8/ogameasure/device/ELVA1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/ELVA1/GPDVC15.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/ELVA1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.470091 ogameasure-0.5.8/ogameasure/device/HEIDENHAIN/
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/HEIDENHAIN/ND287.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/HEIDENHAIN/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.470091 ogameasure-0.5.8/ogameasure/device/KIKUSUI/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/KIKUSUI/PMX18.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/KIKUSUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.470091 ogameasure-0.5.8/ogameasure/device/Lakeshore/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Lakeshore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53861 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Lakeshore/model218.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53982 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Lakeshore/model218_usb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57216 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Lakeshore/model331.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.470091 ogameasure-0.5.8/ogameasure/device/Pfeiffer/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Pfeiffer/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6156 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Pfeiffer/tpg261.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Pfeiffer/tpg261_lan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.470091 ogameasure-0.5.8/ogameasure/device/Phasematrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Phasematrix/QuickSyn_FSW0000.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/Phasematrix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.474091 ogameasure-0.5.8/ogameasure/device/SCPI/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/SCPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22606 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/SCPI/scpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.474091 ogameasure-0.5.8/ogameasure/device/SENA/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/SENA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/SENA/adios.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.474091 ogameasure-0.5.8/ogameasure/device/TandD/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/TandD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/TandD/tr_73u.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/device/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.474091 ogameasure-0.5.8/ogameasure/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:16.000000 ogameasure-0.5.8/ogameasure/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-31 06:35:30.462091 ogameasure-0.5.8/ogameasure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2022-12-31 06:35:30.000000 ogameasure-0.5.8/ogameasure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2022-12-31 06:35:30.000000 ogameasure-0.5.8/ogameasure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-31 06:35:30.000000 ogameasure-0.5.8/ogameasure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-31 06:35:30.000000 ogameasure-0.5.8/ogameasure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-31 06:35:30.000000 ogameasure-0.5.8/ogameasure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-31 06:35:30.474091 ogameasure-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2022-12-31 06:35:16.000000 ogameasure-0.5.8/setup.py
```

### Comparing `ogameasure-0.5.7/PKG-INFO` & `ogameasure-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogameasure
-Version: 0.5.7
+Version: 0.5.8
 Summary: Driver for SCPI device
 Home-page: https://github.com/ogawa-ros/ogameasure
 Author: Shota Ueda
 Author-email: s7u27astr0@gmail.com
 License: MIT
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `ogameasure-0.5.7/ogameasure/communicator/communicator.py` & `ogameasure-0.5.8/ogameasure/communicator/communicator.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,10 +24,7 @@
         pass
 
     def recv(self, byte):
         pass
 
     def readline(self):
         pass
-
-class CommunicatorTimeout(Exception):
-    pass
```

### Comparing `ogameasure-0.5.7/ogameasure/communicator/ethernet.py` & `ogameasure-0.5.8/ogameasure/communicator/ethernet.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/communicator/gpib_prologix.py` & `ogameasure-0.5.8/ogameasure/communicator/gpib_prologix.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/communicator/serial.py` & `ogameasure-0.5.8/ogameasure/communicator/serial.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/communicator/usb.py` & `ogameasure-0.5.8/ogameasure/communicator/usb.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Agilent/E4418.py` & `ogameasure-0.5.8/ogameasure/device/Agilent/E4418.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Agilent/E8247.py` & `ogameasure-0.5.8/ogameasure/device/Agilent/E8247.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Agilent/E8257.py` & `ogameasure-0.5.8/ogameasure/device/Agilent/E8257.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Agilent/N9342.py` & `ogameasure-0.5.8/ogameasure/device/Agilent/N9342.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Agilent/N9938.py` & `ogameasure-0.5.8/ogameasure/device/Agilent/N9938.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Agilent/agilent_11713.py` & `ogameasure-0.5.8/ogameasure/device/Agilent/agilent_11713.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Anritsu/ma24126a.py` & `ogameasure-0.5.8/ogameasure/device/Anritsu/ma24126a.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Anritsu/ml2437a.py` & `ogameasure-0.5.8/ogameasure/device/Anritsu/ml2437a.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Canon/M100_raspi.py` & `ogameasure-0.5.8/ogameasure/device/Canon/M100_raspi.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Cosmotechs/sp100.py` & `ogameasure-0.5.8/ogameasure/device/Cosmotechs/sp100.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/ELVA1/GPDVC15.py` & `ogameasure-0.5.8/ogameasure/device/ELVA1/GPDVC15.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/HEIDENHAIN/ND287.py` & `ogameasure-0.5.8/ogameasure/device/HEIDENHAIN/ND287.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/KIKUSUI/PMX18.py` & `ogameasure-0.5.8/ogameasure/device/KIKUSUI/PMX18.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Lakeshore/model218.py` & `ogameasure-0.5.8/ogameasure/device/Lakeshore/model218.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Lakeshore/model218_usb.py` & `ogameasure-0.5.8/ogameasure/device/Lakeshore/model218_usb.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Lakeshore/model331.py` & `ogameasure-0.5.8/ogameasure/device/Lakeshore/model331.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Pfeiffer/tpg261.py` & `ogameasure-0.5.8/ogameasure/device/Pfeiffer/tpg261.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Pfeiffer/tpg261_lan.py` & `ogameasure-0.5.8/ogameasure/device/Pfeiffer/tpg261_lan.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/Phasematrix/QuickSyn_FSW0000.py` & `ogameasure-0.5.8/ogameasure/device/Phasematrix/QuickSyn_FSW0000.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/SCPI/scpi.py` & `ogameasure-0.5.8/ogameasure/device/SCPI/scpi.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/SENA/adios.py` & `ogameasure-0.5.8/ogameasure/device/SENA/adios.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-from ...communicator import communicator
+from serial import SerialTimeoutException
 
 class adios(object):
 
     off = {'level_off':":17010000000000,000000000011\r\n"}
 
     att = {
             'att1_0dB':":17011111100000,000000000010\r\n",
@@ -86,42 +86,48 @@
         while True:
             try:
                 temp = self.com.recv().decode()
                 if temp.find(':')==-1: continue
                 else: pass
                 #print temp
                 break
-            except (communicator.CommunicatorTimeout, UnicodeDecodeError):
+            except (SerialTimeoutException, TimeoutError, UnicodeDecodeError):
                 print('(error) att1')
                 continue
             continue
         time.sleep(0.1)
 
-        do1 = int(temp[-16])*1
-        do2 = int(temp[-15])*2
-        do3 = int(temp[-14])*4
-        do4 = int(temp[-13])*8
-        do5 = int(temp[-11])*16
-        att1 = do1+do2+do3+do4+do5
+        try:
+            do1 = int(temp[-16])*1
+            do2 = int(temp[-15])*2
+            do3 = int(temp[-14])*4
+            do4 = int(temp[-13])*8
+            do5 = int(temp[-11])*16
+            att1 = do1+do2+do3+do4+do5
+        except ValueError:
+            att1 = -1
         return att1
 
     def get_att2(self):
         self.com.send(self.off['level_off'])
         while True:
             try:
                 temp = self.com.recv().decode()
                 if temp.find(':')==-1: continue
                 else: pass
                 break
-            except (communicator.CommunicatorTimeout, UnicodeDecodeError):
+            except (SerialTimeoutException, TimeoutError, UnicodeDecodeError):
                 print('(error) att2')
                 continue
             continue
         time.sleep(0.1)
 
-        do6 = int(temp[-10])*1
-        do7 = int(temp[-9])*2
-        do8 = int(temp[-8])*4
-        do9 = int(temp[-6])*8
-        do10 = int(temp[-5])*16
-        att2 = do6+do7+do8+do9+do10
+        try:
+            do6 = int(temp[-10])*1
+            do7 = int(temp[-9])*2
+            do8 = int(temp[-8])*4
+            do9 = int(temp[-6])*8
+            do10 = int(temp[-5])*16
+            att2 = do6+do7+do8+do9+do10
+        except ValueError:
+            att2 = -1
         return att2
```

### Comparing `ogameasure-0.5.7/ogameasure/device/TandD/tr_73u.py` & `ogameasure-0.5.8/ogameasure/device/TandD/tr_73u.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure/device/device.py` & `ogameasure-0.5.8/ogameasure/device/device.py`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/ogameasure.egg-info/PKG-INFO` & `ogameasure-0.5.8/ogameasure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogameasure
-Version: 0.5.7
+Version: 0.5.8
 Summary: Driver for SCPI device
 Home-page: https://github.com/ogawa-ros/ogameasure
 Author: Shota Ueda
 Author-email: s7u27astr0@gmail.com
 License: MIT
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `ogameasure-0.5.7/ogameasure.egg-info/SOURCES.txt` & `ogameasure-0.5.8/ogameasure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ogameasure-0.5.7/setup.py` & `ogameasure-0.5.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setuptools.setup(
     name = 'ogameasure',
-    version = "0.5.7",
+    version = "0.5.8",
     description = 'Driver for SCPI device',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/ogawa-ros/ogameasure',
     author = 'Shota Ueda',
     author_email = 's7u27astr0@gmail.com',
     license = 'MIT',
```

