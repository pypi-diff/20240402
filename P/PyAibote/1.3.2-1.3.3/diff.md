# Comparing `tmp/PyAibote-1.3.2.tar.gz` & `tmp/PyAibote-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAibote-1.3.2.tar", last modified: Thu Mar 28 06:38:37 2024, max compression
+gzip compressed data, was "PyAibote-1.3.3.tar", last modified: Tue Apr  2 11:12:23 2024, max compression
```

## Comparing `PyAibote-1.3.2.tar` & `PyAibote-1.3.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 06:38:37.939142 PyAibote-1.3.2/
--rw-rw-rw-   0        0        0     1089 2024-03-28 06:38:37.939142 PyAibote-1.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-28 06:38:37.667878 PyAibote-1.3.2/PyAibote/
--rw-rw-rw-   0        0        0     2788 2024-03-19 01:40:59.000000 PyAibote-1.3.2/PyAibote/AndroidBot.py
-drwxrwxrwx   0        0        0        0 2024-03-28 06:38:37.833999 PyAibote-1.3.2/PyAibote/AndroidBotModel/
--rw-rw-rw-   0        0        0     7670 2024-02-27 11:01:39.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/AndroidHidCorrelation.py
--rw-rw-rw-   0        0        0     2257 2024-03-19 01:39:35.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/AndroidLoadWait.py
--rw-rw-rw-   0        0        0     3104 2024-03-19 01:39:35.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/ColorFindingOperation.py
--rw-rw-rw-   0        0        0     6238 2024-01-18 22:33:52.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/Control.py
--rw-rw-rw-   0        0        0     5580 2024-03-19 01:39:35.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/CoordinateOperation.py
--rw-rw-rw-   0        0        0    13015 2024-01-17 22:58:26.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0    16690 2024-03-22 10:35:59.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/EquipmentOperation.py
--rw-rw-rw-   0        0        0     3094 2024-01-17 08:25:14.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/FileTransfer.py
--rw-rw-rw-   0        0        0     8280 2024-03-28 05:05:11.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/MapFindingOperation.py
--rw-rw-rw-   0        0        0     9184 2024-01-20 09:48:18.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/OcrCorrelation.py
--rw-rw-rw-   0        0        0     1207 2024-01-17 06:31:31.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/ScreenProjectionOperation.py
--rw-rw-rw-   0        0        0     9303 2024-01-18 00:26:45.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/ScreenshotOperation.py
--rw-rw-rw-   0        0        0     1227 2024-01-17 21:32:01.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/UrlRequest.py
--rw-rw-rw-   0        0        0     4476 2024-01-18 22:34:37.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/VerificationCodeOperation.py
--rw-rw-rw-   0        0        0     1867 2024-01-20 10:06:51.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/YoloService.py
--rw-rw-rw-   0        0        0     1088 2024-02-27 23:24:38.000000 PyAibote-1.3.2/PyAibote/AndroidBotModel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 06:38:37.835998 PyAibote-1.3.2/PyAibote/CommonUse/
--rw-rw-rw-   0        0        0     2101 2024-02-15 23:31:42.000000 PyAibote-1.3.2/PyAibote/CommonUse/ChatGenerative.py
--rw-rw-rw-   0        0        0        0 2024-02-27 23:33:36.000000 PyAibote-1.3.2/PyAibote/CommonUse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 06:38:37.859084 PyAibote-1.3.2/PyAibote/Tool/
--rw-rw-rw-   0        0        0     5457 2024-03-19 01:40:59.000000 PyAibote-1.3.2/PyAibote/Tool/DatabaseFunc.py
--rw-rw-rw-   0        0        0     2188 2024-03-19 01:39:35.000000 PyAibote-1.3.2/PyAibote/Tool/DebugStartDriver.py
--rw-rw-rw-   0        0        0     2223 2024-03-19 01:40:59.000000 PyAibote-1.3.2/PyAibote/Tool/Logger.py
--rw-rw-rw-   0        0        0     1749 2024-03-19 01:40:59.000000 PyAibote-1.3.2/PyAibote/Tool/LoggerFunc.py
--rw-rw-rw-   0        0        0      912 2024-03-19 01:40:59.000000 PyAibote-1.3.2/PyAibote/Tool/SendTcpData.py
--rw-rw-rw-   0        0        0      532 2024-01-13 09:10:40.000000 PyAibote-1.3.2/PyAibote/Tool/SocketServer.py
--rw-rw-rw-   0        0        0     3342 2024-03-19 01:40:59.000000 PyAibote-1.3.2/PyAibote/Tool/Sqlite3DataBase.py
--rw-rw-rw-   0        0        0      660 2024-01-18 08:34:16.000000 PyAibote-1.3.2/PyAibote/Tool/UniversalFunction.py
--rw-rw-rw-   0        0        0     4364 2024-03-19 01:40:59.000000 PyAibote-1.3.2/PyAibote/Tool/WriteReadFileFunc.py
--rw-rw-rw-   0        0        0      550 2024-03-19 01:40:59.000000 PyAibote-1.3.2/PyAibote/Tool/__init__.py
--rw-rw-rw-   0        0        0     1998 2024-03-19 01:40:59.000000 PyAibote-1.3.2/PyAibote/WebBot.py
-drwxrwxrwx   0        0        0        0 2024-03-28 06:38:37.904137 PyAibote-1.3.2/PyAibote/WebBotModel/
--rw-rw-rw-   0        0        0     3645 2024-01-26 01:18:21.000000 PyAibote-1.3.2/PyAibote/WebBotModel/CookiesOperation.py
--rw-rw-rw-   0        0        0      392 2024-01-18 22:24:47.000000 PyAibote-1.3.2/PyAibote/WebBotModel/DrivingOperation.py
--rw-rw-rw-   0        0        0     9634 2024-01-13 17:40:41.000000 PyAibote-1.3.2/PyAibote/WebBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0      697 2024-01-12 10:05:13.000000 PyAibote-1.3.2/PyAibote/WebBotModel/IframeOperation.py
--rw-rw-rw-   0        0        0      890 2024-01-18 22:24:31.000000 PyAibote-1.3.2/PyAibote/WebBotModel/JSinjection.py
--rw-rw-rw-   0        0        0     3592 2024-01-26 00:38:04.000000 PyAibote-1.3.2/PyAibote/WebBotModel/KeymouseOperation.py
--rw-rw-rw-   0        0        0     3993 2024-01-13 12:29:13.000000 PyAibote-1.3.2/PyAibote/WebBotModel/PagesAndNavigation.py
--rw-rw-rw-   0        0        0     1091 2024-01-18 22:23:35.000000 PyAibote-1.3.2/PyAibote/WebBotModel/PopUpWindow.py
--rw-rw-rw-   0        0        0     3133 2024-03-19 01:39:35.000000 PyAibote-1.3.2/PyAibote/WebBotModel/WebLoadWait.py
--rw-rw-rw-   0        0        0     5606 2024-01-25 23:04:37.000000 PyAibote-1.3.2/PyAibote/WebBotModel/WindowOperation.py
--rw-rw-rw-   0        0        0      654 2024-02-15 23:42:13.000000 PyAibote-1.3.2/PyAibote/WebBotModel/__init__.py
--rw-rw-rw-   0        0        0     4186 2024-03-19 01:40:59.000000 PyAibote-1.3.2/PyAibote/WindowsBot.py
-drwxrwxrwx   0        0        0        0 2024-03-28 06:38:37.937134 PyAibote-1.3.2/PyAibote/WindowsBotModel/
--rw-rw-rw-   0        0        0    20130 2024-03-28 05:07:36.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/ColorOperation.py
--rw-rw-rw-   0        0        0    21461 2024-03-28 05:02:42.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/DigitalHumanOperation.py
--rw-rw-rw-   0        0        0     1237 2024-03-22 13:46:05.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/DrivingOperation.py
--rw-rw-rw-   0        0        0    14186 2024-01-18 22:29:18.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0     5207 2024-01-22 22:39:26.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/ExcelOperation.py
--rw-rw-rw-   0        0        0     6629 2024-01-13 17:47:39.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/KeymouseOperation.py
--rw-rw-rw-   0        0        0     8395 2024-03-19 01:39:35.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/OcrOperation.py
--rw-rw-rw-   0        0        0      703 2024-01-15 07:27:07.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/OtherOperations.py
--rw-rw-rw-   0        0        0     2379 2024-03-22 11:06:00.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/SystemOperation.py
--rw-rw-rw-   0        0        0     5962 2024-01-22 23:03:02.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/VerificationCodeOperation.py
--rw-rw-rw-   0        0        0     6402 2024-01-22 23:49:04.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/VoiceService.py
--rw-rw-rw-   0        0        0     7513 2024-01-18 22:31:38.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/WinHidCorrelation.py
--rw-rw-rw-   0        0        0     2124 2024-03-19 01:39:35.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/WinLoadWait.py
--rw-rw-rw-   0        0        0     7160 2024-01-14 20:16:53.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/WindowOperation.py
--rw-rw-rw-   0        0        0     2936 2024-01-14 20:29:30.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/YoloOperation.py
--rw-rw-rw-   0        0        0     1115 2024-02-15 23:42:02.000000 PyAibote-1.3.2/PyAibote/WindowsBotModel/__init__.py
--rw-rw-rw-   0        0        0      277 2024-02-27 10:41:36.000000 PyAibote-1.3.2/PyAibote/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 06:38:37.677882 PyAibote-1.3.2/PyAibote.egg-info/
--rw-rw-rw-   0        0        0     1089 2024-03-28 06:38:37.000000 PyAibote-1.3.2/PyAibote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2493 2024-03-28 06:38:37.000000 PyAibote-1.3.2/PyAibote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 06:38:37.000000 PyAibote-1.3.2/PyAibote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-03-28 06:38:37.000000 PyAibote-1.3.2/PyAibote.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-28 06:38:37.000000 PyAibote-1.3.2/PyAibote.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8925 2024-03-19 02:24:43.000000 PyAibote-1.3.2/README.md
--rw-rw-rw-   0        0        0       42 2024-03-28 06:38:37.940136 PyAibote-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1425 2024-03-28 06:36:31.000000 PyAibote-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:12:23.025863 PyAibote-1.3.3/
+-rw-rw-rw-   0        0        0     1089 2024-04-02 11:12:22.987864 PyAibote-1.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 11:12:22.492578 PyAibote-1.3.3/PyAibote/
+-rw-rw-rw-   0        0        0     2788 2024-03-19 01:40:59.000000 PyAibote-1.3.3/PyAibote/AndroidBot.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:12:22.623577 PyAibote-1.3.3/PyAibote/AndroidBotModel/
+-rw-rw-rw-   0        0        0     7670 2024-02-27 11:01:39.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/AndroidHidCorrelation.py
+-rw-rw-rw-   0        0        0     2257 2024-03-19 01:39:35.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/AndroidLoadWait.py
+-rw-rw-rw-   0        0        0     3104 2024-03-19 01:39:35.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/ColorFindingOperation.py
+-rw-rw-rw-   0        0        0     6238 2024-01-18 22:33:52.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/Control.py
+-rw-rw-rw-   0        0        0     5580 2024-03-19 01:39:35.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/CoordinateOperation.py
+-rw-rw-rw-   0        0        0    13015 2024-01-17 22:58:26.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0    16690 2024-03-22 10:35:59.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/EquipmentOperation.py
+-rw-rw-rw-   0        0        0     3094 2024-01-17 08:25:14.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/FileTransfer.py
+-rw-rw-rw-   0        0        0     8280 2024-03-28 05:05:11.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/MapFindingOperation.py
+-rw-rw-rw-   0        0        0     9184 2024-01-20 09:48:18.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/OcrCorrelation.py
+-rw-rw-rw-   0        0        0     1207 2024-01-17 06:31:31.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/ScreenProjectionOperation.py
+-rw-rw-rw-   0        0        0     9303 2024-01-18 00:26:45.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/ScreenshotOperation.py
+-rw-rw-rw-   0        0        0     2012 2024-04-02 11:03:01.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/UrlRequest.py
+-rw-rw-rw-   0        0        0     4476 2024-01-18 22:34:37.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/VerificationCodeOperation.py
+-rw-rw-rw-   0        0        0     1867 2024-01-20 10:06:51.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/YoloService.py
+-rw-rw-rw-   0        0        0     1088 2024-02-27 23:24:38.000000 PyAibote-1.3.3/PyAibote/AndroidBotModel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:12:22.670575 PyAibote-1.3.3/PyAibote/CommonUse/
+-rw-rw-rw-   0        0        0     2101 2024-02-15 23:31:42.000000 PyAibote-1.3.3/PyAibote/CommonUse/ChatGenerative.py
+-rw-rw-rw-   0        0        0        0 2024-02-27 23:33:36.000000 PyAibote-1.3.3/PyAibote/CommonUse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:12:22.771376 PyAibote-1.3.3/PyAibote/Tool/
+-rw-rw-rw-   0        0        0     5457 2024-03-19 01:40:59.000000 PyAibote-1.3.3/PyAibote/Tool/DatabaseFunc.py
+-rw-rw-rw-   0        0        0     2188 2024-03-19 01:39:35.000000 PyAibote-1.3.3/PyAibote/Tool/DebugStartDriver.py
+-rw-rw-rw-   0        0        0     2223 2024-03-19 01:40:59.000000 PyAibote-1.3.3/PyAibote/Tool/Logger.py
+-rw-rw-rw-   0        0        0     1749 2024-03-19 01:40:59.000000 PyAibote-1.3.3/PyAibote/Tool/LoggerFunc.py
+-rw-rw-rw-   0        0        0      912 2024-03-19 01:40:59.000000 PyAibote-1.3.3/PyAibote/Tool/SendTcpData.py
+-rw-rw-rw-   0        0        0      532 2024-01-13 09:10:40.000000 PyAibote-1.3.3/PyAibote/Tool/SocketServer.py
+-rw-rw-rw-   0        0        0     3342 2024-03-19 01:40:59.000000 PyAibote-1.3.3/PyAibote/Tool/Sqlite3DataBase.py
+-rw-rw-rw-   0        0        0      660 2024-01-18 08:34:16.000000 PyAibote-1.3.3/PyAibote/Tool/UniversalFunction.py
+-rw-rw-rw-   0        0        0     4364 2024-03-19 01:40:59.000000 PyAibote-1.3.3/PyAibote/Tool/WriteReadFileFunc.py
+-rw-rw-rw-   0        0        0      550 2024-03-19 01:40:59.000000 PyAibote-1.3.3/PyAibote/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1998 2024-03-19 01:40:59.000000 PyAibote-1.3.3/PyAibote/WebBot.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:12:22.839182 PyAibote-1.3.3/PyAibote/WebBotModel/
+-rw-rw-rw-   0        0        0     3645 2024-01-26 01:18:21.000000 PyAibote-1.3.3/PyAibote/WebBotModel/CookiesOperation.py
+-rw-rw-rw-   0        0        0      392 2024-01-18 22:24:47.000000 PyAibote-1.3.3/PyAibote/WebBotModel/DrivingOperation.py
+-rw-rw-rw-   0        0        0    10613 2024-04-02 11:09:05.000000 PyAibote-1.3.3/PyAibote/WebBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0      697 2024-01-12 10:05:13.000000 PyAibote-1.3.3/PyAibote/WebBotModel/IframeOperation.py
+-rw-rw-rw-   0        0        0      890 2024-01-18 22:24:31.000000 PyAibote-1.3.3/PyAibote/WebBotModel/JSinjection.py
+-rw-rw-rw-   0        0        0     3592 2024-01-26 00:38:04.000000 PyAibote-1.3.3/PyAibote/WebBotModel/KeymouseOperation.py
+-rw-rw-rw-   0        0        0     3993 2024-01-13 12:29:13.000000 PyAibote-1.3.3/PyAibote/WebBotModel/PagesAndNavigation.py
+-rw-rw-rw-   0        0        0     1091 2024-01-18 22:23:35.000000 PyAibote-1.3.3/PyAibote/WebBotModel/PopUpWindow.py
+-rw-rw-rw-   0        0        0     3133 2024-03-19 01:39:35.000000 PyAibote-1.3.3/PyAibote/WebBotModel/WebLoadWait.py
+-rw-rw-rw-   0        0        0     5606 2024-01-25 23:04:37.000000 PyAibote-1.3.3/PyAibote/WebBotModel/WindowOperation.py
+-rw-rw-rw-   0        0        0      654 2024-02-15 23:42:13.000000 PyAibote-1.3.3/PyAibote/WebBotModel/__init__.py
+-rw-rw-rw-   0        0        0     4186 2024-03-19 01:40:59.000000 PyAibote-1.3.3/PyAibote/WindowsBot.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:12:22.985869 PyAibote-1.3.3/PyAibote/WindowsBotModel/
+-rw-rw-rw-   0        0        0    20130 2024-03-28 05:07:36.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/ColorOperation.py
+-rw-rw-rw-   0        0        0    21461 2024-03-28 05:02:42.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/DigitalHumanOperation.py
+-rw-rw-rw-   0        0        0     1237 2024-03-22 13:46:05.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/DrivingOperation.py
+-rw-rw-rw-   0        0        0    14186 2024-01-18 22:29:18.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0     5207 2024-01-22 22:39:26.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/ExcelOperation.py
+-rw-rw-rw-   0        0        0     6629 2024-01-13 17:47:39.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/KeymouseOperation.py
+-rw-rw-rw-   0        0        0     8395 2024-03-19 01:39:35.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/OcrOperation.py
+-rw-rw-rw-   0        0        0      703 2024-01-15 07:27:07.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/OtherOperations.py
+-rw-rw-rw-   0        0        0     2379 2024-03-22 11:06:00.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/SystemOperation.py
+-rw-rw-rw-   0        0        0     5962 2024-01-22 23:03:02.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/VerificationCodeOperation.py
+-rw-rw-rw-   0        0        0     6402 2024-01-22 23:49:04.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/VoiceService.py
+-rw-rw-rw-   0        0        0     7513 2024-01-18 22:31:38.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/WinHidCorrelation.py
+-rw-rw-rw-   0        0        0     2124 2024-03-19 01:39:35.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/WinLoadWait.py
+-rw-rw-rw-   0        0        0     7160 2024-01-14 20:16:53.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/WindowOperation.py
+-rw-rw-rw-   0        0        0     2936 2024-01-14 20:29:30.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/YoloOperation.py
+-rw-rw-rw-   0        0        0     1115 2024-02-15 23:42:02.000000 PyAibote-1.3.3/PyAibote/WindowsBotModel/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-02-27 10:41:36.000000 PyAibote-1.3.3/PyAibote/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 11:12:22.516611 PyAibote-1.3.3/PyAibote.egg-info/
+-rw-rw-rw-   0        0        0     1089 2024-04-02 11:12:21.000000 PyAibote-1.3.3/PyAibote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2493 2024-04-02 11:12:21.000000 PyAibote-1.3.3/PyAibote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 11:12:21.000000 PyAibote-1.3.3/PyAibote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-02 11:12:21.000000 PyAibote-1.3.3/PyAibote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 11:12:21.000000 PyAibote-1.3.3/PyAibote.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8925 2024-03-19 02:24:43.000000 PyAibote-1.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-02 11:12:23.025863 PyAibote-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1425 2024-04-02 11:11:21.000000 PyAibote-1.3.3/setup.py
```

### Comparing `PyAibote-1.3.2/PKG-INFO` & `PyAibote-1.3.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAibote
-Version: 1.3.2
+Version: 1.3.3
 Summary: A pure code RPA office automation framework, which supports Android, Browser and Windows
 Home-page: https://www.pyaibote.com
 Author: Riven
 Author-email: pyaibote@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7,<4.0
```

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBot.py` & `PyAibote-1.3.3/PyAibote/AndroidBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBotModel/AndroidHidCorrelation.py` & `PyAibote-1.3.3/PyAibote/AndroidBotModel/AndroidHidCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBotModel/AndroidLoadWait.py` & `PyAibote-1.3.3/PyAibote/AndroidBotModel/AndroidLoadWait.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBotModel/ColorFindingOperation.py` & `PyAibote-1.3.3/PyAibote/AndroidBotModel/ColorFindingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBotModel/Control.py` & `PyAibote-1.3.3/PyAibote/AndroidBotModel/Control.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBotModel/CoordinateOperation.py` & `PyAibote-1.3.3/PyAibote/AndroidBotModel/CoordinateOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBotModel/ElementOperation.py` & `PyAibote-1.3.3/PyAibote/AndroidBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBotModel/EquipmentOperation.py` & `PyAibote-1.3.3/PyAibote/AndroidBotModel/EquipmentOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBotModel/FileTransfer.py` & `PyAibote-1.3.3/PyAibote/AndroidBotModel/FileTransfer.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBotModel/MapFindingOperation.py` & `PyAibote-1.3.3/PyAibote/AndroidBotModel/MapFindingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBotModel/OcrCorrelation.py` & `PyAibote-1.3.3/PyAibote/AndroidBotModel/OcrCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBotModel/ScreenProjectionOperation.py` & `PyAibote-1.3.3/PyAibote/AndroidBotModel/ScreenProjectionOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBotModel/ScreenshotOperation.py` & `PyAibote-1.3.3/PyAibote/AndroidBotModel/ScreenshotOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBotModel/VerificationCodeOperation.py` & `PyAibote-1.3.3/PyAibote/AndroidBotModel/VerificationCodeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBotModel/YoloService.py` & `PyAibote-1.3.3/PyAibote/AndroidBotModel/YoloService.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/AndroidBotModel/__init__.py` & `PyAibote-1.3.3/PyAibote/AndroidBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/CommonUse/ChatGenerative.py` & `PyAibote-1.3.3/PyAibote/CommonUse/ChatGenerative.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/Tool/DatabaseFunc.py` & `PyAibote-1.3.3/PyAibote/Tool/DatabaseFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/Tool/DebugStartDriver.py` & `PyAibote-1.3.3/PyAibote/Tool/DebugStartDriver.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/Tool/Logger.py` & `PyAibote-1.3.3/PyAibote/Tool/Logger.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/Tool/LoggerFunc.py` & `PyAibote-1.3.3/PyAibote/Tool/LoggerFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/Tool/SendTcpData.py` & `PyAibote-1.3.3/PyAibote/Tool/SendTcpData.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/Tool/SocketServer.py` & `PyAibote-1.3.3/PyAibote/Tool/SocketServer.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/Tool/Sqlite3DataBase.py` & `PyAibote-1.3.3/PyAibote/Tool/Sqlite3DataBase.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/Tool/UniversalFunction.py` & `PyAibote-1.3.3/PyAibote/Tool/UniversalFunction.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/Tool/WriteReadFileFunc.py` & `PyAibote-1.3.3/PyAibote/Tool/WriteReadFileFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/Tool/__init__.py` & `PyAibote-1.3.3/PyAibote/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WebBot.py` & `PyAibote-1.3.3/PyAibote/WebBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WebBotModel/CookiesOperation.py` & `PyAibote-1.3.3/PyAibote/WebBotModel/CookiesOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WebBotModel/ElementOperation.py` & `PyAibote-1.3.3/PyAibote/WebBotModel/ElementOperation.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,7 +281,24 @@
         if "/" in response:
             response = re.findall(r'/(.*)',response)[0]
         if response == "null":
             return None
         if path:
             self.SaveBase64Png(response,path)
         return response
+
+    def show_xpath(self) -> bool:
+        """
+            显示元素xpath路径，页面加载完毕再调用。
+            调用此函数后，可在页面移动鼠标会显示元素区域。移动并按下ctrl键，会在浏览器控制台打印相对xpath 和 绝对xpath路径
+            ifrmae 内的元素，需要先调用 switchFrame 切入进去，再调用showXpath函数
+
+            return: 总是True
+
+            Displays the xpath path of the element, and then calls it after the page is loaded.
+            After calling this function, you can move the mouse on the page to display the element area. 
+            Moving and pressing the ctrl key will print the relative xpath and absolute xpath paths on the browser console.
+            Elements in ifrmae need to be cut in by calling switchFrame first, and then calling the showXpath function.
+
+            return: always True
+        """
+        return "true" in self.SendData("showXpath")
```

### Comparing `PyAibote-1.3.2/PyAibote/WebBotModel/IframeOperation.py` & `PyAibote-1.3.3/PyAibote/WebBotModel/IframeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WebBotModel/JSinjection.py` & `PyAibote-1.3.3/PyAibote/WebBotModel/JSinjection.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WebBotModel/KeymouseOperation.py` & `PyAibote-1.3.3/PyAibote/WebBotModel/KeymouseOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WebBotModel/PagesAndNavigation.py` & `PyAibote-1.3.3/PyAibote/WebBotModel/PagesAndNavigation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WebBotModel/PopUpWindow.py` & `PyAibote-1.3.3/PyAibote/WebBotModel/PopUpWindow.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WebBotModel/WebLoadWait.py` & `PyAibote-1.3.3/PyAibote/WebBotModel/WebLoadWait.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WebBotModel/WindowOperation.py` & `PyAibote-1.3.3/PyAibote/WebBotModel/WindowOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WebBotModel/__init__.py` & `PyAibote-1.3.3/PyAibote/WebBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBot.py` & `PyAibote-1.3.3/PyAibote/WindowsBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/ColorOperation.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/ColorOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/DigitalHumanOperation.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/DigitalHumanOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/DrivingOperation.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/DrivingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/ElementOperation.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/ExcelOperation.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/ExcelOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/KeymouseOperation.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/KeymouseOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/OcrOperation.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/OcrOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/OtherOperations.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/OtherOperations.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/SystemOperation.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/SystemOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/VerificationCodeOperation.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/VerificationCodeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/VoiceService.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/VoiceService.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/WinHidCorrelation.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/WinHidCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/WinLoadWait.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/WinLoadWait.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/WindowOperation.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/WindowOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/YoloOperation.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/YoloOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote/WindowsBotModel/__init__.py` & `PyAibote-1.3.3/PyAibote/WindowsBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/PyAibote.egg-info/PKG-INFO` & `PyAibote-1.3.3/PyAibote.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAibote
-Version: 1.3.2
+Version: 1.3.3
 Summary: A pure code RPA office automation framework, which supports Android, Browser and Windows
 Home-page: https://www.pyaibote.com
 Author: Riven
 Author-email: pyaibote@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7,<4.0
```

### Comparing `PyAibote-1.3.2/PyAibote.egg-info/SOURCES.txt` & `PyAibote-1.3.3/PyAibote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/README.md` & `PyAibote-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `PyAibote-1.3.2/setup.py` & `PyAibote-1.3.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "Pillow",
     "requests",
     "pymysql"
 ]
 
 setup(
     name="PyAibote", 
-    version="1.3.2", 
+    version="1.3.3", 
     author="Riven", 
     author_email="pyaibote@163.com", 
     description="A pure code RPA office automation framework, which supports Android, Browser and Windows", 
     long_description="Support Android native APP and H5 interface elements and color positioning. The speed of element location is 10 times that of Appium framework, and the color location of 2340*1080 image only takes 50 milliseconds, It supports the positioning of window interface elements and colors developed by Windows applications,. NET, WinForm, WPF, QT, Java (GUI libraries such JAVA(Swing and AWT) and Electron. The exclusive xpath algorithm is concise and rapid, and the positioning speed of elements/colors is 3 times and 20 times that of visual RPA, respectively, All browsers and applications that support the chromium kernel. A web automation framework developed by C/C++ language based on browser kernel protocol. Ten times faster than Selenium", # 加载read_me的内容
     long_description_content_type="text/markdown", 
     url="https://www.pyaibote.com",  
     packages=packages,
```

