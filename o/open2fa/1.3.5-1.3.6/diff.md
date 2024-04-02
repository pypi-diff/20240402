# Comparing `tmp/open2fa-1.3.5-py3-none-any.whl.zip` & `tmp/open2fa-1.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 20613 bytes, number of entries: 17
+Zip file size: 20612 bytes, number of entries: 17
 -rw-r--r--  2.0 unx      113 b- defN 24-Feb-12 01:03 open2fa/__init__.py
 -rw-r--r--  2.0 unx    10069 b- defN 24-Mar-25 23:32 open2fa/cli.py
 -rw-r--r--  2.0 unx     4747 b- defN 24-Mar-19 13:19 open2fa/cli_utils.py
 -rw-r--r--  2.0 unx     4334 b- defN 24-Mar-24 22:21 open2fa/common.py
 -rw-r--r--  2.0 unx      659 b- defN 24-Feb-11 08:07 open2fa/config.py
 -rw-r--r--  2.0 unx      923 b- defN 24-Mar-21 19:32 open2fa/ex.py
 -rw-r--r--  2.0 unx    17929 b- defN 24-Mar-25 23:38 open2fa/main.py
 -rw-r--r--  2.0 unx     1742 b- defN 24-Mar-23 03:26 open2fa/msgs.py
 -rw-r--r--  2.0 unx     2289 b- defN 24-Mar-16 18:22 open2fa/totp.py
 -rw-r--r--  2.0 unx     2139 b- defN 24-Mar-21 19:36 open2fa/utils.py
--rw-r--r--  2.0 unx       22 b- defN 24-Mar-26 21:31 open2fa/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Mar-26 21:36 open2fa-1.3.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    11049 b- defN 24-Mar-26 21:36 open2fa-1.3.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-26 21:36 open2fa-1.3.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-Mar-26 21:36 open2fa-1.3.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-Mar-26 21:36 open2fa-1.3.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1284 b- defN 24-Mar-26 21:36 open2fa-1.3.5.dist-info/RECORD
-17 files, 58519 bytes uncompressed, 18543 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-02 21:53 open2fa/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-Apr-02 21:53 open2fa-1.3.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11046 b- defN 24-Apr-02 21:53 open2fa-1.3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 21:53 open2fa-1.3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-Apr-02 21:53 open2fa-1.3.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-02 21:53 open2fa-1.3.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1284 b- defN 24-Apr-02 21:53 open2fa-1.3.6.dist-info/RECORD
+17 files, 58516 bytes uncompressed, 18542 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: open2fa/utils.py
 Comment: 
 
 Filename: open2fa/version.py
 Comment: 
 
-Filename: open2fa-1.3.5.dist-info/LICENSE
+Filename: open2fa-1.3.6.dist-info/LICENSE
 Comment: 
 
-Filename: open2fa-1.3.5.dist-info/METADATA
+Filename: open2fa-1.3.6.dist-info/METADATA
 Comment: 
 
-Filename: open2fa-1.3.5.dist-info/WHEEL
+Filename: open2fa-1.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: open2fa-1.3.5.dist-info/entry_points.txt
+Filename: open2fa-1.3.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: open2fa-1.3.5.dist-info/top_level.txt
+Filename: open2fa-1.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: open2fa-1.3.5.dist-info/RECORD
+Filename: open2fa-1.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## open2fa/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.3.5"
+__version__ = "1.3.6"
```

## Comparing `open2fa-1.3.5.dist-info/LICENSE` & `open2fa-1.3.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `open2fa-1.3.5.dist-info/METADATA` & `open2fa-1.3.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open2fa
-Version: 1.3.5
+Version: 1.3.6
 Summary: A 2FA CLI tool for generating 2FA codes using TOTP secrets, with an optional SECURE remote api, and an optional web ui enabling 2FA code generation from any device
 Author-email: Cary Carter <ccarterdev@gmail.com>
 Project-URL: Homepage, https://open2fa.liberfy.ai
 Project-URL: Repository, https://github.com/cc-d/open2fa
 Project-URL: Issues, https://github.com/cc-d/open2fa/issues
 Project-URL: Server, https://github.com/cc-d/open2fa-server
 Project-URL: Documentation, https://github.com/cc-d/open2fa
@@ -19,15 +19,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: logfunc <=2.4.3
 Requires-Dist: cryptography <=41.0.7
-Requires-Dist: pyshared <=1.2.0
+Requires-Dist: pyshared <1.6
 Requires-Dist: base58 ==2.1.1
 Provides-Extra: dev
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-cov ; extra == 'dev'
 Requires-Dist: pytest-mock ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
```

## Comparing `open2fa-1.3.5.dist-info/RECORD` & `open2fa-1.3.6.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 open2fa/common.py,sha256=44pDlWVJhfGbCW_TczO7Urc_0JFpynfEkP6FJYd6r-Y,4334
 open2fa/config.py,sha256=EYO7Xn0rU8gBeH57zXb8W2uPspEVb5Xv18TrUnaGBhI,659
 open2fa/ex.py,sha256=nc_q0UdNdbk-KFR0XmcQbpdhtqbs1SnWcus4XzqAq70,923
 open2fa/main.py,sha256=1lZm1g3ZTNpt4YCOPsFvNINlY0dXf9IWuvnOqkRBA14,17929
 open2fa/msgs.py,sha256=iMBtZbL-a1zro4FgeYneo1Q6MsfNrGafCL-isbv38Qw,1742
 open2fa/totp.py,sha256=2t0qw9zGC3kdIhVFBvObNEWpw1-o8A6NYn1rFLe0RNo,2289
 open2fa/utils.py,sha256=j6Nom2zc51aDsY79d1sW6qmSyXrGirIa0cP7AE_wNDg,2139
-open2fa/version.py,sha256=tdqvkGH0OryRjjXzO3HS5DyYol-VTO9fC8m43nB2PgI,22
-open2fa-1.3.5.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
-open2fa-1.3.5.dist-info/METADATA,sha256=n6noFnszr4fVVoc78LpHXg5HJWvc-TweznogCADUUcU,11049
-open2fa-1.3.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-open2fa-1.3.5.dist-info/entry_points.txt,sha256=zPU8uscEguG4dPJRNgafME-18JtTcsovmVrjylRQcIU,52
-open2fa-1.3.5.dist-info/top_level.txt,sha256=c_HZ2KecVkcZ3f3dF-SOX7eyDBn9UpLe8IYmZZjXvdA,8
-open2fa-1.3.5.dist-info/RECORD,,
+open2fa/version.py,sha256=5ZbAQtod5QalTI1C2N07edlxplzG_Q2XvGOSyOok4uA,22
+open2fa-1.3.6.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
+open2fa-1.3.6.dist-info/METADATA,sha256=T4JJRQWE_YEhXAPZMqisUK1spkyoi3RyxKSBzKYBI7c,11046
+open2fa-1.3.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+open2fa-1.3.6.dist-info/entry_points.txt,sha256=zPU8uscEguG4dPJRNgafME-18JtTcsovmVrjylRQcIU,52
+open2fa-1.3.6.dist-info/top_level.txt,sha256=c_HZ2KecVkcZ3f3dF-SOX7eyDBn9UpLe8IYmZZjXvdA,8
+open2fa-1.3.6.dist-info/RECORD,,
```

