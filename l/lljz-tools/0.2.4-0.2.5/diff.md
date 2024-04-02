# Comparing `tmp/lljz_tools-0.2.4.tar.gz` & `tmp/lljz_tools-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lljz_tools-0.2.4.tar", last modified: Wed Feb 28 03:53:44 2024, max compression
+gzip compressed data, was "lljz_tools-0.2.5.tar", last modified: Tue Apr  2 10:00:32 2024, max compression
```

## Comparing `lljz_tools-0.2.4.tar` & `lljz_tools-0.2.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 03:53:44.938144 lljz_tools-0.2.4/
--rw-rw-rw-   0        0        0     1073 2024-02-02 08:09:22.000000 lljz_tools-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     4233 2024-02-28 03:53:44.937144 lljz_tools-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     3755 2024-02-03 07:02:42.000000 lljz_tools-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-02-28 03:53:44.923314 lljz_tools-0.2.4/lljz_tools.egg-info/
--rw-rw-rw-   0        0        0     4233 2024-02-28 03:53:44.000000 lljz_tools-0.2.4/lljz_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      493 2024-02-28 03:53:44.000000 lljz_tools-0.2.4/lljz_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 03:53:44.000000 lljz_tools-0.2.4/lljz_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-02-28 03:53:44.000000 lljz_tools-0.2.4/lljz_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-28 03:53:44.000000 lljz_tools-0.2.4/lljz_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-28 03:53:44.930132 lljz_tools-0.2.4/my_tools/
--rw-rw-rw-   0        0        0      179 2024-02-02 08:07:00.000000 lljz_tools-0.2.4/my_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-28 03:53:44.933145 lljz_tools-0.2.4/my_tools/attribute_dict/
--rw-rw-rw-   0        0        0      261 2024-02-03 06:30:03.000000 lljz_tools-0.2.4/my_tools/attribute_dict/__init__.py
--rw-rw-rw-   0        0        0     5886 2024-02-03 06:29:33.000000 lljz_tools-0.2.4/my_tools/attribute_dict/model.py
-drwxrwxrwx   0        0        0        0 2024-02-28 03:53:44.936144 lljz_tools-0.2.4/my_tools/client/
--rw-rw-rw-   0        0        0      179 2024-02-08 04:17:05.000000 lljz_tools-0.2.4/my_tools/client/__init__.py
--rw-rw-rw-   0        0        0     5155 2024-02-28 03:49:18.000000 lljz_tools-0.2.4/my_tools/client/db_client.py
--rw-rw-rw-   0        0        0      407 2024-02-28 03:52:30.000000 lljz_tools-0.2.4/my_tools/client/http_client.py
--rw-rw-rw-   0        0        0     2970 2024-02-03 06:37:05.000000 lljz_tools-0.2.4/my_tools/console_table.py
--rw-rw-rw-   0        0        0     5328 2024-02-28 03:20:05.000000 lljz_tools-0.2.4/my_tools/decorators.py
--rw-rw-rw-   0        0        0     3443 2024-02-22 10:27:08.000000 lljz_tools-0.2.4/my_tools/excel.py
--rw-rw-rw-   0        0        0     4332 2024-02-22 09:50:16.000000 lljz_tools-0.2.4/my_tools/log_manager.py
--rw-rw-rw-   0        0        0     1595 2024-02-22 09:50:16.000000 lljz_tools-0.2.4/my_tools/monkey.py
--rw-rw-rw-   0        0        0       85 2024-02-28 03:53:44.939142 lljz_tools-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      684 2024-02-28 03:53:42.000000 lljz_tools-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:00:32.872407 lljz_tools-0.2.5/
+-rw-rw-rw-   0        0        0     1073 2024-02-02 08:09:22.000000 lljz_tools-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     4233 2024-04-02 10:00:32.871407 lljz_tools-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3755 2024-02-03 07:02:42.000000 lljz_tools-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 10:00:32.855408 lljz_tools-0.2.5/lljz_tools.egg-info/
+-rw-rw-rw-   0        0        0     4233 2024-04-02 10:00:32.000000 lljz_tools-0.2.5/lljz_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2024-04-02 10:00:32.000000 lljz_tools-0.2.5/lljz_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 10:00:32.000000 lljz_tools-0.2.5/lljz_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-02 10:00:32.000000 lljz_tools-0.2.5/lljz_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 10:00:32.000000 lljz_tools-0.2.5/lljz_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 10:00:32.863407 lljz_tools-0.2.5/my_tools/
+-rw-rw-rw-   0        0        0      179 2024-02-02 08:07:00.000000 lljz_tools-0.2.5/my_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:00:32.866407 lljz_tools-0.2.5/my_tools/attribute_dict/
+-rw-rw-rw-   0        0        0      261 2024-02-03 06:30:03.000000 lljz_tools-0.2.5/my_tools/attribute_dict/__init__.py
+-rw-rw-rw-   0        0        0     5886 2024-02-03 06:29:33.000000 lljz_tools-0.2.5/my_tools/attribute_dict/model.py
+drwxrwxrwx   0        0        0        0 2024-04-02 10:00:32.870408 lljz_tools-0.2.5/my_tools/client/
+-rw-rw-rw-   0        0        0      179 2024-02-08 04:17:05.000000 lljz_tools-0.2.5/my_tools/client/__init__.py
+-rw-rw-rw-   0        0        0     5155 2024-02-28 03:49:18.000000 lljz_tools-0.2.5/my_tools/client/db_client.py
+-rw-rw-rw-   0        0        0      432 2024-02-28 06:33:46.000000 lljz_tools-0.2.5/my_tools/client/http_client.py
+-rw-rw-rw-   0        0        0     1417 2024-04-02 09:57:01.000000 lljz_tools-0.2.5/my_tools/color.py
+-rw-rw-rw-   0        0        0     2486 2024-04-02 09:58:38.000000 lljz_tools-0.2.5/my_tools/console_table.py
+-rw-rw-rw-   0        0        0     5328 2024-02-28 03:20:05.000000 lljz_tools-0.2.5/my_tools/decorators.py
+-rw-rw-rw-   0        0        0     3659 2024-02-29 18:00:07.000000 lljz_tools-0.2.5/my_tools/excel.py
+-rw-rw-rw-   0        0        0     4332 2024-02-22 09:50:16.000000 lljz_tools-0.2.5/my_tools/log_manager.py
+-rw-rw-rw-   0        0        0     1595 2024-02-22 09:50:16.000000 lljz_tools-0.2.5/my_tools/monkey.py
+-rw-rw-rw-   0        0        0       85 2024-04-02 10:00:32.874410 lljz_tools-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      684 2024-04-02 10:00:10.000000 lljz_tools-0.2.5/setup.py
```

### Comparing `lljz_tools-0.2.4/LICENSE` & `lljz_tools-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.4/PKG-INFO` & `lljz_tools-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lljz_tools
-Version: 0.2.4
+Version: 0.2.5
 Summary: 常用工具封装
 Home-page: 
 Author: liulangjuanzhou
 Author-email: liulangjuanzhou@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lljz_tools-0.2.4/README.md` & `lljz_tools-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.4/lljz_tools.egg-info/PKG-INFO` & `lljz_tools-0.2.5/lljz_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lljz-tools
-Version: 0.2.4
+Version: 0.2.5
 Summary: 常用工具封装
 Home-page: 
 Author: liulangjuanzhou
 Author-email: liulangjuanzhou@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lljz_tools-0.2.4/my_tools/attribute_dict/model.py` & `lljz_tools-0.2.5/my_tools/attribute_dict/model.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.4/my_tools/client/db_client.py` & `lljz_tools-0.2.5/my_tools/client/db_client.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.4/my_tools/console_table.py` & `lljz_tools-0.2.5/my_tools/console_table.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,72 @@
 # coding=utf-8
-
+from typing import Iterable, Any
+from my_tools.color import _Color
 from my_tools.log_manager import LogManager
 
 logger = LogManager('ConsoleTable').get_logger()
 
 
 class ConsoleTable:
 
-    def __init__(self, data: list[dict]):  # noqa
-        # assert data, 'data is empty!'
-        self.rawData = data
-        self._colWidth = 0
-        self.header = list(data[0].keys()) if data else []
-        self._header = []
-        self._body = []
-        self._stringWidth = {}
-
-    def _getStrWidth(self, string):
-        if string in self._stringWidth:
-            return self._stringWidth[string]
-        width = 0
-
-        for s in string:
-            if u'\u4e00' <= s <= u'\u9fff' or s in '【】（）—…￥！·、？。，《》：；‘“':
-                width += 2
+    def __init__(self, data: Iterable[dict[str, Any]], max_width=100):
+        def init_value(val):
+            if isinstance(val, str | _Color):
+                return val
+            if val is None:
+                return ''
+            return str(val)
+
+        self.data = [{str(k): init_value(v) for k, v in row.items()} for row in data]
+        self.header = list(self.data[0].keys()) if data else []
+        self.max_width = max_width
+        self.col_width = self._get_widths()
+        self._table_str = self._make_table_str()
+
+    @staticmethod
+    def _get_string_width(val: str):
+        w = 0
+        for v in val:
+            if u'\u4e00' <= v <= u'\u9fff' or v in '【】（）—…￥！·、？。，《》：；‘“':
+                w += 2
             else:
-                width += 1
-        self._stringWidth[string] = width
-        self._colWidth = max(width, self._colWidth)
-        return width
-
-    @property
-    def colWidth(self):
-        if self._colWidth:
-            return self._colWidth
-        for h in self.header:
-            self._getStrWidth(h)
-        for row in self.rawData:
-            for b in row:
-                b = str(b)
-                self._getStrWidth(b)
-        return self._colWidth
-
-    def _initStr(self, string):
-        width = self._getStrWidth(string)
-        b = (self.colWidth - width) // 2
-        a = (self.colWidth - width) - b
-        return f'{" " * a}{string}{" " * b}'
+                w += 1
+        return w
+
+    def _get_widths(self):
+        """获取列宽度，列宽度为整列数据中的最大数据宽度"""
+
+        col_width = [self._get_string_width(key) for key in self.header]
+        for row in self.data:
+            for i, key in enumerate(self.header):
+                value = row.get(key, '')
+                width = min(self._get_string_width(value), self.max_width)
+                col_width[i] = max(col_width[i], width)
+        return col_width
+
+    def _make_table_str(self):
+        def format_str(val, width):
+            length = self._get_string_width(val)
+            left = (width - length) // 2
+            right = (width - length) - left
+            return f'{" " * left}{val}{" " * right}'
+
+        header = ' | '.join(format_str(key, w) for w, key in zip(self.col_width, self.header))
+        rows = [' | '.join(format_str(row.get(key, ""), w) for w, key in zip(self.col_width, self.header)) for row in
+                self.data]
+        return '\n'.join([header, '=' * len(header)] + rows)
 
     def __str__(self):
-        if not self.rawData:
-            return 'console table is empty!'
+        return self._table_str
 
-        data = []
-        # 计算每列的最大宽度
-        colWidth = [10] * len(self.header)  # 每列的初始宽度
-        for i, h in enumerate(self.header):
-            colWidth[i] = max(colWidth[i], self._getStrWidth(str(h)))
-        for row in self.rawData:
-            for i, value in enumerate(row.values()):
-                colWidth[i] = max(colWidth[i], self._getStrWidth(str(value)))
-        d = []
-        for w, value in zip(colWidth, self.header):
-            k = self._getStrWidth(str(value))
-            b = (w - k) // 2
-            a = (w - k) - b
-            d.append(f'{" " * a}{value}{" " * b}')
-        data.append(d)
-        for row in self.rawData:
-            d = []
-            for w, value in zip(colWidth, row.values()):
-                k = self._getStrWidth(str(value))
-                b = (w - k) // 2
-                a = (w - k) - b
-                d.append(f'{" " * a}{value}{" " * b}')
-            data.append(d)
-        show = [' | '.join(data[0]), '=' * (sum(colWidth) + (3 * (len(self.header) - 1)))]
-        for i in data[1:]:
-            show.append(' | '.join(i))
-        return '\n'.join(show)
+    __repr__ = __str__
 
     def show(self, message=''):
         logger.info(message + '\n' + str(self.__str__()))
 
 
 if __name__ == '__main__':
-    table = ConsoleTable([{'name': "Tom", 'b': 2}, {'name': "Lucy", 'b': 4}])
+    from my_tools.color import Color
+    table = ConsoleTable([{'name': Color.red("Tom"), 'b': 2}, {'name': Color.blue("Lucy"), 'b': 4}])
     table.show()
     print(table)
     pass
```

### Comparing `lljz_tools-0.2.4/my_tools/decorators.py` & `lljz_tools-0.2.5/my_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.4/my_tools/excel.py` & `lljz_tools-0.2.5/my_tools/excel.py`

 * *Files 16% similar despite different names*

```diff
@@ -66,38 +66,40 @@
 class ExcelWrite:
 
     def __init__(self, excel_filename: str):
         if not excel_filename.endswith('.xlsx'):
             raise TypeError('Only support xlsx file')
         self._file = excel_filename
         self._excel = Workbook(write_only=True)
-        self._sheet_index = 0
+        self._sheets = {}
 
-    def write(self, data, /, *, sheet_name=None):
-        self._sheet_index += 1
-        if not sheet_name:
-            sheet_name = f'Sheet{self._sheet_index}'
-        sheet = self._excel.create_sheet(title=sheet_name)
+    def write(self, data: list[list | dict], /, *, sheet_name=None):
         if not data:
             return
+        if not sheet_name:
+            sheet_name = f'Sheet{len(self._sheets) + 1}'
         data = iter(data)
-        first = next(data)
-        if isinstance(first, dict):
-            sheet.append(first.keys())
-            sheet.append(first.values())
-        else:
-            sheet.append(first)
-        for r in data:
+
+        if sheet_name not in self._sheets:
+            self._sheets[sheet_name] = self._excel.create_sheet(title=sheet_name)
+            first = next(data)
             if isinstance(first, dict):
-                sheet.append(r.values())
+                self._sheets[sheet_name].append(first.keys())
+                self._sheets[sheet_name].append(first.values())
             else:
-                sheet.append(r)
+                self._sheets[sheet_name].append(first)
+        for r in data:
+            if isinstance(r, dict):
+                self._sheets[sheet_name].append(r.values())
+            else:
+                self._sheets[sheet_name].append(r)
 
     def save(self):
         self._excel.save(self._file)
 
+
 if __name__ == '__main__':
     excel = ExcelWrite(r"./test.xlsx")
-    excel.write([["name", "age"], ["aaa", 11], ["bbb", 22], ["ccc", 33]])
-    excel.write([["name", "age"], ["aaa", 11], ["bbb", 22], ["ccc", 33]])
+    excel.write([["name", "age"], ["aaa", 11], ["bbb", 22], ["ccc", 33]], sheet_name="Sheet1")
+    excel.write([["dasdsa", "ff"], ["aaa", 11], ["bbb", 22], ["ccc", 33]], sheet_name="Sheet1")
     excel.save()
     pass
```

### Comparing `lljz_tools-0.2.4/my_tools/log_manager.py` & `lljz_tools-0.2.5/my_tools/log_manager.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.4/my_tools/monkey.py` & `lljz_tools-0.2.5/my_tools/monkey.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.4/setup.py` & `lljz_tools-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lljz_tools",
-    version="0.2.4",
+    version="0.2.5",
     author="liulangjuanzhou",
     author_email="liulangjuanzhou@gmail.com",
     description="常用工具封装",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

