# Comparing `tmp/vnstock-0.2.8.9.tar.gz` & `tmp/vnstock-0.2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnstock-0.2.8.9.tar", last modified: Thu Feb 15 16:08:53 2024, max compression
+gzip compressed data, was "vnstock-0.2.9.0.tar", last modified: Tue Apr  2 06:01:58 2024, max compression
```

## Comparing `vnstock-0.2.8.9.tar` & `vnstock-0.2.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-02-15 16:08:53.962912 vnstock-0.2.8.9/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2024-01-21 15:38:56.000000 vnstock-0.2.8.9/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     7922 2024-02-15 16:08:53.962912 vnstock-0.2.8.9/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7614 2024-01-21 15:38:56.000000 vnstock-0.2.8.9/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      190 2024-02-15 15:48:46.000000 vnstock-0.2.8.9/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      491 2024-02-15 16:08:53.962912 vnstock-0.2.8.9/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-02-15 16:08:53.954912 vnstock-0.2.8.9/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3088 2024-01-21 15:38:57.000000 vnstock-0.2.8.9/tests/test_funds.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-02-15 16:08:53.958912 vnstock-0.2.8.9/vnstock/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      366 2024-01-21 15:38:57.000000 vnstock-0.2.8.9/vnstock/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8290 2024-01-21 15:38:57.000000 vnstock-0.2.8.9/vnstock/chart.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12849 2024-01-21 15:38:57.000000 vnstock-0.2.8.9/vnstock/config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1331 2024-01-21 15:38:57.000000 vnstock-0.2.8.9/vnstock/derivative.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       20 2024-01-21 15:38:57.000000 vnstock-0.2.8.9/vnstock/economics.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26494 2024-02-15 16:03:54.000000 vnstock-0.2.8.9/vnstock/fundamental.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15406 2024-01-21 15:38:57.000000 vnstock-0.2.8.9/vnstock/funds.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21090 2024-01-21 15:38:57.000000 vnstock-0.2.8.9/vnstock/integration.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3855 2024-01-21 15:38:57.000000 vnstock-0.2.8.9/vnstock/market.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1000 2024-01-21 15:38:57.000000 vnstock-0.2.8.9/vnstock/ocr.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11943 2024-01-21 15:38:57.000000 vnstock-0.2.8.9/vnstock/technical.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16430 2024-01-21 15:38:57.000000 vnstock-0.2.8.9/vnstock/trading.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2024-01-21 15:38:57.000000 vnstock-0.2.8.9/vnstock/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-02-15 16:08:53.962912 vnstock-0.2.8.9/vnstock.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     7922 2024-02-15 16:08:53.000000 vnstock-0.2.8.9/vnstock.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      437 2024-02-15 16:08:53.000000 vnstock-0.2.8.9/vnstock.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-02-15 16:08:53.000000 vnstock-0.2.8.9/vnstock.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2024-02-15 16:08:53.000000 vnstock-0.2.8.9/vnstock.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-02 06:01:58.567704 vnstock-0.2.9.0/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2024-04-02 03:21:34.000000 vnstock-0.2.9.0/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     7922 2024-04-02 06:01:58.567704 vnstock-0.2.9.0/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7614 2024-04-02 03:21:34.000000 vnstock-0.2.9.0/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      190 2024-04-02 03:21:35.000000 vnstock-0.2.9.0/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      491 2024-04-02 06:01:58.567704 vnstock-0.2.9.0/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-02 06:01:58.555704 vnstock-0.2.9.0/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3088 2024-04-02 03:21:35.000000 vnstock-0.2.9.0/tests/test_funds.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-02 06:01:58.563704 vnstock-0.2.9.0/vnstock/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      366 2024-04-02 03:21:35.000000 vnstock-0.2.9.0/vnstock/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8290 2024-04-02 03:21:35.000000 vnstock-0.2.9.0/vnstock/chart.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12849 2024-04-02 03:21:35.000000 vnstock-0.2.9.0/vnstock/config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1331 2024-04-02 03:21:35.000000 vnstock-0.2.9.0/vnstock/derivative.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       20 2024-04-02 03:21:35.000000 vnstock-0.2.9.0/vnstock/economics.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    26494 2024-04-02 03:21:35.000000 vnstock-0.2.9.0/vnstock/fundamental.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15406 2024-04-02 03:21:35.000000 vnstock-0.2.9.0/vnstock/funds.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    21130 2024-04-02 03:21:35.000000 vnstock-0.2.9.0/vnstock/integration.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3855 2024-04-02 03:21:35.000000 vnstock-0.2.9.0/vnstock/market.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1000 2024-04-02 03:21:35.000000 vnstock-0.2.9.0/vnstock/ocr.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11943 2024-04-02 03:21:35.000000 vnstock-0.2.9.0/vnstock/technical.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16430 2024-04-02 03:21:35.000000 vnstock-0.2.9.0/vnstock/trading.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2024-04-02 03:21:35.000000 vnstock-0.2.9.0/vnstock/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-02 06:01:58.567704 vnstock-0.2.9.0/vnstock.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     7922 2024-04-02 06:01:58.000000 vnstock-0.2.9.0/vnstock.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      437 2024-04-02 06:01:58.000000 vnstock-0.2.9.0/vnstock.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-02 06:01:58.000000 vnstock-0.2.9.0/vnstock.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2024-04-02 06:01:58.000000 vnstock-0.2.9.0/vnstock.egg-info/top_level.txt
```

### Comparing `vnstock-0.2.8.9/LICENSE` & `vnstock-0.2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vnstock-0.2.8.9/PKG-INFO` & `vnstock-0.2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnstock
-Version: 0.2.8.9
+Version: 0.2.9.0
 Summary: Vietnam Stock Market Data
 Home-page: https://github.com/thinh-vu/vnstock
 Author: Thinh Vu
 Author-email: mrthinh@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vnstock Version: 0.2.8.9 Summary: Vietnam Stock
+Metadata-Version: 2.1 Name: vnstock Version: 0.2.9.0 Summary: Vietnam Stock
 Market Data Home-page: https://github.com/thinh-vu/vnstock Author: Thinh Vu
 Author-email: mrthinh@live.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE
  [![python_course_5](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/
                            docs/docs/assets/images/
```

### Comparing `vnstock-0.2.8.9/README.md` & `vnstock-0.2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `vnstock-0.2.8.9/tests/test_funds.py` & `vnstock-0.2.9.0/tests/test_funds.py`

 * *Files identical despite different names*

### Comparing `vnstock-0.2.8.9/vnstock/chart.py` & `vnstock-0.2.9.0/vnstock/chart.py`

 * *Files identical despite different names*

### Comparing `vnstock-0.2.8.9/vnstock/config.py` & `vnstock-0.2.9.0/vnstock/config.py`

 * *Files identical despite different names*

### Comparing `vnstock-0.2.8.9/vnstock/derivative.py` & `vnstock-0.2.9.0/vnstock/derivative.py`

 * *Files identical despite different names*

### Comparing `vnstock-0.2.8.9/vnstock/fundamental.py` & `vnstock-0.2.9.0/vnstock/fundamental.py`

 * *Files identical despite different names*

### Comparing `vnstock-0.2.8.9/vnstock/funds.py` & `vnstock-0.2.9.0/vnstock/funds.py`

 * *Files identical despite different names*

### Comparing `vnstock-0.2.8.9/vnstock/integration.py` & `vnstock-0.2.9.0/vnstock/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -482,26 +482,27 @@
 
     Returns:
         object: Response object from the Telegram API.
     """
     file_name = file_path.split(get_path_delimiter())[-1]
     file_type = file_name.split('.')[-1]
     files = [('photo', (file_name, open(file_path, 'rb'), 'image/{}'.format(file_type)))]
-    url = 'https://api.telegram.org/{}/sendPhoto'.format(token_key)
+    url = 'https://api.telegram.org/bot{}/sendPhoto'.format(token_key)
     payload = {'chat_id': chat_id, 'caption': message}
     response = requests.post(url, headers={}, data=payload, files=files)
     return response
 
 def telegram_send_message(token_key, chat_id, message):
-    """
-    Send a message to a Telegram group.
+	"""
+	Send a message to a Telegram group.
 
-    Args:
-        token_key (str): Telegram token key.
-        chat_id (str): ID of the target Telegram channel/group, e.g., '-1001439492355'.
-        message (str): Your text message.
+	Args:
+		token_key (str): Telegram token key.
+		chat_id (str): ID of the target Telegram channel/group, e.g., '-1001439492355'.
+		message (str): Your text message.
 
-    Returns:
-        object: Response object from the Telegram API.
-    """
-    tel_url = 'https://api.telegram.org/{}/sendMessage?chat_id={}&text={}'.format(token_key, chat_id, message)
-    return requests.post(tel_url)
+	Returns:
+		object: Response object from the Telegram API.
+	"""
+	tel_url = 'https://api.telegram.org/bot{}/sendMessage?chat_id={}&text={}'.format(token_key, chat_id, message) # thêm chữ bot trước token so với code cũ
+	response = requests.post(tel_url)
+	return response.json()
```

### Comparing `vnstock-0.2.8.9/vnstock/market.py` & `vnstock-0.2.9.0/vnstock/market.py`

 * *Files identical despite different names*

### Comparing `vnstock-0.2.8.9/vnstock/ocr.py` & `vnstock-0.2.9.0/vnstock/ocr.py`

 * *Files identical despite different names*

### Comparing `vnstock-0.2.8.9/vnstock/technical.py` & `vnstock-0.2.9.0/vnstock/technical.py`

 * *Files identical despite different names*

### Comparing `vnstock-0.2.8.9/vnstock/trading.py` & `vnstock-0.2.9.0/vnstock/trading.py`

 * *Files identical despite different names*

### Comparing `vnstock-0.2.8.9/vnstock/utils.py` & `vnstock-0.2.9.0/vnstock/utils.py`

 * *Files identical despite different names*

### Comparing `vnstock-0.2.8.9/vnstock.egg-info/PKG-INFO` & `vnstock-0.2.9.0/vnstock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnstock
-Version: 0.2.8.9
+Version: 0.2.9.0
 Summary: Vietnam Stock Market Data
 Home-page: https://github.com/thinh-vu/vnstock
 Author: Thinh Vu
 Author-email: mrthinh@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vnstock Version: 0.2.8.9 Summary: Vietnam Stock
+Metadata-Version: 2.1 Name: vnstock Version: 0.2.9.0 Summary: Vietnam Stock
 Market Data Home-page: https://github.com/thinh-vu/vnstock Author: Thinh Vu
 Author-email: mrthinh@live.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE
  [![python_course_5](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/
                            docs/docs/assets/images/
```

