# Comparing `tmp/jacksung-0.0.2.96.tar.gz` & `tmp/jacksung-0.0.2.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jacksung-0.0.2.96.tar", last modified: Mon Mar 25 08:19:59 2024, max compression
+gzip compressed data, was "jacksung-0.0.2.97.tar", last modified: Tue Apr  2 09:11:01 2024, max compression
```

## Comparing `jacksung-0.0.2.96.tar` & `jacksung-0.0.2.97.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 08:19:59.431633 jacksung-0.0.2.96/
--rw-rw-rw-   0        0        0    11558 2023-11-22 07:36:29.000000 jacksung-0.0.2.96/LICENSE
--rw-rw-rw-   0        0        0     5413 2024-03-25 08:19:59.431633 jacksung-0.0.2.96/PKG-INFO
--rw-rw-rw-   0        0        0     5255 2024-03-21 14:36:06.000000 jacksung-0.0.2.96/README.md
-drwxrwxrwx   0        0        0        0 2024-03-25 08:19:59.418605 jacksung-0.0.2.96/jacksung/
--rw-rw-rw-   0        0        0       24 2023-08-31 10:50:52.000000 jacksung-0.0.2.96/jacksung/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:19:59.430635 jacksung-0.0.2.96/jacksung/utils/
--rw-rw-rw-   0        0        0       17 2023-08-31 11:05:26.000000 jacksung-0.0.2.96/jacksung/utils/__init__.py
--rw-rw-rw-   0        0        0     1828 2024-03-21 11:56:39.000000 jacksung-0.0.2.96/jacksung/utils/base_db.py
--rw-rw-rw-   0        0        0     1869 2024-03-04 13:31:13.000000 jacksung-0.0.2.96/jacksung/utils/cache.py
--rw-rw-rw-   0        0        0     4744 2024-03-22 08:18:07.000000 jacksung-0.0.2.96/jacksung/utils/data_convert.py
--rw-rw-rw-   0        0        0     3982 2024-03-22 09:19:49.000000 jacksung-0.0.2.96/jacksung/utils/fastnumpy.py
--rw-rw-rw-   0        0        0      803 2023-09-01 08:33:07.000000 jacksung-0.0.2.96/jacksung/utils/hash.py
--rw-rw-rw-   0        0        0     3776 2024-03-25 08:19:57.000000 jacksung-0.0.2.96/jacksung/utils/image.py
--rw-rw-rw-   0        0        0     2578 2023-12-27 05:28:31.000000 jacksung-0.0.2.96/jacksung/utils/log.py
--rw-rw-rw-   0        0        0     5022 2023-12-19 05:11:54.000000 jacksung-0.0.2.96/jacksung/utils/login.py
--rw-rw-rw-   0        0        0     2253 2023-12-27 08:56:29.000000 jacksung-0.0.2.96/jacksung/utils/mean_std.py
--rw-rw-rw-   0        0        0     1836 2024-02-22 09:27:05.000000 jacksung-0.0.2.96/jacksung/utils/multi_task.py
--rw-rw-rw-   0        0        0     4371 2023-11-22 07:25:41.000000 jacksung-0.0.2.96/jacksung/utils/nvidia.py
--rw-rw-rw-   0        0        0     2200 2024-03-22 09:06:48.000000 jacksung-0.0.2.96/jacksung/utils/time.py
-drwxrwxrwx   0        0        0        0 2024-03-25 08:19:59.423101 jacksung-0.0.2.96/jacksung.egg-info/
--rw-rw-rw-   0        0        0     5413 2024-03-25 08:19:59.000000 jacksung-0.0.2.96/jacksung.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      574 2024-03-25 08:19:59.000000 jacksung-0.0.2.96/jacksung.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 08:19:59.000000 jacksung-0.0.2.96/jacksung.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-03-25 08:19:59.000000 jacksung-0.0.2.96/jacksung.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       98 2024-03-25 08:19:59.000000 jacksung-0.0.2.96/jacksung.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-25 08:19:59.000000 jacksung-0.0.2.96/jacksung.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-25 08:19:59.432631 jacksung-0.0.2.96/setup.cfg
--rw-rw-rw-   0        0        0      714 2024-03-25 08:19:57.000000 jacksung-0.0.2.96/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 09:11:01.013861 jacksung-0.0.2.97/
+-rw-rw-rw-   0        0        0    11558 2023-11-22 07:36:29.000000 jacksung-0.0.2.97/LICENSE
+-rw-rw-rw-   0        0        0     5413 2024-04-02 09:11:01.013861 jacksung-0.0.2.97/PKG-INFO
+-rw-rw-rw-   0        0        0     5255 2024-03-21 14:36:06.000000 jacksung-0.0.2.97/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 09:11:00.987895 jacksung-0.0.2.97/jacksung/
+-rw-rw-rw-   0        0        0       24 2023-08-31 10:50:52.000000 jacksung-0.0.2.97/jacksung/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 09:11:01.012861 jacksung-0.0.2.97/jacksung/utils/
+-rw-rw-rw-   0        0        0       17 2023-08-31 11:05:26.000000 jacksung-0.0.2.97/jacksung/utils/__init__.py
+-rw-rw-rw-   0        0        0     1953 2024-04-02 09:10:13.000000 jacksung-0.0.2.97/jacksung/utils/base_db.py
+-rw-rw-rw-   0        0        0     1869 2024-03-04 13:31:13.000000 jacksung-0.0.2.97/jacksung/utils/cache.py
+-rw-rw-rw-   0        0        0     4744 2024-03-22 08:18:07.000000 jacksung-0.0.2.97/jacksung/utils/data_convert.py
+-rw-rw-rw-   0        0        0     3982 2024-03-22 09:19:49.000000 jacksung-0.0.2.97/jacksung/utils/fastnumpy.py
+-rw-rw-rw-   0        0        0      803 2023-09-01 08:33:07.000000 jacksung-0.0.2.97/jacksung/utils/hash.py
+-rw-rw-rw-   0        0        0     3859 2024-03-25 08:25:05.000000 jacksung-0.0.2.97/jacksung/utils/image.py
+-rw-rw-rw-   0        0        0     2705 2024-03-26 08:19:52.000000 jacksung-0.0.2.97/jacksung/utils/log.py
+-rw-rw-rw-   0        0        0     5022 2023-12-19 05:11:54.000000 jacksung-0.0.2.97/jacksung/utils/login.py
+-rw-rw-rw-   0        0        0     2253 2023-12-27 08:56:29.000000 jacksung-0.0.2.97/jacksung/utils/mean_std.py
+-rw-rw-rw-   0        0        0     1836 2024-02-22 09:27:05.000000 jacksung-0.0.2.97/jacksung/utils/multi_task.py
+-rw-rw-rw-   0        0        0     4371 2023-11-22 07:25:41.000000 jacksung-0.0.2.97/jacksung/utils/nvidia.py
+-rw-rw-rw-   0        0        0     2200 2024-03-22 09:06:48.000000 jacksung-0.0.2.97/jacksung/utils/time.py
+drwxrwxrwx   0        0        0        0 2024-04-02 09:11:01.002382 jacksung-0.0.2.97/jacksung.egg-info/
+-rw-rw-rw-   0        0        0     5413 2024-04-02 09:11:00.000000 jacksung-0.0.2.97/jacksung.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2024-04-02 09:11:00.000000 jacksung-0.0.2.97/jacksung.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 09:11:00.000000 jacksung-0.0.2.97/jacksung.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-04-02 09:11:00.000000 jacksung-0.0.2.97/jacksung.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       98 2024-04-02 09:11:00.000000 jacksung-0.0.2.97/jacksung.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 09:11:00.000000 jacksung-0.0.2.97/jacksung.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 09:11:01.013861 jacksung-0.0.2.97/setup.cfg
+-rw-rw-rw-   0        0        0      714 2024-04-02 09:10:13.000000 jacksung-0.0.2.97/setup.py
```

### Comparing `jacksung-0.0.2.96/LICENSE` & `jacksung-0.0.2.97/LICENSE`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.96/PKG-INFO` & `jacksung-0.0.2.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jacksung
-Version: 0.0.2.96
+Version: 0.0.2.97
 Author: Zijiang Song
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Jacksung's utils
 Python version is required above 3.9.
```

### Comparing `jacksung-0.0.2.96/README.md` & `jacksung-0.0.2.97/README.md`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.96/jacksung/utils/base_db.py` & `jacksung-0.0.2.97/jacksung/utils/base_db.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,13 +54,17 @@
         cursor = None
         try:
             cursor = self.conn.cursor()
             result = cursor.execute(sql)
         except Exception as e:
             self.conn = self.reconnect()
             cursor = self.conn.cursor()
-            result = cursor.execute(sql)
+            try:
+                result = cursor.execute(sql)
+            except Exception as e:
+                print(f'err SQL: {sql}')
+                raise e
         finally:
             if cursor:
                 cursor.close()
         self.lock_t.release()
         return result, cursor
```

### Comparing `jacksung-0.0.2.96/jacksung/utils/cache.py` & `jacksung-0.0.2.97/jacksung/utils/cache.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.96/jacksung/utils/data_convert.py` & `jacksung-0.0.2.97/jacksung/utils/data_convert.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.96/jacksung/utils/fastnumpy.py` & `jacksung-0.0.2.97/jacksung/utils/fastnumpy.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.96/jacksung/utils/hash.py` & `jacksung-0.0.2.97/jacksung/utils/hash.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.96/jacksung/utils/image.py` & `jacksung-0.0.2.97/jacksung/utils/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import cv2
 from PIL import Image, ImageFont, ImageDraw
 import numpy as np
+from data_convert import Coordinate
 
 
 def get_pixel_by_coord(img, coord, x, y):
     left, top, x_res, y_res = coord.left, coord.top, coord.x_res, coord.y_res
     if x < left or y > top:
         raise Exception(f'x:{x} or y:{y} is lower than border {left},{top}!'
                         f'left:{left}, top:{top},x_res:{x_res}, y_res:{y_res}.')
@@ -87,9 +88,11 @@
             y_offset += img.shape[0]
     else:
         raise ValueError("Invalid direction. Please choose 'h' or 'v'.")
     return new_img
 
 
 if __name__ == '__main__':
-    data = np.arange(0, 100).reshape((10, 10))
-    print(get_pixel_by_coord(data, 0, 90, 0.25, 0.25, 2.49, 87.6))
+    data = np.arange(0, 50).reshape((10, 5))
+    coord = Coordinate(0, 90, 0.25, 0.25)
+    print(data)
+    print(get_pixel_by_coord(data, coord, 0.76, 87.6))
```

### Comparing `jacksung-0.0.2.96/jacksung/utils/log.py` & `jacksung-0.0.2.97/jacksung/utils/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,8 +76,10 @@
         if self.on:
             try:
                 _thread.start_new_thread(thread_send_log, (self.url, content, name))
             except Exception as e:
                 print("Cloud Log Error")
 
 
-
+if __name__ == '__main__':
+    sys.stdout = StdLog(filename='log.txt', common_path='warning.txt')
+    oprint('this is a log')
```

### Comparing `jacksung-0.0.2.96/jacksung/utils/login.py` & `jacksung-0.0.2.97/jacksung/utils/login.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.96/jacksung/utils/mean_std.py` & `jacksung-0.0.2.97/jacksung/utils/mean_std.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.96/jacksung/utils/multi_task.py` & `jacksung-0.0.2.97/jacksung/utils/multi_task.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.96/jacksung/utils/nvidia.py` & `jacksung-0.0.2.97/jacksung/utils/nvidia.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.96/jacksung/utils/time.py` & `jacksung-0.0.2.97/jacksung/utils/time.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.96/jacksung.egg-info/PKG-INFO` & `jacksung-0.0.2.97/jacksung.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jacksung
-Version: 0.0.2.96
+Version: 0.0.2.97
 Author: Zijiang Song
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Jacksung's utils
 Python version is required above 3.9.
```

### Comparing `jacksung-0.0.2.96/jacksung.egg-info/SOURCES.txt` & `jacksung-0.0.2.97/jacksung.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.96/setup.py` & `jacksung-0.0.2.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jacksung',
-    version='0.0.2.96',
+    version='0.0.2.97',
     author='Zijiang Song',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'tqdm',
         'requests',
```

