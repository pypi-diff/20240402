# Comparing `tmp/globallock-0.1.2.tar.gz` & `tmp/globallock-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globallock-0.1.2.tar", last modified: Sun Mar 31 06:14:35 2024, max compression
+gzip compressed data, was "globallock-0.1.3.tar", last modified: Tue Apr  2 13:40:10 2024, max compression
```

## Comparing `globallock-0.1.2.tar` & `globallock-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-03-31 06:14:35.457399 globallock-0.1.2/
--rw-r--r--   0 test       (501) staff       (20)     1067 2023-08-18 08:36:12.000000 globallock-0.1.2/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      250 2023-08-19 15:07:04.000000 globallock-0.1.2/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     5686 2024-03-31 06:14:35.457276 globallock-0.1.2/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     4885 2024-03-31 06:04:39.000000 globallock-0.1.2/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-03-31 06:14:35.456294 globallock-0.1.2/globallock/
--rw-r--r--   0 test       (501) staff       (20)      308 2023-08-20 04:05:48.000000 globallock-0.1.2/globallock/__init__.py
--rw-r--r--   0 test       (501) staff       (20)     3534 2024-03-31 05:55:17.000000 globallock-0.1.2/globallock/base.py
--rw-r--r--   0 test       (501) staff       (20)      847 2024-03-31 05:55:20.000000 globallock-0.1.2/globallock/config.py
--rw-r--r--   0 test       (501) staff       (20)      619 2024-03-31 06:06:32.000000 globallock-0.1.2/globallock/constants.py
--rw-r--r--   0 test       (501) staff       (20)      887 2024-03-31 06:03:54.000000 globallock-0.1.2/globallock/django.py
--rw-r--r--   0 test       (501) staff       (20)      995 2024-03-31 05:54:59.000000 globallock-0.1.2/globallock/django_redis_global_lock.py
--rw-r--r--   0 test       (501) staff       (20)     1348 2024-03-31 05:55:08.000000 globallock-0.1.2/globallock/etcd_global_lock.py
--rw-r--r--   0 test       (501) staff       (20)      127 2024-03-31 06:06:28.000000 globallock-0.1.2/globallock/exceptions.py
--rw-r--r--   0 test       (501) staff       (20)     1203 2024-03-31 05:55:12.000000 globallock-0.1.2/globallock/redis_global_lock.py
--rw-r--r--   0 test       (501) staff       (20)     1336 2024-03-31 05:55:14.000000 globallock-0.1.2/globallock/zookeeper_global_lock.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-03-31 06:14:35.457079 globallock-0.1.2/globallock.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     5686 2024-03-31 06:14:35.000000 globallock-0.1.2/globallock.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      528 2024-03-31 06:14:35.000000 globallock-0.1.2/globallock.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-03-31 06:14:35.000000 globallock-0.1.2/globallock.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-03-31 06:14:35.000000 globallock-0.1.2/globallock.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)        9 2024-03-31 06:14:35.000000 globallock-0.1.2/globallock.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       11 2024-03-31 06:14:35.000000 globallock-0.1.2/globallock.egg-info/top_level.txt
--rw-r--r--   0 test       (501) staff       (20)        9 2023-09-09 08:53:33.000000 globallock-0.1.2/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2024-03-31 06:14:35.457441 globallock-0.1.2/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1802 2024-03-31 05:49:58.000000 globallock-0.1.2/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-02 13:40:10.277089 globallock-0.1.3/
+-rw-r--r--   0 test       (501) staff       (20)     1067 2023-08-18 08:36:12.000000 globallock-0.1.3/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      250 2023-08-19 15:07:04.000000 globallock-0.1.3/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     5740 2024-04-02 13:40:10.276978 globallock-0.1.3/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     4939 2024-03-31 11:32:45.000000 globallock-0.1.3/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-02 13:40:10.276054 globallock-0.1.3/globallock/
+-rw-r--r--   0 test       (501) staff       (20)      308 2023-08-20 04:05:48.000000 globallock-0.1.3/globallock/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)     3534 2024-03-31 05:55:17.000000 globallock-0.1.3/globallock/base.py
+-rw-r--r--   0 test       (501) staff       (20)      847 2024-03-31 05:55:20.000000 globallock-0.1.3/globallock/config.py
+-rw-r--r--   0 test       (501) staff       (20)      619 2024-03-31 06:06:32.000000 globallock-0.1.3/globallock/constants.py
+-rw-r--r--   0 test       (501) staff       (20)      902 2024-03-31 11:32:23.000000 globallock-0.1.3/globallock/django.py
+-rw-r--r--   0 test       (501) staff       (20)      995 2024-03-31 05:54:59.000000 globallock-0.1.3/globallock/django_redis_global_lock.py
+-rw-r--r--   0 test       (501) staff       (20)     1348 2024-03-31 05:55:08.000000 globallock-0.1.3/globallock/etcd_global_lock.py
+-rw-r--r--   0 test       (501) staff       (20)      127 2024-03-31 06:06:28.000000 globallock-0.1.3/globallock/exceptions.py
+-rw-r--r--   0 test       (501) staff       (20)     1203 2024-03-31 05:55:12.000000 globallock-0.1.3/globallock/redis_global_lock.py
+-rw-r--r--   0 test       (501) staff       (20)     1336 2024-03-31 05:55:14.000000 globallock-0.1.3/globallock/zookeeper_global_lock.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-04-02 13:40:10.276800 globallock-0.1.3/globallock.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     5740 2024-04-02 13:40:10.000000 globallock-0.1.3/globallock.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      528 2024-04-02 13:40:10.000000 globallock-0.1.3/globallock.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-04-02 13:40:10.000000 globallock-0.1.3/globallock.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-04-02 13:40:10.000000 globallock-0.1.3/globallock.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)        9 2024-04-02 13:40:10.000000 globallock-0.1.3/globallock.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       11 2024-04-02 13:40:10.000000 globallock-0.1.3/globallock.egg-info/top_level.txt
+-rw-r--r--   0 test       (501) staff       (20)        9 2023-09-09 08:53:33.000000 globallock-0.1.3/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-04-02 13:40:10.277127 globallock-0.1.3/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1802 2024-03-31 11:32:50.000000 globallock-0.1.3/setup.py
```

### Comparing `globallock-0.1.2/LICENSE` & `globallock-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `globallock-0.1.2/PKG-INFO` & `globallock-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globallock
-Version: 0.1.2
+Version: 0.1.3
 Summary: Distributed lock manager, support many types of backend, e.g. redis, django-redis, etcd, zookeeper...
 Author: Sun HuiBin
 Author-email: sunhuibin@zencore.cn
 Maintainer: Sun HuiBin
 Maintainer-email: sunhuibin@zencore.cn
 License: MIT
 Keywords: global lock,distributed lock,redis lock,django redis lock,zookeeper lock,etcd lock
@@ -164,7 +164,11 @@
 
 - Doc update.
 
 ### v0.1.2
 
 - GlobalLockManager.lock方法参数可以在初始化时设置。
 - 添加globallock.django.get_default_global_lock_manager方法，允许在django中使用全局分布式锁。
+
+### v0.1.3
+
+- 修正globallock.django默认设置。
```

### Comparing `globallock-0.1.2/README.md` & `globallock-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -144,7 +144,11 @@
 
 - Doc update.
 
 ### v0.1.2
 
 - GlobalLockManager.lock方法参数可以在初始化时设置。
 - 添加globallock.django.get_default_global_lock_manager方法，允许在django中使用全局分布式锁。
+
+### v0.1.3
+
+- 修正globallock.django默认设置。
```

### Comparing `globallock-0.1.2/globallock/base.py` & `globallock-0.1.3/globallock/base.py`

 * *Files identical despite different names*

### Comparing `globallock-0.1.2/globallock/config.py` & `globallock-0.1.3/globallock/config.py`

 * *Files identical despite different names*

### Comparing `globallock-0.1.2/globallock/constants.py` & `globallock-0.1.3/globallock/constants.py`

 * *Files identical despite different names*

### Comparing `globallock-0.1.2/globallock/django.py` & `globallock-0.1.3/globallock/django.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,8 +20,9 @@
     if not "redis-cache-name" in config["global_lock_engine_options"]:
         config["global_lock_engine_options"]["redis-cache-name"] = "default"
     return config
 
 
 def get_default_global_lock_manager():
     """根据Django settings.py的设置，获取分布式锁。"""
-    return GlobalLockManager(GLOBAL_LOCK_CONFIG)
+    config = _get_config()
+    return GlobalLockManager(config)
```

### Comparing `globallock-0.1.2/globallock/django_redis_global_lock.py` & `globallock-0.1.3/globallock/django_redis_global_lock.py`

 * *Files identical despite different names*

### Comparing `globallock-0.1.2/globallock/etcd_global_lock.py` & `globallock-0.1.3/globallock/etcd_global_lock.py`

 * *Files identical despite different names*

### Comparing `globallock-0.1.2/globallock/redis_global_lock.py` & `globallock-0.1.3/globallock/redis_global_lock.py`

 * *Files identical despite different names*

### Comparing `globallock-0.1.2/globallock/zookeeper_global_lock.py` & `globallock-0.1.3/globallock/zookeeper_global_lock.py`

 * *Files identical despite different names*

### Comparing `globallock-0.1.2/globallock.egg-info/PKG-INFO` & `globallock-0.1.3/globallock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globallock
-Version: 0.1.2
+Version: 0.1.3
 Summary: Distributed lock manager, support many types of backend, e.g. redis, django-redis, etcd, zookeeper...
 Author: Sun HuiBin
 Author-email: sunhuibin@zencore.cn
 Maintainer: Sun HuiBin
 Maintainer-email: sunhuibin@zencore.cn
 License: MIT
 Keywords: global lock,distributed lock,redis lock,django redis lock,zookeeper lock,etcd lock
@@ -164,7 +164,11 @@
 
 - Doc update.
 
 ### v0.1.2
 
 - GlobalLockManager.lock方法参数可以在初始化时设置。
 - 添加globallock.django.get_default_global_lock_manager方法，允许在django中使用全局分布式锁。
+
+### v0.1.3
+
+- 修正globallock.django默认设置。
```

### Comparing `globallock-0.1.2/globallock.egg-info/SOURCES.txt` & `globallock-0.1.3/globallock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globallock-0.1.2/setup.py` & `globallock-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 requires = []
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires += [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="globallock",
-    version="0.1.2",
+    version="0.1.3",
     description="Distributed lock manager, support many types of backend, e.g. redis, django-redis, etcd, zookeeper...",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Sun HuiBin",
     author_email="sunhuibin@zencore.cn",
     maintainer="Sun HuiBin",
     maintainer_email="sunhuibin@zencore.cn",
```

