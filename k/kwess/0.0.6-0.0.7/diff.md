# Comparing `tmp/kwess-0.0.6.tar.gz` & `tmp/kwess-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Me\forge\python\PyPi Sandbox\questrade_api - clean - PyPi\dist\.tmp-51vpu_2t\kwess-0.0.6.tar", last modified: Sun Mar 24 01:26:31 2024, max compression
+gzip compressed data, was "C:\Users\Me\forge\python\PyPi Sandbox\questrade_api - clean - PyPi\dist\.tmp-39ob1ctc\kwess-0.0.7.tar", last modified: Tue Apr  2 02:59:45 2024, max compression
```

## Comparing `kwess-0.0.6.tar` & `kwess-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 01:26:31.877695 kwess-0.0.6/
--rw-rw-rw-   0        0        0    35821 2022-04-25 03:27:08.000000 kwess-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0    19849 2024-03-24 01:26:31.877695 kwess-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    19048 2024-03-23 18:16:39.000000 kwess-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-03-24 01:26:31.830809 kwess-0.0.6/kwess/
--rw-rw-rw-   0        0        0    43954 2024-03-18 03:50:44.000000 kwess-0.0.6/kwess/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-24 01:26:31.877695 kwess-0.0.6/kwess.egg-info/
--rw-rw-rw-   0        0        0    19849 2024-03-24 01:26:31.000000 kwess-0.0.6/kwess.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-03-24 01:26:31.000000 kwess-0.0.6/kwess.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 01:26:31.000000 kwess-0.0.6/kwess.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-03-24 01:26:31.000000 kwess-0.0.6/kwess.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-24 01:26:31.000000 kwess-0.0.6/kwess.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-11-01 03:16:40.000000 kwess-0.0.6/kwess.egg-info/zip-safe
--rw-rw-rw-   0        0        0       86 2022-04-21 23:21:52.000000 kwess-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0     1006 2024-03-24 01:26:31.893293 kwess-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 02:59:45.636212 kwess-0.0.7/
+-rw-rw-rw-   0        0        0    35821 2022-04-25 03:27:08.000000 kwess-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0    19939 2024-04-02 02:59:45.633754 kwess-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    19138 2024-04-02 02:57:11.000000 kwess-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 02:59:45.593476 kwess-0.0.7/kwess/
+-rw-rw-rw-   0        0        0    43967 2024-04-02 02:57:46.000000 kwess-0.0.7/kwess/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 02:59:45.631754 kwess-0.0.7/kwess.egg-info/
+-rw-rw-rw-   0        0        0    19939 2024-04-02 02:59:45.000000 kwess-0.0.7/kwess.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-04-02 02:59:45.000000 kwess-0.0.7/kwess.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 02:59:45.000000 kwess-0.0.7/kwess.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-02 02:59:45.000000 kwess-0.0.7/kwess.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 02:59:45.000000 kwess-0.0.7/kwess.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-11-01 03:16:40.000000 kwess-0.0.7/kwess.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       86 2022-04-21 23:21:52.000000 kwess-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1006 2024-04-02 02:59:45.646851 kwess-0.0.7/setup.cfg
```

### Comparing `kwess-0.0.6/LICENSE.txt` & `kwess-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kwess-0.0.6/PKG-INFO` & `kwess-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwess
-Version: 0.0.6
+Version: 0.0.7
 Summary: Questrade API wrapper.
 Home-page: https://github.com/kaiyoux/kwess
 Author: Issa Lompo
 Author-email: kaiyoux@gmail.com
 Maintainer: Issa Lompo
 Maintainer-email: kaiyoux@gmail.com
 License: GNU General Public License v3 (GPLv3)
@@ -52,14 +52,15 @@
 # Get account activities from 1/12/1999 to 28/9/2022
 accs = qs.get_account_activities(startdatetime=dt(year=1999, month=12, day=1), \
 enddatetime=dt(year=2022, month=9, day=28), verbose="xxx")
 for acc in accs:
     print(acc, "\n")
 
 # Get (all types of) TFSA account orders from 17/8/2022 to now
+# Questrade does not seem to keep old account orders - only the most recent
 accs = qs.get_account_orders(startdatetime=dt(year=2022, month=8, day=17), \
 verbose="vv")
 for acc in accs:
     print(acc, "\n")
 
 # Get margin account orders that are still open
 accs = qs.get_account_orders(accounttype="margin", startdatetime=dt(year=2022, \
@@ -155,29 +156,29 @@
     in the local file referred to by rt_file.
 Parameters:
     - rt_file name of your local file containing your refresh token.
     Defaults to "refreshToken".
     - server_type could be 2 possible values: "live" or "test". 
     "live" will allow you to interact with your real Questrade account. 
     "test" is for interacting with your test account.
-    - timeout number of seconds to wait for the API server to respond before 
+    - timeout number of seconds to wait for the server to respond before 
     giving up.
     Defaults to 15 seconds. Set timeout to None if you wish to wait forever 
     for a response.
     - verbose level of verbosity represented by the number of characters in a string.
     Defaults to empty string. Maximum verbosity is 1 or "v".
 Returns:
     Trader object.
 
 
 build_datetime_string(self, adatetime=None, gmt=False)
 Description:
     Higher level helper method used to build a Questrade datetime string.
 Parameters:
-    - adatetime a datetime object.
+    - adatetime a datetime object. Defaults to now.
     - gmt optional boolean indicating if datetime is Greenwich Mean Time.
     Default value is False.
 Returns:
     A Questrade datetime string.
 
 
 find_account_number(self, accounttype)
@@ -218,16 +219,16 @@
     - verbose level of verbosity represented by the number of characters in 
     a string. 
     Defaults to empty string. Maximum verbosity is 2 or "vv".
 Returns:
     Account balances as a Python object representation of the returned json.
 
 
-get_account_executions(self, accounttype='TFSA', startdatetime=None, 
-enddatetime=None, verbose='')
+get_account_executions(self, startdatetime, enddatetime=None, 
+accounttype='TFSA', verbose='')
 Description:
     Generator that provides account executions from the account related to 
     account type accounttype, between the range specified by startdatetime and 
     enddatetime. Both objects are datetime objects.
 Parameters:
     - startdatetime datetime object representing the beginning of a range.
     - enddatetime datetime object representing the end of a range.
@@ -300,15 +301,15 @@
     - verbose level of verbosity represented by the number of characters in a string.
     Defaults to empty string. Maximum verbosity is 1 or "v".
 Yields:
     All your Questrade accounts as a Python object representation of the returned 
     json.
 
 
-get_market_candles(self, sid, interval, startdatetime=None, enddatetime=None, 
+get_market_candles(self, sid, interval, startdatetime, enddatetime=None, 
 verbose='')
 Description:
     Provides a list of json formatted market candles.
 Parameters:
     - sid symbol id as a string or numeral.
     - interval is the Historical Data Granularity.
     Examples: "OneMinute", "HalfHour", "OneYear".
@@ -376,15 +377,15 @@
 Returns:
     Information about supported markets as a Python object representation of 
     the returned json.
 
 
 get_new_refresh_token(self, token, server_type, verbose='')
 Description:
-    Obtains a new refresh token (and new access token) from the API server.
+    Obtains a new refresh token (and new access token) from the Authorization server.
     You generally would not need to call this method, as it is potentially called by
     Trader during initialization.
     Trader will only call this method if the access token has expired.
 Parameters:
     - token the refresh token that is stored in the local file pointed to by rt_file.
     - server_type should be "live" or "test" for your live Questrade account or 
     your test Questrade account, respectively.
```

### Comparing `kwess-0.0.6/README.md` & `kwess-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 # Get account activities from 1/12/1999 to 28/9/2022
 accs = qs.get_account_activities(startdatetime=dt(year=1999, month=12, day=1), \
 enddatetime=dt(year=2022, month=9, day=28), verbose="xxx")
 for acc in accs:
     print(acc, "\n")
 
 # Get (all types of) TFSA account orders from 17/8/2022 to now
+# Questrade does not seem to keep old account orders - only the most recent
 accs = qs.get_account_orders(startdatetime=dt(year=2022, month=8, day=17), \
 verbose="vv")
 for acc in accs:
     print(acc, "\n")
 
 # Get margin account orders that are still open
 accs = qs.get_account_orders(accounttype="margin", startdatetime=dt(year=2022, \
@@ -133,29 +134,29 @@
     in the local file referred to by rt_file.
 Parameters:
     - rt_file name of your local file containing your refresh token.
     Defaults to "refreshToken".
     - server_type could be 2 possible values: "live" or "test". 
     "live" will allow you to interact with your real Questrade account. 
     "test" is for interacting with your test account.
-    - timeout number of seconds to wait for the API server to respond before 
+    - timeout number of seconds to wait for the server to respond before 
     giving up.
     Defaults to 15 seconds. Set timeout to None if you wish to wait forever 
     for a response.
     - verbose level of verbosity represented by the number of characters in a string.
     Defaults to empty string. Maximum verbosity is 1 or "v".
 Returns:
     Trader object.
 
 
 build_datetime_string(self, adatetime=None, gmt=False)
 Description:
     Higher level helper method used to build a Questrade datetime string.
 Parameters:
-    - adatetime a datetime object.
+    - adatetime a datetime object. Defaults to now.
     - gmt optional boolean indicating if datetime is Greenwich Mean Time.
     Default value is False.
 Returns:
     A Questrade datetime string.
 
 
 find_account_number(self, accounttype)
@@ -196,16 +197,16 @@
     - verbose level of verbosity represented by the number of characters in 
     a string. 
     Defaults to empty string. Maximum verbosity is 2 or "vv".
 Returns:
     Account balances as a Python object representation of the returned json.
 
 
-get_account_executions(self, accounttype='TFSA', startdatetime=None, 
-enddatetime=None, verbose='')
+get_account_executions(self, startdatetime, enddatetime=None, 
+accounttype='TFSA', verbose='')
 Description:
     Generator that provides account executions from the account related to 
     account type accounttype, between the range specified by startdatetime and 
     enddatetime. Both objects are datetime objects.
 Parameters:
     - startdatetime datetime object representing the beginning of a range.
     - enddatetime datetime object representing the end of a range.
@@ -278,15 +279,15 @@
     - verbose level of verbosity represented by the number of characters in a string.
     Defaults to empty string. Maximum verbosity is 1 or "v".
 Yields:
     All your Questrade accounts as a Python object representation of the returned 
     json.
 
 
-get_market_candles(self, sid, interval, startdatetime=None, enddatetime=None, 
+get_market_candles(self, sid, interval, startdatetime, enddatetime=None, 
 verbose='')
 Description:
     Provides a list of json formatted market candles.
 Parameters:
     - sid symbol id as a string or numeral.
     - interval is the Historical Data Granularity.
     Examples: "OneMinute", "HalfHour", "OneYear".
@@ -354,15 +355,15 @@
 Returns:
     Information about supported markets as a Python object representation of 
     the returned json.
 
 
 get_new_refresh_token(self, token, server_type, verbose='')
 Description:
-    Obtains a new refresh token (and new access token) from the API server.
+    Obtains a new refresh token (and new access token) from the Authorization server.
     You generally would not need to call this method, as it is potentially called by
     Trader during initialization.
     Trader will only call this method if the access token has expired.
 Parameters:
     - token the refresh token that is stored in the local file pointed to by rt_file.
     - server_type should be "live" or "test" for your live Questrade account or 
     your test Questrade account, respectively.
```

### Comparing `kwess-0.0.6/kwess/__init__.py` & `kwess-0.0.7/kwess/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             in the local file referred to by rt_file.
         Parameters:
             - rt_file name of your local file containing your refresh token.
             Defaults to "refreshToken".
             - server_type could be 2 possible values: "live" or "test". "live" will allow you to
             interact with your real Questrade account. "test" is for interacting with your test
             account.
-            - timeout number of seconds to wait for the API server to respond before giving up.
+            - timeout number of seconds to wait for the server to respond before giving up.
             Defaults to 15 seconds. Set timeout to None if you wish to wait forever for a response.
             - verbose level of verbosity represented by the number of characters in a string.
             Defaults to empty string. Maximum verbosity is 1 or "v".
         Returns:
             Trader object.
         """
         self.server_url  = {
@@ -84,15 +84,15 @@
                 print(f"Please log into your Questrade account (APP HUB), generate a new token for manual authorization, and save that token in local file {self.rt_file}, then try again.")
                 sys.exit(1)
             
 
     def get_new_refresh_token(self, token, verbose=''):
         """
         Description:
-            Obtains a new refresh token (and new access token) from the API server.
+            Obtains a new refresh token (and new access token) from the Authorization server.
             You generally would not need to call this method, as it is potentially called by Trader
             during initialization.
             Trader will only call this method if the access token has expired.
         Parameters:
             - token the refresh token that is stored in the local file pointed to by rt_file.
             - verbose level of verbosity represented by the number of characters in a string.
             Defaults to empty string. Maximum verbosity is 1 or "v".
@@ -227,16 +227,16 @@
         """ Description:
                 Generator that returns the account activities from the account related to account
                 type accounttype, 
                 between the range specified by startdatetime and enddatetime. Both objects are
                 datetime objects.
             Parameters:
                 - startdatetime datetime object specifying the start of a range.
-                - enddatetime optional datetime object specifying the end of a range. Defaults to
-                now (datetime.datetime.now()) if not specified.
+                - enddatetime optional datetime object specifying the end of a range.
+                Defaults to now (datetime.datetime.now()) if not specified.
                 - accounttype type of Questrade account. Defaults to "tfsa".
                 - verbose level of verbosity represented by the number of characters in a string.
                 Defaults to empty string. Maximum verbosity is 3 or "vvv".
             Returns:
                 The account activities as a Python object representation of the returned json,
                 between the range startdatetime and enddatetime, in chunks of 30 days.
         """
@@ -330,15 +330,15 @@
 
                             
     def build_datetime_string(self, adatetime=None, gmt=False):
         """
         Description:
             Higher level helper method used to build a Questrade datetime string.
         Parameters:
-            - adatetime a datetime object.
+            - adatetime a datetime object. Defaults to now.
             - gmt optional boolean indicating if datetime is Greenwich Mean Time.
             Default value is False.
         Returns:
             A Questrade datetime string.
         """
         if adatetime is None:
             d2 = dt.now()
@@ -450,15 +450,15 @@
 
         if verbosity > 0:
             pprint(resp.json())
         return resp.json()
     
 
     @get_all
-    def get_account_executions(self, accounttype="TFSA", startdatetime=None, enddatetime=None, verbose=''):
+    def get_account_executions(self, startdatetime, enddatetime=None, accounttype="TFSA", verbose=''):
         """
         Description:
             Generator that provides account executions from the account related to account type
             accounttype, 
             between the range specified by startdatetime and enddatetime.
             Both objects are datetime objects.
         Parameters:
@@ -584,15 +584,15 @@
         rd = resp.json()
         if verbosity > 0:
             pprint(dt.strptime(rd["time"][:-13], '%Y-%m-%dT%X'))
         return dt.strptime(rd["time"][:-13], '%Y-%m-%dT%X'), rd
 
 
     @get_all
-    def get_market_candles(self, sid, interval, startdatetime=None, enddatetime=None, verbose=''):
+    def get_market_candles(self, sid, interval, startdatetime, enddatetime=None, verbose=''):
         """
         Description:
             Provides a list of json formatted market candles.
         Parameters:
             - sid symbol id as a string or numeral.
             - interval is the Historical Data Granularity.
             Examples: "OneMinute", "HalfHour", "OneYear".
```

### Comparing `kwess-0.0.6/kwess.egg-info/PKG-INFO` & `kwess-0.0.7/kwess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwess
-Version: 0.0.6
+Version: 0.0.7
 Summary: Questrade API wrapper.
 Home-page: https://github.com/kaiyoux/kwess
 Author: Issa Lompo
 Author-email: kaiyoux@gmail.com
 Maintainer: Issa Lompo
 Maintainer-email: kaiyoux@gmail.com
 License: GNU General Public License v3 (GPLv3)
@@ -52,14 +52,15 @@
 # Get account activities from 1/12/1999 to 28/9/2022
 accs = qs.get_account_activities(startdatetime=dt(year=1999, month=12, day=1), \
 enddatetime=dt(year=2022, month=9, day=28), verbose="xxx")
 for acc in accs:
     print(acc, "\n")
 
 # Get (all types of) TFSA account orders from 17/8/2022 to now
+# Questrade does not seem to keep old account orders - only the most recent
 accs = qs.get_account_orders(startdatetime=dt(year=2022, month=8, day=17), \
 verbose="vv")
 for acc in accs:
     print(acc, "\n")
 
 # Get margin account orders that are still open
 accs = qs.get_account_orders(accounttype="margin", startdatetime=dt(year=2022, \
@@ -155,29 +156,29 @@
     in the local file referred to by rt_file.
 Parameters:
     - rt_file name of your local file containing your refresh token.
     Defaults to "refreshToken".
     - server_type could be 2 possible values: "live" or "test". 
     "live" will allow you to interact with your real Questrade account. 
     "test" is for interacting with your test account.
-    - timeout number of seconds to wait for the API server to respond before 
+    - timeout number of seconds to wait for the server to respond before 
     giving up.
     Defaults to 15 seconds. Set timeout to None if you wish to wait forever 
     for a response.
     - verbose level of verbosity represented by the number of characters in a string.
     Defaults to empty string. Maximum verbosity is 1 or "v".
 Returns:
     Trader object.
 
 
 build_datetime_string(self, adatetime=None, gmt=False)
 Description:
     Higher level helper method used to build a Questrade datetime string.
 Parameters:
-    - adatetime a datetime object.
+    - adatetime a datetime object. Defaults to now.
     - gmt optional boolean indicating if datetime is Greenwich Mean Time.
     Default value is False.
 Returns:
     A Questrade datetime string.
 
 
 find_account_number(self, accounttype)
@@ -218,16 +219,16 @@
     - verbose level of verbosity represented by the number of characters in 
     a string. 
     Defaults to empty string. Maximum verbosity is 2 or "vv".
 Returns:
     Account balances as a Python object representation of the returned json.
 
 
-get_account_executions(self, accounttype='TFSA', startdatetime=None, 
-enddatetime=None, verbose='')
+get_account_executions(self, startdatetime, enddatetime=None, 
+accounttype='TFSA', verbose='')
 Description:
     Generator that provides account executions from the account related to 
     account type accounttype, between the range specified by startdatetime and 
     enddatetime. Both objects are datetime objects.
 Parameters:
     - startdatetime datetime object representing the beginning of a range.
     - enddatetime datetime object representing the end of a range.
@@ -300,15 +301,15 @@
     - verbose level of verbosity represented by the number of characters in a string.
     Defaults to empty string. Maximum verbosity is 1 or "v".
 Yields:
     All your Questrade accounts as a Python object representation of the returned 
     json.
 
 
-get_market_candles(self, sid, interval, startdatetime=None, enddatetime=None, 
+get_market_candles(self, sid, interval, startdatetime, enddatetime=None, 
 verbose='')
 Description:
     Provides a list of json formatted market candles.
 Parameters:
     - sid symbol id as a string or numeral.
     - interval is the Historical Data Granularity.
     Examples: "OneMinute", "HalfHour", "OneYear".
@@ -376,15 +377,15 @@
 Returns:
     Information about supported markets as a Python object representation of 
     the returned json.
 
 
 get_new_refresh_token(self, token, server_type, verbose='')
 Description:
-    Obtains a new refresh token (and new access token) from the API server.
+    Obtains a new refresh token (and new access token) from the Authorization server.
     You generally would not need to call this method, as it is potentially called by
     Trader during initialization.
     Trader will only call this method if the access token has expired.
 Parameters:
     - token the refresh token that is stored in the local file pointed to by rt_file.
     - server_type should be "live" or "test" for your live Questrade account or 
     your test Questrade account, respectively.
```

### Comparing `kwess-0.0.6/setup.cfg` & `kwess-0.0.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206b 7765 7373 0d0a 7665 7273 696f   = kwess..versio
-00000020: 6e20 3d20 302e 302e 360d 0a61 7574 686f  n = 0.0.6..autho
+00000020: 6e20 3d20 302e 302e 370d 0a61 7574 686f  n = 0.0.7..autho
 00000030: 7220 3d20 4973 7361 204c 6f6d 706f 0d0a  r = Issa Lompo..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 206b  author_email = k
 00000050: 6169 796f 7578 4067 6d61 696c 2e63 6f6d  aiyoux@gmail.com
 00000060: 0d0a 6d61 696e 7461 696e 6572 203d 2049  ..maintainer = I
 00000070: 7373 6120 4c6f 6d70 6f0d 0a6d 6169 6e74  ssa Lompo..maint
 00000080: 6169 6e65 725f 656d 6169 6c20 3d20 6b61  ainer_email = ka
 00000090: 6979 6f75 7840 676d 6169 6c2e 636f 6d0d  iyoux@gmail.com.
```

