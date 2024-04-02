# Comparing `tmp/labda-0.0.2.tar.gz` & `tmp/labda-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labda-0.0.2.tar", max compression
+gzip compressed data, was "labda-0.0.3.tar", max compression
```

## Comparing `labda-0.0.2.tar` & `labda-0.0.3.tar`

### file list

```diff
@@ -1,46 +1,90 @@
--rw-r--r--   0        0        0      548 2024-02-26 06:53:37.641771 labda-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     1203 2024-03-28 15:13:08.428047 labda-0.0.2/README.md
--rw-r--r--   0        0        0       86 2024-03-25 14:51:25.319685 labda-0.0.2/labda/__init__.py
--rw-r--r--   0        0        0      142 2024-03-27 08:58:35.681407 labda-0.0.2/labda/assets/__init__.py
--rw-r--r--   0        0        0     1195 2024-03-27 08:58:35.681407 labda-0.0.2/labda/assets/counts_cut_points.py
--rw-r--r--   0        0        0      466 2024-03-27 18:30:04.051412 labda-0.0.2/labda/assets/transportation_cut_points.py
--rw-r--r--   0        0        0      152 2024-03-25 13:04:22.249679 labda-0.0.2/labda/expanders/__init__.py
--rw-r--r--   0        0        0      656 2024-03-25 12:56:11.749683 labda-0.0.2/labda/expanders/accelerometer.py
--rw-r--r--   0        0        0      964 2024-03-25 12:47:41.359679 labda-0.0.2/labda/expanders/extras.py
--rw-r--r--   0        0        0     7377 2024-03-27 11:47:33.751412 labda-0.0.2/labda/expanders/spatial.py
--rw-r--r--   0        0        0      141 2024-02-26 14:15:18.625593 labda-0.0.2/labda/parsers/__init__.py
--rw-r--r--   0        0        0     6959 2024-03-27 12:05:46.561411 labda-0.0.2/labda/parsers/actigraph.py
--rw-r--r--   0        0        0      802 2024-03-27 13:01:38.871410 labda-0.0.2/labda/parsers/bulk.py
--rw-r--r--   0        0        0     6765 2024-03-25 13:41:53.629684 labda-0.0.2/labda/parsers/gadgetbridge.py
--rw-r--r--   0        0        0     2332 2024-02-26 06:53:37.661771 labda-0.0.2/labda/parsers/garmin.py
--rw-r--r--   0        0        0    10229 2024-03-27 18:32:54.811412 labda-0.0.2/labda/parsers/qstarz.py
--rw-r--r--   0        0        0       36 2024-03-25 13:06:49.889686 labda-0.0.2/labda/processing/__init__.py
--rw-r--r--   0        0        0       88 2024-03-27 08:58:35.681407 labda-0.0.2/labda/processing/accelerometer/__init__.py
--rw-r--r--   0        0        0     1580 2024-03-27 08:58:35.681407 labda-0.0.2/labda/processing/accelerometer/activity_intensity.py
--rw-r--r--   0        0        0      616 2024-03-25 12:03:58.819683 labda-0.0.2/labda/processing/accelerometer/steps.py
--rw-r--r--   0        0        0      913 2024-03-25 13:41:13.789684 labda-0.0.2/labda/processing/accelerometer/wear.py
--rw-r--r--   0        0        0     2803 2024-03-25 10:54:02.059685 labda-0.0.2/labda/processing/bouts.py
--rw-r--r--   0        0        0      751 2024-03-25 13:06:44.719686 labda-0.0.2/labda/processing/domains.py
--rw-r--r--   0        0        0      488 2024-03-23 09:44:54.322376 labda-0.0.2/labda/processing/manipulations.py
--rw-r--r--   0        0        0      197 2024-03-27 08:58:35.681407 labda-0.0.2/labda/processing/spatial/__init__.py
--rw-r--r--   0        0        0     1216 2024-02-26 06:53:37.661771 labda-0.0.2/labda/processing/spatial/environment.py
--rw-r--r--   0        0        0     6041 2024-02-26 06:53:37.661771 labda-0.0.2/labda/processing/spatial/manipulations.py
--rw-r--r--   0        0        0     2820 2024-03-27 11:40:24.361414 labda-0.0.2/labda/processing/spatial/timeline.py
--rw-r--r--   0        0        0     2198 2024-03-27 11:40:29.191414 labda-0.0.2/labda/processing/spatial/transportation.py
--rw-r--r--   0        0        0    22427 2024-03-27 08:58:35.681407 labda-0.0.2/labda/processing/spatial/trips.py
--rw-r--r--   0        0        0     2247 2024-02-27 15:52:47.628900 labda-0.0.2/labda/processing/wear_validity.py
--rw-r--r--   0        0        0      250 2024-03-25 14:44:01.079682 labda-0.0.2/labda/structure/__init__.py
--rw-r--r--   0        0        0     3477 2024-03-27 18:33:12.341413 labda-0.0.2/labda/structure/collection.py
--rw-r--r--   0        0        0      704 2024-02-26 06:53:37.661771 labda-0.0.2/labda/structure/domains.py
--rw-r--r--   0        0        0      568 2024-02-26 06:53:37.661771 labda-0.0.2/labda/structure/linkage.py
--rw-r--r--   0        0        0     4470 2024-03-22 14:01:06.214976 labda-0.0.2/labda/structure/merging.py
--rw-r--r--   0        0        0     2771 2024-03-25 12:40:32.309681 labda-0.0.2/labda/structure/resampling.py
--rw-r--r--   0        0        0     8354 2024-03-27 11:05:01.611410 labda-0.0.2/labda/structure/subject.py
--rw-r--r--   0        0        0        0 2024-03-25 13:38:00.279684 labda-0.0.2/labda/structure/validation/__init__.py
--rw-r--r--   0        0        0      963 2024-02-26 06:53:37.661771 labda-0.0.2/labda/structure/validation/domains.py
--rw-r--r--   0        0        0      833 2024-02-26 06:53:37.661771 labda-0.0.2/labda/structure/validation/linkage.py
--rw-r--r--   0        0        0     9662 2024-03-25 14:32:26.579684 labda-0.0.2/labda/structure/validation/subject.py
--rw-r--r--   0        0        0     7515 2024-03-27 09:43:47.831414 labda-0.0.2/labda/utils.py
--rw-r--r--   0        0        0        0 2024-02-26 06:53:37.661771 labda-0.0.2/labda/visualisation/__init__.py
--rw-r--r--   0        0        0     1445 2024-03-28 15:18:34.238043 labda-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2501 1970-01-01 00:00:00.000000 labda-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      548 2024-02-06 17:52:16.166389 labda-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      570 2024-04-02 08:48:51.335892 labda-0.0.3/README.md
+-rw-r--r--   0        0        0      151 2024-04-02 08:48:51.335892 labda-0.0.3/labda/__init__.py
+-rw-r--r--   0        0        0      142 2024-03-26 12:17:08.741130 labda-0.0.3/labda/assets/__init__.py
+-rw-r--r--   0        0        0      329 2024-03-26 12:57:17.697713 labda-0.0.3/labda/assets/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1080 2024-04-02 08:49:41.505981 labda-0.0.3/labda/assets/__pycache__/counts_cut_points.cpython-311.pyc
+-rw-r--r--   0        0        0      630 2024-04-02 11:28:55.363245 labda-0.0.3/labda/assets/__pycache__/transportation_cut_points.cpython-311.pyc
+-rw-r--r--   0        0        0     1195 2024-03-26 15:39:19.404282 labda-0.0.3/labda/assets/counts_cut_points.py
+-rw-r--r--   0        0        0      459 2024-04-02 11:28:47.324035 labda-0.0.3/labda/assets/transportation_cut_points.py
+-rw-r--r--   0        0        0      152 2024-02-06 17:52:16.176389 labda-0.0.3/labda/expanders/__init__.py
+-rw-r--r--   0        0        0      432 2024-02-06 18:20:13.138435 labda-0.0.3/labda/expanders/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1351 2024-03-26 08:50:45.871038 labda-0.0.3/labda/expanders/__pycache__/accelerometer.cpython-311.pyc
+-rw-r--r--   0        0        0     1469 2024-03-26 08:50:44.271381 labda-0.0.3/labda/expanders/__pycache__/extras.cpython-311.pyc
+-rw-r--r--   0        0        0     9044 2024-04-02 08:49:41.475981 labda-0.0.3/labda/expanders/__pycache__/spatial.cpython-311.pyc
+-rw-r--r--   0        0        0      656 2024-03-26 07:45:27.272975 labda-0.0.3/labda/expanders/accelerometer.py
+-rw-r--r--   0        0        0      964 2024-03-26 07:45:27.272975 labda-0.0.3/labda/expanders/extras.py
+-rw-r--r--   0        0        0     7377 2024-04-02 08:48:51.335892 labda-0.0.3/labda/expanders/spatial.py
+-rw-r--r--   0        0        0     1140 2024-04-02 08:51:28.536242 labda-0.0.3/labda/logging.py
+-rw-r--r--   0        0        0     1073 2024-04-02 14:15:23.256237 labda-0.0.3/labda/parallel.py
+-rw-r--r--   0        0        0      141 2024-03-05 08:22:02.089665 labda-0.0.3/labda/parsers/__init__.py
+-rw-r--r--   0        0        0      394 2024-04-02 08:49:41.505981 labda-0.0.3/labda/parsers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    11178 2024-04-02 08:52:02.746325 labda-0.0.3/labda/parsers/__pycache__/actigraph.cpython-311.pyc
+-rw-r--r--   0        0        0     1802 2024-04-02 08:49:42.015982 labda-0.0.3/labda/parsers/__pycache__/bulk.cpython-311.pyc
+-rw-r--r--   0        0        0    10001 2024-04-02 08:49:41.505981 labda-0.0.3/labda/parsers/__pycache__/gadgetbridge.cpython-311.pyc
+-rw-r--r--   0        0        0    18382 2024-04-02 10:22:16.092741 labda-0.0.3/labda/parsers/__pycache__/qstarz.cpython-311.pyc
+-rw-r--r--   0        0        0     2120 2024-04-02 10:56:34.978296 labda-0.0.3/labda/parsers/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0      617 2024-02-06 18:20:13.168428 labda-0.0.3/labda/parsers/__pycache__/vendors.cpython-311.pyc
+-rw-r--r--   0        0        0     6854 2024-04-02 08:51:54.456305 labda-0.0.3/labda/parsers/actigraph.py
+-rw-r--r--   0        0        0      930 2024-04-02 08:48:51.335892 labda-0.0.3/labda/parsers/bulk.py
+-rw-r--r--   0        0        0     6765 2024-03-26 07:45:27.282975 labda-0.0.3/labda/parsers/gadgetbridge.py
+-rw-r--r--   0        0        0     2332 2024-02-06 17:52:16.176389 labda-0.0.3/labda/parsers/garmin.py
+-rw-r--r--   0        0        0    10772 2024-04-02 10:20:55.340245 labda-0.0.3/labda/parsers/qstarz.py
+-rw-r--r--   0        0        0     1157 2024-04-02 10:31:20.628801 labda-0.0.3/labda/parsers/utils.py
+-rw-r--r--   0        0        0       36 2024-02-09 10:52:49.204568 labda-0.0.3/labda/processing/__init__.py
+-rw-r--r--   0        0        0      224 2024-02-09 10:55:00.040194 labda-0.0.3/labda/processing/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3222 2024-03-26 08:50:45.871038 labda-0.0.3/labda/processing/__pycache__/bouts.cpython-311.pyc
+-rw-r--r--   0        0        0     1222 2024-03-26 08:50:45.871038 labda-0.0.3/labda/processing/__pycache__/domains.cpython-311.pyc
+-rw-r--r--   0        0        0     1302 2024-03-26 08:50:45.881036 labda-0.0.3/labda/processing/__pycache__/manipulations.cpython-311.pyc
+-rw-r--r--   0        0        0       88 2024-03-26 13:31:05.536930 labda-0.0.3/labda/processing/accelerometer/__init__.py
+-rw-r--r--   0        0        0      316 2024-03-26 14:32:40.821163 labda-0.0.3/labda/processing/accelerometer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2770 2024-03-26 14:32:40.821163 labda-0.0.3/labda/processing/accelerometer/__pycache__/activity_intensity.cpython-311.pyc
+-rw-r--r--   0        0        0     2754 2024-03-26 08:50:45.871038 labda-0.0.3/labda/processing/accelerometer/__pycache__/cut_points.cpython-311.pyc
+-rw-r--r--   0        0        0     1282 2024-02-09 11:45:26.255590 labda-0.0.3/labda/processing/accelerometer/__pycache__/steps.cpython-311.pyc
+-rw-r--r--   0        0        0     1411 2024-03-26 08:50:45.871038 labda-0.0.3/labda/processing/accelerometer/__pycache__/wear.cpython-311.pyc
+-rw-r--r--   0        0        0     1580 2024-03-26 13:51:21.538869 labda-0.0.3/labda/processing/accelerometer/activity_intensity.py
+-rw-r--r--   0        0        0      616 2024-03-26 07:45:27.282975 labda-0.0.3/labda/processing/accelerometer/steps.py
+-rw-r--r--   0        0        0      913 2024-03-26 07:45:27.282975 labda-0.0.3/labda/processing/accelerometer/wear.py
+-rw-r--r--   0        0        0     2803 2024-03-26 07:45:27.282975 labda-0.0.3/labda/processing/bouts.py
+-rw-r--r--   0        0        0      751 2024-03-26 07:45:27.282975 labda-0.0.3/labda/processing/domains.py
+-rw-r--r--   0        0        0      488 2024-03-26 07:45:27.282975 labda-0.0.3/labda/processing/manipulations.py
+-rw-r--r--   0        0        0      197 2024-03-26 14:28:15.353873 labda-0.0.3/labda/processing/spatial/__init__.py
+-rw-r--r--   0        0        0      501 2024-03-26 14:32:40.821163 labda-0.0.3/labda/processing/spatial/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7768 2024-04-02 09:40:11.576062 labda-0.0.3/labda/processing/spatial/__pycache__/manipulations.cpython-311.pyc
+-rw-r--r--   0        0        0     5145 2024-04-02 12:07:44.826996 labda-0.0.3/labda/processing/spatial/__pycache__/timeline.cpython-311.pyc
+-rw-r--r--   0        0        0     4487 2024-04-02 08:49:41.485981 labda-0.0.3/labda/processing/spatial/__pycache__/transportation.cpython-311.pyc
+-rw-r--r--   0        0        0    27515 2024-04-02 13:47:45.136539 labda-0.0.3/labda/processing/spatial/__pycache__/trips.cpython-311.pyc
+-rw-r--r--   0        0        0     6142 2024-04-02 09:39:10.496322 labda-0.0.3/labda/processing/spatial/manipulations.py
+-rw-r--r--   0        0        0     3061 2024-04-02 12:07:23.697246 labda-0.0.3/labda/processing/spatial/timeline.py
+-rw-r--r--   0        0        0     2198 2024-04-02 08:48:51.335892 labda-0.0.3/labda/processing/spatial/transportation.py
+-rw-r--r--   0        0        0    24216 2024-04-02 13:46:22.410849 labda-0.0.3/labda/processing/spatial/trips.py
+-rw-r--r--   0        0        0     2247 2024-03-05 08:22:02.089665 labda-0.0.3/labda/processing/wear_validity.py
+-rw-r--r--   0        0        0      250 2024-03-12 09:04:33.383063 labda-0.0.3/labda/structure/__init__.py
+-rw-r--r--   0        0        0      621 2024-03-26 08:50:43.151621 labda-0.0.3/labda/structure/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8409 2024-04-02 13:59:02.487227 labda-0.0.3/labda/structure/__pycache__/collection.cpython-311.pyc
+-rw-r--r--   0        0        0     1158 2024-02-09 12:27:22.799138 labda-0.0.3/labda/structure/__pycache__/domains.cpython-311.pyc
+-rw-r--r--   0        0        0     1186 2024-02-09 12:27:23.249118 labda-0.0.3/labda/structure/__pycache__/linkage.cpython-311.pyc
+-rw-r--r--   0        0        0     6562 2024-04-02 08:49:41.495981 labda-0.0.3/labda/structure/__pycache__/merging.cpython-311.pyc
+-rw-r--r--   0        0        0     3595 2024-03-26 08:50:45.881036 labda-0.0.3/labda/structure/__pycache__/resampling.cpython-311.pyc
+-rw-r--r--   0        0        0    14577 2024-04-02 13:47:44.916549 labda-0.0.3/labda/structure/__pycache__/subject.cpython-311.pyc
+-rw-r--r--   0        0        0     4586 2024-04-02 13:58:21.046661 labda-0.0.3/labda/structure/collection.py
+-rw-r--r--   0        0        0      704 2024-02-09 12:27:12.019606 labda-0.0.3/labda/structure/domains.py
+-rw-r--r--   0        0        0      568 2024-02-09 12:27:12.019606 labda-0.0.3/labda/structure/linkage.py
+-rw-r--r--   0        0        0     5000 2024-04-02 08:48:51.335892 labda-0.0.3/labda/structure/merging.py
+-rw-r--r--   0        0        0     2771 2024-03-26 07:45:27.282975 labda-0.0.3/labda/structure/resampling.py
+-rw-r--r--   0        0        0     9043 2024-04-02 13:46:05.711935 labda-0.0.3/labda/structure/subject.py
+-rw-r--r--   0        0        0        0 2024-03-26 07:45:27.282975 labda-0.0.3/labda/structure/validation/__init__.py
+-rw-r--r--   0        0        0      174 2024-03-26 08:50:43.151621 labda-0.0.3/labda/structure/validation/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      912 2024-02-09 12:27:22.809137 labda-0.0.3/labda/structure/validation/__pycache__/domains.cpython-311.pyc
+-rw-r--r--   0        0        0      840 2024-02-09 20:01:56.329810 labda-0.0.3/labda/structure/validation/__pycache__/linkage.cpython-311.pyc
+-rw-r--r--   0        0        0     8243 2024-04-02 11:44:31.779533 labda-0.0.3/labda/structure/validation/__pycache__/subject.cpython-311.pyc
+-rw-r--r--   0        0        0      963 2024-02-09 12:27:12.019606 labda-0.0.3/labda/structure/validation/domains.py
+-rw-r--r--   0        0        0      833 2024-02-09 12:37:10.070190 labda-0.0.3/labda/structure/validation/linkage.py
+-rw-r--r--   0        0        0     9704 2024-04-02 11:44:21.091638 labda-0.0.3/labda/structure/validation/subject.py
+-rw-r--r--   0        0        0     8338 2024-04-02 08:48:51.335892 labda-0.0.3/labda/utils.py
+-rw-r--r--   0        0        0        0 2024-02-06 17:52:16.176389 labda-0.0.3/labda/visualisation/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-02 13:25:04.160019 labda-0.0.3/labda/visualisation/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3643 2024-04-02 14:25:41.270154 labda-0.0.3/labda/visualisation/__pycache__/spatial.cpython-311.pyc
+-rw-r--r--   0        0        0     2510 2024-04-02 14:25:35.290436 labda-0.0.3/labda/visualisation/spatial.py
+-rw-r--r--   0        0        0     1434 2024-04-02 14:29:13.641929 labda-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 labda-0.0.3/PKG-INFO
```

### Comparing `labda-0.0.2/CHANGELOG.md` & `labda-0.0.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/assets/counts_cut_points.py` & `labda-0.0.3/labda/assets/counts_cut_points.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/expanders/accelerometer.py` & `labda-0.0.3/labda/expanders/accelerometer.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/expanders/extras.py` & `labda-0.0.3/labda/expanders/extras.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/expanders/spatial.py` & `labda-0.0.3/labda/expanders/spatial.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/parsers/actigraph.py` & `labda-0.0.3/labda/parsers/actigraph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,28 @@
 from datetime import datetime
 from pathlib import Path
-from typing import Any
+from typing import Any, Tuple
 
 import pandas as pd
 from dateutil.parser import parse as parse_dt
 
+from ..logging import success_parsing_log
 from ..structure.subject import Metadata, Sensor, Subject, Vendor
 from ..structure.validation.subject import SCHEMA, Column
-from ..utils import get_sampling_frequency
+from ..utils import (
+    align_datetimes,
+    filter_datetime,
+    get_sampling_frequency,
+)
+from .utils import set_timezone
 
 # TODO: Add param for column mapping if there is no header.
 # TODO: It is not perfect, but it is a start and it should be able to parse automatically almost all ActiGraph files from SDU.
 
 
-def filter_datetime(
-    df: pd.DataFrame,
-    start: datetime | None = None,
-    end: datetime | None = None,
-) -> pd.DataFrame:
-    if start and end:
-        if end < start:
-            raise ValueError("The end time must be after the start time.")
-
-    if start:
-        df = df[df[Column.DATETIME] >= start]
-
-    if end:
-        df = df[df[Column.DATETIME] <= end]
-
-    return df
-
-
 def get_metadata(metadata: list[str]) -> dict[str, Any]:
     model = metadata[0].split("ActiGraph")[-1].split()[0].strip()
     firmware = metadata[0].split("Firmware")[-1].split()[0].strip()
     serial_number = metadata[1].split()[-1].strip()
     start_time = metadata[2].split()[-1].strip()
     start_date = metadata[3].split()[-1].strip()
     start_datetime = parse_dt(start_date + " " + start_time)
@@ -133,23 +121,23 @@
 
 def from_csv(
     path: str | Path,
     line: int = 10,
     metadata: bool = True,
     *,
     subject_id: str | None = None,
-    sensor_id: str | None = None,
+    sensor_id: str | None = None,  # type: ignore
     serial_number: str | None = None,
     model: str | None = None,
     vendor: Vendor = Vendor.ACTIGRAPH,
     firmware_version: str | None = None,
     start: datetime | None = None,
     end: datetime | None = None,
-    timezone: str | None = None,
-    dt_format: str | None = None,
+    timezone: str | None | Tuple[str, str] = None,
+    datetime_format: str | None = None,
 ) -> Subject:
     if isinstance(path, str):
         path = Path(path)
 
     if not path.is_file():
         raise ValueError(f"Invalid file path: {path}")
 
@@ -179,25 +167,26 @@
         df = df.iloc[:, :3]
         df.columns = [
             Column.VERTICAL_COUNTS,
             Column.HORIZONTAL_COUNTS,
             Column.PERPENDICULAR_COUNTS,
         ]
 
-    df = handle_datetime(df, parsed_metadata, dt_format)
-    df = filter_datetime(df, start, end)
+    df = handle_datetime(df, parsed_metadata, datetime_format)
 
     df.set_index(Column.DATETIME, inplace=True)
-    sampling_frequency = parsed_metadata.get("sampling_frequency")
+    df, timezone = set_timezone(df, timezone)
 
-    df.dropna(how="all", inplace=True)
+    df = filter_datetime(df, start, end)
 
+    sampling_frequency = parsed_metadata.get("sampling_frequency")
     if not sampling_frequency:
         sampling_frequency = get_sampling_frequency(df)
-    df = df.resample(f"{sampling_frequency}s").nearest()
+
+    df = align_datetimes(df, sampling_frequency)
 
     columns = [col.value for col in Column]
     ordered_columns = [col for col in columns if col in df.columns]
     df = df[ordered_columns]
 
     df = SCHEMA.validate(df)
 
@@ -225,8 +214,13 @@
     metadata = Metadata(
         id=subject_id,
         sensor=[sensor],
         sampling_frequency=sampling_frequency,
         timezone=timezone,
     )  # type: ignore
 
-    return Subject(metadata=metadata, df=df)  # type: ignore
+    subject = Subject(metadata=metadata, df=df)  # type: ignore
+
+    func = f"{__name__}:from_csv"
+    success_parsing_log(subject, path, func)
+
+    return subject
```

### Comparing `labda-0.0.2/labda/parsers/bulk.py` & `labda-0.0.3/labda/parsers/bulk.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 from pathlib import Path
 from typing import Callable
 
-from labda.structure import Collection
+from ..parallel import parallel_processing, process_obj
+from ..structure import Collection
 
 # TODO: Add bulk parsing with linkage file
-# TODO: Add parallel processing of files.
 
 
-def bulk_parser(folder: str | Path, parser: Callable, id: str | None = None, **kwargs):
+def bulk_parser(
+    folder: str | Path,
+    parser: Callable,
+    id: str | None = None,
+    parallel: bool = True,
+    n_cores: int | str = "max",
+    **kwargs,
+):
     if isinstance(folder, str):
         folder = Path(folder)
 
     if not folder.is_dir():
         raise ValueError(f"'{folder}' is not a valid folder.")
 
     files = list(Path(folder).glob("*"))
 
     if id is None:
         id = folder.name
 
-    collection = Collection(id=id)
+    if parallel:
+        results = parallel_processing(parser, files, n_cores, **kwargs)
+    else:
+        results = [process_obj(file, parser, **kwargs) for file in files]
 
-    for file in files:
-        try:
-            subject = parser(file, **kwargs)
-            collection.add_subject(subject)
-        except Exception as e:
-            print(f"Error while parsing | {file} | {e}")  # TODO: Log error
+    # Remove None values from results
+    results = list(filter(None, results))
+
+    collection = Collection(id=id, subjects=results)
 
     return collection
```

### Comparing `labda-0.0.2/labda/parsers/gadgetbridge.py` & `labda-0.0.3/labda/parsers/gadgetbridge.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/parsers/garmin.py` & `labda-0.0.3/labda/parsers/garmin.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/parsers/qstarz.py` & `labda-0.0.3/labda/parsers/qstarz.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,50 @@
 from datetime import datetime
 from pathlib import Path
+from typing import Tuple
 
+import numpy as np
 import pandas as pd
 
+from ..logging import success_parsing_log
 from ..structure.subject import Metadata, Sensor, Subject, Vendor
 from ..structure.validation.subject import SCHEMA, Column
 from ..utils import (
     align_datetimes,
     columns_exists,
-    convert_to_dataframe,
-    convert_to_geodataframe,
-    get_crs,
+    filter_datetime,
     get_sampling_frequency,
-    get_timezone,
 )
+from .utils import set_crs, set_timezone
 
 # TODO: Can be refactored.,
-# TODO: Remove all spaces from the column names, so there is no need to check if there is space or not.
+
+
+def detect_environment_from_gps_signal(
+    df: pd.DataFrame,
+    method: str,
+    limit: int | float,
+) -> pd.DataFrame:
+    df = df.copy()
+
+    methods = [
+        Column.SNR_VIEWED,  # 260
+        Column.NSAT_RATIO,  # 70
+    ]
+    if method not in methods:
+        raise ValueError(f"Method muset be one of {methods}")
+
+    if method not in df.columns:
+        raise ValueError(f"Column '{method}' does not exist in dataframe")
+
+    mask = df[method].notna()
+    df.loc[mask, Column.ENVIRONMENT] = "outdoor"
+    df.loc[mask & (df[method] <= limit), Column.ENVIRONMENT] = "indoor"
+
+    return df
 
 
 def parse_snr(df: pd.DataFrame) -> pd.DataFrame:
     df = df.copy()
 
     sat_info_4 = "SAT INFO (SID-ELE-AZI-SNR)"
     sat_info_2 = "SAT INFO (SID-SNR)"
@@ -158,45 +182,18 @@
         df[column] = df[column].str.strip("M")
     df[column] = pd.to_numeric(df[column])
     df[column] = df[column].round(2)
     df.rename(columns={column: Column.ELEVATION}, inplace=True)
     return df
 
 
-def filter_datetime(
-    df: pd.DataFrame,
-    start: datetime | None = None,
-    end: datetime | None = None,
-) -> pd.DataFrame:
-    if start and end:
-        if end < start:
-            raise ValueError("The end time must be after the start time.")
-
-    if start:
-        df = df[df[Column.DATETIME] >= start]
-
-    if end:
-        df = df[df[Column.DATETIME] <= end]
-
-    return df
-
-
-def handle_crs(df: pd.DataFrame, crs: str) -> pd.DataFrame:
-    gdf = convert_to_geodataframe(df, crs="WGS84")
-    gdf.to_crs(crs, inplace=True)
-    df = convert_to_dataframe(gdf)
-
-    return df
-
-
 def parse_datetime(df: pd.DataFrame, dt_format: str | None = None) -> pd.DataFrame:
     df = df.copy()
     column = None
 
-    # FIXME: Fix this...
     if "DATE" in df.columns and "TIME" in df.columns:
         date = "DATE"
         time = "TIME"
     elif "LOCAL DATE" in df.columns and "LOCAL TIME" in df.columns:
         date = "LOCAL DATE"
         time = "LOCAL TIME"
     elif "LOCAL TIME" in df.columns:
@@ -224,16 +221,23 @@
         columns={"LATITUDE": Column.LATITUDE, "LONGITUDE": Column.LONGITUDE},
         inplace=True,
     )
     df[[Column.LATITUDE, Column.LONGITUDE]] = df[
         [Column.LATITUDE, Column.LONGITUDE]
     ].apply(pd.to_numeric)
 
-    df.loc[df["N/S"] == "S", Column.LATITUDE] = -df[Column.LATITUDE]
-    df.loc[df["E/W"] == "W", Column.LONGITUDE] = -df[Column.LONGITUDE]
+    df["N/S"] = df["N/S"].str.strip()
+    df[Column.LATITUDE] = np.where(
+        df["N/S"] == "S", -df[Column.LATITUDE], df[Column.LATITUDE]
+    )
+
+    df["E/W"] = df["E/W"].str.strip()
+    df[Column.LONGITUDE] = np.where(
+        df["E/W"] == "W", -df[Column.LONGITUDE], df[Column.LONGITUDE]
+    )
 
     return df
 
 
 def drop_empty_columns(df: pd.DataFrame) -> None:
     """
     Drops the columns with empty names from the DataFrame.
@@ -275,17 +279,19 @@
     serial_number: str | None = None,
     model: str | None = None,
     vendor: Vendor = Vendor.QSTARZ,
     firmware_version: str | None = None,
     start: datetime | None = None,
     end: datetime | None = None,
     sampling_frequency: float | None = None,
-    crs: str | None = None,
-    timezone: str | None = None,
-    dt_format: str | None = None,
+    crs: str | None | Tuple[str, str] = None,
+    timezone: str | None | Tuple[str, str] = None,
+    datetime_format: str | None = None,
+    nsat_ratio: float = 70,
+    snr_viewed: int = 260,
 ) -> Subject:
     if isinstance(path, str):
         path = Path(path)
 
     if not path.is_file():
         raise ValueError(f"Invalid file path: {path}")
 
@@ -295,46 +301,46 @@
     df = pd.read_csv(path, engine="pyarrow")
     drop_empty_columns(df)
     df.columns = df.columns.str.strip()
 
     remove_repeated_headers(df)
 
     df = parse_coordinates(df)
-    df = parse_datetime(df, dt_format)
-
-    if not crs:
-        crs = get_crs(df)
-
-    df = handle_crs(df, crs)
-
-    if not timezone:
-        timezone = get_timezone(df)
+    df = parse_datetime(df, datetime_format)
 
     df.drop_duplicates(
         subset=[Column.DATETIME], inplace=True
     )  # If there are duplicates, keep only the first one - because later with resample, datetime needs to be unique.
 
     # Remove rows with "Estimated (dead reckoning)" in the "VALID" column.
     if "VALID" in df.columns:
         df = df[~(df["VALID"] == "Estimated (dead reckoning)")]
 
-    df = filter_datetime(df, start, end)
     df = parse_distance(df)
     df = parse_speed(df)
     df = parse_elevation(df)
     df = parse_dop(df)
     df = parse_nsat(df)
     df = parse_snr(df)
 
     if Column.NSAT_USED in df.columns and Column.NSAT_VIEWED in df.columns:
         df[Column.NSAT_RATIO] = (
             (df[Column.NSAT_USED] * 100) / df[Column.NSAT_VIEWED]
         ).round(2)
 
+    if Column.SNR_VIEWED in df.columns and snr_viewed:
+        df = detect_environment_from_gps_signal(df, Column.SNR_VIEWED, snr_viewed)
+    elif Column.NSAT_RATIO in df.columns and nsat_ratio:
+        df = detect_environment_from_gps_signal(df, Column.NSAT_RATIO, nsat_ratio)
+
     df.set_index(Column.DATETIME, inplace=True)
+    df, timezone = set_timezone(df, timezone)
+    df, crs = set_crs(df, crs)
+
+    df = filter_datetime(df, start, end)
 
     if not sampling_frequency:
         sampling_frequency = get_sampling_frequency(df)
 
     df = align_datetimes(df, sampling_frequency)
 
     # Order columns as defined in Column, remove extra columns
@@ -359,8 +365,13 @@
         id=subject_id,
         sensor=[sensor],
         sampling_frequency=sampling_frequency,
         crs=crs,
         timezone=timezone,
     )
 
-    return Subject(metadata=metadata, df=df)
+    subject = Subject(metadata=metadata, df=df)
+
+    func = f"{__name__}:from_csv"
+    success_parsing_log(subject, path, func)
+
+    return subject
```

### Comparing `labda-0.0.2/labda/processing/accelerometer/activity_intensity.py` & `labda-0.0.3/labda/processing/accelerometer/activity_intensity.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/processing/accelerometer/steps.py` & `labda-0.0.3/labda/processing/accelerometer/steps.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/processing/accelerometer/wear.py` & `labda-0.0.3/labda/processing/accelerometer/wear.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/processing/bouts.py` & `labda-0.0.3/labda/processing/bouts.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/processing/domains.py` & `labda-0.0.3/labda/processing/domains.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/processing/spatial/manipulations.py` & `labda-0.0.3/labda/processing/spatial/manipulations.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
     Raises:
         ValueError: If the specified column name already exists in the DataFrame and overwrite is set to False.
     """
 
     columns_not_exists(df, [name], overwrite=overwrite)
 
+    # TODO: How to handle NA values, maybe just filter to have only valid points (with coordinates).
     df = df.copy()
     df[name] = False
 
     gdf = convert_to_geodataframe(df, crs=crs)
     if gdf.crs is None:
         crs = get_crs(gdf)
         gdf = gdf.set_crs(crs)
```

### Comparing `labda-0.0.2/labda/processing/spatial/timeline.py` & `labda-0.0.3/labda/processing/spatial/timeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 def get_information(df: pd.DataFrame, crs: str) -> pd.Series:
     df = df.copy()
     start = df.index.min()
     end = df.index.max()
     duration = end - start
+    segment_id = df["segment_id"].iloc[0]
 
     distance_col = get_unique_column_name(df)
     df = add_distance(df, crs=crs, name=distance_col)
     distance = df[distance_col].sum()
 
     gdf = convert_to_geodataframe(df[[Column.LATITUDE, Column.LONGITUDE]], crs=crs)
     geometry = gdf["geometry"]
@@ -24,15 +25,19 @@
         trip_id = df[Column.TRIP_ID].iloc[0]
         if df["stationary_id"].notna().all():
             status = "pause"
             mode = pd.NA
             location_id = df["stationary_id"].iloc[0]
         else:
             status = "transport"
-            mode = df["trip_mode"].iloc[0]
+
+            if Column.TRIP_MODE in df.columns:
+                mode = df[Column.TRIP_MODE].iloc[0]
+            else:
+                mode = pd.NA
             location_id = pd.NA
     else:
         status = "stationary"
         trip_id = pd.NA
         mode = pd.NA
         location_id = df["stationary_id"].iloc[0]
 
@@ -40,14 +45,15 @@
         geometry = LineString(geometry.tolist())  # type: ignore
 
     else:
         geometry = geometry.unary_union  # type: ignore
 
     return pd.Series(
         {
+            "segment_id": segment_id,
             "trip_id": trip_id,
             "stationary_id": location_id,
             "start": start,
             "end": end,
             "duration": duration,
             "distance": distance,
             "status": status,
@@ -83,15 +89,19 @@
         .reset_index(drop=True)
     )
 
     stops = df.groupby("stationary_id", as_index=False).apply(
         lambda x: get_information(x, crs=crs)
     )
 
-    summary = pd.concat([trips, stops], ignore_index=True).sort_values(["start", "end"])
+    summary = (
+        pd.concat([trips, stops], ignore_index=True)
+        .sort_values(["start", "end"])
+        .reset_index(drop=True)
+    )
 
     return summary.astype(
         {
             "status": "category",
             "mode": "category",
             "trip_id": "UInt16",
             "stationary_id": "UInt16",
```

### Comparing `labda-0.0.2/labda/processing/spatial/transportation.py` & `labda-0.0.3/labda/processing/spatial/transportation.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/processing/spatial/trips.py` & `labda-0.0.3/labda/processing/spatial/trips.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 from datetime import timedelta
+from operator import ge
+from xml import dom
 
 import numpy as np
 import pandas as pd
+from requests import get
 
 from ...expanders import add_distance
 from ...structure.validation.subject import SCHEMA
-from ...utils import columns_exists, columns_not_exists, convert_distance_parameter
+from ...utils import (
+    columns_exists,
+    columns_not_exists,
+    convert_distance_parameter,
+    get_unique_column_name,
+)
 from ..manipulations import gap_splitter
 from .manipulations import max_speed_filter, min_distance_filter, stop_splitter
 
 # TODO: Fix docstring.
 # TODO: Test params.
 # TODO: Change column names to constants (Column).
 
@@ -33,15 +41,20 @@
         max_radius (int | float): The maximum radius to use when splitting stops.
         stop_duration (timedelta): The minimum duration to consider a stop.
 
     Returns:
         pd.DataFrame: The processed DataFrame with added 'stop_id' and 'trip_status' columns.
     """
     # Returns a new DataFrame with a 'stop' column.
-    df = stop_splitter(df, max_radius=stop_radius, min_duration=stop_duration, crs=crs)
+    df = stop_splitter(
+        df,
+        max_radius=stop_radius,
+        min_duration=stop_duration,
+        crs=crs,
+    )
 
     # Unique ID for each stop.
     df["stop_id"] = (df["stop"].diff() != 0).cumsum()
 
     # Set the trip status to 'stationary' if the point is a stop, otherwise 'transport'.
     df["trip_status"] = np.where(df["stop"], "stationary", "transport")
 
@@ -240,29 +253,14 @@
     # Use cumsum to generate the ID
     df[id_column] = mask.cumsum().astype("UInt16")
 
     # Set ID to NA for rows that don't match any of the target values
     df.loc[~df[column].isin(target_values), id_column] = pd.NA
 
 
-def get_distance(df: pd.DataFrame, crs: str) -> float:
-    """
-    Calculates the total distance traveled in a DataFrame.
-
-    Args:
-        df (pd.DataFrame): The DataFrame containing the trip data.
-        crs (str): The coordinate reference system of the data.
-
-    Returns:
-        float: The total distance traveled, rounded to 2 decimal places.
-    """
-    df = add_distance(df, crs=crs)
-    return df["distance"].sum().round(2)
-
-
 def remove_trips_by_duration(df: pd.DataFrame, min_duration: timedelta) -> None:
     """
     Removes trips from the DataFrame that are shorter than a specified minimum duration.
 
     Args:
         df (pd.DataFrame): The DataFrame containing the trips.
         min_duration (timedelta): The minimum duration for a trip to be kept in the DataFrame.
@@ -308,15 +306,15 @@
     Returns:
         None: The function modifies the DataFrame in-place, and does not return anything.
     """
     # Select only the rows that are part of a trip.
     trips = df[
         df["trip_id"].notna()
         & df["trip_status"].isin(["start", "transport", "end", "start-end"])
-    ].copy()
+    ][["segment_id", "trip_id", "latitude", "longitude"]].copy()
 
     # Calculate the distance traveled for each trip.
     trips = trips.groupby(["segment_id", "trip_id"], as_index=False).apply(
         lambda x: add_distance(x, crs=crs)["distance"].sum()
     )
     trips.rename(columns={None: "length"}, inplace=True)  # type: ignore
 
@@ -331,14 +329,55 @@
     # df.loc[mask, "trip_status"] = (
     #     pd.NA  # HACK: Possibly set this to "stationary" if removed trips should be part of locations, but then need to adjust the stationary_id as well.
     # )
     df.loc[mask, "trip_status"] = "stationary"
     df.loc[mask, "stationary_id"] = df.loc[mask, "stationary_id"].ffill()
 
 
+def _change_indoor_trip_to_stationary(df: pd.DataFrame, limit: float) -> str | None:
+    environment = df["environment"].value_counts()
+    dominant_environment = environment.idxmax()
+
+    if len(environment) >= 2 and dominant_environment == "indoor" and limit:
+        total_values = environment.sum()
+        dominant_values = environment[dominant_environment]
+
+        if (dominant_values / total_values * 100) <= limit:
+            return None
+
+    return dominant_environment  # type: ignore
+
+
+def remove_indoor_trips(df: pd.DataFrame, indoor_limit: float):
+    # Select only the rows that are part of a trip.
+    trips = df[
+        df["trip_id"].notna()
+        & df["trip_status"].isin(["start", "transport", "end", "start-end"])
+    ].copy()
+
+    trips = trips.groupby(["segment_id", "trip_id"], as_index=False).apply(
+        lambda x: _change_indoor_trip_to_stationary(x, indoor_limit)  # type: ignore
+    )
+    trips.rename(columns={None: "environment"}, inplace=True)  # type: ignore
+    trips = trips.astype({"environment": "category"})
+
+    removed_trips = trips[trips["environment"] == "indoor"][["segment_id", "trip_id"]]
+
+    # Change rows based on both segment_id and trip_id and set the trip_id and trip_status to NA.
+    mask = df.set_index(["segment_id", "trip_id"]).index.isin(
+        removed_trips.set_index(["segment_id", "trip_id"]).index
+    )
+    df.loc[mask, "trip_id"] = pd.NA
+    # df.loc[mask, "trip_status"] = (
+    #     pd.NA  # HACK: Possibly set this to "stationary" if removed trips should be part of locations, but then need to adjust the stationary_id as well.
+    # )
+    df.loc[mask, "trip_status"] = "stationary"
+    df.loc[mask, "stationary_id"] = df.loc[mask, "stationary_id"].bfill()
+
+
 def get_segment_trips(
     df: pd.DataFrame,
     crs: str,
     sampling_frequency: float,
     stop_radius: int | float,
     stop_duration: timedelta,
     pause_radius: int | float | None = None,
@@ -439,14 +478,15 @@
     stop_duration: timedelta,
     pause_radius: int | float | None = None,
     pause_duration: timedelta | None = None,
     min_duration: timedelta | None = None,
     min_length: int | float | None = None,
     min_distance: int | float | None = None,
     max_speed: int | float | None = None,
+    indoor_limit: float | None = None,
     overwrite: bool = False,
 ) -> pd.DataFrame:
     """
     Detects trips in the given DataFrame based on various parameters.
 
     This function applies several filters to the DataFrame, including a minimum length filter, a minimum distance filter, and a maximum speed filter.
     It then identifies and labels trips based on the given maximum radius, stop duration, and pause duration.
@@ -471,28 +511,35 @@
 
     columns_not_exists(
         df,
         ["segment_id", "trip_id", "trip_status", "stationary_id"],
         overwrite=overwrite,
     )
 
-    # Keep a copy of the original DataFrame.
-    temp_df = df.copy()
+    working_cols = ["latitude", "longitude"]
 
     # Get the segments from the DataFrame.
     segments = gap_splitter(
-        temp_df[["latitude", "longitude"]], name="segment_id", min_duration=gap_duration
+        df[working_cols],
+        name="segment_id",
+        min_duration=gap_duration,
+        overwrite=overwrite,
     )
     df = df.join(
         segments[["segment_id"]],
         how="left",
     )
 
+    working_cols.append("segment_id")
+    if "environment" in df.columns:
+        working_cols.append("environment")
+
     temp_df = (
-        segments.groupby("segment_id")
+        df[working_cols]
+        .groupby("segment_id")
         .apply(
             lambda x: get_segment_trips(
                 x,
                 crs=crs,
                 sampling_frequency=sampling_frequency,
                 stop_radius=stop_radius,
                 stop_duration=stop_duration,
@@ -509,14 +556,17 @@
     if min_duration:
         remove_trips_by_duration(temp_df, min_duration=min_duration)
 
     # Remove trips that are too short (length).
     if min_length:
         remove_trips_by_length(temp_df, min_length=min_length, crs=crs)
 
+    if "environment" in temp_df.columns and indoor_limit:
+        remove_indoor_trips(temp_df, indoor_limit)
+
     temp_df = temp_df[temp_df["trip_status"].notna()]
     trip_mask = temp_df["trip_id"].notna()
     stationary_mask = temp_df["stationary_id"].notna()
 
     # Renumbers the trip IDs to be unique across all segments.
     temp_df.loc[trip_mask, "trip_id"] = (
         pd.factorize(
```

### Comparing `labda-0.0.2/labda/processing/wear_validity.py` & `labda-0.0.3/labda/processing/wear_validity.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/structure/collection.py` & `labda-0.0.3/labda/structure/collection.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import multiprocessing as mp
 import secrets
 from functools import partial
 from pathlib import Path
 from typing import Optional
 
 from pydantic import BaseModel, Field
 
+from ..parallel import parallel_processing
 from .subject import Subject
 
 
-def _process_subject(subject, func, **kwargs):
-    func(subject, **kwargs)
-
-    return subject
+def _to_parquet_with_path(subject, path, overwrite):
+    subject_path = path / f"{subject.metadata.id}.parquet"
+    return Subject.to_parquet(subject, path=subject_path, overwrite=overwrite)
 
 
 class Collection(BaseModel):
     id: Optional[str] = Field(default_factory=lambda: secrets.token_hex(4))
     subjects: list[Subject] = Field(default_factory=list)
 
     def __repr__(self):
@@ -41,45 +40,89 @@
         raise ValueError(f"Subject with id '{id}' not found.")
 
     @classmethod
     def from_folder(cls, path: str | Path, id: str | None = None) -> "Collection":
         if isinstance(path, str):
             path = Path(path)
 
-        subjects = [Subject.from_parquet(file) for file in path.glob("*.parquet")]
+        files = list(path.glob("*.parquet"))
+
+        if not files:
+            raise ValueError(f"No parquet files found in '{path}'.")
+
+        subjects = [Subject.from_parquet(file) for file in files]
         return cls(id=id, subjects=subjects)
 
-    def to_folder(self, path: str | Path, overwrite: bool = False):
+    def to_folder(
+        self,
+        path: str | Path,
+        *,
+        parallel: bool = True,
+        n_cores: int | str = "max",
+        overwrite: bool = False,
+    ):
         if isinstance(path, str):
             path = Path(path)
 
         path.mkdir(parents=True, exist_ok=True)
-        for subject in self.subjects:
-            subject.to_parquet(
-                path / f"{subject.metadata.id}.parquet", overwrite=overwrite
-            )
 
-    def detect_trips(self, **kwargs):
-        with mp.Pool(mp.cpu_count()) as pool:
-            self.subjects = pool.map(
-                partial(_process_subject, func=Subject.detect_trips, **kwargs),
+        if not path.is_dir():
+            raise ValueError(f"'{path}' is not a valid directory.")
+
+        if parallel:
+            self.subjects = parallel_processing(
+                partial(_to_parquet_with_path, path=path, overwrite=overwrite),
                 self.subjects,
+                n_cores,
             )
-
-    def detect_activity_intensity(self, **kwargs) -> None:
-        with mp.Pool(mp.cpu_count()) as pool:
-            self.subjects = pool.map(
-                partial(
-                    _process_subject, func=Subject.detect_activity_intensity, **kwargs
-                ),
+        else:
+            for subject in self.subjects:
+                subject.to_parquet(
+                    path / f"{subject.metadata.id}.parquet", overwrite=overwrite
+                )
+
+    def detect_trips(
+        self,
+        *,
+        parallel: bool = True,
+        n_cores: int | str = "max",
+        **kwargs,
+    ):
+        if parallel:
+            self.subjects = parallel_processing(
+                Subject.detect_trips,
+                self.subjects,
+                n_cores,
+                **kwargs,
+            )
+        else:
+            for subject in self.subjects:
+                subject.detect_trips(**kwargs)
+
+    def detect_activity_intensity(
+        self,
+        *,
+        parallel: bool = True,
+        n_cores: int | str = "max",
+        **kwargs,
+    ) -> None:
+        if parallel:
+            self.subjects = parallel_processing(
+                Subject.detect_activity_intensity,
                 self.subjects,
+                n_cores,
+                **kwargs,
             )
+        else:
+            for subject in self.subjects:
+                subject.detect_activity_intensity(**kwargs)
 
     # TODO: Rework whole consistency check
     # TODO: Add also check columns consistency
+    # TODO: Check if collection is not empty.
     def _check_consistency(self, attribute, error_message):
         # TODO: Add docstring, better name for method
         values = [getattr(subject.metadata, attribute) for subject in self.subjects]
         unique = set(values)
 
         if len(unique) != 1:
             print(f"{error_message}: {unique}")
```

### Comparing `labda-0.0.2/labda/structure/domains.py` & `labda-0.0.3/labda/structure/domains.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/structure/linkage.py` & `labda-0.0.3/labda/structure/linkage.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/structure/merging.py` & `labda-0.0.3/labda/structure/merging.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,15 +50,18 @@
     return left.metadata.crs or right.metadata.crs
 
 
 def _get_subjects(collection: Collection) -> list[str]:
     return [subject.metadata.id for subject in collection.subjects]
 
 
-def merge_subjects(left: Subject, right: Subject, **kwargs) -> Subject:
+def merge_subjects(
+    left: Subject, right: Subject, how: str = "inner", **kwargs
+) -> Subject:
+    # TODO: Log not overlapping rows.
     if not isinstance(left, Subject) and not isinstance(right, Subject):
         raise ValueError(f"Unsupported types: {type(left)} and {type(right)}")
 
     id = _check_ids(left, right)
     sf = _check_sampling_frequency(left, right)
     tz = _check_timezones(left, right)
     crs = _check_crs(left, right)
@@ -70,23 +73,26 @@
         timezone=tz,
         crs=crs,
     )
 
     # FIXME: Add suffixes to columns, even if not duplicated
     if not kwargs.get("suffixes"):
         _check_duplicate_cols(left.df, right.df)
-    merged = pd.merge(left.df, right.df, left_index=True, right_index=True, **kwargs)
+    merged = pd.merge(
+        left.df, right.df, left_index=True, right_index=True, how=how, **kwargs
+    )  # type: ignore
 
     return Subject(metadata=metadata, df=merged)
 
 
 def merge_collections(
     left: Collection,
     right: Collection,
     *,
+    how: str = "inner",
     keep: bool = False,
     **kwargs,
 ) -> Collection:
     if not isinstance(left, Collection) and not isinstance(right, Collection):
         raise ValueError(f"Unsupported types: {type(left)} and {type(right)}")
 
     left_ids = _get_subjects(left)
@@ -103,24 +109,34 @@
 
         try:
             right_subject = right.get_subject(subject)
         except Exception:
             right_subject = None
 
         if left_subject and right_subject:
-            merged_subject = merge_subjects(left_subject, right_subject, **kwargs)
-            collection.add_subject(merged_subject)
+            merged_subject = merge_subjects(
+                left_subject, right_subject, how=how, **kwargs
+            )
+
+            if not merged_subject.df.empty:
+                collection.add_subject(merged_subject)
+            else:
+                print(
+                    f"Error while merging | {subject} | Merged subject is empty and will be dropped."
+                )
         else:
             print(
                 f"Error while merging | {subject} | Subject not found in both collections."
             )
 
             # FIXME: Fix, it is not working
             # FIXME: Suffix to check if exists
-            # FIXME: Native pd.merge function adds suffixes to columns with the same name otherwise not (no suffixe and we don't know the origin of the column)
+            # FIXME: Native pd.merge function adds suffixes to columns with the same name otherwise not (no suffixes and we don't know the origin of the column)
+            # TODO: This could be reworked, maybe not needed to do KEEP, just outer join.
+            # TODO: Maybe completely remove the keep argument.
 
             if keep:
                 if left_subject:
                     # suffix = kwargs.get("suffixes")
                     # if suffix:
                     #     left_subject.df = left_subject.df.add_suffix(suffix[0])
                     collection.add_subject(left_subject)
```

### Comparing `labda-0.0.2/labda/structure/resampling.py` & `labda-0.0.3/labda/structure/resampling.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/structure/subject.py` & `labda-0.0.3/labda/structure/subject.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     add_speed,
     add_timedelta,
 )
 from ..processing import detect_domains
 from ..processing.accelerometer import detect_activity_intensity, detect_wear
 from ..processing.spatial import detect_transportation, detect_trips, get_timeline
 from ..structure.resampling import upsample
-from ..utils import columns_exists, columns_not_exists
+from ..utils import columns_exists, columns_not_exists, convert_to_geodataframe
+from ..visualisation.spatial import plot
 from .validation.domains import SCHEMA as DOMAINS_SCHEMA
 from .validation.subject import SCHEMA, Column
 
 
 class Vendor(StrEnum):
     ACTIGRAPH = "ActiGraph"
     XIAOMI = "Xiaomi"
@@ -64,34 +65,25 @@
         coerce_numbers_to_str = True
 
 
 class Subject(BaseModel):
     metadata: Metadata
     collection: Optional["Collection"] = None
     df: pd.DataFrame
+    timeline: pd.DataFrame | None = None
+
+    # TODO: Add check for not empty dataframe.
 
     class Config:
         arbitrary_types_allowed = True
 
     def __str__(self):
         return str(f"{self.metadata}\n{self.df}")
 
     @property
-    def timeline(self):
-        if not self.metadata.crs:
-            raise ValueError("Records object does not have a crs defined.")
-
-        columns_exists(
-            self.df,
-            [Column.TRIP_ID, Column.TRIP_STATUS, Column.STATIONARY_ID],
-        )
-
-        return get_timeline(self.df, crs=self.metadata.crs)
-
-    @property
     def domains(self):
         # TODO: Implement this property.
         raise NotImplementedError("This method is not implemented yet.")
 
     def to_parquet(
         self,
         path: str | Path,
@@ -134,14 +126,17 @@
         return cls
 
     def validate(
         self,
         *,
         extra_columns: bool = False,
     ):
+        if self.df.empty:
+            raise ValueError("DataFrame is empty.")
+
         self.df = SCHEMA.validate(self.df)
 
         # Order columns as defined in Column
         records_columns = [col.value for col in Column]
         ordered_columns = [col for col in records_columns if col in self.df.columns]
 
         # Append extra columns that are not in Column at the end, alphabetically
@@ -207,14 +202,15 @@
         window: int | None = 3,
         pause_radius: int | float | None = None,
         pause_duration: timedelta | None = None,
         min_duration: timedelta | None = None,
         min_length: int | float | None = None,
         min_distance: int | float | None = None,
         max_speed: int | float | None = None,
+        indoor_limit: float | None = None,
         overwrite: bool = False,
     ) -> None:
         if not self.metadata.crs:
             raise ValueError("Records object does not have a CRS defined.")
 
         self.df = detect_trips(
             self.df,
@@ -226,25 +222,31 @@
             stop_duration=stop_duration,
             pause_radius=pause_radius,
             pause_duration=pause_duration,
             min_duration=min_duration,
             min_length=min_length,
             min_distance=min_distance,
             max_speed=max_speed,
+            indoor_limit=indoor_limit,
         )
 
         if cut_points:
             self.df = detect_transportation(
                 self.df,
                 self.metadata.crs,
                 cut_points,
                 window=window,
                 overwrite=overwrite,
             )
 
+        if not overwrite and self.timeline:
+            raise ValueError("Timeline already exists. Set 'overwrite' to 'True'.")
+        else:
+            self.timeline = get_timeline(self.df, crs=self.metadata.crs)
+
     def detect_domains(
         self,
         domains: pd.DataFrame,
         *,
         overwrite: bool = False,
     ) -> None:
         domains = DOMAINS_SCHEMA.validate(domains)
@@ -288,7 +290,21 @@
         *,
         mapper: list[dict[str, Any]] | None = None,
     ) -> None:
         self.df = upsample(
             self.df, self.metadata.sampling_frequency, sampling_frequency, mapper
         )
         self.metadata.sampling_frequency = sampling_frequency
+
+    def plot(self, kind: str = "gps") -> Any:
+        match kind:
+            case "timeline":
+                if isinstance(self.timeline, pd.DataFrame):
+                    df = self.timeline
+                else:
+                    raise ValueError("Timeline does not exist. Run 'detect_trips'.")
+            case "gps":
+                df = self.df
+            case _:
+                raise ValueError(f"Kind '{kind}' not supported.")
+
+        return plot(df, kind, crs=self.metadata.crs)
```

### Comparing `labda-0.0.2/labda/structure/validation/domains.py` & `labda-0.0.3/labda/structure/validation/domains.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/structure/validation/linkage.py` & `labda-0.0.3/labda/structure/validation/linkage.py`

 * *Files identical despite different names*

### Comparing `labda-0.0.2/labda/structure/validation/subject.py` & `labda-0.0.3/labda/structure/validation/subject.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
             checks=[
                 pr.Check(
                     lambda s: s[s.notna()].isin(
                         [
                             "indoor",
                             "outdoor",
                             "vehicle",
-                            "mixed",
+                            "unknown",
                         ]
                     ),
                 )
             ],
         ),
         Column.SPEED: pr.Column(
             dtype="Float32",
@@ -247,14 +247,15 @@
             nullable=True,
             checks=[
                 pr.Check(
                     lambda s: s[s.notna()].isin(
                         [
                             "walk",
                             "run",
+                            "walk/run",
                             "bicycle",
                             "scooter",
                             "vehicle",
                             "train",
                         ]
                     ),
                 )
```

### Comparing `labda-0.0.2/labda/utils.py` & `labda-0.0.3/labda/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import secrets
+from datetime import datetime
 
 import geopandas as gpd
 import pandas as pd
 import pyproj
 from timezonefinder import TimezoneFinder
 
 from .structure.validation.subject import Column
@@ -234,7 +235,40 @@
 
 
 def get_crs_units(crs: str) -> str:
     crs = pyproj.CRS(crs)  # type: ignore
     units = crs.axis_info[0].unit_name  # type: ignore
 
     return units
+
+
+def change_crs(df: pd.DataFrame, source: str, target: str) -> pd.DataFrame:
+    gdf = convert_to_geodataframe(df, crs=source)
+    gdf.to_crs(target, inplace=True)
+    df = convert_to_dataframe(gdf)
+
+    return df
+
+
+def change_timezone(df: pd.DataFrame, source: str, target: str) -> pd.DataFrame:
+    df = df.copy()
+    df.index = df.index.tz_localize(source).tz_convert(target).tz_localize(None)  # type: ignore
+
+    return df
+
+
+def filter_datetime(
+    df: pd.DataFrame,
+    start: datetime | None = None,
+    end: datetime | None = None,
+) -> pd.DataFrame:
+    if start and end:
+        if end < start:
+            raise ValueError("The end time must be after the start time.")
+
+    if start:
+        df = df[df.index >= start]
+
+    if end:
+        df = df[df.index <= end]
+
+    return df
```

### Comparing `labda-0.0.2/pyproject.toml` & `labda-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,53 @@
 [tool.poetry]
 name = "labda"
-version = "0.0.2"
+version = "0.0.3"
 description = "Library for Advanced Behavioural Data Analysis"
-authors = [
-    "Josef Heidler <jheidler@health.sdu.dk>",
-]
-maintainers = [
-    "Josef Heidler <jheidler@health.sdu.dk>"
-]
+authors = ["Josef Heidler <jheidler@health.sdu.dk>"]
+maintainers = ["Josef Heidler <jheidler@health.sdu.dk>"]
 
 readme = "README.md"
 license = "	CC-BY-SA-4.0"
 homepage = "https://labda.josefheidler.cz"
 repository = "https://github.com/josefheidler/labda"
 documentation = "https://labda.josefheidler.cz"
 
-keywords = [
-    "analysis",
-    "health",
-    "behaviour",
-    "data",
-    "spatial",
-    "temporal"
-]
+keywords = ["analysis", "health", "behaviour", "data", "spatial", "temporal"]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
 ]
 
-packages = [{include = "labda"}]
+packages = [{ include = "labda" }]
 include = ["CHANGELOG.md"]
 
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pandas = "^2.2.0"
 geopandas = "^0.14.2"
 timezonefinder = "^6.2.0"
 pyarrow = "^15.0.0"
 pandera = "^0.18.0"
 openpyxl = "^3.1.2"
 sqlalchemy = "^2.0.25"
 pydeck = "^0.8.0"
+loguru = "^0.7.2"
 
 
 [tool.poetry.group.dev.dependencies]
 mkdocs-material = "^9.5.6"
 mkdocstrings = "^0.24.0"
 scikit-learn = "^1.4.0"
-resampy = "^0.4.2" # Remove after Axivity CWA/CSV parser and RAW to counts conversion is implemented
+resampy = "^0.4.2"         # Remove after Axivity CWA/CSV parser and RAW to counts conversion is implemented
 
 [tool.poetry.group.jupyter.dependencies]
 ipykernel = "^6.29.0"
 nbformat = "^5.9.2"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `labda-0.0.2/PKG-INFO` & `labda-0.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6c61 6264  : 2.1.Name: labd
-00000020: 610a 5665 7273 696f 6e3a 2030 2e30 2e32  a.Version: 0.0.2
+00000020: 610a 5665 7273 696f 6e3a 2030 2e30 2e33  a.Version: 0.0.3
 00000030: 0a53 756d 6d61 7279 3a20 4c69 6272 6172  .Summary: Librar
 00000040: 7920 666f 7220 4164 7661 6e63 6564 2042  y for Advanced B
 00000050: 6568 6176 696f 7572 616c 2044 6174 6120  ehavioural Data 
 00000060: 416e 616c 7973 6973 0a48 6f6d 652d 7061  Analysis.Home-pa
 00000070: 6765 3a20 6874 7470 733a 2f2f 6c61 6264  ge: https://labd
 00000080: 612e 6a6f 7365 6668 6569 646c 6572 2e63  a.josefheidler.c
 00000090: 7a0a 4c69 6365 6e73 653a 2009 4343 2d42  z.License: .CC-B
@@ -47,111 +47,74 @@
 000002e0: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
 000002f0: 0a43 6c61 7373 6966 6965 723a 2054 6f70  .Classifier: Top
 00000300: 6963 203a 3a20 5363 6965 6e74 6966 6963  ic :: Scientific
 00000310: 2f45 6e67 696e 6565 7269 6e67 0a52 6571  /Engineering.Req
 00000320: 7569 7265 732d 4469 7374 3a20 6765 6f70  uires-Dist: geop
 00000330: 616e 6461 7320 283e 3d30 2e31 342e 322c  andas (>=0.14.2,
 00000340: 3c30 2e31 352e 3029 0a52 6571 7569 7265  <0.15.0).Require
-00000350: 732d 4469 7374 3a20 6f70 656e 7079 786c  s-Dist: openpyxl
-00000360: 2028 3e3d 332e 312e 322c 3c34 2e30 2e30   (>=3.1.2,<4.0.0
-00000370: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-00000380: 2070 616e 6461 7320 283e 3d32 2e32 2e30   pandas (>=2.2.0
-00000390: 2c3c 332e 302e 3029 0a52 6571 7569 7265  ,<3.0.0).Require
-000003a0: 732d 4469 7374 3a20 7061 6e64 6572 6120  s-Dist: pandera 
-000003b0: 283e 3d30 2e31 382e 302c 3c30 2e31 392e  (>=0.18.0,<0.19.
-000003c0: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
-000003d0: 3a20 7079 6172 726f 7720 283e 3d31 352e  : pyarrow (>=15.
-000003e0: 302e 302c 3c31 362e 302e 3029 0a52 6571  0.0,<16.0.0).Req
-000003f0: 7569 7265 732d 4469 7374 3a20 7079 6465  uires-Dist: pyde
-00000400: 636b 2028 3e3d 302e 382e 302c 3c30 2e39  ck (>=0.8.0,<0.9
+00000350: 732d 4469 7374 3a20 6c6f 6775 7275 2028  s-Dist: loguru (
+00000360: 3e3d 302e 372e 322c 3c30 2e38 2e30 290a  >=0.7.2,<0.8.0).
+00000370: 5265 7175 6972 6573 2d44 6973 743a 206f  Requires-Dist: o
+00000380: 7065 6e70 7978 6c20 283e 3d33 2e31 2e32  penpyxl (>=3.1.2
+00000390: 2c3c 342e 302e 3029 0a52 6571 7569 7265  ,<4.0.0).Require
+000003a0: 732d 4469 7374 3a20 7061 6e64 6173 2028  s-Dist: pandas (
+000003b0: 3e3d 322e 322e 302c 3c33 2e30 2e30 290a  >=2.2.0,<3.0.0).
+000003c0: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
+000003d0: 616e 6465 7261 2028 3e3d 302e 3138 2e30  andera (>=0.18.0
+000003e0: 2c3c 302e 3139 2e30 290a 5265 7175 6972  ,<0.19.0).Requir
+000003f0: 6573 2d44 6973 743a 2070 7961 7272 6f77  es-Dist: pyarrow
+00000400: 2028 3e3d 3135 2e30 2e30 2c3c 3136 2e30   (>=15.0.0,<16.0
 00000410: 2e30 290a 5265 7175 6972 6573 2d44 6973  .0).Requires-Dis
-00000420: 743a 2073 716c 616c 6368 656d 7920 283e  t: sqlalchemy (>
-00000430: 3d32 2e30 2e32 352c 3c33 2e30 2e30 290a  =2.0.25,<3.0.0).
-00000440: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
-00000450: 696d 657a 6f6e 6566 696e 6465 7220 283e  imezonefinder (>
-00000460: 3d36 2e32 2e30 2c3c 372e 302e 3029 0a50  =6.2.0,<7.0.0).P
-00000470: 726f 6a65 6374 2d55 524c 3a20 446f 6375  roject-URL: Docu
-00000480: 6d65 6e74 6174 696f 6e2c 2068 7474 7073  mentation, https
-00000490: 3a2f 2f6c 6162 6461 2e6a 6f73 6566 6865  ://labda.josefhe
-000004a0: 6964 6c65 722e 637a 0a50 726f 6a65 6374  idler.cz.Project
-000004b0: 2d55 524c 3a20 5265 706f 7369 746f 7279  -URL: Repository
-000004c0: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-000004d0: 2e63 6f6d 2f6a 6f73 6566 6865 6964 6c65  .com/josefheidle
-000004e0: 722f 6c61 6264 610a 4465 7363 7269 7074  r/labda.Descript
-000004f0: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-00000500: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-00000510: 0a23 204c 4142 4441 3a20 4c69 6272 6172  .# LABDA: Librar
-00000520: 7920 666f 7220 4164 7661 6e63 6564 2042  y for Advanced B
-00000530: 6568 6176 696f 7572 616c 2044 6174 6120  ehavioural Data 
-00000540: 416e 616c 7973 6973 0a0a 2a2a 4c41 4244  Analysis..**LABD
-00000550: 4120 6973 2063 7572 7265 6e74 6c79 2075  A is currently u
-00000560: 6e64 6572 2064 6576 656c 6f70 6d65 6e74  nder development
-00000570: 2061 6e64 206d 6179 2075 6e64 6572 676f   and may undergo
-00000580: 2073 6967 6e69 6669 6361 6e74 2041 5049   significant API
-00000590: 2063 6861 6e67 6573 2074 6861 7420 636f   changes that co
-000005a0: 756c 6420 7265 7375 6c74 2069 6e20 6272  uld result in br
-000005b0: 6561 6b69 6e67 2063 6861 6e67 6573 2e2a  eaking changes.*
-000005c0: 2a0a 0a23 2320 5768 6174 2069 7320 6974  *..## What is it
-000005d0: 3f0a 0a54 4f2d 444f 2e2e 2e0a 0a23 2320  ?..TO-DO.....## 
-000005e0: 4d61 696e 2046 6561 7475 7265 730a 0a54  Main Features..T
-000005f0: 4f2d 444f 2e2e 2e0a 0a23 2320 4c69 6365  O-DO.....## Lice
-00000600: 6e73 650a 3c70 2078 6d6c 6e73 3a63 633d  nse.<p xmlns:cc=
-00000610: 2268 7474 703a 2f2f 6372 6561 7469 7665  "http://creative
-00000620: 636f 6d6d 6f6e 732e 6f72 672f 6e73 2322  commons.org/ns#"
-00000630: 2078 6d6c 6e73 3a64 6374 3d22 6874 7470   xmlns:dct="http
-00000640: 3a2f 2f70 7572 6c2e 6f72 672f 6463 2f74  ://purl.org/dc/t
-00000650: 6572 6d73 2f22 3e3c 6120 7072 6f70 6572  erms/"><a proper
-00000660: 7479 3d22 6463 743a 7469 746c 6522 2072  ty="dct:title" r
-00000670: 656c 3d22 6363 3a61 7474 7269 6275 7469  el="cc:attributi
-00000680: 6f6e 5552 4c22 2068 7265 663d 2268 7474  onURL" href="htt
-00000690: 7073 3a2f 2f6c 6162 6461 2e6a 6f73 6566  ps://labda.josef
-000006a0: 6865 6964 6c65 722e 637a 2f22 3e4c 6962  heidler.cz/">Lib
-000006b0: 7261 7279 2066 6f72 2041 6476 616e 6365  rary for Advance
-000006c0: 6420 4265 6861 7669 6f75 7261 6c20 4461  d Behavioural Da
-000006d0: 7461 2041 6e61 6c79 7369 733c 2f61 3e20  ta Analysis</a> 
-000006e0: 6279 203c 6120 7265 6c3d 2263 633a 6174  by <a rel="cc:at
-000006f0: 7472 6962 7574 696f 6e55 524c 2064 6374  tributionURL dct
-00000700: 3a63 7265 6174 6f72 2220 7072 6f70 6572  :creator" proper
-00000710: 7479 3d22 6363 3a61 7474 7269 6275 7469  ty="cc:attributi
-00000720: 6f6e 4e61 6d65 2220 6872 6566 3d22 6874  onName" href="ht
-00000730: 7470 733a 2f2f 6a6f 7365 6668 6569 646c  tps://josefheidl
-00000740: 6572 2e63 7a2f 223e 4a6f 7365 6620 4865  er.cz/">Josef He
-00000750: 6964 6c65 723c 2f61 3e20 6973 206c 6963  idler</a> is lic
-00000760: 656e 7365 6420 756e 6465 7220 3c61 2068  ensed under <a h
-00000770: 7265 663d 2268 7474 703a 2f2f 6372 6561  ref="http://crea
-00000780: 7469 7665 636f 6d6d 6f6e 732e 6f72 672f  tivecommons.org/
-00000790: 6c69 6365 6e73 6573 2f62 792f 342e 302f  licenses/by/4.0/
-000007a0: 3f72 6566 3d63 686f 6f73 6572 2d76 3122  ?ref=chooser-v1"
-000007b0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
-000007c0: 2072 656c 3d22 6c69 6365 6e73 6520 6e6f   rel="license no
-000007d0: 6f70 656e 6572 206e 6f72 6566 6572 7265  opener noreferre
-000007e0: 7222 2073 7479 6c65 3d22 6469 7370 6c61  r" style="displa
-000007f0: 793a 696e 6c69 6e65 2d62 6c6f 636b 3b22  y:inline-block;"
-00000800: 3e43 4320 4259 2034 2e30 3c69 6d67 2073  >CC BY 4.0<img s
-00000810: 7479 6c65 3d22 6865 6967 6874 3a32 3270  tyle="height:22p
-00000820: 7821 696d 706f 7274 616e 743b 6d61 7267  x!important;marg
-00000830: 696e 2d6c 6566 743a 3370 783b 7665 7274  in-left:3px;vert
-00000840: 6963 616c 2d61 6c69 676e 3a74 6578 742d  ical-align:text-
-00000850: 626f 7474 6f6d 3b22 2073 7263 3d22 6874  bottom;" src="ht
-00000860: 7470 733a 2f2f 6d69 7272 6f72 732e 6372  tps://mirrors.cr
-00000870: 6561 7469 7665 636f 6d6d 6f6e 732e 6f72  eativecommons.or
-00000880: 672f 7072 6573 736b 6974 2f69 636f 6e73  g/presskit/icons
-00000890: 2f63 632e 7376 673f 7265 663d 6368 6f6f  /cc.svg?ref=choo
-000008a0: 7365 722d 7631 223e 3c69 6d67 2073 7479  ser-v1"><img sty
-000008b0: 6c65 3d22 6865 6967 6874 3a32 3270 7821  le="height:22px!
-000008c0: 696d 706f 7274 616e 743b 6d61 7267 696e  important;margin
-000008d0: 2d6c 6566 743a 3370 783b 7665 7274 6963  -left:3px;vertic
-000008e0: 616c 2d61 6c69 676e 3a74 6578 742d 626f  al-align:text-bo
-000008f0: 7474 6f6d 3b22 2073 7263 3d22 6874 7470  ttom;" src="http
-00000900: 733a 2f2f 6d69 7272 6f72 732e 6372 6561  s://mirrors.crea
-00000910: 7469 7665 636f 6d6d 6f6e 732e 6f72 672f  tivecommons.org/
-00000920: 7072 6573 736b 6974 2f69 636f 6e73 2f62  presskit/icons/b
-00000930: 792e 7376 673f 7265 663d 6368 6f6f 7365  y.svg?ref=choose
-00000940: 722d 7631 223e 3c2f 613e 3c2f 703e 0a0a  r-v1"></a></p>..
-00000950: 2323 2044 6f63 756d 656e 7461 7469 6f6e  ## Documentation
-00000960: 0a0a 544f 2d44 4f2e 2e2e 0a0a 2323 2047  ..TO-DO.....## G
-00000970: 6574 7469 6e67 2048 656c 702c 2044 6973  etting Help, Dis
-00000980: 6375 7373 696f 6e20 616e 6420 4465 7665  cussion and Deve
-00000990: 6c6f 706d 656e 740a 0a54 4f2d 444f 2e2e  lopment..TO-DO..
-000009a0: 2e0a 0a23 2320 436f 6e74 7269 6275 7469  ...## Contributi
-000009b0: 6e67 2074 6f20 6c61 6264 610a 0a54 4f2d  ng to labda..TO-
-000009c0: 444f 2e2e 0a                             DO...
+00000420: 743a 2070 7964 6563 6b20 283e 3d30 2e38  t: pydeck (>=0.8
+00000430: 2e30 2c3c 302e 392e 3029 0a52 6571 7569  .0,<0.9.0).Requi
+00000440: 7265 732d 4469 7374 3a20 7371 6c61 6c63  res-Dist: sqlalc
+00000450: 6865 6d79 2028 3e3d 322e 302e 3235 2c3c  hemy (>=2.0.25,<
+00000460: 332e 302e 3029 0a52 6571 7569 7265 732d  3.0.0).Requires-
+00000470: 4469 7374 3a20 7469 6d65 7a6f 6e65 6669  Dist: timezonefi
+00000480: 6e64 6572 2028 3e3d 362e 322e 302c 3c37  nder (>=6.2.0,<7
+00000490: 2e30 2e30 290a 5072 6f6a 6563 742d 5552  .0.0).Project-UR
+000004a0: 4c3a 2044 6f63 756d 656e 7461 7469 6f6e  L: Documentation
+000004b0: 2c20 6874 7470 733a 2f2f 6c61 6264 612e  , https://labda.
+000004c0: 6a6f 7365 6668 6569 646c 6572 2e63 7a0a  josefheidler.cz.
+000004d0: 5072 6f6a 6563 742d 5552 4c3a 2052 6570  Project-URL: Rep
+000004e0: 6f73 6974 6f72 792c 2068 7474 7073 3a2f  ository, https:/
+000004f0: 2f67 6974 6875 622e 636f 6d2f 6a6f 7365  /github.com/jose
+00000500: 6668 6569 646c 6572 2f6c 6162 6461 0a44  fheidler/labda.D
+00000510: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+00000520: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+00000530: 726b 646f 776e 0a0a 2320 4c41 4244 413a  rkdown..# LABDA:
+00000540: 204c 6962 7261 7279 2066 6f72 2041 6476   Library for Adv
+00000550: 616e 6365 6420 4265 6861 7669 6f75 7261  anced Behavioura
+00000560: 6c20 4461 7461 2041 6e61 6c79 7369 730a  l Data Analysis.
+00000570: 0a2a 2a4c 4142 4441 2069 7320 6375 7272  .**LABDA is curr
+00000580: 656e 746c 7920 756e 6465 7220 6465 7665  ently under deve
+00000590: 6c6f 706d 656e 7420 616e 6420 6d61 7920  lopment and may 
+000005a0: 756e 6465 7267 6f20 7369 676e 6966 6963  undergo signific
+000005b0: 616e 7420 4150 4920 6368 616e 6765 7320  ant API changes 
+000005c0: 7468 6174 2063 6f75 6c64 2072 6573 756c  that could resul
+000005d0: 7420 696e 2062 7265 616b 696e 6720 6368  t in breaking ch
+000005e0: 616e 6765 732e 2a2a 0a0a 2323 2057 6861  anges.**..## Wha
+000005f0: 7420 6973 2069 743f 0a0a 544f 2d44 4f2e  t is it?..TO-DO.
+00000600: 2e2e 0a0a 2323 204d 6169 6e20 4665 6174  ....## Main Feat
+00000610: 7572 6573 0a0a 544f 2d44 4f2e 2e2e 0a0a  ures..TO-DO.....
+00000620: 2323 204c 6963 656e 7365 0a0a 5b4c 6962  ## License..[Lib
+00000630: 7261 7279 2066 6f72 2041 6476 616e 6365  rary for Advance
+00000640: 6420 4265 6861 7669 6f75 7261 6c20 4461  d Behavioural Da
+00000650: 7461 2041 6e61 6c79 7369 735d 2868 7474  ta Analysis](htt
+00000660: 7073 3a2f 2f6c 6162 6461 2e6a 6f73 6566  ps://labda.josef
+00000670: 6865 6964 6c65 722e 637a 2f29 2062 7920  heidler.cz/) by 
+00000680: 5b4a 6f73 6566 2048 6569 646c 6572 5d28  [Josef Heidler](
+00000690: 6874 7470 733a 2f2f 6c61 6264 612e 6a6f  https://labda.jo
+000006a0: 7365 6668 6569 646c 6572 2e63 7a2f 2920  sefheidler.cz/) 
+000006b0: 6973 206c 6963 656e 7365 6420 756e 6465  is licensed unde
+000006c0: 7220 5b43 4320 4259 2034 2e30 5d28 6874  r [CC BY 4.0](ht
+000006d0: 7470 733a 2f2f 6372 6561 7469 7665 636f  tps://creativeco
+000006e0: 6d6d 6f6e 732e 6f72 672f 6c69 6365 6e73  mmons.org/licens
+000006f0: 6573 2f62 792f 342e 302f 292e 0a0a 2323  es/by/4.0/)...##
+00000700: 2044 6f63 756d 656e 7461 7469 6f6e 0a0a   Documentation..
+00000710: 544f 2d44 4f2e 2e2e 0a0a 2323 2047 6574  TO-DO.....## Get
+00000720: 7469 6e67 2048 656c 702c 2044 6973 6375  ting Help, Discu
+00000730: 7373 696f 6e20 616e 6420 4465 7665 6c6f  ssion and Develo
+00000740: 706d 656e 740a 0a54 4f2d 444f 2e2e 2e0a  pment..TO-DO....
+00000750: 0a23 2320 436f 6e74 7269 6275 7469 6e67  .## Contributing
+00000760: 2074 6f20 6c61 6264 610a 0a54 4f2d 444f   to labda..TO-DO
+00000770: 2e2e 0a                                  ...
```

