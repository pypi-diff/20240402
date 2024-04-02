# Comparing `tmp/pdfminer.aemc-20221116.tar.gz` & `tmp/pdfminer.aemc-20221117.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfminer.aemc-20221116.tar", last modified: Wed Mar 27 08:11:12 2024, max compression
+gzip compressed data, was "pdfminer.aemc-20221117.tar", last modified: Tue Apr  2 09:53:54 2024, max compression
```

## Comparing `pdfminer.aemc-20221116.tar` & `pdfminer.aemc-20221117.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-03-27 08:11:12.179748 pdfminer.aemc-20221116/
--rw-rw-r--   0 jun        (501) staff       (20)    14906 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/CHANGELOG.md
--rw-rw-r--   0 jun        (501) staff       (20)     2397 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/CONTRIBUTING.md
--rw-rw-r--   0 jun        (501) staff       (20)     1093 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/LICENSE
--rw-rw-r--   0 jun        (501) staff       (20)      160 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/MANIFEST.in
--rw-rw-r--   0 jun        (501) staff       (20)     1141 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/Makefile
--rw-r--r--   0 jun        (501) staff       (20)     3519 2024-03-27 08:11:12.179610 pdfminer.aemc-20221116/PKG-INFO
--rw-rw-r--   0 jun        (501) staff       (20)     2573 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/README.md
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-03-27 08:11:12.140220 pdfminer.aemc-20221116/cmaprsrc/
--rw-rw-r--   0 jun        (501) staff       (20)     2917 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/cmaprsrc/README.txt
--rw-rw-r--   0 jun        (501) staff       (20)  2046762 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/cmaprsrc/cid2code_Adobe_CNS1.txt
--rw-rw-r--   0 jun        (501) staff       (20)  1900416 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/cmaprsrc/cid2code_Adobe_GB1.txt
--rw-rw-r--   0 jun        (501) staff       (20)  2681742 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/cmaprsrc/cid2code_Adobe_Japan1.txt
--rw-rw-r--   0 jun        (501) staff       (20)  1028252 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/cmaprsrc/cid2code_Adobe_Korea1.txt
--rw-rw-r--   0 jun        (501) staff       (20)     1181 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/noxfile.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-03-27 08:11:12.153626 pdfminer.aemc-20221116/pdfminer/
--rw-rw-r--   0 jun        (501) staff       (20)      196 2024-03-27 08:09:27.000000 pdfminer.aemc-20221116/pdfminer/__init__.py
--rw-rw-r--   0 jun        (501) staff       (20)     3600 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/_saslprep.py
--rw-rw-r--   0 jun        (501) staff       (20)      929 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/arcfour.py
--rw-rw-r--   0 jun        (501) staff       (20)     2097 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/ascii85.py
--rw-rw-r--   0 jun        (501) staff       (20)    21391 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/ccitt.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-03-27 08:11:12.174849 pdfminer.aemc-20221116/pdfminer/cmap/
--rw-rw-r--   0 jun        (501) staff       (20)    20532 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/78-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    20551 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/78-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    19882 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/78-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22969 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/78-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22990 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/78-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    19883 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/78-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25942 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/78ms-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25964 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/78ms-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    26305 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/83pv-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    26305 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/83pv-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25732 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/90ms-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25757 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/90ms-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25670 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/90msp-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25688 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/90msp-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24226 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/90pv-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24021 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/90pv-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21027 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Add-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24275 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Add-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24079 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Add-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    20874 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Add-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    42594 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    42549 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    42602 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/B5pc-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    42557 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/B5pc-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    56990 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/CNS-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    56943 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/CNS-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    17615 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/CNS1-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    17564 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/CNS1-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21723 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/CNS2-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21723 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/CNS2-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    59548 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/ETHK-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    59481 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/ETHK-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    43982 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/ETen-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    43924 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/ETen-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      320 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/ETenms-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      438 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/ETenms-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    20429 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    20455 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22272 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Ext-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25721 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Ext-RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    25750 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Ext-RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22307 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Ext-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22118 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GB-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    22111 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GB-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21699 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GB-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21694 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GB-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    68254 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GBK-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    68199 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GBK-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    89917 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GBK2K-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    89872 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GBK2K-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    68148 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GBKp-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    68102 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GBKp-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23815 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GBT-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23806 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GBT-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23339 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GBT-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23322 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GBT-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23650 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GBTpc-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23647 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GBTpc-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21945 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GBpc-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21956 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/GBpc-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    19781 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    45212 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/HKdla-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    45167 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/HKdla-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    44853 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/HKdlb-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    44816 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/HKdlb-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    53104 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/HKgccs-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    53050 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/HKgccs-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    43667 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/HKm314-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    43618 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/HKm314-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    44187 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/HKm471-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    44144 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/HKm471-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    59508 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/HKscs-B5-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    59473 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/HKscs-B5-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      840 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Hankaku-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      839 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Hankaku-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      391 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Hiragana-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      391 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Hiragana-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24040 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/KSC-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    24078 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/KSC-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23563 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/KSC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    55016 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/KSC-Johab-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    55041 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/KSC-Johab-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23644 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/KSC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    51667 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/KSCms-UHC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    51788 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    51821 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    51698 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/KSCms-UHC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    27769 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/KSCpc-EUC-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    27820 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/KSCpc-EUC-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      404 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Katakana-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      404 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Katakana-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21708 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/NWP-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    21779 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/NWP-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)     3917 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/README.txt
--rw-rw-r--   0 jun        (501) staff       (20)    23030 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/RKSJ-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    23048 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/RKSJ-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      394 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Roman-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      394 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/Roman-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    67459 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    67395 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    87819 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    87751 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    87400 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    87327 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    82631 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    82562 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    97445 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UCS2-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    97441 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UCS2-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   101459 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UTF16-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   101331 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UTF16-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   101490 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   101357 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    90500 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UTF8-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    90368 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UTF8-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    35934 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      412 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UCS2-HW-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)     1402 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    35852 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    58054 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57928 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57910 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57780 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54764 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54684 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    58081 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57960 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57940 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57811 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54829 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54749 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57903 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57778 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57930 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    57808 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    60683 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UCS2-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    60699 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UCS2-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    61278 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UTF16-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    61298 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UTF16-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    61286 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UTF32-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    61309 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UTF32-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54151 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UTF8-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    54172 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UTF8-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    19826 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      505 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/WP-Symbol-H.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)      505 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/WP-Symbol-V.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   138237 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   204425 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   112987 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)   120859 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz
--rw-rw-r--   0 jun        (501) staff       (20)    16163 2024-03-27 08:04:45.000000 pdfminer.aemc-20221116/pdfminer/cmapdb.py
--rw-rw-r--   0 jun        (501) staff       (20)    34968 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/converter.py
--rw-rw-r--   0 jun        (501) staff       (20)     1654 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/data_structures.py
--rw-rw-r--   0 jun        (501) staff       (20)     3983 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/encodingdb.py
--rw-rw-r--   0 jun        (501) staff       (20)   112611 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/fontmetrics.py
--rw-rw-r--   0 jun        (501) staff       (20)   130804 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/glyphlist.py
--rw-rw-r--   0 jun        (501) staff       (20)     7276 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/high_level.py
--rw-rw-r--   0 jun        (501) staff       (20)     9299 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/image.py
--rw-rw-r--   0 jun        (501) staff       (20)    11391 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/jbig2.py
--rw-rw-r--   0 jun        (501) staff       (20)     8531 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/latin_enc.py
--rw-rw-r--   0 jun        (501) staff       (20)    35231 2024-03-27 08:00:50.000000 pdfminer.aemc-20221116/pdfminer/layout.py
--rw-rw-r--   0 jun        (501) staff       (20)     3177 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/lzw.py
--rw-rw-r--   0 jun        (501) staff       (20)      821 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/pdfcolor.py
--rw-rw-r--   0 jun        (501) staff       (20)     8787 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/pdfdevice.py
--rw-rw-r--   0 jun        (501) staff       (20)    37267 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/pdfdocument.py
--rw-rw-r--   0 jun        (501) staff       (20)    37786 2024-03-27 08:00:02.000000 pdfminer.aemc-20221116/pdfminer/pdffont.py
--rw-rw-r--   0 jun        (501) staff       (20)    34539 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/pdfinterp.py
--rw-rw-r--   0 jun        (501) staff       (20)     6803 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/pdfpage.py
--rw-rw-r--   0 jun        (501) staff       (20)     5896 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/pdfparser.py
--rw-rw-r--   0 jun        (501) staff       (20)    12109 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/pdftypes.py
--rwxr-xr-x   0 jun        (501) staff       (20)    19649 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/psparser.py
--rw-rw-r--   0 jun        (501) staff       (20)        0 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/py.typed
--rw-rw-r--   0 jun        (501) staff       (20)     1358 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/runlength.py
--rw-rw-r--   0 jun        (501) staff       (20)       15 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/settings.py
--rw-rw-r--   0 jun        (501) staff       (20)    20804 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/pdfminer/utils.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-03-27 08:11:12.154378 pdfminer.aemc-20221116/pdfminer.aemc.egg-info/
--rw-r--r--   0 jun        (501) staff       (20)     3519 2024-03-27 08:11:12.000000 pdfminer.aemc-20221116/pdfminer.aemc.egg-info/PKG-INFO
--rw-r--r--   0 jun        (501) staff       (20)     6521 2024-03-27 08:11:12.000000 pdfminer.aemc-20221116/pdfminer.aemc.egg-info/SOURCES.txt
--rw-r--r--   0 jun        (501) staff       (20)        1 2024-03-27 08:11:12.000000 pdfminer.aemc-20221116/pdfminer.aemc.egg-info/dependency_links.txt
--rw-r--r--   0 jun        (501) staff       (20)      175 2024-03-27 08:11:12.000000 pdfminer.aemc-20221116/pdfminer.aemc.egg-info/requires.txt
--rw-r--r--   0 jun        (501) staff       (20)        9 2024-03-27 08:11:12.000000 pdfminer.aemc-20221116/pdfminer.aemc.egg-info/top_level.txt
--rw-r--r--   0 jun        (501) staff       (20)       38 2024-03-27 08:11:12.179792 pdfminer.aemc-20221116/setup.cfg
--rw-rw-r--   0 jun        (501) staff       (20)     1776 2024-03-27 08:10:12.000000 pdfminer.aemc-20221116/setup.py
-drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-03-27 08:11:12.179196 pdfminer.aemc-20221116/tools/
--rw-rw-r--   0 jun        (501) staff       (20)        0 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/tools/__init__.py
--rwxr-xr-x   0 jun        (501) staff       (20)     1646 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/tools/conv_afm.py
--rwxr-xr-x   0 jun        (501) staff       (20)     6089 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/tools/conv_cmap.py
--rwxr-xr-x   0 jun        (501) staff       (20)      911 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/tools/conv_glyphlist.py
--rwxr-xr-x   0 jun        (501) staff       (20)    14316 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/tools/dumppdf.py
--rwxr-xr-x   0 jun        (501) staff       (20)     9779 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/tools/pdf2txt.py
--rw-rw-r--   0 jun        (501) staff       (20)     6266 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/tools/pdfdiff.py
--rwxr-xr-x   0 jun        (501) staff       (20)     2761 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/tools/pdfstats.py
--rw-rw-r--   0 jun        (501) staff       (20)     1415 2022-11-05 16:22:08.000000 pdfminer.aemc-20221116/tools/prof.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-04-02 09:53:54.953666 pdfminer.aemc-20221117/
+-rw-rw-r--   0 jun        (501) staff       (20)    14906 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/CHANGELOG.md
+-rw-rw-r--   0 jun        (501) staff       (20)     2397 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/CONTRIBUTING.md
+-rw-rw-r--   0 jun        (501) staff       (20)     1093 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/LICENSE
+-rw-rw-r--   0 jun        (501) staff       (20)      160 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/MANIFEST.in
+-rw-rw-r--   0 jun        (501) staff       (20)     1141 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/Makefile
+-rw-r--r--   0 jun        (501) staff       (20)     3519 2024-04-02 09:53:54.953525 pdfminer.aemc-20221117/PKG-INFO
+-rw-rw-r--   0 jun        (501) staff       (20)     2573 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/README.md
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-04-02 09:53:54.883715 pdfminer.aemc-20221117/cmaprsrc/
+-rw-rw-r--   0 jun        (501) staff       (20)     2917 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/cmaprsrc/README.txt
+-rw-rw-r--   0 jun        (501) staff       (20)  2046762 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/cmaprsrc/cid2code_Adobe_CNS1.txt
+-rw-rw-r--   0 jun        (501) staff       (20)  1900416 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/cmaprsrc/cid2code_Adobe_GB1.txt
+-rw-rw-r--   0 jun        (501) staff       (20)  2681742 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/cmaprsrc/cid2code_Adobe_Japan1.txt
+-rw-rw-r--   0 jun        (501) staff       (20)  1028252 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/cmaprsrc/cid2code_Adobe_Korea1.txt
+-rw-rw-r--   0 jun        (501) staff       (20)     1181 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/noxfile.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-04-02 09:53:54.898667 pdfminer.aemc-20221117/pdfminer/
+-rw-rw-r--   0 jun        (501) staff       (20)      196 2024-04-02 09:51:34.000000 pdfminer.aemc-20221117/pdfminer/__init__.py
+-rw-rw-r--   0 jun        (501) staff       (20)     3600 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/_saslprep.py
+-rw-rw-r--   0 jun        (501) staff       (20)      929 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/arcfour.py
+-rw-rw-r--   0 jun        (501) staff       (20)     2097 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/ascii85.py
+-rw-rw-r--   0 jun        (501) staff       (20)    21391 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/ccitt.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-04-02 09:53:54.949106 pdfminer.aemc-20221117/pdfminer/cmap/
+-rw-rw-r--   0 jun        (501) staff       (20)    20532 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/78-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    20551 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/78-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    19882 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/78-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22969 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/78-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22990 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/78-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    19883 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/78-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25942 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/78ms-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25964 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/78ms-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    26305 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/83pv-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    26305 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/83pv-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25732 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/90ms-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25757 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/90ms-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25670 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/90msp-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25688 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/90msp-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24226 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/90pv-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24021 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/90pv-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21027 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Add-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24275 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Add-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24079 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Add-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    20874 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Add-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    42594 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    42549 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    42602 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/B5pc-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    42557 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/B5pc-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    56990 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/CNS-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    56943 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/CNS-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    17615 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/CNS1-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    17564 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/CNS1-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21723 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/CNS2-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21723 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/CNS2-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    59548 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/ETHK-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    59481 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/ETHK-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    43982 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/ETen-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    43924 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/ETen-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      320 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/ETenms-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      438 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/ETenms-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    20429 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    20455 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22272 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Ext-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25721 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Ext-RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    25750 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Ext-RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22307 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Ext-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22118 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GB-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    22111 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GB-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21699 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GB-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21694 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GB-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    68254 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GBK-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    68199 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GBK-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    89917 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GBK2K-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    89872 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GBK2K-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    68148 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GBKp-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    68102 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GBKp-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23815 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GBT-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23806 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GBT-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23339 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GBT-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23322 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GBT-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23650 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GBTpc-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23647 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GBTpc-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21945 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GBpc-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21956 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/GBpc-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    19781 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    45212 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/HKdla-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    45167 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/HKdla-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    44853 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/HKdlb-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    44816 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/HKdlb-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    53104 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/HKgccs-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    53050 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/HKgccs-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    43667 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/HKm314-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    43618 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/HKm314-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    44187 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/HKm471-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    44144 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/HKm471-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    59508 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/HKscs-B5-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    59473 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/HKscs-B5-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      840 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Hankaku-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      839 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Hankaku-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      391 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Hiragana-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      391 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Hiragana-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24040 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/KSC-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    24078 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/KSC-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23563 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/KSC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    55016 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/KSC-Johab-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    55041 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/KSC-Johab-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23644 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/KSC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    51667 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/KSCms-UHC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    51788 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    51821 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    51698 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/KSCms-UHC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    27769 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/KSCpc-EUC-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    27820 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/KSCpc-EUC-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      404 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Katakana-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      404 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Katakana-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21708 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/NWP-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    21779 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/NWP-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)     3917 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/README.txt
+-rw-rw-r--   0 jun        (501) staff       (20)    23030 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/RKSJ-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    23048 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/RKSJ-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      394 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Roman-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      394 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/Roman-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    67459 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    67395 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    87819 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    87751 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    87400 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    87327 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    82631 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    82562 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    97445 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UCS2-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    97441 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UCS2-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   101459 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UTF16-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   101331 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UTF16-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   101490 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   101357 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    90500 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UTF8-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    90368 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UTF8-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    35934 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      412 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UCS2-HW-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)     1402 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    35852 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    58054 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57928 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57910 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57780 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54764 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54684 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    58081 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57960 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57940 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57811 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54829 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54749 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57903 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57778 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57930 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    57808 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    60683 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UCS2-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    60699 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UCS2-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    61278 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UTF16-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    61298 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UTF16-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    61286 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UTF32-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    61309 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UTF32-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54151 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UTF8-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    54172 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UTF8-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    19826 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      505 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/WP-Symbol-H.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)      505 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/WP-Symbol-V.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   138237 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   204425 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   112987 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)   120859 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz
+-rw-rw-r--   0 jun        (501) staff       (20)    16163 2024-03-27 08:04:45.000000 pdfminer.aemc-20221117/pdfminer/cmapdb.py
+-rw-rw-r--   0 jun        (501) staff       (20)    34968 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/converter.py
+-rw-rw-r--   0 jun        (501) staff       (20)     1654 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/data_structures.py
+-rw-rw-r--   0 jun        (501) staff       (20)     3983 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/encodingdb.py
+-rw-rw-r--   0 jun        (501) staff       (20)   112611 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/fontmetrics.py
+-rw-rw-r--   0 jun        (501) staff       (20)   130804 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/glyphlist.py
+-rw-rw-r--   0 jun        (501) staff       (20)     7276 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/high_level.py
+-rw-rw-r--   0 jun        (501) staff       (20)     9299 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/image.py
+-rw-rw-r--   0 jun        (501) staff       (20)    11391 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/jbig2.py
+-rw-rw-r--   0 jun        (501) staff       (20)     8531 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/latin_enc.py
+-rw-rw-r--   0 jun        (501) staff       (20)    35733 2024-04-02 09:52:59.000000 pdfminer.aemc-20221117/pdfminer/layout.py
+-rw-rw-r--   0 jun        (501) staff       (20)     3177 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/lzw.py
+-rw-rw-r--   0 jun        (501) staff       (20)      821 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/pdfcolor.py
+-rw-rw-r--   0 jun        (501) staff       (20)     8787 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/pdfdevice.py
+-rw-rw-r--   0 jun        (501) staff       (20)    37267 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/pdfdocument.py
+-rw-rw-r--   0 jun        (501) staff       (20)    37786 2024-03-27 08:00:02.000000 pdfminer.aemc-20221117/pdfminer/pdffont.py
+-rw-rw-r--   0 jun        (501) staff       (20)    34539 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/pdfinterp.py
+-rw-rw-r--   0 jun        (501) staff       (20)     6803 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/pdfpage.py
+-rw-rw-r--   0 jun        (501) staff       (20)     5896 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/pdfparser.py
+-rw-rw-r--   0 jun        (501) staff       (20)    12109 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/pdftypes.py
+-rwxr-xr-x   0 jun        (501) staff       (20)    19649 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/psparser.py
+-rw-rw-r--   0 jun        (501) staff       (20)        0 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/py.typed
+-rw-rw-r--   0 jun        (501) staff       (20)     1358 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/runlength.py
+-rw-rw-r--   0 jun        (501) staff       (20)       15 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/settings.py
+-rw-rw-r--   0 jun        (501) staff       (20)    20804 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/pdfminer/utils.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-04-02 09:53:54.899381 pdfminer.aemc-20221117/pdfminer.aemc.egg-info/
+-rw-r--r--   0 jun        (501) staff       (20)     3519 2024-04-02 09:53:54.000000 pdfminer.aemc-20221117/pdfminer.aemc.egg-info/PKG-INFO
+-rw-r--r--   0 jun        (501) staff       (20)     6521 2024-04-02 09:53:54.000000 pdfminer.aemc-20221117/pdfminer.aemc.egg-info/SOURCES.txt
+-rw-r--r--   0 jun        (501) staff       (20)        1 2024-04-02 09:53:54.000000 pdfminer.aemc-20221117/pdfminer.aemc.egg-info/dependency_links.txt
+-rw-r--r--   0 jun        (501) staff       (20)      175 2024-04-02 09:53:54.000000 pdfminer.aemc-20221117/pdfminer.aemc.egg-info/requires.txt
+-rw-r--r--   0 jun        (501) staff       (20)        9 2024-04-02 09:53:54.000000 pdfminer.aemc-20221117/pdfminer.aemc.egg-info/top_level.txt
+-rw-r--r--   0 jun        (501) staff       (20)       38 2024-04-02 09:53:54.953726 pdfminer.aemc-20221117/setup.cfg
+-rw-rw-r--   0 jun        (501) staff       (20)     1776 2024-03-27 08:10:12.000000 pdfminer.aemc-20221117/setup.py
+drwxr-xr-x   0 jun        (501) staff       (20)        0 2024-04-02 09:53:54.952918 pdfminer.aemc-20221117/tools/
+-rw-rw-r--   0 jun        (501) staff       (20)        0 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/tools/__init__.py
+-rwxr-xr-x   0 jun        (501) staff       (20)     1646 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/tools/conv_afm.py
+-rwxr-xr-x   0 jun        (501) staff       (20)     6089 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/tools/conv_cmap.py
+-rwxr-xr-x   0 jun        (501) staff       (20)      911 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/tools/conv_glyphlist.py
+-rwxr-xr-x   0 jun        (501) staff       (20)    14316 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/tools/dumppdf.py
+-rwxr-xr-x   0 jun        (501) staff       (20)     9779 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/tools/pdf2txt.py
+-rw-rw-r--   0 jun        (501) staff       (20)     6266 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/tools/pdfdiff.py
+-rwxr-xr-x   0 jun        (501) staff       (20)     2761 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/tools/pdfstats.py
+-rw-rw-r--   0 jun        (501) staff       (20)     1415 2022-11-05 16:22:08.000000 pdfminer.aemc-20221117/tools/prof.py
```

### Comparing `pdfminer.aemc-20221116/CHANGELOG.md` & `pdfminer.aemc-20221117/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/CONTRIBUTING.md` & `pdfminer.aemc-20221117/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/LICENSE` & `pdfminer.aemc-20221117/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/Makefile` & `pdfminer.aemc-20221117/Makefile`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/PKG-INFO` & `pdfminer.aemc-20221117/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfminer.aemc
-Version: 20221116
+Version: 20221117
 Summary: PDF parser and analyzer
 Home-page: https://github.com/pdfminer/pdfminer.aemc
 Author: Yusuke Shinyama + Philippe Guglielmetti + Liew Chun Fui
 Author-email: wargreymon28@gmail.com
 License: MIT/X
 Keywords: pdf parser,pdf converter,layout analysis,text mining
 Classifier: Programming Language :: Python
```

### Comparing `pdfminer.aemc-20221116/README.md` & `pdfminer.aemc-20221117/README.md`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/cmaprsrc/README.txt` & `pdfminer.aemc-20221117/cmaprsrc/README.txt`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/cmaprsrc/cid2code_Adobe_CNS1.txt` & `pdfminer.aemc-20221117/cmaprsrc/cid2code_Adobe_CNS1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/cmaprsrc/cid2code_Adobe_GB1.txt` & `pdfminer.aemc-20221117/cmaprsrc/cid2code_Adobe_GB1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/cmaprsrc/cid2code_Adobe_Japan1.txt` & `pdfminer.aemc-20221117/cmaprsrc/cid2code_Adobe_Japan1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/cmaprsrc/cid2code_Adobe_Korea1.txt` & `pdfminer.aemc-20221117/cmaprsrc/cid2code_Adobe_Korea1.txt`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/noxfile.py` & `pdfminer.aemc-20221117/noxfile.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/_saslprep.py` & `pdfminer.aemc-20221117/pdfminer/_saslprep.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/arcfour.py` & `pdfminer.aemc-20221117/pdfminer/arcfour.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/ascii85.py` & `pdfminer.aemc-20221117/pdfminer/ascii85.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/ccitt.py` & `pdfminer.aemc-20221117/pdfminer/ccitt.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/78-EUC-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/78-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/78-EUC-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/78-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/78-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/78-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/78-RKSJ-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/78-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/78-RKSJ-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/78-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/78-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/78-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/78ms-RKSJ-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/78ms-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/78ms-RKSJ-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/78ms-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/83pv-RKSJ-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/83pv-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/83pv-RKSJ-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/83pv-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/90ms-RKSJ-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/90ms-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/90ms-RKSJ-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/90ms-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/90msp-RKSJ-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/90msp-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/90msp-RKSJ-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/90msp-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/90pv-RKSJ-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/90pv-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/90pv-RKSJ-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/90pv-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/Add-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/Add-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/Add-RKSJ-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/Add-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/Add-RKSJ-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/Add-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/Add-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/Add-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/B5-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/B5-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/B5pc-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/B5pc-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/B5pc-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/B5pc-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/CNS-EUC-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/CNS-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/CNS-EUC-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/CNS-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/CNS1-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/CNS1-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/CNS1-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/CNS1-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/CNS2-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/CNS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/CNS2-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/CNS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/ETHK-B5-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/ETHK-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/ETHK-B5-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/ETHK-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/ETen-B5-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/ETen-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/ETen-B5-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/ETen-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/EUC-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/EUC-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/Ext-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/Ext-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/Ext-RKSJ-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/Ext-RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/Ext-RKSJ-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/Ext-RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/Ext-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/Ext-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GB-EUC-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GB-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GB-EUC-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GB-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GB-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GB-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GB-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GB-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GBK-EUC-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GBK-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GBK-EUC-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GBK-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GBK2K-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GBK2K-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GBK2K-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GBK2K-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GBKp-EUC-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GBKp-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GBKp-EUC-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GBKp-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GBT-EUC-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GBT-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GBT-EUC-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GBT-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GBT-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GBT-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GBT-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GBT-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GBTpc-EUC-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GBTpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GBTpc-EUC-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GBTpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GBpc-EUC-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GBpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/GBpc-EUC-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/GBpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/HKdla-B5-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/HKdla-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/HKdla-B5-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/HKdla-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/HKdlb-B5-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/HKdlb-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/HKdlb-B5-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/HKdlb-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/HKgccs-B5-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/HKgccs-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/HKgccs-B5-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/HKgccs-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/HKm314-B5-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/HKm314-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/HKm314-B5-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/HKm314-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/HKm471-B5-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/HKm471-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/HKm471-B5-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/HKm471-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/HKscs-B5-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/HKscs-B5-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/HKscs-B5-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/HKscs-B5-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/Hankaku-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/Hankaku-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/Hankaku-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/Hankaku-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/KSC-EUC-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/KSC-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/KSC-EUC-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/KSC-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/KSC-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/KSC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/KSC-Johab-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/KSC-Johab-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/KSC-Johab-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/KSC-Johab-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/KSC-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/KSC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/KSCms-UHC-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/KSCms-UHC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/KSCms-UHC-HW-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/KSCms-UHC-HW-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/KSCms-UHC-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/KSCms-UHC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/KSCpc-EUC-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/KSCpc-EUC-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/KSCpc-EUC-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/KSCpc-EUC-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/NWP-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/NWP-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/NWP-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/NWP-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/README.txt` & `pdfminer.aemc-20221117/pdfminer/cmap/README.txt`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/RKSJ-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/RKSJ-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/RKSJ-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/RKSJ-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniCNS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UCS2-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UCS2-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UTF16-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UTF16-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UTF32-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UTF32-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UTF8-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniGB-UTF8-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniGB-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UCS2-HW-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJIS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJIS2004-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJIS2004-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJIS2004-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJIS2004-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJIS2004-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJIS2004-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJISX0213-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJISX0213-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJISX02132004-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniJISX02132004-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UCS2-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UCS2-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UCS2-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UCS2-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UTF16-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UTF16-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UTF16-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UTF16-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UTF32-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UTF32-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UTF32-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UTF32-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UTF8-H.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UTF8-H.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/UniKS-UTF8-V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/UniKS-UTF8-V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/V.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/V.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/to-unicode-Adobe-CNS1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/to-unicode-Adobe-GB1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/to-unicode-Adobe-Japan1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz` & `pdfminer.aemc-20221117/pdfminer/cmap/to-unicode-Adobe-Korea1.pickle.gz`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/cmapdb.py` & `pdfminer.aemc-20221117/pdfminer/cmapdb.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/converter.py` & `pdfminer.aemc-20221117/pdfminer/converter.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/data_structures.py` & `pdfminer.aemc-20221117/pdfminer/data_structures.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/encodingdb.py` & `pdfminer.aemc-20221117/pdfminer/encodingdb.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/fontmetrics.py` & `pdfminer.aemc-20221117/pdfminer/fontmetrics.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/glyphlist.py` & `pdfminer.aemc-20221117/pdfminer/glyphlist.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/high_level.py` & `pdfminer.aemc-20221117/pdfminer/high_level.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/image.py` & `pdfminer.aemc-20221117/pdfminer/image.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/jbig2.py` & `pdfminer.aemc-20221117/pdfminer/jbig2.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/latin_enc.py` & `pdfminer.aemc-20221117/pdfminer/latin_enc.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/layout.py` & `pdfminer.aemc-20221117/pdfminer/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,36 +368,44 @@
             else:
                 vx = vx * fontsize * 0.001
             vy = (1000 - vy) * fontsize * 0.001
             bbox_lower_left = (-vx, vy + rise + self.adv)
             bbox_upper_right = (-vx + fontsize, vy + rise)
         else:
             # horizontal
-            # Original (not good)
-            #descent = font.get_descent() * fontsize
-            #bbox_lower_left = (0, descent + rise)
-            #bbox_upper_right = (self.adv, descent + rise + fontsize)
+            Original (not good)
+            descent = font.get_descent() * fontsize
+            bbox_lower_left = (0, descent + rise)
+            bbox_upper_right = (self.adv, descent + rise + fontsize)
             # Trial 1: Divided by 2 (overall a little bit better)
             #ascent = font.get_ascent() * fontsize / 2.0
             #descent = font.get_descent() * fontsize / 2.0
             #bbox_lower_left = (0, descent + rise)
             #bbox_upper_right = (self.adv, descent + rise + fontsize)
             # Trial 2: Offset by 0.2 (mostly better but not always)
             #ascent = (font.get_ascent() - 0.2) * fontsize
             #descent = (font.get_descent() + 0.2) * fontsize
             #bbox_lower_left = (0, descent + rise)
             #bbox_upper_right = (self.adv, descent + rise + fontsize)
-            # Trial 3: Using StemV instead of descent (overall much better)
-            ascent = font.get_ascent() * fontsize
-            descent = font.get_descent() * fontsize
-            height = font.get_height() * fontsize
-            stemv = font.get_stemv() * fontsize
-            yAdj = -stemv if abs(stemv) < abs(descent) else 0
-            bbox_lower_left = (0, yAdj + rise)
-            bbox_upper_right = (self.adv, yAdj + rise + fontsize)
+            # # Trial 3: Using StemV instead of descent (overall much better in 20201018)
+            # ascent = font.get_ascent() * fontsize
+            # descent = font.get_descent() * fontsize
+            # height = font.get_height() * fontsize
+            # stemv = font.get_stemv() * fontsize
+            # yAdj = -stemv if abs(stemv) < abs(descent) else 0
+            # bbox_lower_left = (0, yAdj + rise)
+            # bbox_upper_right = (self.adv, yAdj + rise + fontsize)
+            # # Trial 4: Using StemV instead of descent (overall much better in 20221105)
+            # ascent = font.get_ascent() * fontsize
+            # descent = font.get_descent() * fontsize
+            # height = font.get_height() * fontsize
+            # stemv = font.get_stemv() * fontsize
+            # yAdj = -stemv if abs(stemv) < abs(descent) else 0
+            # bbox_lower_left = (0, yAdj + rise)
+            # bbox_upper_right = (self.adv, yAdj + rise + fontsize)
         (a, b, c, d, e, f) = self.matrix
         self.upright = 0 < a * d * scaling and b * c <= 0
         (x0, y0) = apply_matrix_pt(self.matrix, bbox_lower_left)
         (x1, y1) = apply_matrix_pt(self.matrix, bbox_upper_right)
         if x1 < x0:
             (x0, x1) = (x1, x0)
         if y1 < y0:
```

### Comparing `pdfminer.aemc-20221116/pdfminer/lzw.py` & `pdfminer.aemc-20221117/pdfminer/lzw.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/pdfcolor.py` & `pdfminer.aemc-20221117/pdfminer/pdfcolor.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/pdfdevice.py` & `pdfminer.aemc-20221117/pdfminer/pdfdevice.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/pdfdocument.py` & `pdfminer.aemc-20221117/pdfminer/pdfdocument.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/pdffont.py` & `pdfminer.aemc-20221117/pdfminer/pdffont.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/pdfinterp.py` & `pdfminer.aemc-20221117/pdfminer/pdfinterp.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/pdfpage.py` & `pdfminer.aemc-20221117/pdfminer/pdfpage.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/pdfparser.py` & `pdfminer.aemc-20221117/pdfminer/pdfparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/pdftypes.py` & `pdfminer.aemc-20221117/pdfminer/pdftypes.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/psparser.py` & `pdfminer.aemc-20221117/pdfminer/psparser.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/runlength.py` & `pdfminer.aemc-20221117/pdfminer/runlength.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer/utils.py` & `pdfminer.aemc-20221117/pdfminer/utils.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/pdfminer.aemc.egg-info/PKG-INFO` & `pdfminer.aemc-20221117/pdfminer.aemc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfminer.aemc
-Version: 20221116
+Version: 20221117
 Summary: PDF parser and analyzer
 Home-page: https://github.com/pdfminer/pdfminer.aemc
 Author: Yusuke Shinyama + Philippe Guglielmetti + Liew Chun Fui
 Author-email: wargreymon28@gmail.com
 License: MIT/X
 Keywords: pdf parser,pdf converter,layout analysis,text mining
 Classifier: Programming Language :: Python
```

### Comparing `pdfminer.aemc-20221116/pdfminer.aemc.egg-info/SOURCES.txt` & `pdfminer.aemc-20221117/pdfminer.aemc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/setup.py` & `pdfminer.aemc-20221117/setup.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/tools/conv_afm.py` & `pdfminer.aemc-20221117/tools/conv_afm.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/tools/conv_cmap.py` & `pdfminer.aemc-20221117/tools/conv_cmap.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/tools/conv_glyphlist.py` & `pdfminer.aemc-20221117/tools/conv_glyphlist.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/tools/dumppdf.py` & `pdfminer.aemc-20221117/tools/dumppdf.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/tools/pdf2txt.py` & `pdfminer.aemc-20221117/tools/pdf2txt.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/tools/pdfdiff.py` & `pdfminer.aemc-20221117/tools/pdfdiff.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/tools/pdfstats.py` & `pdfminer.aemc-20221117/tools/pdfstats.py`

 * *Files identical despite different names*

### Comparing `pdfminer.aemc-20221116/tools/prof.py` & `pdfminer.aemc-20221117/tools/prof.py`

 * *Files identical despite different names*

