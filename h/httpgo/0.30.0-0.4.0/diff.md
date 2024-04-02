# Comparing `tmp/httpgo-0.30.0.tar.gz` & `tmp/httpgo-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpgo-0.30.0.tar", last modified: Tue Apr  2 11:26:05 2024, max compression
+gzip compressed data, was "httpgo-0.4.0.tar", max compression
```

## Comparing `httpgo-0.30.0.tar` & `httpgo-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,11 @@
--rw-r--r--   0        0        0      187 2024-04-02 08:32:13.755759 httpgo-0.30.0/README.md
--rw-r--r--   0        0        0        0 2024-04-02 08:32:13.755759 httpgo-0.30.0/httpgo/__init__.py
--rw-r--r--   0        0        0      340 2024-04-02 11:20:57.774356 httpgo-0.30.0/httpgo/__version__.py
--rw-r--r--   0        0        0     4402 2024-04-02 10:36:14.477960 httpgo-0.30.0/httpgo/main.py
--rw-r--r--   0        0        0        0 2024-04-02 08:32:13.756759 httpgo-0.30.0/httpgo/utils/__init__.py
--rw-r--r--   0        0        0     1366 2024-04-02 11:24:49.307092 httpgo-0.30.0/httpgo/utils/_callback.py
--rw-r--r--   0        0        0      228 2024-04-02 08:32:13.756759 httpgo-0.30.0/httpgo/utils/_enum.py
--rw-r--r--   0        0        0      146 2024-04-02 10:27:52.129925 httpgo-0.30.0/httpgo/utils/_exception.py
--rw-r--r--   0        0        0     2227 2024-04-02 10:30:38.274723 httpgo-0.30.0/httpgo/utils/_type.py
--rw-r--r--   0        0        0      755 2024-04-02 11:26:05.065119 httpgo-0.30.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 08:32:13.757759 httpgo-0.30.0/tests/__init__.py
--rw-r--r--   0        0        0      876 2024-04-02 08:32:13.757759 httpgo-0.30.0/tests/test_command.py
--rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 httpgo-0.30.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-11-21 02:09:36.081157 httpgo-0.4.0/httpgo/__init__.py
+-rw-r--r--   0        0        0      340 2023-11-23 08:32:38.023792 httpgo-0.4.0/httpgo/__version__.py
+-rw-r--r--   0        0        0     4043 2023-11-24 06:51:46.777788 httpgo-0.4.0/httpgo/main.py
+-rw-r--r--   0        0        0        0 2023-11-21 02:09:36.081157 httpgo-0.4.0/httpgo/utils/__init__.py
+-rw-r--r--   0        0        0     1289 2023-11-24 02:54:45.352830 httpgo-0.4.0/httpgo/utils/_callback.py
+-rw-r--r--   0        0        0      228 2023-11-23 07:55:10.077577 httpgo-0.4.0/httpgo/utils/_enum.py
+-rw-r--r--   0        0        0      410 2023-11-24 06:58:57.834768 httpgo-0.4.0/httpgo/utils/_exception.py
+-rw-r--r--   0        0        0     2874 2023-11-24 07:18:14.138818 httpgo-0.4.0/httpgo/utils/_type.py
+-rw-r--r--   0        0        0      593 2023-11-24 06:49:37.120885 httpgo-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-11-21 09:32:19.090631 httpgo-0.4.0/README.md
+-rw-r--r--   0        0        0      897 1970-01-01 00:00:00.000000 httpgo-0.4.0/PKG-INFO
```

### Comparing `httpgo-0.30.0/httpgo/main.py` & `httpgo-0.4.0/httpgo/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import requests
 import typer
 import time
 from typing import List
 from rich import print
-from rich.progress import Progress, SpinnerColumn, TextColumn
 from json.decoder import JSONDecodeError
 from .utils._callback import process_list_data, version_callback
 from .utils._enum import HttpMethod
 from .utils._type import UrlType, NameValueType, JsonType
 
 
 app = typer.Typer(add_completion=False)
@@ -42,37 +41,37 @@
         show_default=False,
         click_type=NameValueType(),
     ),
     json: str = typer.Option(
         None,
         "--json",
         "-j",
-        help=r"请求体使用JSON数据.example: -j '{\"name\":\"admin\"}'",
+        help='请求体使用JSON数据.example: -j \'{"name":"admin"}\'',
         show_default=False,
         click_type=JsonType(),
     ),
     headers: str = typer.Option(
         None,
         "--headers",
         "-h",
-        help=r"设置请求头.example: -h '{\"Content-Type\":\"application/json\"}'",
+        help="设置请求头.example: -h \"{'Content-Type':'application/json'}\"",
         show_default=False,
         click_type=JsonType(),
     ),
     timeout: float = typer.Option(
         None,
         "--timeout",
         "-t",
         help="超时时间,单位秒(s).example: -t 3.2",
         show_default=False,
     ),
     cookies: str = typer.Option(
         None,
         "--cookies",
-        help=r"cookie包含在请求中.example: --cookies '{\"cookie name\":\"your cookies\"}'",
+        help="cookie包含在请求中.example: --cookies \"{'your cookie name':'your cookies'}\"",
         show_default=False,
         click_type=JsonType(),
     ),
     proxies: str = typer.Option(
         None,
         "--proxies",
         "-P",
@@ -102,31 +101,25 @@
     if params:
         params = process_list_data(params)
     if data:
         data = process_list_data(data)
     try:
         first_time = time.time()
         # 请求
-        with Progress(
-            SpinnerColumn(),
-            TextColumn("[progress.description]{task.description}"),
-            transient=True,
-        ) as progress:
-            progress.add_task(description="Requesting...", total=None)
-            res = requests.request(
-                method=method,
-                url=url,
-                params=params,
-                json=json,
-                data=data,
-                headers=headers,
-                timeout=timeout,
-                cookies=cookies,
-                proxies=proxies,
-            )
+        res = requests.request(
+            method=method,
+            url=url,
+            params=params,
+            json=json,
+            data=data,
+            headers=headers,
+            timeout=timeout,
+            cookies=cookies,
+            proxies=proxies,
+        )
         last_time = time.time() - first_time
     except Exception as e:
         print("[bold red]Error:[/bold red]", e)
         raise typer.Exit()
     # 打印url
     print(method, res.status_code, url, f"ResponseTime:{last_time}s", end="\n\n")
     # 判断verbose
```

### Comparing `httpgo-0.30.0/httpgo/utils/_callback.py` & `httpgo-0.4.0/httpgo/utils/_callback.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import json
-from rich import print
 import typer
 from ..__version__ import package_version, package_name
+from ..utils._exception import FormatError
 
 
 def process_list_data(value: list) -> dict:
     """处理列表"""
     try:
         list_to_dict = dict(map(lambda item: item.split("="), value))
-    except ValueError:
-        print(f"[bold red]Error:[/bold red] 参数格式错误。example:limit=20")
-        raise typer.Exit()
-    else:
         return list_to_dict
+    except ValueError:
+        raise FormatError
 
 
 # def process_json_data(value: str) -> str:
 #     """处理json"""
 #     # 如果字符串以单引号或双引号包裹，则去掉外围的引号
 #     try:
 #         if value.startswith("'") and value.endswith("'"):
```

### Comparing `httpgo-0.30.0/httpgo/utils/_type.py` & `httpgo-0.4.0/httpgo/utils/_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import json, typer
+import re, ast, typer
 from click import ParamType
 from rich import print
+from ._exception import UrlVerifyError
 
 # from pydantic import HttpUrl, validate_arguments
 
 
 # @validate_arguments
 # def url(value: HttpUrl) -> HttpUrl:
 #     """自定义Url类型提示,
@@ -58,25 +59,44 @@
         #     raise typer.Exit()
         return value
 
 
 class NameValueType(ParamType):
     """键值类型提示"""
 
-    name = "<NAME VALUE> ..."
+    name = "<NAME VALUE>"
+
+    def convert(self, value, param, ctx):
+        return value
 
 
 class JsonType(ParamType):
     """JSON类型提示并解析"""
 
     name = "JSON"
 
+    def parse_powershell_input(self, key_value: tuple):
+        """对powershell输入进行操作
+
+        Args:
+            key_value (tuple): k,v元组
+
+        Returns:
+            _type_: _description_
+        """
+        key, value = key_value
+        return (
+            key,
+            str(value) if isinstance(value, int) or isinstance(value, float) else value,
+        )
 
     def convert(self, value, param, ctx):
-        """转化json为dict"""
         try:
-            dict_data = json.loads(value)
-        except json.JSONDecodeError:
-            print(f"[bold red]Error:[/bold red]  '--json' / '-j': 无效json格式")
-            raise typer.Exit()
-        else:
-            return dict_data
+            # 使用 ast.literal_eval 将字符串转换为字典
+            dict_data = ast.literal_eval(value)
+        except Exception:
+            # 使用正则表达式提取键值对
+            pattern = re.compile(r"(\w+):([^,}]+)")
+            matches = pattern.findall(value)
+            # 进行解析
+            dict_data = dict(map(self.parse_powershell_input, matches))
+        return dict_data
```

