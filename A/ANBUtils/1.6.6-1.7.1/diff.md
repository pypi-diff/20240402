# Comparing `tmp/ANBUtils-1.6.6.tar.gz` & `tmp/ANBUtils-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANBUtils-1.6.6.tar", last modified: Tue Mar 12 17:12:33 2024, max compression
+gzip compressed data, was "dist/ANBUtils-1.7.1.tar", last modified: Thu Mar 28 11:47:25 2024, max compression
```

## Comparing `ANBUtils-1.6.6.tar` & `ANBUtils-1.7.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2024-03-12 17:12:33.088605 ANBUtils-1.6.6/
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2024-03-12 17:12:33.085800 ANBUtils-1.6.6/ANBUtils/
--rw-r--r--   0 redbson    (501) staff       (20)      849 2023-07-03 10:31:48.000000 ANBUtils-1.6.6/ANBUtils/__init__.py
--rw-r--r--   0 redbson    (501) staff       (20)     3129 2023-07-11 07:09:11.000000 ANBUtils-1.6.6/ANBUtils/a.py
--rw-r--r--   0 redbson    (501) staff       (20)    11957 2024-03-12 17:12:01.000000 ANBUtils-1.6.6/ANBUtils/db_worker.py
--rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.6.6/ANBUtils/easy_pickle.py
--rw-r--r--   0 redbson    (501) staff       (20)     1092 2023-07-03 10:30:53.000000 ANBUtils-1.6.6/ANBUtils/environ.py
--rw-r--r--   0 redbson    (501) staff       (20)     3520 2023-06-13 11:04:14.000000 ANBUtils-1.6.6/ANBUtils/id_work.py
--rw-r--r--   0 redbson    (501) staff       (20)     1954 2023-06-13 04:36:50.000000 ANBUtils-1.6.6/ANBUtils/messenger.py
--rw-r--r--   0 redbson    (501) staff       (20)     4852 2023-07-24 12:48:21.000000 ANBUtils-1.6.6/ANBUtils/tbox.py
-drwxr-xr-x   0 redbson    (501) staff       (20)        0 2024-03-12 17:12:33.087457 ANBUtils-1.6.6/ANBUtils.egg-info/
--rw-r--r--   0 redbson    (501) staff       (20)     5499 2024-03-12 17:12:33.000000 ANBUtils-1.6.6/ANBUtils.egg-info/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)      337 2024-03-12 17:12:33.000000 ANBUtils-1.6.6/ANBUtils.egg-info/SOURCES.txt
--rw-r--r--   0 redbson    (501) staff       (20)        1 2024-03-12 17:12:33.000000 ANBUtils-1.6.6/ANBUtils.egg-info/dependency_links.txt
--rw-r--r--   0 redbson    (501) staff       (20)      108 2024-03-12 17:12:33.000000 ANBUtils-1.6.6/ANBUtils.egg-info/requires.txt
--rw-r--r--   0 redbson    (501) staff       (20)        9 2024-03-12 17:12:33.000000 ANBUtils-1.6.6/ANBUtils.egg-info/top_level.txt
--rw-r--r--   0 redbson    (501) staff       (20)     5499 2024-03-12 17:12:33.088161 ANBUtils-1.6.6/PKG-INFO
--rw-r--r--   0 redbson    (501) staff       (20)     4894 2023-06-13 11:16:05.000000 ANBUtils-1.6.6/README.md
--rw-r--r--   0 redbson    (501) staff       (20)       38 2024-03-12 17:12:33.088811 ANBUtils-1.6.6/setup.cfg
--rw-r--r--   0 redbson    (501) staff       (20)      844 2024-03-12 17:12:01.000000 ANBUtils-1.6.6/setup.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2024-03-28 11:47:25.251522 ANBUtils-1.7.1/
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2024-03-28 11:47:25.249799 ANBUtils-1.7.1/ANBUtils/
+-rw-r--r--   0 redbson    (501) staff       (20)    13920 2024-03-28 11:45:47.000000 ANBUtils-1.7.1/ANBUtils/DBWorker.py
+-rw-r--r--   0 redbson    (501) staff       (20)      865 2024-03-28 10:31:28.000000 ANBUtils-1.7.1/ANBUtils/__init__.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3129 2023-07-11 07:09:11.000000 ANBUtils-1.7.1/ANBUtils/a.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3186 2024-03-28 10:27:52.000000 ANBUtils-1.7.1/ANBUtils/db_tools.py
+-rw-r--r--   0 redbson    (501) staff       (20)      932 2023-06-06 05:14:52.000000 ANBUtils-1.7.1/ANBUtils/easy_pickle.py
+-rw-r--r--   0 redbson    (501) staff       (20)     1092 2023-07-03 10:30:53.000000 ANBUtils-1.7.1/ANBUtils/environ.py
+-rw-r--r--   0 redbson    (501) staff       (20)     3520 2023-06-13 11:04:14.000000 ANBUtils-1.7.1/ANBUtils/id_work.py
+-rw-r--r--   0 redbson    (501) staff       (20)     2427 2024-03-28 04:40:26.000000 ANBUtils-1.7.1/ANBUtils/messenger.py
+-rw-r--r--   0 redbson    (501) staff       (20)     4978 2024-03-18 10:37:34.000000 ANBUtils-1.7.1/ANBUtils/tbox.py
+drwxr-xr-x   0 redbson    (501) staff       (20)        0 2024-03-28 11:47:25.250798 ANBUtils-1.7.1/ANBUtils.egg-info/
+-rw-r--r--   0 redbson    (501) staff       (20)     5498 2024-03-28 11:47:25.000000 ANBUtils-1.7.1/ANBUtils.egg-info/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)      357 2024-03-28 11:47:25.000000 ANBUtils-1.7.1/ANBUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        1 2024-03-28 11:47:25.000000 ANBUtils-1.7.1/ANBUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 redbson    (501) staff       (20)      108 2024-03-28 11:47:25.000000 ANBUtils-1.7.1/ANBUtils.egg-info/requires.txt
+-rw-r--r--   0 redbson    (501) staff       (20)        9 2024-03-28 11:47:25.000000 ANBUtils-1.7.1/ANBUtils.egg-info/top_level.txt
+-rw-r--r--   0 redbson    (501) staff       (20)     5498 2024-03-28 11:47:25.251232 ANBUtils-1.7.1/PKG-INFO
+-rw-r--r--   0 redbson    (501) staff       (20)     4893 2024-03-28 07:19:01.000000 ANBUtils-1.7.1/README.md
+-rw-r--r--   0 redbson    (501) staff       (20)       38 2024-03-28 11:47:25.251597 ANBUtils-1.7.1/setup.cfg
+-rw-r--r--   0 redbson    (501) staff       (20)      859 2024-03-28 10:36:16.000000 ANBUtils-1.7.1/setup.py
```

### Comparing `ANBUtils-1.6.6/ANBUtils/__init__.py` & `ANBUtils-1.7.1/ANBUtils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-
 from .environ import environment_checker as _checker
+
 _checker()
 
-from .environ import(
+from .environ import (
     set_environ
 )
 
 from .a import (
     print_rate_progress, set_date_index, digit, count, value, count2int, data_browser
 )
 
-from .db_worker import (
-    DBWorker, crawler_starter, log_db, read_log, dblink, dblink_add, dblink_remove, dblink_update, collection_show,
-    df2mongo, mongo2df, get_db_info, get_mongodb, dblink_help, get_token,
-    in_severs
+from .db_tools import (
+    crawler_starter, dblink, dblink_add, dblink_remove, dblink_update, collection_show,
+    df2mongo, mongo2df, get_db_info, get_mongodb, dblink_help, get_token
+)
+
+from .DBWorker import (
+    DBWorker
 )
 
 from .easy_pickle import (
     easy_dump, easy_load
 )
 
 from .id_work import (
     int_mark, id_analyst, matplot_set
 )
 
 from .messenger import (
-    qywechat_message, qywechat_text_message, dingtalk_message, dingtalk_text_message, message_mark_A, message_mark_B, message_mark_C, message_mark_D
+    qywechat_message, qywechat_text_message, dingtalk_message, dingtalk_text_message, message_mark_A, message_mark_B,
+    message_mark_C, message_mark_D
 )
 
 from .tbox import (
-    future, future_base, date_format, today, yesterday, tomorrow, ts2str, now, utc2tz
+    future, future_base, date_format, today, yesterday, tomorrow, ts2str, now, utc2tz, previous_date
 )
```

### Comparing `ANBUtils-1.6.6/ANBUtils/a.py` & `ANBUtils-1.7.1/ANBUtils/a.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.6/ANBUtils/easy_pickle.py` & `ANBUtils-1.7.1/ANBUtils/easy_pickle.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.6/ANBUtils/environ.py` & `ANBUtils-1.7.1/ANBUtils/environ.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.6/ANBUtils/id_work.py` & `ANBUtils-1.7.1/ANBUtils/id_work.py`

 * *Files identical despite different names*

### Comparing `ANBUtils-1.6.6/ANBUtils/messenger.py` & `ANBUtils-1.7.1/ANBUtils/messenger.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,90 +14,92 @@
     "msgtype": "text",
     "text": {
         "content": "%s"
     }
 }'''
 
 
-def dingtalk_message(data):
+def dingtalk_message(data, webhook=None):
     """
     发送钉钉消息。
 
     根据给定的数据，通过钉钉机器人的Webhook发送消息。
 
     参数：
         data: 消息数据。
+        webhook: Webhook地址（默认为环境变量'DINGTALK_WEBHOOK'）。
 
     返回：
         str: 发送结果。
 
     异常：
         None
     """
-    webhook = os.environ.get('DINGTALK_WEBHOOK')
+    webhook = os.environ.get( 'DINGTALK_WEBHOOK' )  if webhook is None else webhook
     headers = {
         'Content-Type': 'application/json',
     }
-    response = requests.post(webhook, headers=headers, data=data.encode("UTF-8"))
+    response = requests.post( webhook, headers=headers, data=data.encode( "UTF-8" ) )
     return response.text
 
 
-
-
-def qywechat_message(data):
+def qywechat_message(data, webhook=None):
     """
     发送企业微信消息。
 
     根据给定的数据，通过企业微信的机器人的Webhook发送消息。
 
     参数：
         data: 消息数据。
+        webhook: Webhook地址（默认为环境变量'QYWECHAT_WEB
 
     返回：
         str: 发送结果。
 
     异常：
         None
     """
-    webhook = os.environ.get('QYWECHAT_WEBHOOK')
+    webhook = os.environ.get( 'QYWECHAT_WEBHOOK' ) if webhook is None else webhook
     headers = {
         'Content-Type': 'application/json',
     }
-    response = requests.post(webhook, headers=headers, data=data.encode("UTF-8"))
+    response = requests.post( webhook, headers=headers, data=data.encode( "UTF-8" ) )
     return response.text
 
-def qywechat_text_message(text: str):
+
+def qywechat_text_message(text: str, webhook=None):
     """
     发送企业微信文本消息。
 
     根据给定的文本内容，通过企业微信机器人发送文本消息。
 
     参数：
         text (str): 文本内容。
+        webhook: Webhook地址（默认为环境变量'QYWECHAT_WEBHOOK'）。
+
 
     返回：
         None
 
     异常：
         None
     """
-    qywechat_message(msg_text % text)
-
-
+    qywechat_message( msg_text % text, webhook=webhook)
 
 
-def dingtalk_text_message(text: str):
+def dingtalk_text_message(text: str, webhook=None):
     """
     发送钉钉文本消息。
 
     根据给定的文本内容，通过钉钉机器人发送文本消息。
 
     参数：
         text (str): 文本内容。
+        webhook: Webhook地址（默认为环境变量'DINGTALK_WEBHOOK'）。
 
     返回：
         None
 
     异常：
         None
     """
-    dingtalk_message(msg_text % text)
+    dingtalk_message( msg_text % text, webhook=webhook)
```

### Comparing `ANBUtils-1.6.6/ANBUtils/tbox.py` & `ANBUtils-1.7.1/ANBUtils/tbox.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     返回：
         str: 未来日期的字符串表示（格式：YYYY-MM-DD）。
 
     异常：
         None
     """
-    return (datetime.now() + timedelta(days=x)).strftime('%Y-%m-%d')
+    return (datetime.now() + timedelta( days=x )).strftime( '%Y-%m-%d' )
 
 
 def utc2tz(dt, tz='E8'):
     """
     将UTC时间转换为指定时区的时间。
 
     根据给定的UTC时间和时区偏移量，将UTC时间转换为指定时区的时间。
@@ -35,73 +35,73 @@
     返回：
         datetime: 指定时区的时间。
 
     异常：
         ValueError: 当时区偏移量不在'E0'至'W12'范围内时，引发该异常。
     """
     if tz[0].upper() == 'E':
-        h = int(tz[1:])
+        h = int( tz[1:] )
     elif tz[0].upper() == 'W':
-        h = int(tz[1:]) * -1
+        h = int( tz[1:] ) * -1
     else:
-        raise ValueError('[utc2tz] tz is KeyError!')
+        raise ValueError( '[utc2tz] tz is KeyError!' )
 
-    return dt + timedelta(hours=h)
+    return dt + timedelta( hours=h )
 
 
 def today():
     """
     获取当前日期。
 
     返回：
         str: 当前日期的字符串表示（格式：YYYY-MM-DD）。
 
     异常：
         None
     """
-    return datetime.now().strftime("%Y-%m-%d")
+    return datetime.now().strftime( "%Y-%m-%d" )
 
 
 def tomorrow():
     """
     获取明天的日期。
 
     返回：
         str: 明天的日期的字符串表示（格式：YYYY-MM-DD）。
 
     异常：
         None
     """
-    return future(1)
+    return future( 1 )
 
 
 def yesterday():
     """
     获取昨天的日期。
 
     返回：
         str: 昨天的日期的字符串表示（格式：YYYY-MM-DD）。
 
     异常：
         None
     """
-    return future(-1)
+    return future( -1 )
 
 
 def now():
     """
     获取当前日期和时间。
 
     返回：
         str: 当前日期和时间的字符串表示（格式：YYYY-MM-DD HH:MM）。
 
     异常：
         None
     """
-    return datetime.now().strftime('%Y-%m-%d %H:%M')
+    return datetime.now().strftime( '%Y-%m-%d %H:%M' )
 
 
 def future_base(date, x):
     """
     根据基准日期计算未来日期。
 
     根据给定的基准日期和天数偏移量，计算未来的日期。
@@ -112,16 +112,16 @@
 
     返回：
         str: 未来日期的字符串表示（格式：YYYY-MM-DD）。
 
     异常：
         None
     """
-    base = datetime.strptime(date, "%Y-%m-%d")
-    return (base + timedelta(days=x)).strftime('%Y-%m-%d')
+    base = datetime.strptime( date, "%Y-%m-%d" )
+    return (base + timedelta( days=x )).strftime( '%Y-%m-%d' )
 
 
 def ts2str(x):
     """
     将时间戳转换为日期字符串。
 
     根据给定的时间戳，将其转换为日期字符串（格式：YYYY-MM-DD）。
@@ -131,17 +131,17 @@
 
     返回：
         str: 日期字符串（格式：YYYY-MM-DD）。
 
     异常：
         None
     """
-    if type(x) == str:
-        x = int(x)
-    return time.strftime("%Y-%m-%d", time.localtime(x))
+    if type( x ) == str:
+        x = int( x )
+    return time.strftime( "%Y-%m-%d", time.localtime( x ) )
 
 
 def date_format(date, date_format='YYYY-MM-DD'):
     """
     格式化日期字符串。
 
     根据给定的日期字符串和日期格式，将日期字符串格式化为指定的日期格式。
@@ -152,65 +152,66 @@
 
     返回：
         str: 格式化后的日期字符串。
 
     异常：
         None
     """
-    if len(date) == 10:
-        if len(date.split('-')) == 3:
+    if len( date ) == 10:
+        if len( date.split( '-' ) ) == 3:
             date = date
-        elif len(date.split('/')) == 3:
-            date = date.replace('/', '-')
-        elif len(date.split('_')) == 3:
-            date = date.replace('_', '-')
+        elif len( date.split( '/' ) ) == 3:
+            date = date.replace( '/', '-' )
+        elif len( date.split( '_' ) ) == 3:
+            date = date.replace( '_', '-' )
 
-    if len(date) == 6:
+    if len( date ) == 6:
         y = date[:2]
         m = date[2:4]
         d = date[4:]
-        if int(y) <= 30:
+        if int( y ) <= 30:
             y = '20' + y
         else:
             y = '19' + y
-        date = '-'.join([y, m, d])
+        date = '-'.join( [y, m, d] )
 
     if date_format == 'YYYY-MM-DD':
         return date
     elif date_format == 'YYMMDD':
-        return date.replace('-', '')[2:]
+        return date.replace( '-', '' )[2:]
     elif date_format == 'YYYY_MM_DD':
-        return date.replace('-', '_')
+        return date.replace( '-', '_' )
 
 
-from datetime import datetime, timedelta
-
-def previous_day(n, mode = 'm'):
-    base_day = datetime.today()
+def previous_date(n, base_day=None, mode='m'):
+    if base_day is None:
+        base_day = datetime.today()
+    else:
+        base_day = datetime.strptime( base_day, '%Y-%m-%d' )
 
     if mode == 'm':
         pass
 
-    elif  mode == 'q':
+    elif mode == 'q':
         current_month = base_day.month
-        base_day = datetime(base_day.year, ((current_month - 1) // 3) * 3 + 1, 1)
+        base_day = datetime( base_day.year, ((current_month - 1) // 3) * 3 + 1, 1 )
 
     else:
-        raise ValueError('mode must be m or q')
+        raise ValueError( 'mode must be m or q' )
 
     # 获取当前月份的年份和月份
     current_year, current_month = base_day.year, base_day.month
 
     # 计算当前月份之前的n个月
-    n =  n if mode =='m' else n * 3
-    for _ in range(n):
+    n = n if mode == 'm' else n * 3
+    for _ in range( n ):
         # 减去一个月
         if current_month == 1:
             current_month = 12
             current_year -= 1
         else:
             current_month -= 1
 
     # 得到所需日期
-    previous_date = datetime(current_year, current_month, 1)
+    _date = datetime( current_year, current_month, 1 )
 
-    return previous_date
+    return _date
```

### Comparing `ANBUtils-1.6.6/ANBUtils.egg-info/PKG-INFO` & `ANBUtils-1.7.1/ANBUtils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ANBUtils
-Version: 1.6.6
+Version: 1.7.1
 Summary: ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.
 Home-page: https://github.com/redbson/ANBUtils
 Author: Yafei Hou
 Author-email: redbson@gmail.com
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib>=3.0.0
 Requires-Dist: numpy>=1.0.0
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: pymongo>=4.0.2
 Requires-Dist: requests>=2.0.0
 Requires-Dist: matplotlib>=3.0.0
@@ -17,24 +17,24 @@
 
 # ANBUtils
 
 ANBUtils is a Python package that provides various utility functions for common tasks in data analysis and database operations. It includes functions for working with MongoDB, sending messages via DingTalk, and handling date and time operations.
 
 
 ## Stable Version 
-- Version: 1.6.0
-- Release Date: June 13, 2023
+- Version: 1.7.0
+- Release Date: Mar 28, 2024
 
 
 ## Installation
 
 You can install ANBUtils using pip:
 
 ```
-pip install ANBUtils == 1.6.0
+pip install ANBUtils == 1.7.0
 ```
 
 ## Functions
 
 ### MongoDB Operations
 
 - `DBWorker`: A class that provides convenient methods for working with MongoDB databases and collections. It allows you to perform operations such as querying data, inserting data, updating data, and more.
```

### Comparing `ANBUtils-1.6.6/PKG-INFO` & `ANBUtils-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ANBUtils
-Version: 1.6.6
+Version: 1.7.1
 Summary: ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.
 Home-page: https://github.com/redbson/ANBUtils
 Author: Yafei Hou
 Author-email: redbson@gmail.com
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib>=3.0.0
 Requires-Dist: numpy>=1.0.0
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: pymongo>=4.0.2
 Requires-Dist: requests>=2.0.0
 Requires-Dist: matplotlib>=3.0.0
@@ -17,24 +17,24 @@
 
 # ANBUtils
 
 ANBUtils is a Python package that provides various utility functions for common tasks in data analysis and database operations. It includes functions for working with MongoDB, sending messages via DingTalk, and handling date and time operations.
 
 
 ## Stable Version 
-- Version: 1.6.0
-- Release Date: June 13, 2023
+- Version: 1.7.0
+- Release Date: Mar 28, 2024
 
 
 ## Installation
 
 You can install ANBUtils using pip:
 
 ```
-pip install ANBUtils == 1.6.0
+pip install ANBUtils == 1.7.0
 ```
 
 ## Functions
 
 ### MongoDB Operations
 
 - `DBWorker`: A class that provides convenient methods for working with MongoDB databases and collections. It allows you to perform operations such as querying data, inserting data, updating data, and more.
```

### Comparing `ANBUtils-1.6.6/README.md` & `ANBUtils-1.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # ANBUtils
 
 ANBUtils is a Python package that provides various utility functions for common tasks in data analysis and database operations. It includes functions for working with MongoDB, sending messages via DingTalk, and handling date and time operations.
 
 
 ## Stable Version 
-- Version: 1.6.0
-- Release Date: June 13, 2023
+- Version: 1.7.0
+- Release Date: Mar 28, 2024
 
 
 ## Installation
 
 You can install ANBUtils using pip:
 
 ```
-pip install ANBUtils == 1.6.0
+pip install ANBUtils == 1.7.0
 ```
 
 ## Functions
 
 ### MongoDB Operations
 
 - `DBWorker`: A class that provides convenient methods for working with MongoDB databases and collections. It allows you to perform operations such as querying data, inserting data, updating data, and more.
```

### Comparing `ANBUtils-1.6.6/setup.py` & `ANBUtils-1.7.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
-with open('README.md', 'r', encoding='utf-8') as f:
-    long_description = f.read()
+with open('README.md', 'r', encoding='utf-8') as f :
+    long_description=f.read()
 
 setup(
     name="ANBUtils",
-    version='1.6.6',
+    version='1.7.1',
     packages=find_packages(),
     author='Yafei Hou',
     author_email='redbson@gmail.com',
-    url= 'https://github.com/redbson/ANBUtils',
-    description = "ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and tools for data analysis, database operations, and messaging integration.",
+    url='https://github.com/redbson/ANBUtils',
+    description='ANBUilts is a versatile Python package that offers a comprehensive set of utility functions and '
+                'tools for data analysis, database operations, and messaging integration.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     install_requires=[
         "matplotlib>=3.0.0",
         "numpy>=1.0.0",
         "pandas>=1.0.0",
         "pymongo>=4.0.2",
         "requests>=2.0.0",
         "matplotlib>=3.0.0",
```

