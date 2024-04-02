# Comparing `tmp/viam_sdk-0.9.0rc1-py3-none-manylinux2014_x86_64.whl.zip` & `tmp/viam_sdk-0.9.1-py3-none-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 10090496 bytes, number of entries: 407
+Zip file size: 10090516 bytes, number of entries: 407
 -rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx     1565 b- defN 80-Jan-01 00:00 viam/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 viam/app/__init__.py
 -rw-r--r--  2.0 unx      947 b- defN 80-Jan-01 00:00 viam/app/_logs.py
 -rw-r--r--  2.0 unx    51316 b- defN 80-Jan-01 00:00 viam/app/app_client.py
 -rw-r--r--  2.0 unx     3766 b- defN 80-Jan-01 00:00 viam/app/billing_client.py
 -rw-r--r--  2.0 unx    31650 b- defN 80-Jan-01 00:00 viam/app/data_client.py
@@ -62,15 +62,15 @@
 -rw-r--r--  2.0 unx     1887 b- defN 80-Jan-01 00:00 viam/components/pose_tracker/client.py
 -rw-r--r--  2.0 unx     1305 b- defN 80-Jan-01 00:00 viam/components/pose_tracker/pose_tracker.py
 -rw-r--r--  2.0 unx     2231 b- defN 80-Jan-01 00:00 viam/components/pose_tracker/service.py
 -rw-r--r--  2.0 unx      398 b- defN 80-Jan-01 00:00 viam/components/power_sensor/__init__.py
 -rw-r--r--  2.0 unx     2841 b- defN 80-Jan-01 00:00 viam/components/power_sensor/client.py
 -rw-r--r--  2.0 unx     2192 b- defN 80-Jan-01 00:00 viam/components/power_sensor/power_sensor.py
 -rw-r--r--  2.0 unx     3533 b- defN 80-Jan-01 00:00 viam/components/power_sensor/service.py
--rw-r--r--  2.0 unx      357 b- defN 80-Jan-01 00:00 viam/components/sensor/__init__.py
+-rw-r--r--  2.0 unx      466 b- defN 80-Jan-01 00:00 viam/components/sensor/__init__.py
 -rw-r--r--  2.0 unx     1767 b- defN 80-Jan-01 00:00 viam/components/sensor/client.py
 -rw-r--r--  2.0 unx     1010 b- defN 80-Jan-01 00:00 viam/components/sensor/sensor.py
 -rw-r--r--  2.0 unx     2261 b- defN 80-Jan-01 00:00 viam/components/sensor/service.py
 -rw-r--r--  2.0 unx      800 b- defN 80-Jan-01 00:00 viam/components/servo/__init__.py
 -rw-r--r--  2.0 unx     2630 b- defN 80-Jan-01 00:00 viam/components/servo/client.py
 -rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 viam/components/servo/service.py
 -rw-r--r--  2.0 unx     1704 b- defN 80-Jan-01 00:00 viam/components/servo/servo.py
@@ -398,12 +398,12 @@
 -rw-r--r--  2.0 unx     1954 b- defN 80-Jan-01 00:00 viam/services/slam/slam.py
 -rw-r--r--  2.0 unx      426 b- defN 80-Jan-01 00:00 viam/services/vision/__init__.py
 -rw-r--r--  2.0 unx     5176 b- defN 80-Jan-01 00:00 viam/services/vision/client.py
 -rw-r--r--  2.0 unx     5076 b- defN 80-Jan-01 00:00 viam/services/vision/service.py
 -rw-r--r--  2.0 unx     5066 b- defN 80-Jan-01 00:00 viam/services/vision/vision.py
 -rw-r--r--  2.0 unx     6403 b- defN 80-Jan-01 00:00 viam/sessions_client.py
 -rw-r--r--  2.0 unx    12252 b- defN 80-Jan-01 00:00 viam/utils.py
--rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 viam_sdk-0.9.0rc1.dist-info/LICENSE
--rw-r--r--  2.0 unx     9528 b- defN 80-Jan-01 00:00 viam_sdk-0.9.0rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 viam_sdk-0.9.0rc1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    37583 b- defN 16-Jan-01 00:00 viam_sdk-0.9.0rc1.dist-info/RECORD
-407 files, 31050829 bytes uncompressed, 10030004 bytes compressed:  67.7%
+-rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 viam_sdk-0.9.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9525 b- defN 80-Jan-01 00:00 viam_sdk-0.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 viam_sdk-0.9.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    37571 b- defN 16-Jan-01 00:00 viam_sdk-0.9.1.dist-info/RECORD
+407 files, 31050923 bytes uncompressed, 10030048 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -1203,20 +1203,20 @@
 
 Filename: viam/sessions_client.py
 Comment: 
 
 Filename: viam/utils.py
 Comment: 
 
-Filename: viam_sdk-0.9.0rc1.dist-info/LICENSE
+Filename: viam_sdk-0.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: viam_sdk-0.9.0rc1.dist-info/METADATA
+Filename: viam_sdk-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: viam_sdk-0.9.0rc1.dist-info/WHEEL
+Filename: viam_sdk-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: viam_sdk-0.9.0rc1.dist-info/RECORD
+Filename: viam_sdk-0.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## viam/components/sensor/__init__.py

```diff
@@ -1,7 +1,8 @@
+import viam.gen.component.sensor.v1.sensor_pb2  # Need this import for Sensor service descriptors to resolve
 from viam.resource.registry import Registry, ResourceRegistration
 
 from .client import SensorClient
 from .sensor import Sensor
 from .service import SensorRPCService
 
 __all__ = [
```

## Comparing `viam_sdk-0.9.0rc1.dist-info/LICENSE` & `viam_sdk-0.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `viam_sdk-0.9.0rc1.dist-info/METADATA` & `viam_sdk-0.9.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viam-sdk
-Version: 0.9.0rc1
+Version: 0.9.1
 Summary: Viam Robotics Python SDK
 License: Apache-2.0
 Author: Naveed
 Author-email: naveed@viam.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `viam_sdk-0.9.0rc1.dist-info/RECORD` & `viam_sdk-0.9.1.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 viam/components/pose_tracker/client.py,sha256=yojTpkj-ICbz1zUw-N0V6PyYceSD3xiHg0Ng0ZE1_9w,1887
 viam/components/pose_tracker/pose_tracker.py,sha256=r3cmWisuMUS3ya47ylJUyQ-9Tu8SlEBkrKB6aSMcQkY,1305
 viam/components/pose_tracker/service.py,sha256=D7-GUvt4cDYZuEAf_i6cKTiuwB5llCh0d19STyC0ZfY,2231
 viam/components/power_sensor/__init__.py,sha256=Uu2jZESQytQx7fv_QOQ52OXh1WU8bnMbit9w52-8FHg,398
 viam/components/power_sensor/client.py,sha256=M5qs0kLqCXDB3P1Lhy5paOTBg2riHJUox8auPqKRa9U,2841
 viam/components/power_sensor/power_sensor.py,sha256=lho4t2ZLhwTwyhc0jmHS0VRdS_Com2UBOGvq5yWHP8s,2192
 viam/components/power_sensor/service.py,sha256=pYCUPHpQR2X8oYLYjty2TMCyIkLV2aBb0vjMOBRJJqs,3533
-viam/components/sensor/__init__.py,sha256=fwCcBeKmbX6du3xwU9R0RnuIyqsnz0cWnBxaWw_4jM0,357
+viam/components/sensor/__init__.py,sha256=DYppn0JIKrlPCAuDZXNqgy43yN-9pPEmLF6yiXiSSSQ,466
 viam/components/sensor/client.py,sha256=BRyoldfobUCKDMAqW9zc9AH1lrTMLm_9OWA4E6S21Bg,1767
 viam/components/sensor/sensor.py,sha256=dGdtWXQ7wy-zzpKzRs6vN3YAX2yGyVHv2_cgWFu6fZU,1010
 viam/components/sensor/service.py,sha256=j-PtzID7LstuafQdVia23zRsnEQOoaa4qWXvxiiLTR8,2261
 viam/components/servo/__init__.py,sha256=9NeRbi2cFPnwliKXMEFPqjmeYjBGziffYlkFx5hOtrI,800
 viam/components/servo/client.py,sha256=5qpdWJhff6hetjvcDwC3JE_LtpDiZD7fPlBycT78McQ,2630
 viam/components/servo/service.py,sha256=CB3DUXK6xNtBXHWSyzxOLYHD0C7-G2hqMmrJOHL-39I,3569
 viam/components/servo/servo.py,sha256=1YqyzxQdmhg6v-Wjq-5jtmv-yJIye9uKQBGWS4U3gW4,1704
@@ -397,11 +397,11 @@
 viam/services/slam/slam.py,sha256=9fxqVL3lHGfjsoSDF_YrhyuXVDJ0hubVIdwI71rdSvI,1954
 viam/services/vision/__init__.py,sha256=8DPwRKggv0cMb3Z4R5-pAHvbAIIMBfNYWUktuh58gyE,426
 viam/services/vision/client.py,sha256=EHiVW1R2JgS_DzyenmJzcIhQdtiegeUUBy2lYBpKemg,5176
 viam/services/vision/service.py,sha256=ae0zUVBi-QiNYoxfT7KurCUvdy0umdUdFVqMLprF_3c,5076
 viam/services/vision/vision.py,sha256=4JGFJVU8yv5poFnF-LaS_cd2SMRTNHp3XWKlfWWCO4I,5066
 viam/sessions_client.py,sha256=FsPaJZjHkE0NDZGnoFzGxoWeas21zJFfwza1h_AY1oA,6403
 viam/utils.py,sha256=qFgR_kNvoOdkNuXmpdXu6N9ptNVi7fTHtG8dBKFjL0c,12252
-viam_sdk-0.9.0rc1.dist-info/LICENSE,sha256=yVuuHRzgI17MzTVgt3LsHvuX80innw--CmNPDCzO_iw,11358
-viam_sdk-0.9.0rc1.dist-info/METADATA,sha256=fMGQLtuyRzBeonK5Mx5Y0TTVxvNBwUxfsZDgHNExnR4,9528
-viam_sdk-0.9.0rc1.dist-info/WHEEL,sha256=d2fvjOD7sXsVzChCqf0Ty0JbHKBaLYwDbGQDwQTnJ50,88
-viam_sdk-0.9.0rc1.dist-info/RECORD,,
+viam_sdk-0.9.1.dist-info/LICENSE,sha256=yVuuHRzgI17MzTVgt3LsHvuX80innw--CmNPDCzO_iw,11358
+viam_sdk-0.9.1.dist-info/METADATA,sha256=2_D7V50l-ZZFbb_9A-oG6Z3Boyx73s780zDwIceUyiA,9525
+viam_sdk-0.9.1.dist-info/WHEEL,sha256=d2fvjOD7sXsVzChCqf0Ty0JbHKBaLYwDbGQDwQTnJ50,88
+viam_sdk-0.9.1.dist-info/RECORD,,
```

