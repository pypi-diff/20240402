# Comparing `tmp/pyakamai-2.35-py3-none-any.whl.zip` & `tmp/pyakamai-2.36-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 37335 bytes, number of entries: 26
+Zip file size: 37350 bytes, number of entries: 26
 -rw-r--r--  2.0 unx      588 b- defN 23-Dec-31 08:48 pyakamai/__init__.py
 -rw-r--r--  2.0 unx     2239 b- defN 23-Jul-20 07:24 pyakamai/akamaiapidefinition.py
 -rw-r--r--  2.0 unx     3789 b- defN 23-Dec-09 13:10 pyakamai/akamaicasemanagement.py
 -rw-r--r--  2.0 unx     5202 b- defN 23-Dec-28 16:49 pyakamai/akamaichinacdn.py
 -rw-r--r--  2.0 unx     4743 b- defN 23-Dec-29 09:33 pyakamai/akamaicloudlets.py
 -rw-r--r--  2.0 unx     1473 b- defN 23-May-01 03:29 pyakamai/akamaicpcode.py
 -rw-r--r--  2.0 unx     3676 b- defN 23-Dec-09 13:49 pyakamai/akamaicps.py
@@ -11,18 +11,18 @@
 -rw-r--r--  2.0 unx     6903 b- defN 24-Feb-09 07:33 pyakamai/akamaiedns.py
 -rw-r--r--  2.0 unx     4712 b- defN 23-Dec-28 17:30 pyakamai/akamaiehn.py
 -rw-r--r--  2.0 unx    14193 b- defN 23-May-01 03:54 pyakamai/akamaiksd1.py
 -rw-r--r--  2.0 unx     5689 b- defN 23-May-01 03:31 pyakamai/akamaiksd2.py
 -rw-r--r--  2.0 unx     2443 b- defN 23-Dec-28 18:16 pyakamai/akamailds.py
 -rw-r--r--  2.0 unx     5361 b- defN 24-Jan-25 08:15 pyakamai/akamaimsl.py
 -rw-r--r--  2.0 unx     1486 b- defN 23-Dec-28 18:04 pyakamai/akamains.py
--rw-r--r--  2.0 unx    30870 b- defN 24-Mar-27 11:21 pyakamai/akamaiproperty.py
+-rw-r--r--  2.0 unx    30939 b- defN 24-Apr-02 12:00 pyakamai/akamaiproperty.py
 -rw-r--r--  2.0 unx     3506 b- defN 23-Apr-30 15:04 pyakamai/akamaipurge.py
 -rw-r--r--  2.0 unx     1893 b- defN 23-Dec-31 08:55 pyakamai/akamaireporting.py
 -rw-r--r--  2.0 unx     1472 b- defN 23-Dec-28 18:12 pyakamai/akamaiss.py
 -rw-r--r--  2.0 unx     9664 b- defN 24-Feb-09 07:30 pyakamai/http_calls.py
 -rw-r--r--  2.0 unx     4052 b- defN 24-Feb-06 08:20 pyakamai/pyakamai.py
--rw-r--r--  2.0 unx    12832 b- defN 24-Mar-27 11:23 pyakamai-2.35.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-27 11:23 pyakamai-2.35.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Mar-27 11:23 pyakamai-2.35.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2082 b- defN 24-Mar-27 11:23 pyakamai-2.35.dist-info/RECORD
-26 files, 139994 bytes uncompressed, 34023 bytes compressed:  75.7%
+-rw-r--r--  2.0 unx    12832 b- defN 24-Apr-02 12:03 pyakamai-2.36.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 12:03 pyakamai-2.36.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-02 12:03 pyakamai-2.36.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2082 b- defN 24-Apr-02 12:03 pyakamai-2.36.dist-info/RECORD
+26 files, 140063 bytes uncompressed, 34038 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -60,20 +60,20 @@
 
 Filename: pyakamai/http_calls.py
 Comment: 
 
 Filename: pyakamai/pyakamai.py
 Comment: 
 
-Filename: pyakamai-2.35.dist-info/METADATA
+Filename: pyakamai-2.36.dist-info/METADATA
 Comment: 
 
-Filename: pyakamai-2.35.dist-info/WHEEL
+Filename: pyakamai-2.36.dist-info/WHEEL
 Comment: 
 
-Filename: pyakamai-2.35.dist-info/top_level.txt
+Filename: pyakamai-2.36.dist-info/top_level.txt
 Comment: 
 
-Filename: pyakamai-2.35.dist-info/RECORD
+Filename: pyakamai-2.36.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyakamai/akamaiproperty.py

```diff
@@ -202,14 +202,16 @@
         params["groupId"] = self.groupId
 
         if self.accountSwitchKey:
             params["accountSwitchKey"] = self.accountSwitchKey
 
         status,getHostnameJson = self._prdHttpCaller.getResult(getHostNameEndPoint,params)
         hostNameList = []
+        if 'hostnames' not in getHostnameJson:
+            return []
         for hostname in  getHostnameJson["hostnames"]["items"]:
             hostNameList.append(hostname["cnameFrom"])
         return hostNameList
 
 
     def createVersion(self,baseVersion):
         if self._invalidconfig == True:
```

## Comparing `pyakamai-2.35.dist-info/METADATA` & `pyakamai-2.36.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyakamai
-Version: 2.35
+Version: 2.36
 Summary: A Boto3 like SDK for Akamai
 Home-page: https://github.com/Achuthananda/pyakamai
 Author: Achuthananda M P
 Author-email: achuthadivine@gmail.com
 Project-URL: Source, https://github.com/Achuthananda/pyakamai
 Keywords: Akamai Python CDN SDK Edge
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyakamai-2.35.dist-info/RECORD` & `pyakamai-2.36.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 pyakamai/akamaiedns.py,sha256=TFyzmO8zjn54rMwffyfXQrpADRWMNmG5AKgszp5wZEA,6903
 pyakamai/akamaiehn.py,sha256=SleqTYdEeKUHzRTVn5hIA4YBUvy9iJGouEFSNiBW2A0,4712
 pyakamai/akamaiksd1.py,sha256=7RslIDB6oR3KA4nyC7infxXqH4Jr7dM0t3znyDfCUPI,14193
 pyakamai/akamaiksd2.py,sha256=CWo_ejWDPoyiTWROrbc_OTmcq7RXZBb8n8xOYVXQ3w8,5689
 pyakamai/akamailds.py,sha256=Rt4Lp4Hmu6T5sx0jCp3iB7YMowKSdIrk6E2NP_JWYXA,2443
 pyakamai/akamaimsl.py,sha256=F4FZcI2pAli2HshbGAtRiUVpm0XdZwBGvhSfmlAH5QE,5361
 pyakamai/akamains.py,sha256=X7i51U7NdUJz07S8lGevDKdrUP_CpTJOHNM4ur5O0Eg,1486
-pyakamai/akamaiproperty.py,sha256=lXFUSm6n8EX9prGnsaaEa0ihX_U_gJxvmIZsl5V-YYk,30870
+pyakamai/akamaiproperty.py,sha256=bjKCzJNzjGFF0QukSmD_EVbJHOcPwIy18JJIXmnee3c,30939
 pyakamai/akamaipurge.py,sha256=FLwfjbhjn0PZyRRq68SpKFF9f8JPk76DKvCmmVg2NtU,3506
 pyakamai/akamaireporting.py,sha256=nRw0npxiya6YVvF1Q0alSsoZIOQNeLXYDDWK03VW2WA,1893
 pyakamai/akamaiss.py,sha256=i5PKpfb0ESkPGKtgZLMYGs9Kij9jEcRd-jIvKak792Q,1472
 pyakamai/http_calls.py,sha256=smAuBLwb76oGxDBJALZedxqDzPXsBdYY7IE1YZMidX0,9664
 pyakamai/pyakamai.py,sha256=_JsStTBV-5zqU6QzXBDZiGCtPBVtOallr03rDR4om68,4052
-pyakamai-2.35.dist-info/METADATA,sha256=XNYYAdRhMz0ekFe2saqHAzfeeFAZ5lxOGqeq2oq2iqs,12832
-pyakamai-2.35.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyakamai-2.35.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
-pyakamai-2.35.dist-info/RECORD,,
+pyakamai-2.36.dist-info/METADATA,sha256=KsGSoQ9XnGOs8Dkw1th_kUclnDygR8K7sGtsdNJAEU0,12832
+pyakamai-2.36.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyakamai-2.36.dist-info/top_level.txt,sha256=9Nh6eAgz4Nynio3dNZWYC6gKw0ly2NfcXshvK-PQI0U,9
+pyakamai-2.36.dist-info/RECORD,,
```

