# Comparing `tmp/MobileInventoryCLI-0.4.36.tar.gz` & `tmp/MobileInventoryCLI-0.4.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.36.tar", last modified: Tue Apr  2 14:44:15 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.37.tar", last modified: Tue Apr  2 19:05:36 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.36.tar` & `MobileInventoryCLI-0.4.37.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.272792 MobileInventoryCLI-0.4.36/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.262792 MobileInventoryCLI-0.4.36/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.262792 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.266126 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.266126 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    24225 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.266126 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.266126 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.266126 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    99999 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5460 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.266126 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.266126 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.266126 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     3921 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.266126 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.269459 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.269459 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.269459 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.269459 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.269459 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    12508 2024-04-02 14:43:18.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.269459 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    19940 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
--rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.269459 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.269459 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.269459 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-02 14:44:09.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      278 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.269459 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.269459 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.269459 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.269459 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.272792 MobileInventoryCLI-0.4.36/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.272792 MobileInventoryCLI-0.4.36/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.272792 MobileInventoryCLI-0.4.36/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.272792 MobileInventoryCLI-0.4.36/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-01 23:29:54.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:15.272792 MobileInventoryCLI-0.4.36/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-02 14:44:15.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     4805 2024-04-02 14:44:15.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-02 14:44:15.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      118 2024-04-02 14:44:15.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-02 14:44:15.000000 MobileInventoryCLI-0.4.36/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-02 14:44:15.272792 MobileInventoryCLI-0.4.36/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-02 14:44:15.272792 MobileInventoryCLI-0.4.36/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      802 2024-04-02 14:44:14.000000 MobileInventoryCLI-0.4.36/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.630134 MobileInventoryCLI-0.4.37/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.620134 MobileInventoryCLI-0.4.37/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.620134 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.620134 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    24225 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   100711 2024-04-02 18:41:37.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5460 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3921 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34423 2024-04-02 19:04:12.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    19940 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-02 19:05:30.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      390 2024-04-02 19:05:27.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.630134 MobileInventoryCLI-0.4.37/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.630134 MobileInventoryCLI-0.4.37/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.630134 MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-02 19:05:36.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     4805 2024-04-02 19:05:36.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-02 19:05:36.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      118 2024-04-02 19:05:36.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-02 19:05:36.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-02 19:05:36.630134 MobileInventoryCLI-0.4.37/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-02 19:05:36.630134 MobileInventoryCLI-0.4.37/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      802 2024-04-02 19:05:36.000000 MobileInventoryCLI-0.4.37/setup.py
```

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -2288,63 +2288,86 @@
         
 
 Shift.metadata.create_all(ENGINE)
 
 
 class Template:
     def init(self,**kwargs):
-        __tablename__=self.__class__.__name__
+        __tablename__=kwargs.get("__tablename__")
         fields=[i.name for i in self.__table__.columns]
         for i in fields:
             if i in list(kwargs.keys()):
                 setattr(self,i,kwargs.get(i))
 
     def __str__(self,vc=Fore.light_yellow,fc=Fore.light_green,cc=Fore.light_magenta):
         m=[]
-        m.append(f"{cc}{__class__.__name__}{Style.reset}(")
+        m.append(f"{cc}{self.__tablename__}{Style.reset}(")
         fields=[i.name for i in self.__table__.columns]
         for i in fields:
             m.append(f"\t{fc}{i}{Style.reset}={vc}{getattr(self,i)}{Style.reset}")
         m.append(")")
         return '\n'.join(m)
 
 class Billing(BASE,Template):
     __tablename__="Billing"
     default=Column(Boolean)
     sellerAddress=Column(String)
     sellerName=Column(String)
+    sellerPhone=Column(String)
+    sellerEmail=Column(String)
+    purchaserEmail=Column(String)
+    purchaserPhone=Column(String)
     purchaserName=Column(String)
     purchaserAddress=Column(String)
     BillingId=Column(Integer,primary_key=True)
     Date=Column(Date)
     RetailersPermitSerial=Column(String)
     CertofReg=Column(String)
+    PaymentType=Column(String)
     def __init__(self,**kwargs):
-        self.init(**kwargs)
+        #kwargs['__tablename__']="Billing"
+        kwargs['__tablename__']=self.__tablename__
+        self.init(**kwargs,)
 
 class RecieptEntry(BASE,Template):
     __tablename__="RecieptEntry"
-    BillingId=Column(Integer,primary_key=True)
-    BillingDate=Column(Date)
+    ReceiptEntryId=Column(Integer,primary_key=True)
+    RecieptId=Column(Integer)
+    Date=Column(Date)
     EntryCode=Column(String)
     EntryBarcode=Column(String)
     EntryName=Column(String)
     EntryId=Column(Integer)
     EntryPrice=Column(Float)
     QtySold=Column(Float)
     def __init__(self,**kwargs):
+        kwargs['__tablename__']=self.__tablename__
         self.init(**kwargs)
 
 class AdditionalExpenseOrFee(BASE,Template):
     __tablename__="AdditionalExpenseOrFee"
     AdditionalExpenseId=Column(Integer,primary_key=True)
+    RecieptId=Column(Integer)
     Value=Column(Integer)
     Name=Column(String)
     Comment=Column(String)
     DOE=Column(Date)#Date of Entry
     DD=Column(Date)#Due Date
     def __init__(self,**kwargs):
+        kwargs['__tablename__']=self.__tablename__
         self.init(**kwargs)
 
 Billing.metadata.create_all(ENGINE)
 RecieptEntry.metadata.create_all(ENGINE)
 AdditionalExpenseOrFee.metadata.create_all(ENGINE)
+
+class Reciept(BASE,Template):
+    __tablename__="Reciept"
+    RecieptId=Column(Integer,primary_key=True)
+    BillingId=Column(Integer)
+    Date=Column(Date)
+    
+    def __init__(self,**kwargs):
+        self.init(**kwargs)
+        __tablename__="Reciept"
+
+Reciept.metadata.create_all(ENGINE)
```

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.36
+Version: 0.4.37
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.36/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.36/PKG-INFO` & `MobileInventoryCLI-0.4.37/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.36
+Version: 0.4.37
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.36/setup.py` & `MobileInventoryCLI-0.4.37/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.36'
+version='0.4.37'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

