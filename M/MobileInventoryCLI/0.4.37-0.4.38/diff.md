# Comparing `tmp/MobileInventoryCLI-0.4.37.tar.gz` & `tmp/MobileInventoryCLI-0.4.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.37.tar", last modified: Tue Apr  2 19:05:36 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.38.tar", last modified: Tue Apr  2 20:16:42 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.37.tar` & `MobileInventoryCLI-0.4.38.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.630134 MobileInventoryCLI-0.4.37/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.620134 MobileInventoryCLI-0.4.37/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.620134 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.620134 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    24225 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   100711 2024-04-02 18:41:37.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5460 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     3921 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.623467 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34423 2024-04-02 19:04:12.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    19940 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
--rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-02 19:05:30.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      390 2024-04-02 19:05:27.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.626800 MobileInventoryCLI-0.4.37/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.630134 MobileInventoryCLI-0.4.37/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.630134 MobileInventoryCLI-0.4.37/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-02 14:44:32.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:36.630134 MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-02 19:05:36.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     4805 2024-04-02 19:05:36.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-02 19:05:36.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      118 2024-04-02 19:05:36.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-02 19:05:36.000000 MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-02 19:05:36.630134 MobileInventoryCLI-0.4.37/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-02 19:05:36.630134 MobileInventoryCLI-0.4.37/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      802 2024-04-02 19:05:36.000000 MobileInventoryCLI-0.4.37/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.444238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.444238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.447572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.447572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    24225 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.447572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.447572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   101415 2024-04-02 20:05:34.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5460 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4238 2024-04-02 19:58:57.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.454238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.454238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34423 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.454238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    19940 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.454238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.454238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.454238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-02 20:16:36.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      390 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.454238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-02 20:16:42.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     4805 2024-04-02 20:16:42.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-02 20:16:42.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      118 2024-04-02 20:16:42.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-02 20:16:42.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      802 2024-04-02 20:16:41.000000 MobileInventoryCLI-0.4.38/setup.py
```

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,14 +270,17 @@
     #note {Entryid} {new_value}
     
     #size {Entryid} 
     #size {Entryid} {new_value}
     '''
     Name=Column(String)
     Price=Column(Float)
+    CRV=Column(Float)
+    Tax=Column(Float)
+    TaxNote=Column(String)
     Note=Column(String)
     Size=Column(String)
     
     CaseCount=Column(Integer)
 
     Shelf=Column(Integer)
     BackRoom=Column(Integer)
@@ -339,17 +342,20 @@
         part.append("-")
         for num in range(4):
             part.append(f[random.randint(0,len(f)-1)])
         return ''.join(part)
 
 
 
-    def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=0,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode=''):
+    def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=0,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode='',CRV=0.0,Tax=0.0,TaxNote=''):
         if EntryId:
             self.EntryId=EntryId
+        self.CRV=CRV
+        self.Tax=Tax
+        self.TaxNote=TaxNote
         self.Barcode=Barcode
         self.Code=Code
         self.Name=Name
         self.Price=Price
         self.Note=Note
         self.Size=Size
         self.Shelf=Shelf
@@ -778,14 +784,17 @@
         m= f"""
 {Style.bold}{Style.underline}{Fore.pale_green_1b}Entry{Style.reset}(
 {Fore.hot_pink_2}{Style.bold}{Style.underline}EntryId{Style.reset}={self.EntryId}
 {Fore.violet}{Style.underline}Code{Style.reset}='{self.Code}',
 {Fore.orange_3}{Style.bold}Barcode{Style.reset}='{self.Barcode}',
 {Fore.orange_3}{Style.underline}UPCE from UPCA[if any]{Style.reset}='{self.upce2upca}',
 {Fore.green}{Style.bold}Price{Style.reset}=${self.Price},
+{Fore.green}{Style.bold}CRV{Style.reset}=${self.CRV},
+{Fore.green}{Style.bold}Tax{Style.reset}=${self.Tax},
+{Fore.green}{Style.bold}TaxNote{Style.reset}='{self.TaxNote}',
 {Fore.red}Name{Style.reset}='{self.Name}',
 {Fore.tan}Note{Style.reset}='{self.Note}',
 {Fore.grey_50}ALT_Barcode{Style.reset}={Fore.grey_70}{self.ALT_Barcode}{Style.reset}
 {Fore.grey_50}DUP_Barcode{Style.reset}={Fore.grey_70}{self.DUP_Barcode}{Style.reset}
 {Fore.grey_50}CaseID_BR{Style.reset}={Fore.grey_70}{self.CaseID_BR}{Style.reset}
 {Fore.grey_50}CaseID_LD{Style.reset}={Fore.grey_70}{self.CaseID_LD}{Style.reset}
 {Fore.grey_50}CaseID_6W{Style.reset}={Fore.grey_70}{self.CaseID_6W}{Style.reset}
@@ -854,14 +863,18 @@
     #note {Entryid} {new_value}
     
     #size {Entryid} 
     #size {Entryid} {new_value}
     '''
     Name=Column(String)
     Price=Column(Float)
+    CRV=Column(Float)
+    Tax=Column(Float)
+    TaxNote=Column(String)
+
     Note=Column(String)
     Size=Column(String)
     
     CaseCount=Column(Integer)
 
     Shelf=Column(Integer)
     BackRoom=Column(Integer)
@@ -916,18 +929,20 @@
         part.append("-")
         for num in range(4):
             part.append(f[random.randint(0,len(f)-1)])
         return ''.join(part)
 
 
 
-    def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=0,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode='',DayLogDate=datetime.now(),DayLogId=None):
+    def __init__(self,Barcode,Code,upce2upca='',Name='',InList=False,Price=0.0,Note='',Size='',CaseCount=0,Shelf=0,BackRoom=0,Display_1=0,Display_2=0,Display_3=0,Display_4=0,Display_5=0,Display_6=0,Stock_Total=0,Timestamp=datetime.now().timestamp(),EntryId=None,Location='///',ListQty=0.0,Image='',CHKSTND_SPLY=0,WD_DSPLY=0,FLRL_CHP_DSPLY=0,FLRL_WTR_DSPLY=0,SBX_WTR_KLR=0,SBX_CHP_DSPLY=0,SBX_WTR_DSPLY=0,Facings=0,Tags='',CaseID_6W='',CaseID_BR='',CaseID_LD='',ALT_Barcode='',DUP_Barcode='',DayLogDate=datetime.now(),DayLogId=None,CRV=0.0,Tax=0.0,TaxNote=''):
         if EntryId:
             self.EntryId=EntryId
-
+        self.CRV=CRV
+        self.Tax=Tax
+        self.TaxNote=TaxNote
         self.Barcode=Barcode
         self.Code=Code
         self.Name=Name
         self.Price=Price
         self.Note=Note
         self.Size=Size
         self.Shelf=Shelf
@@ -1276,14 +1291,17 @@
         {Fore.cyan}DayLogId = {self.DayLogId}{Style.reset},
         {Fore.cyan}DayLogDate = {self.DayLogDate}{Style.reset},
         {Fore.hot_pink_2}{Style.bold}{Style.underline}EntryId{Style.reset}={self.EntryId}
         {Fore.violet}{Style.underline}Code{Style.reset}='{self.Code}',
         {Fore.orange_3}{Style.bold}Barcode{Style.reset}='{self.Barcode}',
         {Fore.orange_3}{Style.underline}UPCE from UPCA[if any]{Style.reset}='{self.upce2upca}',
         {Fore.green}{Style.bold}Price{Style.reset}=${self.Price},
+        {Fore.green}{Style.bold}CRV{Style.reset}=${self.CRV},
+        {Fore.green}{Style.bold}Tax{Style.reset}=${self.Tax},
+        {Fore.green}{Style.bold}TaxNote{Style.reset}='{self.TaxNote}',
         {Fore.red}Name{Style.reset}='{self.Name}',
         {Fore.tan}Note{Style.reset}='{self.Note}',
         {Fore.grey_50}ALT_Barcode{Style.reset}={Fore.grey_70}{self.ALT_Barcode}{Style.reset}
         {Fore.grey_50}DUP_Barcode{Style.reset}={Fore.grey_70}{self.DUP_Barcode}{Style.reset}
         {Fore.grey_50}CaseID_BR{Style.reset}={Fore.grey_70}{self.CaseID_BR}{Style.reset}
         {Fore.grey_50}CaseID_LD{Style.reset}={Fore.grey_70}{self.CaseID_LD}{Style.reset}
         {Fore.grey_50}CaseID_6W{Style.reset}={Fore.grey_70}{self.CaseID_6W}{Style.reset}
```

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files 12% similar despite different names*

```diff
@@ -81,15 +81,25 @@
 												for cf in cfresults:
 													#print(cf.Name)
 													if cf.Name in fields:
 														#item_cf_ids.append(cf.CustomFieldId)
 														#print(item_cf_ids)
 														cfdata=ses.query(ltbl.ItemCustomField).filter(ltbl.ItemCustomField.ItemId==item.ItemId,ltbl.ItemCustomField.CustomFieldId==cf.CustomFieldId).first()
 														if cfdata != None:
-															dt[cf.Name]=cfdata.Value
+															if cf.Type == 0:
+																pass
+																#text
+															elif cf.Type == 1:
+																print(cf.Name)
+																if cfdata.Value in [None,'']:
+																	dt[cf.Name]=float(1)
+																else:
+																	dt[cf.Name]=float(cfdata.Value)
+															else:
+																dt[cf.Name]=cfdata.Value
 												dt["Name"]=item.Name
 												dt["Barcode"]=item.Barcode
 												dt["Code"]=item.Code
 												dt["Price"]=item.Price
 												dt["Image"]=n
 												dt["Note"]=json.dumps({'Note':item.Note,'MeasurementUnit':item.MeasurementUnit})
 												dt["Size"]=f"SIZE:{dt.get('Size')}|Unit:{dt.get('SizeUnit')}"
```

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.37
+Version: 0.4.38
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.37/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.37/PKG-INFO` & `MobileInventoryCLI-0.4.38/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.37
+Version: 0.4.38
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.37/setup.py` & `MobileInventoryCLI-0.4.38/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.37'
+version='0.4.38'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

