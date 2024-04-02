# Comparing `tmp/pr_properties-1.8.4.tar.gz` & `tmp/pr_properties-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_properties-1.8.4.tar", max compression
+gzip compressed data, was "pr_properties-1.8.5.tar", max compression
```

## Comparing `pr_properties-1.8.4.tar` & `pr_properties-1.8.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35823 2023-10-24 13:34:44.381986 pr_properties-1.8.4/LICENSE
--rw-r--r--   0        0        0      590 2023-10-24 13:34:44.381986 pr_properties-1.8.4/license.txt
--rw-r--r--   0        0        0       73 2023-10-24 12:05:04.847276 pr_properties-1.8.4/pr_properties/__init__.py
--rw-r--r--   0        0        0     4734 2023-11-01 15:50:58.714861 pr_properties-1.8.4/pr_properties/pr_properties.py
--rw-r--r--   0        0        0        0 2023-10-24 12:05:04.847276 pr_properties-1.8.4/pr_properties/test_case/__init__.py
--rw-r--r--   0        0        0      104 2023-10-25 14:24:08.260109 pr_properties-1.8.4/pr_properties/test_case/pool.properties
--rw-r--r--   0        0        0       42 2023-10-24 12:05:04.848465 pr_properties-1.8.4/pr_properties/test_case/pool.properties.bak
--rw-r--r--   0        0        0       79 2023-10-24 12:54:14.484122 pr_properties-1.8.4/pr_properties/test_case/pool.properties.pr_bak
--rw-r--r--   0        0        0     1036 2023-11-01 15:54:38.973037 pr_properties-1.8.4/pr_properties/test_case/test_properties.py
--rw-r--r--   0        0        0      475 2023-11-01 15:56:19.400199 pr_properties-1.8.4/pyproject.toml
--rw-r--r--   0        0        0      552 2023-10-24 13:26:21.048473 pr_properties-1.8.4/README.md
--rw-r--r--   0        0        0     1226 1970-01-01 00:00:00.000000 pr_properties-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-08-17 01:56:54.560103 pr_properties-1.8.5/LICENSE
+-rw-r--r--   0        0        0      590 2023-08-17 01:56:54.561108 pr_properties-1.8.5/license.txt
+-rw-r--r--   0        0        0       73 2023-08-17 03:17:40.436000 pr_properties-1.8.5/pr_properties/__init__.py
+-rw-r--r--   0        0        0     5395 2024-04-02 07:06:21.889755 pr_properties-1.8.5/pr_properties/pr_properties.py
+-rw-r--r--   0        0        0        0 2023-08-17 02:30:25.407000 pr_properties-1.8.5/pr_properties/test_case/__init__.py
+-rw-r--r--   0        0        0      104 2023-10-25 08:19:30.893258 pr_properties-1.8.5/pr_properties/test_case/pool.properties
+-rw-r--r--   0        0        0       42 2023-08-17 01:56:54.563963 pr_properties-1.8.5/pr_properties/test_case/pool.properties.bak
+-rw-r--r--   0        0        0       79 2023-10-24 13:43:33.465741 pr_properties-1.8.5/pr_properties/test_case/pool.properties.pr_bak
+-rw-r--r--   0        0        0     1036 2024-04-02 07:05:38.083706 pr_properties-1.8.5/pr_properties/test_case/test_properties.py
+-rw-r--r--   0        0        0      475 2024-04-02 07:06:21.893088 pr_properties-1.8.5/pyproject.toml
+-rw-r--r--   0        0        0      552 2023-10-24 13:43:33.462629 pr_properties-1.8.5/README.md
+-rw-r--r--   0        0        0     1277 1970-01-01 00:00:00.000000 pr_properties-1.8.5/PKG-INFO
```

### Comparing `pr_properties-1.8.4/LICENSE` & `pr_properties-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_properties-1.8.4/license.txt` & `pr_properties-1.8.5/license.txt`

 * *Files identical despite different names*

### Comparing `pr_properties-1.8.4/pr_properties/pr_properties.py` & `pr_properties-1.8.5/pr_properties/pr_properties.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,23 +24,24 @@
         backup_file_path = self.file_path + '.pr_bak'
         if not os.path.exists(backup_file_path):
             try:
                 shutil.copy2(self.file_path, backup_file_path)
             except IOError as e:
                 raise Exception(f"备份文件时出现错误：{e}")
 
-    def _read(self):
+    def _read(self, encoding='utf-8', ignore_errors=False):
         if not os.path.exists(self.file_path):
             raise FileNotFoundError("文件路径不存在")
 
         try:
             lock = filelock.FileLock(self.file_path + '.lock')
 
             with lock.acquire(timeout=10):
-                with open(self.file_path, 'r', encoding='utf-8') as file:
+                with open(self.file_path, 'r', encoding=encoding,
+                          errors='ignore' if ignore_errors else 'strict') as file:
                     lines = file.readlines()
             # 释放文件锁
             lock.release()
 
             for line in lines:
                 line = line.strip()
 
@@ -65,28 +66,30 @@
                 self.properties[key] = value
 
         except IOError as e:
             raise Exception(f"读取文件时出现错误：{e}")
 
         return self
 
-    def read(self, file_path=None):
+    def read(self, file_path=None, encoding='utf-8', ignore_errors=False):
         """
-        从文件中读取属性。
+        读取文件内容。
 
-        参数：
-        - file_path：文件路径，默认为None。
-
-        返回：
-        - properties：读取到的属性字典。
+        :param file_path: 指定要读取的文件路径，如果为None，则使用对象初始化时指定的路径。
+        :param encoding: 读取文件时使用的编码格式，默认为'utf-8'。
+        :param ignore_errors: 是否忽略读取过程中出现的编码错误，默认为False。
+        :return: 返回文件内容。
         """
+        # 如果提供了文件路径，则更新对象的文件路径
         if file_path is not None:
             self.file_path = file_path
-        self.__class__(self.file_path)
-        return self._read()
+        # 重新初始化文件读取器，确保文件路径是最新的
+        self.__init__(self.file_path)
+        # 使用指定的编码和错误处理方式读取文件内容
+        return self._read(encoding=encoding, ignore_errors=ignore_errors)
 
     def write(self):
         """
         将属性写入文件。
         """
         self.backup()
 
@@ -158,8 +161,9 @@
                     output += line_str  # 如果是最后一个属性，不再添加换行符
                 else:
                     output += line_str + '\n'  # 写入属性和对应的值
         output = output.rstrip('\n')  # 删除末尾的换行符
         return output
 
 
+# 多线程的情况下请勿使用单例模式
 pr_properties = PropertiesHandler()
```

### Comparing `pr_properties-1.8.4/pr_properties/test_case/test_properties.py` & `pr_properties-1.8.5/pr_properties/test_case/test_properties.py`

 * *Files identical despite different names*

### Comparing `pr_properties-1.8.4/README.md` & `pr_properties-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pr_properties-1.8.4/PKG-INFO` & `pr_properties-1.8.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pr_properties
-Version: 1.8.4
+Version: 1.8.5
 Summary: 
 License: Apache-2.0
 Author: Franciz
 Author-email: Franciz467@163.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: filelock (==3.12.2)
 Description-Content-Type: text/markdown
 
 安装
 pip install pr-properties
 
 这是一个读写properties工具
```

