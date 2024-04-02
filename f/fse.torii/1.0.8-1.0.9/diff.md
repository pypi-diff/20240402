# Comparing `tmp/fse.torii-1.0.8-py3-none-any.whl.zip` & `tmp/fse.torii-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 64151 bytes, number of entries: 49
+Zip file size: 64181 bytes, number of entries: 49
 -rw-rw----  2.0 unx      135 b- defN 24-Feb-05 09:46 torii/__init__.py
 -rw-rw----  2.0 unx      209 b- defN 22-Mar-31 12:08 torii/exception.py
 -rw-rw----  2.0 unx      497 b- defN 22-Mar-31 12:08 torii/generate_doc.py
 -rw-rw----  2.0 unx      401 b- defN 22-Mar-31 12:08 torii/generate_pythonApi_doc.py
 -rw-rw----  2.0 unx    19060 b- defN 24-Feb-05 09:46 torii/torii_main.py
 -rw-rw----  2.0 unx        0 b- defN 24-Feb-05 09:46 torii/dao/__init__.py
 -rw-rw----  2.0 unx     9905 b- defN 24-Feb-05 09:46 torii/dao/abstract_dao.py
@@ -23,15 +23,15 @@
 -rw-rw----  2.0 unx     4906 b- defN 22-Mar-31 12:08 torii/executor/executor.py
 -rw-rw----  2.0 unx    11005 b- defN 22-Mar-31 12:08 torii/executor/job_executor.py
 -rw-rw----  2.0 unx     3895 b- defN 22-Mar-31 12:08 torii/executor/notification_manager.py
 -rw-rw----  2.0 unx     7933 b- defN 22-Mar-31 12:08 torii/executor/offline_task_service.py
 -rw-rw----  2.0 unx     8549 b- defN 22-Mar-31 12:08 torii/executor/picom_executor.py
 -rw-rw----  2.0 unx     5429 b- defN 22-Mar-31 12:08 torii/executor/policy_executor.py
 -rw-rw----  2.0 unx        0 b- defN 24-Feb-05 09:46 torii/managers/__init__.py
--rw-rw----  2.0 unx     1897 b- defN 24-Feb-05 09:46 torii/managers/dao_manager.py
+-rw-rw----  2.0 unx     2043 b- defN 24-Feb-05 14:51 torii/managers/dao_manager.py
 -rw-rw----  2.0 unx     3469 b- defN 24-Feb-05 09:46 torii/managers/user_manager.py
 -rw-rw----  2.0 unx      943 b- defN 22-Mar-31 12:08 torii/services/__init__.py
 -rw-rw----  2.0 unx     3894 b- defN 22-Mar-31 12:08 torii/services/addon_service.py
 -rw-rw----  2.0 unx     3374 b- defN 22-Mar-31 12:08 torii/services/ai_service.py
 -rw-rw----  2.0 unx    24330 b- defN 24-Feb-05 09:46 torii/services/application_service.py
 -rw-rw----  2.0 unx      403 b- defN 24-Feb-05 09:46 torii/services/bo_service.py
 -rw-rw----  2.0 unx     1874 b- defN 24-Feb-05 09:46 torii/services/bs_service.py
@@ -40,12 +40,12 @@
 -rw-rw----  2.0 unx      476 b- defN 22-Mar-31 12:08 torii/services/organisation_service.py
 -rw-rw----  2.0 unx      333 b- defN 22-Mar-31 12:08 torii/services/picom_service.py
 -rw-rw----  2.0 unx     2890 b- defN 22-Mar-31 12:08 torii/services/profile_service.py
 -rw-rw----  2.0 unx     8102 b- defN 24-Feb-05 09:46 torii/services/service.py
 -rw-rw----  2.0 unx     4950 b- defN 24-Feb-05 09:46 torii/services/session_service.py
 -rw-rw----  2.0 unx    11633 b- defN 22-Mar-31 12:08 torii/services/task_service.py
 -rw-rw----  2.0 unx    17032 b- defN 24-Feb-05 09:46 torii/services/torii_service.py
--rw-rw----  2.0 unx      252 b- defN 24-Feb-05 10:09 fse.torii-1.0.8.dist-info/METADATA
--rw-rw----  2.0 unx       92 b- defN 24-Feb-05 10:09 fse.torii-1.0.8.dist-info/WHEEL
--rw-rw----  2.0 unx        6 b- defN 24-Feb-05 10:09 fse.torii-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4086 b- defN 24-Feb-05 10:09 fse.torii-1.0.8.dist-info/RECORD
-49 files, 223590 bytes uncompressed, 57667 bytes compressed:  74.2%
+-rw-rw----  2.0 unx      252 b- defN 24-Feb-05 14:53 fse.torii-1.0.9.dist-info/METADATA
+-rw-rw----  2.0 unx       92 b- defN 24-Feb-05 14:53 fse.torii-1.0.9.dist-info/WHEEL
+-rw-rw----  2.0 unx        6 b- defN 24-Feb-05 14:53 fse.torii-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4086 b- defN 24-Feb-05 14:53 fse.torii-1.0.9.dist-info/RECORD
+49 files, 223736 bytes uncompressed, 57697 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -129,20 +129,20 @@
 
 Filename: torii/services/task_service.py
 Comment: 
 
 Filename: torii/services/torii_service.py
 Comment: 
 
-Filename: fse.torii-1.0.8.dist-info/METADATA
+Filename: fse.torii-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: fse.torii-1.0.8.dist-info/WHEEL
+Filename: fse.torii-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: fse.torii-1.0.8.dist-info/top_level.txt
+Filename: fse.torii-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: fse.torii-1.0.8.dist-info/RECORD
+Filename: fse.torii-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torii/managers/dao_manager.py

```diff
@@ -16,15 +16,18 @@
     }
 
     def __init__(self, torii):
         self._torii = torii
         self._logger = logging.getLogger('torii')
 
         for key, bo in self.services.items():
-            self.services[key] = bo(torii)
+            try:
+                self.services[key] = bo(torii)
+            except Exception as e:
+                self._logger.info(f'Error instantiating service {bo} in DAO Manager:', e)
 
     def run_service(self, intent: str, path: str, params=None, json=None, data=None, files=None, timeout=None):
         """
         Runs the intended service corresponding to the given intent and path.
         Passes the defined arguments to the service.
 
         :param intent: The Http method (GET, POST, PUT, DELETE or PATCH).
```

## Comparing `fse.torii-1.0.8.dist-info/RECORD` & `fse.torii-1.0.9.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 torii/executor/executor.py,sha256=jtP0yJ5Z8FdRhFUPs2RYr708f2Kc5MWfLcqP75-jWA8,4906
 torii/executor/job_executor.py,sha256=TbUyCFLkDBSIyqltGJs9r9zxE-HU5iTSuA3MAOsh6gk,11005
 torii/executor/notification_manager.py,sha256=Vj_z7uSJw2apcAi2lgdUQTwWh6VtcB-F0IQb-w_3j6A,3895
 torii/executor/offline_task_service.py,sha256=5OOfA0vImP2U2y1WB5qxgrI6yGrcVQUx7g8urcqAmno,7933
 torii/executor/picom_executor.py,sha256=X8X7ascUgzVM62LB_9Jsq0uK07AbRkajlUszUpHEMKo,8549
 torii/executor/policy_executor.py,sha256=qD7Gs9o5iKW_t9zbszBzMHpNyxTHQxuxCzwlHyJS88U,5429
 torii/managers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-torii/managers/dao_manager.py,sha256=aTcqAQBU6MgYaJdzRP5zMVNJdvQBvspGVsFsYQKqDoc,1897
+torii/managers/dao_manager.py,sha256=GtAks53fd2A5Dr9-brWyXrAmMf2Y6vzMCEqaWA2cGwQ,2043
 torii/managers/user_manager.py,sha256=7q4ufJ8hHXZiHQ8L8kV_3OQfuwM5sCCFdAvDGNaUpFw,3469
 torii/services/__init__.py,sha256=bEGGVUoL0NU8uWkC6faJXRNlIVmEdZVEEcqV7wc8Ibg,943
 torii/services/addon_service.py,sha256=owIWwdcILMfN0LdNp5SBcRRS7g4R4mD-HcqicjNeBEE,3894
 torii/services/ai_service.py,sha256=a_Xz5c58tFGolxuPWLifs6yLrmjO3oPFD9S6TEB2WUs,3374
 torii/services/application_service.py,sha256=GwB_6Mok2nL1-xJ7BYQe8G0upZuB4HUIW8zR0jEwLHg,24330
 torii/services/bo_service.py,sha256=lBBSzxUcdvIEvg22eXDeskrdtof6hXoNLLLRZGqYL9U,403
 torii/services/bs_service.py,sha256=jhwSTsppC1lg9J3S4y2eJcIkLujqk3FKU2LTpaU84zc,1874
@@ -39,11 +39,11 @@
 torii/services/organisation_service.py,sha256=x9ZxOTT0HT-evPQquGcvnI9ojaIb9GRXs6TGLAViJ3c,476
 torii/services/picom_service.py,sha256=Lzn05huZjBlyy-R7DYiwgcRi20gy-1ABTcrpsHnmmCg,333
 torii/services/profile_service.py,sha256=5vjaYkQlFl82zymXqCuLj-Xh_AuojHmP_9cYJFqOt8o,2890
 torii/services/service.py,sha256=BEMks8AAZMFnd4Wr1VVS3aZmzbd9Yv8H8gsualPyk4w,8102
 torii/services/session_service.py,sha256=BhlomGSDLQgfH4SzoN2vDaUKfstEZwgHS2mUGqpR8EE,4950
 torii/services/task_service.py,sha256=9XTLzV2PlBt46nA2esOg4leN40HHOpELaSADEd0Km70,11633
 torii/services/torii_service.py,sha256=USVriJ9xcrk0dkZFphsZVm4kWaAiyfEHpeRBWoW1bk0,17032
-fse.torii-1.0.8.dist-info/METADATA,sha256=ZApNfFAmsp1xEo7zN3RO2oXhuZ4CtJ6HcN07Lx8vUEg,252
-fse.torii-1.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-fse.torii-1.0.8.dist-info/top_level.txt,sha256=wcDyeOaJvCCkeWf_b-xwJP40NmFCYD2e6WClxnLH7gI,6
-fse.torii-1.0.8.dist-info/RECORD,,
+fse.torii-1.0.9.dist-info/METADATA,sha256=_F3sFqTrKKPyLAyZD32IV_6pAv-9K-B4udtuwoWjiFo,252
+fse.torii-1.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+fse.torii-1.0.9.dist-info/top_level.txt,sha256=wcDyeOaJvCCkeWf_b-xwJP40NmFCYD2e6WClxnLH7gI,6
+fse.torii-1.0.9.dist-info/RECORD,,
```

