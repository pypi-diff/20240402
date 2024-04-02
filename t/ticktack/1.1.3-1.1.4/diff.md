# Comparing `tmp/ticktack-1.1.3.tar.gz` & `tmp/ticktack-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ticktack-1.1.3.tar", last modified: Wed Nov 29 08:31:43 2023, max compression
+gzip compressed data, was "ticktack-1.1.4.tar", last modified: Tue Apr  2 01:30:49 2024, max compression
```

## Comparing `ticktack-1.1.3.tar` & `ticktack-1.1.4.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.498462 ticktack-1.1.3/
--rw-r--r--   0 benpope    (503) staff       (20)     1071 2022-09-07 04:26:11.000000 ticktack-1.1.3/LICENSE
--rw-r--r--   0 benpope    (503) staff       (20)       90 2023-03-01 04:49:32.000000 ticktack-1.1.3/MANIFEST.in
--rw-r--r--   0 benpope    (503) staff       (20)      688 2023-11-29 08:31:43.498255 ticktack-1.1.3/PKG-INFO
--rw-r--r--   0 benpope    (503) staff       (20)     2777 2023-08-18 02:54:57.000000 ticktack-1.1.3/README.md
--rw-r--r--   0 benpope    (503) staff       (20)      119 2023-08-18 05:30:37.000000 ticktack-1.1.3/requirements.txt
--rw-r--r--   0 benpope    (503) staff       (20)       38 2023-11-29 08:31:43.498559 ticktack-1.1.3/setup.cfg
--rw-r--r--   0 benpope    (503) staff       (20)     2369 2023-03-01 04:49:32.000000 ticktack-1.1.3/setup.py
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.470166 ticktack-1.1.3/src/
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.477357 ticktack-1.1.3/src/ticktack/
--rw-r--r--   0 benpope    (503) staff       (20)       65 2023-11-29 08:31:22.000000 ticktack-1.1.3/src/ticktack/__init__.py
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.481363 ticktack-1.1.3/src/ticktack/data/
--rw-r--r--   0 benpope    (503) staff       (20)    34944 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/Brehm21.hd5
--rw-r--r--   0 benpope    (503) staff       (20)    30848 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/Buntgen18.hd5
--rw-r--r--   0 benpope    (503) staff       (20)    10240 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/Guttler15.hd5
--rw-r--r--   0 benpope    (503) staff       (20)    26688 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/Miyake17.hd5
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.472311 ticktack-1.1.3/src/ticktack/data/datasets/
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.482997 ticktack-1.1.3/src/ticktack/data/datasets/5259BCE/
--rw-r--r--   0 benpope    (503) staff       (20)      464 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/5259BCE/Brehm21_AlpineLarch.csv
--rw-r--r--   0 benpope    (503) staff       (20)      430 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/5259BCE/Brehm21_IrishOak.csv
--rw-r--r--   0 benpope    (503) staff       (20)      450 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/5259BCE/Brehm21_SibirianLarch.csv
--rw-r--r--   0 benpope    (503) staff       (20)      380 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/5259BCE/Brehm21_USABristlecone.csv
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.484101 ticktack-1.1.3/src/ticktack/data/datasets/5410BCE/
--rw-r--r--   0 benpope    (503) staff       (20)      301 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/5410BCE/Miyake21_Bristlecone.csv
--rw-r--r--   0 benpope    (503) staff       (20)      323 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/5410BCE/Miyake21_Finland1.csv
--rw-r--r--   0 benpope    (503) staff       (20)      594 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/5410BCE/Miyake21_Switzerland.csv
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.484466 ticktack-1.1.3/src/ticktack/data/datasets/660BCE-Ew/
--rw-r--r--   0 benpope    (503) staff       (20)      397 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/660BCE-Ew/Sakurai20_CedarEw.csv
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.484780 ticktack-1.1.3/src/ticktack/data/datasets/660BCE-Lw/
--rw-r--r--   0 benpope    (503) staff       (20)      401 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/660BCE-Lw/Sakurai20_CedarLw.csv
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.485806 ticktack-1.1.3/src/ticktack/data/datasets/7176BCE/
--rw-r--r--   0 benpope    (503) staff       (20)      811 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/7176BCE/Brehm21_AlpineLarch.csv
--rw-r--r--   0 benpope    (503) staff       (20)      821 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/7176BCE/Brehm21_GermanOak.csv
--rw-r--r--   0 benpope    (503) staff       (20)      708 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/7176BCE/Brehm21_USABristlecone.csv
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.490063 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-N/
--rw-r--r--   0 benpope    (503) staff       (20)      166 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-N/Büntgen18_ALT01.csv
--rw-r--r--   0 benpope    (503) staff       (20)      165 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-N/Büntgen18_AUT02.csv
--rw-r--r--   0 benpope    (503) staff       (20)      166 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-N/Büntgen18_CAN06.csv
--rw-r--r--   0 benpope    (503) staff       (20)      199 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-N/Büntgen18_GRE02.csv
--rw-r--r--   0 benpope    (503) staff       (20)      151 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-N/Büntgen18_MON09.csv
--rw-r--r--   0 benpope    (503) staff       (20)      163 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-N/Büntgen18_PAK04.csv
--rw-r--r--   0 benpope    (503) staff       (20)      163 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-N/Büntgen18_RUS15.csv
--rw-r--r--   0 benpope    (503) staff       (20)      162 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-N/Büntgen18_RUS17.csv
--rw-r--r--   0 benpope    (503) staff       (20)      157 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-N/Büntgen18_RUS20.csv
--rw-r--r--   0 benpope    (503) staff       (20)      145 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-N/Büntgen18_SWE02.csv
--rw-r--r--   0 benpope    (503) staff       (20)      166 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-N/Büntgen18_TIB01.csv
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.491867 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-S/
--rw-r--r--   0 benpope    (503) staff       (20)      169 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-S/Büntgen18_DAR01.csv
--rw-r--r--   0 benpope    (503) staff       (20)      170 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-S/Büntgen18_DAR06.csv
--rw-r--r--   0 benpope    (503) staff       (20)      169 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-S/Büntgen18_DAR07.csv
--rw-r--r--   0 benpope    (503) staff       (20)      169 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-S/Büntgen18_PAT02.csv
--rw-r--r--   0 benpope    (503) staff       (20)      169 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-S/Büntgen18_PAT03.csv
--rw-r--r--   0 benpope    (503) staff       (20)      166 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-early-S/Büntgen18_TAS01.csv
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.494970 ticktack-1.1.3/src/ticktack/data/datasets/775AD-late-N/
--rw-r--r--   0 benpope    (503) staff       (20)      163 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-late-N/Büntgen18_CHN01.csv
--rw-r--r--   0 benpope    (503) staff       (20)      283 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-late-N/Büntgen18_GER01.csv
--rw-r--r--   0 benpope    (503) staff       (20)      163 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-late-N/Büntgen18_GER07.csv
--rw-r--r--   0 benpope    (503) staff       (20)      163 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-late-N/Büntgen18_JAP01.csv
--rw-r--r--   0 benpope    (503) staff       (20)      332 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-late-N/Büntgen18_MON03.csv
--rw-r--r--   0 benpope    (503) staff       (20)      149 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-late-N/Büntgen18_RUS04.csv
--rw-r--r--   0 benpope    (503) staff       (20)      164 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-late-N/Büntgen18_SWE05.csv
--rw-r--r--   0 benpope    (503) staff       (20)      149 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-late-N/Büntgen18_USA02.csv
--rw-r--r--   0 benpope    (503) staff       (20)      145 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-late-N/Büntgen18_USA11.csv
--rw-r--r--   0 benpope    (503) staff       (20)      167 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-late-N/Büntgen18_USA18.csv
--rw-r--r--   0 benpope    (503) staff       (20)      159 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/775AD-late-N/Scifo19_Oak.csv
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.496984 ticktack-1.1.3/src/ticktack/data/datasets/993AD-N/
--rw-r--r--   0 benpope    (503) staff       (20)      173 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/993AD-N/Büntgen18_ALT02.csv
--rw-r--r--   0 benpope    (503) staff       (20)      171 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/993AD-N/Büntgen18_CHI01.csv
--rw-r--r--   0 benpope    (503) staff       (20)      170 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/993AD-N/Büntgen18_MON05.csv
--rw-r--r--   0 benpope    (503) staff       (20)      191 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/993AD-N/Büntgen18_SWE01.csv
--rw-r--r--   0 benpope    (503) staff       (20)      179 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/993AD-N/Büntgen18_SWE02.csv
--rw-r--r--   0 benpope    (503) staff       (20)      196 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/993AD-N/Büntgen18_SWE03.csv
--rw-r--r--   0 benpope    (503) staff       (20)      177 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/993AD-N/Büntgen18_SWE04.csv
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.497488 ticktack-1.1.3/src/ticktack/data/datasets/993AD-S/
--rw-r--r--   0 benpope    (503) staff       (20)      196 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/993AD-S/Büntgen18_DAR01.csv
--rw-r--r--   0 benpope    (503) staff       (20)      196 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/data/datasets/993AD-S/Büntgen18_PAT03.csv
--rw-r--r--   0 benpope    (503) staff       (20)    74567 2023-11-29 08:31:22.000000 ticktack-1.1.3/src/ticktack/fitting.py
--rw-r--r--   0 benpope    (503) staff       (20)     8531 2023-03-01 04:49:32.000000 ticktack-1.1.3/src/ticktack/model_builder.py
--rw-r--r--   0 benpope    (503) staff       (20)     1418 2023-03-16 06:33:58.000000 ticktack-1.1.3/src/ticktack/resample.py
--rw-r--r--   0 benpope    (503) staff       (20)    29166 2023-08-18 05:11:11.000000 ticktack-1.1.3/src/ticktack/ticktack.py
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.479575 ticktack-1.1.3/src/ticktack.egg-info/
--rw-r--r--   0 benpope    (503) staff       (20)      688 2023-11-29 08:31:43.000000 ticktack-1.1.3/src/ticktack.egg-info/PKG-INFO
--rw-r--r--   0 benpope    (503) staff       (20)     3468 2023-11-29 08:31:43.000000 ticktack-1.1.3/src/ticktack.egg-info/SOURCES.txt
--rw-r--r--   0 benpope    (503) staff       (20)        1 2023-11-29 08:31:43.000000 ticktack-1.1.3/src/ticktack.egg-info/dependency_links.txt
--rw-r--r--   0 benpope    (503) staff       (20)      165 2023-11-29 08:31:43.000000 ticktack-1.1.3/src/ticktack.egg-info/requires.txt
--rw-r--r--   0 benpope    (503) staff       (20)        9 2023-11-29 08:31:43.000000 ticktack-1.1.3/src/ticktack.egg-info/top_level.txt
-drwxr-xr-x   0 benpope    (503) staff       (20)        0 2023-11-29 08:31:43.497970 ticktack-1.1.3/tests/
--rw-r--r--   0 benpope    (503) staff       (20)    15101 2023-03-01 04:49:32.000000 ticktack-1.1.3/tests/test_fitting.py
--rw-r--r--   0 benpope    (503) staff       (20)     8071 2023-03-01 04:49:32.000000 ticktack-1.1.3/tests/test_ticktack.py
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.170494 ticktack-1.1.4/
+-rw-r--r--   0 benpope    (503) staff       (20)     1071 2022-09-07 04:26:11.000000 ticktack-1.1.4/LICENSE
+-rw-r--r--   0 benpope    (503) staff       (20)       90 2023-03-01 04:49:32.000000 ticktack-1.1.4/MANIFEST.in
+-rw-r--r--   0 benpope    (503) staff       (20)     1168 2024-04-02 01:30:49.170188 ticktack-1.1.4/PKG-INFO
+-rw-r--r--   0 benpope    (503) staff       (20)     2777 2023-08-18 02:54:57.000000 ticktack-1.1.4/README.md
+-rw-r--r--   0 benpope    (503) staff       (20)      119 2023-08-18 05:30:37.000000 ticktack-1.1.4/requirements.txt
+-rw-r--r--   0 benpope    (503) staff       (20)       38 2024-04-02 01:30:49.170542 ticktack-1.1.4/setup.cfg
+-rw-r--r--   0 benpope    (503) staff       (20)     2369 2023-03-01 04:49:32.000000 ticktack-1.1.4/setup.py
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.139246 ticktack-1.1.4/src/
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.145357 ticktack-1.1.4/src/ticktack/
+-rw-r--r--   0 benpope    (503) staff       (20)       65 2024-04-02 01:29:40.000000 ticktack-1.1.4/src/ticktack/__init__.py
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.149304 ticktack-1.1.4/src/ticktack/data/
+-rw-r--r--   0 benpope    (503) staff       (20)    34944 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/Brehm21.hd5
+-rw-r--r--   0 benpope    (503) staff       (20)    30848 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/Buntgen18.hd5
+-rw-r--r--   0 benpope    (503) staff       (20)    10240 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/Guttler15.hd5
+-rw-r--r--   0 benpope    (503) staff       (20)    26688 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/Miyake17.hd5
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.141363 ticktack-1.1.4/src/ticktack/data/datasets/
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.151023 ticktack-1.1.4/src/ticktack/data/datasets/5259BCE/
+-rw-r--r--   0 benpope    (503) staff       (20)      464 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/5259BCE/Brehm21_AlpineLarch.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      430 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/5259BCE/Brehm21_IrishOak.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      450 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/5259BCE/Brehm21_SibirianLarch.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      380 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/5259BCE/Brehm21_USABristlecone.csv
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.152180 ticktack-1.1.4/src/ticktack/data/datasets/5410BCE/
+-rw-r--r--   0 benpope    (503) staff       (20)      301 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/5410BCE/Miyake21_Bristlecone.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      323 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/5410BCE/Miyake21_Finland1.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      594 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/5410BCE/Miyake21_Switzerland.csv
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.152581 ticktack-1.1.4/src/ticktack/data/datasets/660BCE-Ew/
+-rw-r--r--   0 benpope    (503) staff       (20)      397 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/660BCE-Ew/Sakurai20_CedarEw.csv
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.152946 ticktack-1.1.4/src/ticktack/data/datasets/660BCE-Lw/
+-rw-r--r--   0 benpope    (503) staff       (20)      401 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/660BCE-Lw/Sakurai20_CedarLw.csv
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.154093 ticktack-1.1.4/src/ticktack/data/datasets/7176BCE/
+-rw-r--r--   0 benpope    (503) staff       (20)      811 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/7176BCE/Brehm21_AlpineLarch.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      821 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/7176BCE/Brehm21_GermanOak.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      708 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/7176BCE/Brehm21_USABristlecone.csv
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.158714 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-N/
+-rw-r--r--   0 benpope    (503) staff       (20)      166 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-N/Büntgen18_ALT01.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      165 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-N/Büntgen18_AUT02.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      166 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-N/Büntgen18_CAN06.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      199 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-N/Büntgen18_GRE02.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      151 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-N/Büntgen18_MON09.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      163 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-N/Büntgen18_PAK04.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      163 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-N/Büntgen18_RUS15.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      162 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-N/Büntgen18_RUS17.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      157 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-N/Büntgen18_RUS20.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      145 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-N/Büntgen18_SWE02.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      166 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-N/Büntgen18_TIB01.csv
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.161637 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-S/
+-rw-r--r--   0 benpope    (503) staff       (20)      169 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-S/Büntgen18_DAR01.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      170 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-S/Büntgen18_DAR06.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      169 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-S/Büntgen18_DAR07.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      169 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-S/Büntgen18_PAT02.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      169 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-S/Büntgen18_PAT03.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      166 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-early-S/Büntgen18_TAS01.csv
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.165930 ticktack-1.1.4/src/ticktack/data/datasets/775AD-late-N/
+-rw-r--r--   0 benpope    (503) staff       (20)      163 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-late-N/Büntgen18_CHN01.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      283 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-late-N/Büntgen18_GER01.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      163 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-late-N/Büntgen18_GER07.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      163 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-late-N/Büntgen18_JAP01.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      332 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-late-N/Büntgen18_MON03.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      149 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-late-N/Büntgen18_RUS04.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      164 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-late-N/Büntgen18_SWE05.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      149 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-late-N/Büntgen18_USA02.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      145 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-late-N/Büntgen18_USA11.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      167 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-late-N/Büntgen18_USA18.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      159 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/775AD-late-N/Scifo19_Oak.csv
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.167883 ticktack-1.1.4/src/ticktack/data/datasets/993AD-N/
+-rw-r--r--   0 benpope    (503) staff       (20)      173 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/993AD-N/Büntgen18_ALT02.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      171 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/993AD-N/Büntgen18_CHI01.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      170 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/993AD-N/Büntgen18_MON05.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      191 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/993AD-N/Büntgen18_SWE01.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      179 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/993AD-N/Büntgen18_SWE02.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      196 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/993AD-N/Büntgen18_SWE03.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      177 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/993AD-N/Büntgen18_SWE04.csv
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.168432 ticktack-1.1.4/src/ticktack/data/datasets/993AD-S/
+-rw-r--r--   0 benpope    (503) staff       (20)      196 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/993AD-S/Büntgen18_DAR01.csv
+-rw-r--r--   0 benpope    (503) staff       (20)      196 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/data/datasets/993AD-S/Büntgen18_PAT03.csv
+-rw-r--r--   0 benpope    (503) staff       (20)    74567 2024-04-02 01:27:50.000000 ticktack-1.1.4/src/ticktack/fitting.py
+-rw-r--r--   0 benpope    (503) staff       (20)     8531 2023-03-01 04:49:32.000000 ticktack-1.1.4/src/ticktack/model_builder.py
+-rw-r--r--   0 benpope    (503) staff       (20)     1418 2023-03-16 06:33:58.000000 ticktack-1.1.4/src/ticktack/resample.py
+-rw-r--r--   0 benpope    (503) staff       (20)    29140 2024-04-02 01:23:20.000000 ticktack-1.1.4/src/ticktack/ticktack.py
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.169591 ticktack-1.1.4/src/ticktack.egg-info/
+-rw-r--r--   0 benpope    (503) staff       (20)     1168 2024-04-02 01:30:49.000000 ticktack-1.1.4/src/ticktack.egg-info/PKG-INFO
+-rw-r--r--   0 benpope    (503) staff       (20)     3468 2024-04-02 01:30:49.000000 ticktack-1.1.4/src/ticktack.egg-info/SOURCES.txt
+-rw-r--r--   0 benpope    (503) staff       (20)        1 2024-04-02 01:30:49.000000 ticktack-1.1.4/src/ticktack.egg-info/dependency_links.txt
+-rw-r--r--   0 benpope    (503) staff       (20)      165 2024-04-02 01:30:49.000000 ticktack-1.1.4/src/ticktack.egg-info/requires.txt
+-rw-r--r--   0 benpope    (503) staff       (20)        9 2024-04-02 01:30:49.000000 ticktack-1.1.4/src/ticktack.egg-info/top_level.txt
+drwxr-xr-x   0 benpope    (503) staff       (20)        0 2024-04-02 01:30:49.169218 ticktack-1.1.4/tests/
+-rw-r--r--   0 benpope    (503) staff       (20)    15101 2024-04-02 01:27:00.000000 ticktack-1.1.4/tests/test_fitting.py
+-rw-r--r--   0 benpope    (503) staff       (20)     8071 2023-03-01 04:49:32.000000 ticktack-1.1.4/tests/test_ticktack.py
```

### Comparing `ticktack-1.1.3/LICENSE` & `ticktack-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ticktack-1.1.3/README.md` & `ticktack-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ticktack-1.1.3/setup.py` & `ticktack-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `ticktack-1.1.3/src/ticktack/data/Brehm21.hd5` & `ticktack-1.1.4/src/ticktack/data/Brehm21.hd5`

 * *Files identical despite different names*

### Comparing `ticktack-1.1.3/src/ticktack/data/Buntgen18.hd5` & `ticktack-1.1.4/src/ticktack/data/Buntgen18.hd5`

 * *Files identical despite different names*

### Comparing `ticktack-1.1.3/src/ticktack/data/Guttler15.hd5` & `ticktack-1.1.4/src/ticktack/data/Guttler15.hd5`

 * *Files identical despite different names*

### Comparing `ticktack-1.1.3/src/ticktack/data/Miyake17.hd5` & `ticktack-1.1.4/src/ticktack/data/Miyake17.hd5`

 * *Files identical despite different names*

### Comparing `ticktack-1.1.3/src/ticktack/data/datasets/5410BCE/Miyake21_Switzerland.csv` & `ticktack-1.1.4/src/ticktack/data/datasets/5410BCE/Miyake21_Switzerland.csv`

 * *Files identical despite different names*

### Comparing `ticktack-1.1.3/src/ticktack/data/datasets/7176BCE/Brehm21_AlpineLarch.csv` & `ticktack-1.1.4/src/ticktack/data/datasets/7176BCE/Brehm21_AlpineLarch.csv`

 * *Files identical despite different names*

### Comparing `ticktack-1.1.3/src/ticktack/data/datasets/7176BCE/Brehm21_GermanOak.csv` & `ticktack-1.1.4/src/ticktack/data/datasets/7176BCE/Brehm21_GermanOak.csv`

 * *Files identical despite different names*

### Comparing `ticktack-1.1.3/src/ticktack/data/datasets/7176BCE/Brehm21_USABristlecone.csv` & `ticktack-1.1.4/src/ticktack/data/datasets/7176BCE/Brehm21_USABristlecone.csv`

 * *Files identical despite different names*

### Comparing `ticktack-1.1.3/src/ticktack/fitting.py` & `ticktack-1.1.4/src/ticktack/fitting.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,15 +427,15 @@
         self.start = np.nanmin(self.time_data)
         self.end = np.nanmax(self.time_data)
         self.burn_in_time = jnp.arange(self.start - burnin_time, self.start + 1, 1.)
         self.oversample = oversample
         self.burnin_oversample = burnin_oversample
         self.offset = jnp.mean(self.d14c_data[:num_offset])
         self.annual = jnp.arange(self.start, self.end + 1)
-        self.mask = jnp.in1d(self.annual, self.time_data)
+        self.mask = jnp.isin(self.annual, self.time_data)
         self.time_data_fine = jnp.linspace(jnp.min(self.annual), jnp.max(self.annual) + 2,
                                            (self.annual.size + 1) * self.oversample)
         try:
             self.growth = self.get_growth_vector(data["growth_season"][0])
             if verbose:
                 with open('data_log.txt', 'a') as f:
                     f.write(" Custom Growth Season")
@@ -1145,15 +1145,15 @@
         if self.production_model == 'flexible sinusoid affine variant':
             self.production = self.flexible_sinusoid_affine_variant
         self.burn_in_time = jnp.arange(self.start - 2000, self.start + 1, 1.)
         self.annual = jnp.arange(self.start, self.end + 1)
         self.time_data_fine = jnp.linspace(jnp.min(self.annual), jnp.max(self.annual) + 2,
                                            (self.annual.size + 1) * self.oversample)
         for sf in self.MultiFitter:
-            sf.multi_mask = jnp.in1d(self.annual, sf.time_data)
+            sf.multi_mask = jnp.isin(self.annual, sf.time_data)
         if self.production_model == 'control points':
             self.control_points_time = jnp.arange(self.start, self.end)
             self.production = self.multi_interp_gp
         self.steady_state_box = self.steady_state_y0[self.box_idx]
 
     @partial(jit, static_argnums=(0,))
     def multi_interp_gp(self, tval, *args):
```

### Comparing `ticktack-1.1.3/src/ticktack/model_builder.py` & `ticktack-1.1.4/src/ticktack/model_builder.py`

 * *Files identical despite different names*

### Comparing `ticktack-1.1.3/src/ticktack/resample.py` & `ticktack-1.1.4/src/ticktack/resample.py`

 * *Files identical despite different names*

### Comparing `ticktack-1.1.3/src/ticktack/ticktack.py` & `ticktack-1.1.4/src/ticktack/ticktack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import jax.numpy as jnp
 import numpy as np # for the non-jitted functions
 from jax import jit
 import jax
 from functools import partial
-from jax.config import config
 
 from jax.lax import cond, dynamic_update_slice, fori_loop, dynamic_slice
 import diffrax
 
 import h5py
 
 import scipy as scipy
 import scipy.integrate
 import scipy.optimize
 
 import pkg_resources
 from typing import Union
 
-config.update("jax_enable_x64", True) # run in 64 bit by default or else you will lack the dynamic range required
+jax.config.update("jax_enable_x64", True) # run in 64 bit by default or else you will lack the dynamic range required
 
 
 
 def sanitize(data):
     # if dtype is 'object', decode, otherwise don't
     if data.dtype == 'object':
         return np.array([x.decode('utf-8') for x in data])
```

### Comparing `ticktack-1.1.3/src/ticktack.egg-info/SOURCES.txt` & `ticktack-1.1.4/src/ticktack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ticktack-1.1.3/tests/test_fitting.py` & `ticktack-1.1.4/tests/test_fitting.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     sf.start = np.nanmin(sf.time_data)
     sf.end = np.nanmax(sf.time_data)
     sf.burn_in_time = jnp.arange(sf.start - 1000, sf.start, 1.)
     sf.oversample = 1008
     sf.annual = jnp.arange(sf.start, sf.end + 1)
     sf.time_data_fine = jnp.linspace(jnp.min(sf.annual), jnp.max(sf.annual) + 2, (sf.annual.size + 1) * sf.oversample)
     sf.offset = jnp.mean(sf.d14c_data[:4])
-    sf.mask = jnp.in1d(sf.annual, sf.time_data)
+    sf.mask = jnp.isin(sf.annual, sf.time_data)
     sf.growth = sf.get_growth_vector("april-september")
     return sf
 
 @pytest.fixture
 def MultiFitter_creation(SingleFitter_creation):
     mf = fitting.MultiFitter()
     SingleFitter_creation.compile_production_model(model="simple_sinusoid")
```

### Comparing `ticktack-1.1.3/tests/test_ticktack.py` & `ticktack-1.1.4/tests/test_ticktack.py`

 * *Files identical despite different names*

