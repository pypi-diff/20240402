# Comparing `tmp/twikit-1.4.1.tar.gz` & `tmp/twikit-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.4.1.tar", last modified: Sat Mar 30 16:49:39 2024, max compression
+gzip compressed data, was "twikit-1.4.2.tar", last modified: Tue Apr  2 02:34:04 2024, max compression
```

## Comparing `twikit-1.4.1.tar` & `twikit-1.4.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 16:49:39.496043 twikit-1.4.1/
--rw-rw-rw-   0        0        0     1079 2024-03-23 06:08:25.000000 twikit-1.4.1/LICENSE
--rw-rw-rw-   0        0        0     3534 2024-03-30 16:49:39.494051 twikit-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     3264 2024-03-23 06:08:25.000000 twikit-1.4.1/README.md
--rw-rw-rw-   0        0        0       42 2024-03-30 16:49:39.497042 twikit-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      693 2024-03-28 12:25:18.000000 twikit-1.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-30 16:49:39.413266 twikit-1.4.1/twikit/
--rw-rw-rw-   0        0        0      601 2024-03-30 16:33:44.000000 twikit-1.4.1/twikit/__init__.py
--rw-rw-rw-   0        0        0   108902 2024-03-30 16:48:29.000000 twikit-1.4.1/twikit/client.py
--rw-rw-rw-   0        0        0     2076 2024-03-29 07:12:11.000000 twikit-1.4.1/twikit/errors.py
--rw-rw-rw-   0        0        0     6859 2024-03-23 06:08:25.000000 twikit-1.4.1/twikit/group.py
--rw-rw-rw-   0        0        0     1887 2024-03-28 18:57:41.000000 twikit-1.4.1/twikit/http.py
--rw-rw-rw-   0        0        0     7276 2024-03-23 06:08:25.000000 twikit-1.4.1/twikit/list.py
--rw-rw-rw-   0        0        0     3800 2024-03-23 06:08:25.000000 twikit-1.4.1/twikit/message.py
--rw-rw-rw-   0        0        0     1385 2024-03-23 06:08:25.000000 twikit-1.4.1/twikit/notification.py
--rw-rw-rw-   0        0        0     1034 2024-03-23 06:08:25.000000 twikit-1.4.1/twikit/trend.py
--rw-rw-rw-   0        0        0    16514 2024-03-28 12:21:55.000000 twikit-1.4.1/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-03-30 16:49:39.489063 twikit-1.4.1/twikit/twikit_async/
--rw-rw-rw-   0        0        0      553 2024-03-23 06:08:25.000000 twikit-1.4.1/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0   112410 2024-03-30 16:49:28.000000 twikit-1.4.1/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0      875 2024-03-23 06:08:25.000000 twikit-1.4.1/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7041 2024-03-23 06:08:25.000000 twikit-1.4.1/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     1929 2024-03-23 06:08:25.000000 twikit-1.4.1/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7427 2024-03-23 06:08:25.000000 twikit-1.4.1/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3866 2024-03-23 06:08:25.000000 twikit-1.4.1/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1385 2024-03-23 06:08:25.000000 twikit-1.4.1/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     1034 2024-03-23 06:08:25.000000 twikit-1.4.1/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    16609 2024-03-28 12:26:57.000000 twikit-1.4.1/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    13987 2024-03-29 18:11:33.000000 twikit-1.4.1/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     2215 2024-03-29 18:39:44.000000 twikit-1.4.1/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    13776 2024-03-29 18:11:04.000000 twikit-1.4.1/twikit/user.py
--rw-rw-rw-   0        0        0    19707 2024-03-29 18:38:52.000000 twikit-1.4.1/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-30 16:49:39.436206 twikit-1.4.1/twikit.egg-info/
--rw-rw-rw-   0        0        0     3534 2024-03-30 16:49:39.000000 twikit-1.4.1/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2024-03-30 16:49:39.000000 twikit-1.4.1/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 16:49:39.000000 twikit-1.4.1/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-03-30 16:49:39.000000 twikit-1.4.1/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-30 16:49:39.000000 twikit-1.4.1/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 02:34:04.921992 twikit-1.4.2/
+-rw-rw-rw-   0        0        0     1079 2024-03-23 06:08:25.000000 twikit-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0     3534 2024-04-02 02:34:04.918995 twikit-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3264 2024-03-23 06:08:25.000000 twikit-1.4.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-02 02:34:04.921992 twikit-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      693 2024-03-28 12:25:18.000000 twikit-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 02:34:04.833226 twikit-1.4.2/twikit/
+-rw-rw-rw-   0        0        0      601 2024-04-02 02:33:47.000000 twikit-1.4.2/twikit/__init__.py
+-rw-rw-rw-   0        0        0   108902 2024-04-01 07:28:24.000000 twikit-1.4.2/twikit/client.py
+-rw-rw-rw-   0        0        0     2076 2024-03-29 07:12:11.000000 twikit-1.4.2/twikit/errors.py
+-rw-rw-rw-   0        0        0     6983 2024-04-02 02:28:49.000000 twikit-1.4.2/twikit/group.py
+-rw-rw-rw-   0        0        0     1887 2024-04-01 07:48:50.000000 twikit-1.4.2/twikit/http.py
+-rw-rw-rw-   0        0        0     7399 2024-04-02 02:28:12.000000 twikit-1.4.2/twikit/list.py
+-rw-rw-rw-   0        0        0     3800 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/message.py
+-rw-rw-rw-   0        0        0     1385 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/notification.py
+-rw-rw-rw-   0        0        0     1034 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/trend.py
+-rw-rw-rw-   0        0        0    16644 2024-04-02 02:26:56.000000 twikit-1.4.2/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-04-02 02:34:04.915008 twikit-1.4.2/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      553 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0   112410 2024-03-30 16:49:28.000000 twikit-1.4.2/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0      875 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7177 2024-04-02 02:30:57.000000 twikit-1.4.2/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     1929 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7562 2024-04-02 02:30:39.000000 twikit-1.4.2/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3866 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1385 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     1034 2024-03-23 06:08:25.000000 twikit-1.4.2/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    16751 2024-04-02 02:29:48.000000 twikit-1.4.2/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14128 2024-04-02 02:29:20.000000 twikit-1.4.2/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     2215 2024-03-29 18:39:44.000000 twikit-1.4.2/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    13905 2024-04-02 02:27:48.000000 twikit-1.4.2/twikit/user.py
+-rw-rw-rw-   0        0        0    19707 2024-04-01 07:29:32.000000 twikit-1.4.2/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 02:34:04.856166 twikit-1.4.2/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3534 2024-04-02 02:34:04.000000 twikit-1.4.2/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2024-04-02 02:34:04.000000 twikit-1.4.2/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 02:34:04.000000 twikit-1.4.2/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-02 02:34:04.000000 twikit-1.4.2/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 02:34:04.000000 twikit-1.4.2/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.4.1/LICENSE` & `twikit-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/PKG-INFO` & `twikit-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.4.1
+Version: 1.4.2
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.4.1/README.md` & `twikit-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/setup.py` & `twikit-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit/__init__.py` & `twikit-1.4.2/twikit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 )
 from .message import Message
 from .trend import Trend
 from .tweet import ScheduledTweet, Tweet
 from .user import User
 from .utils import build_query
 
-__version__ = '1.4.1'
+__version__ = '1.4.2'
```

### Comparing `twikit-1.4.1/twikit/client.py` & `twikit-1.4.2/twikit/client.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit/errors.py` & `twikit-1.4.2/twikit/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit/group.py` & `twikit-1.4.2/twikit/group.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,14 +143,18 @@
         >>> media_id = client.upload_media('image.png')
         >>> message = group.send_message('text', media_id)
         >>> print(message)
         <GroupMessage id='...'>
         """
         return self._client.send_dm_to_group(self.id, text, media_id, reply_to)
 
+    def update(self) -> None:
+        new = self._client.get_group(self.id)
+        self.__dict__.update(new.__dict__)
+
     def __repr__(self) -> str:
         return f'<Group id="{self.id}">'
 
 
 class GroupMessage(Message):
     """
     Represents a direct message.
```

### Comparing `twikit-1.4.1/twikit/http.py` & `twikit-1.4.2/twikit/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit/list.py` & `twikit-1.4.2/twikit/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,18 @@
         <User id="...">
         ...
         ...
         >>> more_subscribers = subscribers.next()  # Retrieve more subscribers
         """
         return self._client.get_list_subscribers(self.id, count, cursor)
 
+    def update(self) -> None:
+        new = self._client.get_list(self.id)
+        self.__dict__.update(new.__dict__)
+
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, List) and self.id == __value.id
 
     def __ne__(self, __value: object) -> bool:
         return not self == __value
 
     def __repr__(self) -> str:
```

### Comparing `twikit-1.4.1/twikit/message.py` & `twikit-1.4.2/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit/notification.py` & `twikit-1.4.2/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit/trend.py` & `twikit-1.4.2/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit/tweet.py` & `twikit-1.4.2/twikit/tweet.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,14 +384,18 @@
 
         >>> more_favoriters = favoriters.next()  # Retrieve more favoriters.
         >>> print(more_favoriters)
         [<User id="...">, <User id="...">, ..., <User id="...">]
         """
         return self._client.get_favoriters(self.id, count, cursor)
 
+    def update(self) -> None:
+        new = self._client.get_tweet_by_id(self.id)
+        self.__dict__.update(new.__dict__)
+
     def __repr__(self) -> str:
         return f'<Tweet id="{self.id}">'
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, Tweet) and self.id == __value.id
 
     def __ne__(self, __value: object) -> bool:
```

### Comparing `twikit-1.4.1/twikit/twikit_async/__init__.py` & `twikit-1.4.2/twikit/twikit_async/__init__.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit/twikit_async/client.py` & `twikit-1.4.2/twikit/twikit_async/client.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit/twikit_async/errors.py` & `twikit-1.4.2/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit/twikit_async/group.py` & `twikit-1.4.2/twikit/twikit_async/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,18 @@
         >>> print(message)
         <GroupMessage id='...'>
         """
         return await self._client.send_dm_to_group(
             self.id, text, media_id, reply_to
         )
 
+    async def update(self) -> None:
+        new = await self._client.get_group(self.id)
+        self.__dict__.update(new.__dict__)
+
     def __repr__(self) -> str:
         return f'<Group id="{self.id}">'
 
 
 class GroupMessage(Message):
     """
     Represents a direct message.
```

### Comparing `twikit-1.4.1/twikit/twikit_async/http.py` & `twikit-1.4.2/twikit/twikit_async/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit/twikit_async/list.py` & `twikit-1.4.2/twikit/twikit_async/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,14 +237,18 @@
         <User id="...">
         ...
         ...
         >>> more_subscribers = subscribers.next()  # Retrieve more subscribers
         """
         return await self._client.get_list_subscribers(self.id, count, cursor)
 
+    async def update(self) -> None:
+        new = await self._client.get_list(self.id)
+        self.__dict__.update(new.__dict__)
+
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, List) and self.id == __value.id
 
     def __ne__(self, __value: object) -> bool:
         return not self == __value
 
     def __repr__(self) -> str:
```

### Comparing `twikit-1.4.1/twikit/twikit_async/message.py` & `twikit-1.4.2/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit/twikit_async/notification.py` & `twikit-1.4.2/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit/twikit_async/trend.py` & `twikit-1.4.2/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit/twikit_async/tweet.py` & `twikit-1.4.2/twikit/twikit_async/tweet.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,14 +382,18 @@
 
         >>> more_favoriters = favoriters.next()  # Retrieve more favoriters.
         >>> print(more_favoriters)
         [<User id="...">, <User id="...">, ..., <User id="...">]
         """
         return await self._client.get_favoriters(self.id, count, cursor)
 
+    async def update(self) -> None:
+        new = await self._client.get_tweet_by_id(self.id)
+        self.__dict__.update(new.__dict__)
+
     def __repr__(self) -> str:
         return f'<Tweet id="{self.id}">'
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, Tweet) and self.id == __value.id
 
     def __ne__(self, __value: object) -> bool:
```

### Comparing `twikit-1.4.1/twikit/twikit_async/user.py` & `twikit-1.4.2/twikit/twikit_async/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,14 +446,18 @@
         <Message id="...">
         <Message id="...">
         ...
         ...
         """
         return await self._client.get_dm_history(self.id, max_id)
 
+    async def update(self) -> None:
+        new = await self._client.get_user_by_id(self.id)
+        self.__dict__.update(new.__dict__)
+
     def __repr__(self) -> str:
         return f'<User id="{self.id}">'
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, User) and self.id == __value.id
 
     def __ne__(self, __value: object) -> bool:
```

### Comparing `twikit-1.4.1/twikit/twikit_async/utils.py` & `twikit-1.4.2/twikit/twikit_async/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit/user.py` & `twikit-1.4.2/twikit/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,14 +446,18 @@
         <Message id="...">
         <Message id="...">
         ...
         ...
         """
         return self._client.get_dm_history(self.id, max_id)
 
+    def update(self) -> None:
+        new = self._client.get_user_by_id(self.id)
+        self.__dict__.update(new.__dict__)
+
     def __repr__(self) -> str:
         return f'<User id="{self.id}">'
 
     def __eq__(self, __value: object) -> bool:
         return isinstance(__value, User) and self.id == __value.id
 
     def __ne__(self, __value: object) -> bool:
```

### Comparing `twikit-1.4.1/twikit/utils.py` & `twikit-1.4.2/twikit/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.1/twikit.egg-info/PKG-INFO` & `twikit-1.4.2/twikit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.4.1
+Version: 1.4.2
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.4.1/twikit.egg-info/SOURCES.txt` & `twikit-1.4.2/twikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

