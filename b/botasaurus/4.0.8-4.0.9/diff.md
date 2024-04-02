# Comparing `tmp/botasaurus-4.0.8.tar.gz` & `tmp/botasaurus-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus-4.0.8.tar", last modified: Wed Mar 20 09:33:46 2024, max compression
+gzip compressed data, was "botasaurus-4.0.9.tar", last modified: Wed Mar 20 09:35:24 2024, max compression
```

## Comparing `botasaurus-4.0.8.tar` & `botasaurus-4.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 09:33:46.166781 botasaurus-4.0.8/
--rw-rw-rw-   0        0        0      222 2023-10-14 07:30:38.000000 botasaurus-4.0.8/AUTHORS
--rw-rw-rw-   0        0        0     1094 2024-03-03 08:47:03.000000 botasaurus-4.0.8/LICENSE
--rw-rw-rw-   0        0        0    54382 2024-03-20 09:33:46.165713 botasaurus-4.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    52343 2024-03-12 13:06:58.000000 botasaurus-4.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-20 09:33:46.124170 botasaurus-4.0.8/botasaurus/
--rw-rw-rw-   0        0        0      218 2024-02-27 02:47:12.000000 botasaurus-4.0.8/botasaurus/__init__.py
--rw-rw-rw-   0        0        0      223 2023-11-12 07:58:52.000000 botasaurus-4.0.8/botasaurus/_id.py
--rw-rw-rw-   0        0        0     1065 2023-12-13 10:40:15.000000 botasaurus-4.0.8/botasaurus/accept_google_cookies.py
--rw-rw-rw-   0        0        0    16521 2024-03-03 13:39:19.000000 botasaurus-4.0.8/botasaurus/anti_detect_driver.py
--rw-rw-rw-   0        0        0     4607 2024-03-20 09:03:25.000000 botasaurus-4.0.8/botasaurus/anti_detect_requests.py
--rw-rw-rw-   0        0        0     3681 2023-11-10 07:08:04.000000 botasaurus-4.0.8/botasaurus/base_data.py
--rw-rw-rw-   0        0        0      831 2023-11-13 08:37:04.000000 botasaurus-4.0.8/botasaurus/beep_utils.py
--rw-rw-rw-   0        0        0     2968 2024-01-26 08:27:08.000000 botasaurus-4.0.8/botasaurus/botasaurus_storage.py
--rw-rw-rw-   0        0        0      716 2024-02-25 10:26:09.000000 botasaurus-4.0.8/botasaurus/bt.py
--rw-rw-rw-   0        0        0     7727 2024-02-10 13:54:33.000000 botasaurus-4.0.8/botasaurus/cache.py
--rw-rw-rw-   0        0        0     2164 2023-12-03 11:14:41.000000 botasaurus-4.0.8/botasaurus/calc_max_parallel_browsers.py
--rw-rw-rw-   0        0        0      589 2023-11-14 05:58:34.000000 botasaurus-4.0.8/botasaurus/check_and_download_driver.py
--rw-rw-rw-   0        0        0      378 2024-03-20 08:15:53.000000 botasaurus-4.0.8/botasaurus/chrome_launcher_adapter.py
--rw-rw-rw-   0        0        0    15403 2024-01-25 05:44:39.000000 botasaurus-4.0.8/botasaurus/cl.py
--rw-rw-rw-   0        0        0      970 2023-11-17 11:12:26.000000 botasaurus-4.0.8/botasaurus/close.py
--rw-rw-rw-   0        0        0    14580 2024-03-20 07:51:02.000000 botasaurus-4.0.8/botasaurus/create_driver_utils.py
--rw-rw-rw-   0        0        0    12652 2024-03-20 09:33:39.000000 botasaurus-4.0.8/botasaurus/create_stealth_driver.py
--rw-rw-rw-   0        0        0     1870 2024-02-21 07:59:48.000000 botasaurus-4.0.8/botasaurus/creators.py
--rw-rw-rw-   0        0        0     4259 2024-02-03 10:50:05.000000 botasaurus-4.0.8/botasaurus/decorator_helpers.py
--rw-rw-rw-   0        0        0    39354 2024-03-20 09:33:36.000000 botasaurus-4.0.8/botasaurus/decorators.py
--rw-rw-rw-   0        0        0      507 2023-11-10 06:55:51.000000 botasaurus-4.0.8/botasaurus/decorators_utils.py
--rw-rw-rw-   0        0        0     1674 2024-02-13 18:57:46.000000 botasaurus-4.0.8/botasaurus/download_driver.py
--rw-rw-rw-   0        0        0      472 2024-01-18 06:53:27.000000 botasaurus-4.0.8/botasaurus/driver_about.py
--rw-rw-rw-   0        0        0       51 2024-01-10 08:23:31.000000 botasaurus-4.0.8/botasaurus/exceptions.py
--rw-rw-rw-   0        0        0       88 2023-11-10 09:39:46.000000 botasaurus-4.0.8/botasaurus/formats.py
--rw-rw-rw-   0        0        0    15215 2023-12-03 07:18:51.000000 botasaurus-4.0.8/botasaurus/get_chrome_version.py
--rw-rw-rw-   0        0        0     8919 2024-03-20 09:07:08.000000 botasaurus-4.0.8/botasaurus/got_adapter.py
--rw-rw-rw-   0        0        0     2524 2024-02-03 08:58:25.000000 botasaurus-4.0.8/botasaurus/ip_utils.py
--rw-rw-rw-   0        0        0     1595 2023-11-10 06:45:23.000000 botasaurus-4.0.8/botasaurus/list_utils.py
--rw-rw-rw-   0        0        0     3185 2023-06-29 08:54:46.000000 botasaurus-4.0.8/botasaurus/local_storage.py
--rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.000000 botasaurus-4.0.8/botasaurus/local_storage_driver.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.000000 botasaurus-4.0.8/botasaurus/opponent.py
--rw-rw-rw-   0        0        0     7583 2024-03-15 09:19:07.000000 botasaurus-4.0.8/botasaurus/output.py
--rw-rw-rw-   0        0        0     4879 2023-11-30 08:41:54.000000 botasaurus-4.0.8/botasaurus/profile.py
--rw-rw-rw-   0        0        0    23238 2024-03-01 09:04:58.000000 botasaurus-4.0.8/botasaurus/sitemap.py
--rw-rw-rw-   0        0        0     2094 2024-03-15 10:09:30.000000 botasaurus-4.0.8/botasaurus/str_utils.py
--rw-rw-rw-   0        0        0     6527 2023-11-30 07:34:28.000000 botasaurus-4.0.8/botasaurus/temp_mail.py
--rw-rw-rw-   0        0        0       56 2023-12-10 05:13:46.000000 botasaurus-4.0.8/botasaurus/usage.py
--rw-rw-rw-   0        0        0     7608 2023-12-23 11:30:20.000000 botasaurus-4.0.8/botasaurus/user_agent.py
--rw-rw-rw-   0        0        0     4337 2024-01-09 09:32:34.000000 botasaurus-4.0.8/botasaurus/user_generator.py
--rw-rw-rw-   0        0        0     6965 2024-03-15 09:19:39.000000 botasaurus-4.0.8/botasaurus/utils.py
--rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.000000 botasaurus-4.0.8/botasaurus/wait.py
--rw-rw-rw-   0        0        0     1222 2023-07-01 17:18:01.000000 botasaurus-4.0.8/botasaurus/window_size.py
-drwxrwxrwx   0        0        0        0 2024-03-20 09:33:46.163380 botasaurus-4.0.8/botasaurus.egg-info/
--rw-rw-rw-   0        0        0    54382 2024-03-20 09:33:45.000000 botasaurus-4.0.8/botasaurus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1363 2024-03-20 09:33:45.000000 botasaurus-4.0.8/botasaurus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 09:33:45.000000 botasaurus-4.0.8/botasaurus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      199 2024-03-20 09:33:45.000000 botasaurus-4.0.8/botasaurus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-20 09:33:45.000000 botasaurus-4.0.8/botasaurus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-20 09:33:46.172813 botasaurus-4.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2660 2024-03-20 09:33:45.000000 botasaurus-4.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-20 09:35:24.487155 botasaurus-4.0.9/
+-rw-rw-rw-   0        0        0      222 2023-10-14 07:30:38.000000 botasaurus-4.0.9/AUTHORS
+-rw-rw-rw-   0        0        0     1094 2024-03-03 08:47:03.000000 botasaurus-4.0.9/LICENSE
+-rw-rw-rw-   0        0        0    54382 2024-03-20 09:35:24.486024 botasaurus-4.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    52343 2024-03-12 13:06:58.000000 botasaurus-4.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-20 09:35:24.461124 botasaurus-4.0.9/botasaurus/
+-rw-rw-rw-   0        0        0      218 2024-02-27 02:47:12.000000 botasaurus-4.0.9/botasaurus/__init__.py
+-rw-rw-rw-   0        0        0      223 2023-11-12 07:58:52.000000 botasaurus-4.0.9/botasaurus/_id.py
+-rw-rw-rw-   0        0        0     1065 2023-12-13 10:40:15.000000 botasaurus-4.0.9/botasaurus/accept_google_cookies.py
+-rw-rw-rw-   0        0        0    16521 2024-03-03 13:39:19.000000 botasaurus-4.0.9/botasaurus/anti_detect_driver.py
+-rw-rw-rw-   0        0        0     4607 2024-03-20 09:03:25.000000 botasaurus-4.0.9/botasaurus/anti_detect_requests.py
+-rw-rw-rw-   0        0        0     3681 2023-11-10 07:08:04.000000 botasaurus-4.0.9/botasaurus/base_data.py
+-rw-rw-rw-   0        0        0      831 2023-11-13 08:37:04.000000 botasaurus-4.0.9/botasaurus/beep_utils.py
+-rw-rw-rw-   0        0        0     2968 2024-01-26 08:27:08.000000 botasaurus-4.0.9/botasaurus/botasaurus_storage.py
+-rw-rw-rw-   0        0        0      716 2024-02-25 10:26:09.000000 botasaurus-4.0.9/botasaurus/bt.py
+-rw-rw-rw-   0        0        0     7727 2024-02-10 13:54:33.000000 botasaurus-4.0.9/botasaurus/cache.py
+-rw-rw-rw-   0        0        0     2164 2023-12-03 11:14:41.000000 botasaurus-4.0.9/botasaurus/calc_max_parallel_browsers.py
+-rw-rw-rw-   0        0        0      589 2023-11-14 05:58:34.000000 botasaurus-4.0.9/botasaurus/check_and_download_driver.py
+-rw-rw-rw-   0        0        0      378 2024-03-20 08:15:53.000000 botasaurus-4.0.9/botasaurus/chrome_launcher_adapter.py
+-rw-rw-rw-   0        0        0    15403 2024-01-25 05:44:39.000000 botasaurus-4.0.9/botasaurus/cl.py
+-rw-rw-rw-   0        0        0      970 2023-11-17 11:12:26.000000 botasaurus-4.0.9/botasaurus/close.py
+-rw-rw-rw-   0        0        0    14580 2024-03-20 07:51:02.000000 botasaurus-4.0.9/botasaurus/create_driver_utils.py
+-rw-rw-rw-   0        0        0    12565 2024-03-20 09:35:14.000000 botasaurus-4.0.9/botasaurus/create_stealth_driver.py
+-rw-rw-rw-   0        0        0     1870 2024-02-21 07:59:48.000000 botasaurus-4.0.9/botasaurus/creators.py
+-rw-rw-rw-   0        0        0     4259 2024-02-03 10:50:05.000000 botasaurus-4.0.9/botasaurus/decorator_helpers.py
+-rw-rw-rw-   0        0        0    39354 2024-03-20 09:33:36.000000 botasaurus-4.0.9/botasaurus/decorators.py
+-rw-rw-rw-   0        0        0      507 2023-11-10 06:55:51.000000 botasaurus-4.0.9/botasaurus/decorators_utils.py
+-rw-rw-rw-   0        0        0     1674 2024-02-13 18:57:46.000000 botasaurus-4.0.9/botasaurus/download_driver.py
+-rw-rw-rw-   0        0        0      472 2024-01-18 06:53:27.000000 botasaurus-4.0.9/botasaurus/driver_about.py
+-rw-rw-rw-   0        0        0       51 2024-01-10 08:23:31.000000 botasaurus-4.0.9/botasaurus/exceptions.py
+-rw-rw-rw-   0        0        0       88 2023-11-10 09:39:46.000000 botasaurus-4.0.9/botasaurus/formats.py
+-rw-rw-rw-   0        0        0    15215 2023-12-03 07:18:51.000000 botasaurus-4.0.9/botasaurus/get_chrome_version.py
+-rw-rw-rw-   0        0        0     8919 2024-03-20 09:07:08.000000 botasaurus-4.0.9/botasaurus/got_adapter.py
+-rw-rw-rw-   0        0        0     2524 2024-02-03 08:58:25.000000 botasaurus-4.0.9/botasaurus/ip_utils.py
+-rw-rw-rw-   0        0        0     1595 2023-11-10 06:45:23.000000 botasaurus-4.0.9/botasaurus/list_utils.py
+-rw-rw-rw-   0        0        0     3185 2023-06-29 08:54:46.000000 botasaurus-4.0.9/botasaurus/local_storage.py
+-rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.000000 botasaurus-4.0.9/botasaurus/local_storage_driver.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.000000 botasaurus-4.0.9/botasaurus/opponent.py
+-rw-rw-rw-   0        0        0     7583 2024-03-15 09:19:07.000000 botasaurus-4.0.9/botasaurus/output.py
+-rw-rw-rw-   0        0        0     4879 2023-11-30 08:41:54.000000 botasaurus-4.0.9/botasaurus/profile.py
+-rw-rw-rw-   0        0        0    23238 2024-03-01 09:04:58.000000 botasaurus-4.0.9/botasaurus/sitemap.py
+-rw-rw-rw-   0        0        0     2094 2024-03-15 10:09:30.000000 botasaurus-4.0.9/botasaurus/str_utils.py
+-rw-rw-rw-   0        0        0     6527 2023-11-30 07:34:28.000000 botasaurus-4.0.9/botasaurus/temp_mail.py
+-rw-rw-rw-   0        0        0       56 2023-12-10 05:13:46.000000 botasaurus-4.0.9/botasaurus/usage.py
+-rw-rw-rw-   0        0        0     7608 2023-12-23 11:30:20.000000 botasaurus-4.0.9/botasaurus/user_agent.py
+-rw-rw-rw-   0        0        0     4337 2024-01-09 09:32:34.000000 botasaurus-4.0.9/botasaurus/user_generator.py
+-rw-rw-rw-   0        0        0     6965 2024-03-15 09:19:39.000000 botasaurus-4.0.9/botasaurus/utils.py
+-rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.000000 botasaurus-4.0.9/botasaurus/wait.py
+-rw-rw-rw-   0        0        0     1222 2023-07-01 17:18:01.000000 botasaurus-4.0.9/botasaurus/window_size.py
+drwxrwxrwx   0        0        0        0 2024-03-20 09:35:24.485020 botasaurus-4.0.9/botasaurus.egg-info/
+-rw-rw-rw-   0        0        0    54382 2024-03-20 09:35:24.000000 botasaurus-4.0.9/botasaurus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1363 2024-03-20 09:35:24.000000 botasaurus-4.0.9/botasaurus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-20 09:35:24.000000 botasaurus-4.0.9/botasaurus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      199 2024-03-20 09:35:24.000000 botasaurus-4.0.9/botasaurus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-20 09:35:24.000000 botasaurus-4.0.9/botasaurus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-03-20 09:35:24.494530 botasaurus-4.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2660 2024-03-20 09:35:23.000000 botasaurus-4.0.9/setup.py
```

### Comparing `botasaurus-4.0.8/LICENSE` & `botasaurus-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/PKG-INFO` & `botasaurus-4.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus
-Version: 4.0.8
+Version: 4.0.9
 Summary: The All in One Web Scraping Framework
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 Maintainer: Chetan Jain
 Maintainer-email: chetan@omkar.cloud
 License: MIT
 Project-URL: Documentation, https://omkar.cloud/botasaurus/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botasaurus Version: 4.0.8 Summary: The All in One
+Metadata-Version: 2.1 Name: botasaurus Version: 4.0.9 Summary: The All in One
 Web Scraping Framework Author: Chetan Jain Author-email: chetan@omkar.cloud
 Maintainer: Chetan Jain Maintainer-email: chetan@omkar.cloud License: MIT
 Project-URL: Documentation, https://omkar.cloud/botasaurus/ Project-URL:
 Source, https://github.com/omkarcloud/botasaurus Project-URL: Tracker, https://
 github.com/omkarcloud/botasaurus/issues Keywords:
 crawler,framework,scraping,crawling,web-scraping,web-scraping-
 python,cloudflare-bypass,anti-detection,bot-
```

### Comparing `botasaurus-4.0.8/README.md` & `botasaurus-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/accept_google_cookies.py` & `botasaurus-4.0.9/botasaurus/accept_google_cookies.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/anti_detect_driver.py` & `botasaurus-4.0.9/botasaurus/anti_detect_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/anti_detect_requests.py` & `botasaurus-4.0.9/botasaurus/anti_detect_requests.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/base_data.py` & `botasaurus-4.0.9/botasaurus/base_data.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/beep_utils.py` & `botasaurus-4.0.9/botasaurus/beep_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/botasaurus_storage.py` & `botasaurus-4.0.9/botasaurus/botasaurus_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/bt.py` & `botasaurus-4.0.9/botasaurus/bt.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/cache.py` & `botasaurus-4.0.9/botasaurus/cache.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/calc_max_parallel_browsers.py` & `botasaurus-4.0.9/botasaurus/calc_max_parallel_browsers.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/check_and_download_driver.py` & `botasaurus-4.0.9/botasaurus/check_and_download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/cl.py` & `botasaurus-4.0.9/botasaurus/cl.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/close.py` & `botasaurus-4.0.9/botasaurus/close.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/create_driver_utils.py` & `botasaurus-4.0.9/botasaurus/create_driver_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/create_stealth_driver.py` & `botasaurus-4.0.9/botasaurus/create_stealth_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,18 +234,16 @@
 
 def is_server_mode():
     # Check if '--server' is in the list of command-line arguments
     return '--server' in argv
 
 def launch_server_safe_chrome(options, start_url):
     try:
-        print("args",options._arguments)
         return launch_chrome(start_url, options._arguments)
     except JavaScriptError as e:
-        print("argserr",options._arguments)
         if "ECONNREFUSED" in e.js and not is_server_mode():
             add_server_args(options)
             print("Chrome failed to launch. Retrying with additional server options. To add server options by default, include '--server' in your launch command.")
             return launch_chrome(start_url, options._arguments)
         raise
 
 def do_create_stealth_driver(data, options, desired_capabilities, start_url, wait,  raise_exception,add_arguments):
```

### Comparing `botasaurus-4.0.8/botasaurus/creators.py` & `botasaurus-4.0.9/botasaurus/creators.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/decorator_helpers.py` & `botasaurus-4.0.9/botasaurus/decorator_helpers.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/decorators.py` & `botasaurus-4.0.9/botasaurus/decorators.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/download_driver.py` & `botasaurus-4.0.9/botasaurus/download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/get_chrome_version.py` & `botasaurus-4.0.9/botasaurus/get_chrome_version.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/got_adapter.py` & `botasaurus-4.0.9/botasaurus/got_adapter.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/ip_utils.py` & `botasaurus-4.0.9/botasaurus/ip_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/list_utils.py` & `botasaurus-4.0.9/botasaurus/list_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/local_storage.py` & `botasaurus-4.0.9/botasaurus/local_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/local_storage_driver.py` & `botasaurus-4.0.9/botasaurus/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/output.py` & `botasaurus-4.0.9/botasaurus/output.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/profile.py` & `botasaurus-4.0.9/botasaurus/profile.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/sitemap.py` & `botasaurus-4.0.9/botasaurus/sitemap.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/str_utils.py` & `botasaurus-4.0.9/botasaurus/str_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/temp_mail.py` & `botasaurus-4.0.9/botasaurus/temp_mail.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/user_agent.py` & `botasaurus-4.0.9/botasaurus/user_agent.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/user_generator.py` & `botasaurus-4.0.9/botasaurus/user_generator.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/utils.py` & `botasaurus-4.0.9/botasaurus/utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus/window_size.py` & `botasaurus-4.0.9/botasaurus/window_size.py`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/botasaurus.egg-info/PKG-INFO` & `botasaurus-4.0.9/botasaurus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus
-Version: 4.0.8
+Version: 4.0.9
 Summary: The All in One Web Scraping Framework
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 Maintainer: Chetan Jain
 Maintainer-email: chetan@omkar.cloud
 License: MIT
 Project-URL: Documentation, https://omkar.cloud/botasaurus/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botasaurus Version: 4.0.8 Summary: The All in One
+Metadata-Version: 2.1 Name: botasaurus Version: 4.0.9 Summary: The All in One
 Web Scraping Framework Author: Chetan Jain Author-email: chetan@omkar.cloud
 Maintainer: Chetan Jain Maintainer-email: chetan@omkar.cloud License: MIT
 Project-URL: Documentation, https://omkar.cloud/botasaurus/ Project-URL:
 Source, https://github.com/omkarcloud/botasaurus Project-URL: Tracker, https://
 github.com/omkarcloud/botasaurus/issues Keywords:
 crawler,framework,scraping,crawling,web-scraping,web-scraping-
 python,cloudflare-bypass,anti-detection,bot-
```

### Comparing `botasaurus-4.0.8/botasaurus.egg-info/SOURCES.txt` & `botasaurus-4.0.9/botasaurus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botasaurus-4.0.8/setup.py` & `botasaurus-4.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         return long_description
     except:
         return None
 
 setup(
     name="botasaurus",
     packages=["botasaurus"],
-    version='4.0.8',
+    version='4.0.9',
     license="MIT",
     project_urls={
         "Documentation": "https://omkar.cloud/botasaurus/",
         "Source": "https://github.com/omkarcloud/botasaurus",
         "Tracker": "https://github.com/omkarcloud/botasaurus/issues",
     },
     description="The All in One Web Scraping Framework",
```

