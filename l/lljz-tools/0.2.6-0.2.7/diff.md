# Comparing `tmp/lljz_tools-0.2.6.tar.gz` & `tmp/lljz_tools-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lljz_tools-0.2.6.tar", last modified: Tue Apr  2 10:37:34 2024, max compression
+gzip compressed data, was "lljz_tools-0.2.7.tar", last modified: Tue Apr  2 12:51:56 2024, max compression
```

## Comparing `lljz_tools-0.2.6.tar` & `lljz_tools-0.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:34.881381 lljz_tools-0.2.6/
--rw-rw-rw-   0        0        0     1073 2024-02-02 08:09:22.000000 lljz_tools-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     4233 2024-04-02 10:37:34.881381 lljz_tools-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     3755 2024-02-03 07:02:42.000000 lljz_tools-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:34.868378 lljz_tools-0.2.6/lljz_tools.egg-info/
--rw-rw-rw-   0        0        0     4233 2024-04-02 10:37:34.000000 lljz_tools-0.2.6/lljz_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      511 2024-04-02 10:37:34.000000 lljz_tools-0.2.6/lljz_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 10:37:34.000000 lljz_tools-0.2.6/lljz_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-02 10:37:34.000000 lljz_tools-0.2.6/lljz_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 10:37:34.000000 lljz_tools-0.2.6/lljz_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:34.875379 lljz_tools-0.2.6/my_tools/
--rw-rw-rw-   0        0        0      179 2024-02-02 08:07:00.000000 lljz_tools-0.2.6/my_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:34.877379 lljz_tools-0.2.6/my_tools/attribute_dict/
--rw-rw-rw-   0        0        0      261 2024-02-03 06:30:03.000000 lljz_tools-0.2.6/my_tools/attribute_dict/__init__.py
--rw-rw-rw-   0        0        0     5886 2024-02-03 06:29:33.000000 lljz_tools-0.2.6/my_tools/attribute_dict/model.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:37:34.880378 lljz_tools-0.2.6/my_tools/client/
--rw-rw-rw-   0        0        0      179 2024-02-08 04:17:05.000000 lljz_tools-0.2.6/my_tools/client/__init__.py
--rw-rw-rw-   0        0        0     5155 2024-02-28 03:49:18.000000 lljz_tools-0.2.6/my_tools/client/db_client.py
--rw-rw-rw-   0        0        0      432 2024-02-28 06:33:46.000000 lljz_tools-0.2.6/my_tools/client/http_client.py
--rw-rw-rw-   0        0        0     1417 2024-04-02 09:57:01.000000 lljz_tools-0.2.6/my_tools/color.py
--rw-rw-rw-   0        0        0     2486 2024-04-02 09:58:38.000000 lljz_tools-0.2.6/my_tools/console_table.py
--rw-rw-rw-   0        0        0     5328 2024-02-28 03:20:05.000000 lljz_tools-0.2.6/my_tools/decorators.py
--rw-rw-rw-   0        0        0     3659 2024-02-29 18:00:07.000000 lljz_tools-0.2.6/my_tools/excel.py
--rw-rw-rw-   0        0        0     5180 2024-04-02 10:36:48.000000 lljz_tools-0.2.6/my_tools/log_manager.py
--rw-rw-rw-   0        0        0     1595 2024-02-22 09:50:16.000000 lljz_tools-0.2.6/my_tools/monkey.py
--rw-rw-rw-   0        0        0       85 2024-04-02 10:37:34.883380 lljz_tools-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      684 2024-04-02 10:37:33.000000 lljz_tools-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:51:56.727055 lljz_tools-0.2.7/
+-rw-rw-rw-   0        0        0     1073 2024-02-02 08:09:22.000000 lljz_tools-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0     4188 2024-04-02 12:51:56.726054 lljz_tools-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3755 2024-02-03 07:02:42.000000 lljz_tools-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 12:51:56.712056 lljz_tools-0.2.7/lljz_tools.egg-info/
+-rw-rw-rw-   0        0        0     4188 2024-04-02 12:51:56.000000 lljz_tools-0.2.7/lljz_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2024-04-02 12:51:56.000000 lljz_tools-0.2.7/lljz_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 12:51:56.000000 lljz_tools-0.2.7/lljz_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-02 12:51:56.000000 lljz_tools-0.2.7/lljz_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 12:51:56.000000 lljz_tools-0.2.7/lljz_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 12:51:56.719056 lljz_tools-0.2.7/my_tools/
+-rw-rw-rw-   0        0        0      179 2024-02-02 08:07:00.000000 lljz_tools-0.2.7/my_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:51:56.721056 lljz_tools-0.2.7/my_tools/attribute_dict/
+-rw-rw-rw-   0        0        0      261 2024-02-03 06:30:03.000000 lljz_tools-0.2.7/my_tools/attribute_dict/__init__.py
+-rw-rw-rw-   0        0        0     5886 2024-02-03 06:29:33.000000 lljz_tools-0.2.7/my_tools/attribute_dict/model.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:51:56.725056 lljz_tools-0.2.7/my_tools/client/
+-rw-rw-rw-   0        0        0      179 2024-02-08 04:17:05.000000 lljz_tools-0.2.7/my_tools/client/__init__.py
+-rw-rw-rw-   0        0        0     5155 2024-02-28 03:49:18.000000 lljz_tools-0.2.7/my_tools/client/db_client.py
+-rw-rw-rw-   0        0        0      434 2024-04-02 11:32:23.000000 lljz_tools-0.2.7/my_tools/client/http_client.py
+-rw-rw-rw-   0        0        0     1417 2024-04-02 09:57:01.000000 lljz_tools-0.2.7/my_tools/color.py
+-rw-rw-rw-   0        0        0     2458 2024-04-02 12:02:46.000000 lljz_tools-0.2.7/my_tools/console_table.py
+-rw-rw-rw-   0        0        0     5328 2024-02-28 03:20:05.000000 lljz_tools-0.2.7/my_tools/decorators.py
+-rw-rw-rw-   0        0        0     4543 2024-04-02 11:51:16.000000 lljz_tools-0.2.7/my_tools/excel.py
+-rw-rw-rw-   0        0        0     5180 2024-04-02 10:36:48.000000 lljz_tools-0.2.7/my_tools/log_manager.py
+-rw-rw-rw-   0        0        0     1595 2024-02-22 09:50:16.000000 lljz_tools-0.2.7/my_tools/monkey.py
+-rw-rw-rw-   0        0        0       85 2024-04-02 12:51:56.728057 lljz_tools-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      665 2024-04-02 12:51:52.000000 lljz_tools-0.2.7/setup.py
```

### Comparing `lljz_tools-0.2.6/LICENSE` & `lljz_tools-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.6/PKG-INFO` & `lljz_tools-0.2.7/lljz_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
-Name: lljz_tools
-Version: 0.2.6
+Name: lljz-tools
+Version: 0.2.7
 Summary: 常用工具封装
 Home-page: 
 Author: liulangjuanzhou
 Author-email: liulangjuanzhou@gmail.com
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorlog
 Requires-Dist: openpyxl
-Requires-Dist: pymysql
-Requires-Dist: DBUtils
 
 ## 简介
 包含了一些常用方法的封装，安装方法
 ```
 pip install lljz_tools
 ```
 内含
```

### Comparing `lljz_tools-0.2.6/README.md` & `lljz_tools-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.6/lljz_tools.egg-info/PKG-INFO` & `lljz_tools-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
-Name: lljz-tools
-Version: 0.2.6
+Name: lljz_tools
+Version: 0.2.7
 Summary: 常用工具封装
 Home-page: 
 Author: liulangjuanzhou
 Author-email: liulangjuanzhou@gmail.com
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorlog
 Requires-Dist: openpyxl
-Requires-Dist: pymysql
-Requires-Dist: DBUtils
 
 ## 简介
 包含了一些常用方法的封装，安装方法
 ```
 pip install lljz_tools
 ```
 内含
```

### Comparing `lljz_tools-0.2.6/my_tools/attribute_dict/model.py` & `lljz_tools-0.2.7/my_tools/attribute_dict/model.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.6/my_tools/client/db_client.py` & `lljz_tools-0.2.7/my_tools/client/db_client.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.6/my_tools/color.py` & `lljz_tools-0.2.7/my_tools/color.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.6/my_tools/console_table.py` & `lljz_tools-0.2.7/my_tools/console_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,9 +64,7 @@
         logger.info(message + '\n' + str(self.__str__()))
 
 
 if __name__ == '__main__':
     from my_tools.color import Color
     table = ConsoleTable([{'name': Color.red("Tom"), 'b': 2}, {'name': Color.blue("Lucy"), 'b': 4}])
     table.show()
-    print(table)
-    pass
```

### Comparing `lljz_tools-0.2.6/my_tools/decorators.py` & `lljz_tools-0.2.7/my_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.6/my_tools/excel.py` & `lljz_tools-0.2.7/my_tools/excel.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,15 +14,19 @@
 class ExcelReader:
 
     def __init__(self, excel_filename: str):
         if not excel_filename.endswith('.xlsx'):
             raise TypeError('Only support xlsx file')
         if not os.path.exists(excel_filename):
             raise FileNotFoundError(f"{excel_filename} not found!")
-        self._excel = load_workbook(excel_filename, read_only=True, data_only=True)
+        self._file = excel_filename
+        self._excel = self._get_excel()
+
+    def _get_excel(self):
+        return load_workbook(self._file, read_only=True, data_only=True)
 
     def _get_sheet(self, sheet: int | None | str) -> Worksheet:
         if isinstance(sheet, int):
             return self._excel.worksheets[sheet]
         elif isinstance(sheet, str):
             return self._excel[sheet]
         return self._excel.active
@@ -65,41 +69,67 @@
 
 class ExcelWrite:
 
     def __init__(self, excel_filename: str):
         if not excel_filename.endswith('.xlsx'):
             raise TypeError('Only support xlsx file')
         self._file = excel_filename
-        self._excel = Workbook(write_only=True)
-        self._sheets = {}
+        self._sheets: dict[str, Worksheet] = {}
+        self._excel = self._get_excel()
 
-    def write(self, data: list[list | dict], /, *, sheet_name=None):
-        if not data:
-            return
+    def _get_excel(self) -> Workbook:  # noqa
+        return Workbook(write_only=True)
+
+    def write(self, data: list[list | dict], /, *, sheet_name=None) -> Worksheet:
         if not sheet_name:
             sheet_name = f'Sheet{len(self._sheets) + 1}'
-        data = iter(data)
-
         if sheet_name not in self._sheets:
             self._sheets[sheet_name] = self._excel.create_sheet(title=sheet_name)
-            first = next(data)
-            if isinstance(first, dict):
-                self._sheets[sheet_name].append(first.keys())
-                self._sheets[sheet_name].append(first.values())
-            else:
-                self._sheets[sheet_name].append(first)
+        if not data:
+            return self._sheets[sheet_name]
+
+        data = iter(data)
+        first = next(data)
+        if isinstance(first, dict):
+            self._sheets[sheet_name].append(tuple(first.keys()))  # write_title
+            self._sheets[sheet_name].append(tuple(first.values()))
+        else:
+            self._sheets[sheet_name].append(first)
         for r in data:
             if isinstance(r, dict):
-                self._sheets[sheet_name].append(r.values())
+                self._sheets[sheet_name].append(tuple(r.values()))
             else:
                 self._sheets[sheet_name].append(r)
+        return self._sheets[sheet_name]
 
     def save(self):
         self._excel.save(self._file)
 
 
+class Excel(ExcelReader, ExcelWrite):
+
+    def __init__(self, excel_filename: str):
+        super().__init__(excel_filename=excel_filename)
+        self._sheets = {name: self._excel[name] for name in self._excel.sheetnames}
+
+    def _get_excel(self):  # noqa
+        return load_workbook(self._file, data_only=True)
+
+    def write(self, data, /, *, sheet_name=None):
+        if not sheet_name:
+            sheet_name = self._excel.active.title
+        return super().write(data, sheet_name=sheet_name)
+
+    def __getitem__(self, item) -> Worksheet:
+        return self._excel[item]
+
+
 if __name__ == '__main__':
-    excel = ExcelWrite(r"./test.xlsx")
-    excel.write([["name", "age"], ["aaa", 11], ["bbb", 22], ["ccc", 33]], sheet_name="Sheet1")
-    excel.write([["dasdsa", "ff"], ["aaa", 11], ["bbb", 22], ["ccc", 33]], sheet_name="Sheet1")
-    excel.save()
+    # excel = Excel(r"./test.xlsx")
+    # sheet = excel['Sheet2']
+    # print(sheet)
+    # for row in excel.read(has_title=True):
+    #     print(row)
+    # print()
+    # excel.write([{"name": 'Jack', 'age': 77}])
+    # excel.save()
     pass
```

### Comparing `lljz_tools-0.2.6/my_tools/log_manager.py` & `lljz_tools-0.2.7/my_tools/log_manager.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.6/my_tools/monkey.py` & `lljz_tools-0.2.7/my_tools/monkey.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.6/setup.py` & `lljz_tools-0.2.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lljz_tools",
-    version="0.2.6",
+    version="0.2.7",
     author="liulangjuanzhou",
     author_email="liulangjuanzhou@gmail.com",
     description="常用工具封装",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
-    install_requires=['colorlog', 'openpyxl', 'pymysql', 'DBUtils'],
+    install_requires=['colorlog', 'openpyxl'],
     classifiers=[
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

