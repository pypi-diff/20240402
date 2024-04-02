# Comparing `tmp/libsrg-3.8.4-py3-none-any.whl.zip` & `tmp/libsrg-3.8.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 37449 bytes, number of entries: 27
+Zip file size: 37451 bytes, number of entries: 27
 -rw-r--r--  2.0 unx     1027 b- defN 24-Feb-08 14:38 libsrg/AppTemplate.py
 -rw-r--r--  2.0 unx     1878 b- defN 24-Apr-02 14:40 libsrg/ElapsedTime.py
--rw-r--r--  2.0 unx     6514 b- defN 24-Apr-02 15:00 libsrg/Info.py
+-rw-r--r--  2.0 unx     6509 b- defN 24-Apr-02 16:11 libsrg/Info.py
 -rw-r--r--  2.0 unx     3532 b- defN 23-Jan-31 15:26 libsrg/LevelBanner.py
 -rw-r--r--  2.0 unx     1492 b- defN 23-Jan-18 20:30 libsrg/LoggerGUIProxy.py
 -rw-r--r--  2.0 unx     6093 b- defN 24-Apr-02 15:52 libsrg/LoggingAppBase.py
 -rw-r--r--  2.0 unx     5875 b- defN 24-Apr-02 15:44 libsrg/LoggingCounter.py
 -rw-r--r--  2.0 unx      413 b- defN 23-Jan-31 15:26 libsrg/LoggingUtils.py
 -rw-r--r--  2.0 unx     1376 b- defN 23-Jan-08 15:03 libsrg/LoggingWatcher.py
 -rw-r--r--  2.0 unx     2680 b- defN 23-Jan-31 15:30 libsrg/NagiosBase.py
@@ -17,13 +17,13 @@
 -rw-r--r--  2.0 unx     1027 b- defN 24-Feb-08 14:35 libsrg/template.py
 -rw-r--r--  2.0 unx    26527 b- defN 24-Jan-08 17:22 libsrg/ztool.py
 -rw-r--r--  2.0 unx     2214 b- defN 23-Feb-05 15:02 libsrg/TKGUI/GuiBase.py
 -rw-r--r--  2.0 unx      447 b- defN 22-Mar-14 16:04 libsrg/TKGUI/GuiRequest.py
 -rw-r--r--  2.0 unx     3414 b- defN 23-Feb-05 15:22 libsrg/TKGUI/GuiRequestQueue.py
 -rw-r--r--  2.0 unx    10692 b- defN 23-May-15 18:18 libsrg/TKGUI/LoggerGUI.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Jan-31 17:16 libsrg/TKGUI/__init__.py
--rw-rw-rw-  2.0 unx     1069 b- defN 24-Apr-02 15:57 libsrg-3.8.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3357 b- defN 24-Apr-02 15:57 libsrg-3.8.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 15:57 libsrg-3.8.4.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        7 b- defN 24-Apr-02 15:57 libsrg-3.8.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2092 b- defN 24-Apr-02 15:57 libsrg-3.8.4.dist-info/RECORD
-27 files, 114425 bytes uncompressed, 34141 bytes compressed:  70.2%
+-rw-rw-rw-  2.0 unx     1069 b- defN 24-Apr-02 16:11 libsrg-3.8.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3357 b- defN 24-Apr-02 16:11 libsrg-3.8.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 16:11 libsrg-3.8.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        7 b- defN 24-Apr-02 16:11 libsrg-3.8.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2092 b- defN 24-Apr-02 16:11 libsrg-3.8.5.dist-info/RECORD
+27 files, 114420 bytes uncompressed, 34143 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -60,23 +60,23 @@
 
 Filename: libsrg/TKGUI/LoggerGUI.py
 Comment: 
 
 Filename: libsrg/TKGUI/__init__.py
 Comment: 
 
-Filename: libsrg-3.8.4.dist-info/LICENSE.txt
+Filename: libsrg-3.8.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: libsrg-3.8.4.dist-info/METADATA
+Filename: libsrg-3.8.5.dist-info/METADATA
 Comment: 
 
-Filename: libsrg-3.8.4.dist-info/WHEEL
+Filename: libsrg-3.8.5.dist-info/WHEEL
 Comment: 
 
-Filename: libsrg-3.8.4.dist-info/top_level.txt
+Filename: libsrg-3.8.5.dist-info/top_level.txt
 Comment: 
 
-Filename: libsrg-3.8.4.dist-info/RECORD
+Filename: libsrg-3.8.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libsrg/Info.py

```diff
@@ -117,15 +117,15 @@
         self.like_redhat = self.like_fedora or self.like_rhel
 
         self.uid = os.getuid()
         bios = "ARM" if "aarch64" in self.machine else "BIOS"
         # These next few Runner calls may return non zero status
         rhow = Runner(f"test -d /sys/firmware/efi", userat=self.userat, rethrow=True, timeout=timeout, throw=True,
                       retries=retries)
-        self.boot_mode = "UEFI" if rhow.success else bios
+        self.uefi = "UEFI" if rhow.success else bios
 
         r2 = Runner("grep 'exclude=kernel' /etc/dnf/dnf.conf", userat=self.userat, rethrow=False, timeout=timeout,
                     throw=False, retries=retries)
         ret = r2.ret
         if ret == 0:
             self.kernel_dnf = "locked"
         elif ret == 1:
```

## Comparing `libsrg-3.8.4.dist-info/LICENSE.txt` & `libsrg-3.8.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `libsrg-3.8.4.dist-info/METADATA` & `libsrg-3.8.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsrg
-Version: 3.8.4
+Version: 3.8.5
 Summary: Base class for logging apps, Nagios, utilities
 Home-page: https://gitlab.com/SRG_gitlab/libsrg
 Author: Steven Goncalo
 Author-email: srg_pypi@ice9mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `libsrg-3.8.4.dist-info/RECORD` & `libsrg-3.8.5.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 libsrg/AppTemplate.py,sha256=539vznudLggwi-PtQIljiMlsQWIXMZ5ruSMQ3SGqNNM,1027
 libsrg/ElapsedTime.py,sha256=m-DxzdpfbElWAPpC0aZXWfrAOODUDb0I-x4w8FWlrZw,1878
-libsrg/Info.py,sha256=0b5hU-Hc8Vut-04fppvPAMwGCWhMKWLkBc7wVsf3QH4,6514
+libsrg/Info.py,sha256=O_VPtKLusFvxSXTAY8ht-TGsRWhSYUp2eTAnYFG0_sc,6509
 libsrg/LevelBanner.py,sha256=k2JC41LkQz9_bPCiGhejqkd7SO7_fiuBmo4Y_ETW9H4,3532
 libsrg/LoggerGUIProxy.py,sha256=qrgLnB0Gtmu5IXP9EzBpIpKWYphcVVQOmIpqWOH9Y6k,1492
 libsrg/LoggingAppBase.py,sha256=7-eaWR0QyPbpG7MSb_56lEsYREbQnKpJFypRM3o0fcQ,6093
 libsrg/LoggingCounter.py,sha256=42YlyNOvebDk9c1kXhSzklPD-nlzxDz6DkwfApw8p80,5875
 libsrg/LoggingUtils.py,sha256=brhP-2YaCd69vI0CKWTFUZtiTRhj1ud4i-tApP4FWg0,413
 libsrg/LoggingWatcher.py,sha256=tZ803wbw_qvW8tSRDwAbBRQSCrMzhz-FIJsf_hCNIFo,1376
 libsrg/NagiosBase.py,sha256=5FniCUJ8ywFX8oM2q0gKQX2Wvz6J6yt0HT_WYfPniik,2680
@@ -16,12 +16,12 @@
 libsrg/template.py,sha256=539vznudLggwi-PtQIljiMlsQWIXMZ5ruSMQ3SGqNNM,1027
 libsrg/ztool.py,sha256=vnBTbN6cTqaTF6JukVeoOBrXJ3eCu1uIv3qhBrUAGzo,26527
 libsrg/TKGUI/GuiBase.py,sha256=MG4D10voRxszQvglABmHG8GHqRNXNo6gWZmY77fpkGU,2214
 libsrg/TKGUI/GuiRequest.py,sha256=ZrUBxrpkAV8ITqbcr7br0-sX9iK69bx1_Fu7COKB5uc,447
 libsrg/TKGUI/GuiRequestQueue.py,sha256=SLoT-PdXgK4JgU-WcESlRwehZIEPBwRgPORn0Tm8Mws,3414
 libsrg/TKGUI/LoggerGUI.py,sha256=A2XBTtlvtNwnxFlw8xTkHkuCITxvgZlQfWjWeaAmejQ,10692
 libsrg/TKGUI/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-libsrg-3.8.4.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
-libsrg-3.8.4.dist-info/METADATA,sha256=2TM0LxGU-EKv5ck5lC4NwxfO0V8nd-A-bFJfc1YTb_c,3357
-libsrg-3.8.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-libsrg-3.8.4.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
-libsrg-3.8.4.dist-info/RECORD,,
+libsrg-3.8.5.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
+libsrg-3.8.5.dist-info/METADATA,sha256=8pGmidDImrGXeQz4jNbv2igl9_TC1RHGcM4WMTgEb20,3357
+libsrg-3.8.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+libsrg-3.8.5.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
+libsrg-3.8.5.dist-info/RECORD,,
```

