# Comparing `tmp/python_115-0.0.4.9.tar.gz` & `tmp/python_115-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.4.9.tar", max compression
+gzip compressed data, was "python_115-0.0.5.tar", max compression
```

## Comparing `python_115-0.0.4.9.tar` & `python_115-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.4.9/LICENSE
--rw-r--r--   0        0        0   245214 2024-03-26 07:24:15.904488 python_115-0.0.4.9/p115/__init__.py
--rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.4.9/p115/__main__.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.4.9/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.4.9/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.4.9/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.4.9/p115/util/_init_mimetypes.py
--rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.4.9/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.4.9/p115/util/cipher.py
--rw-r--r--   0        0        0     4974 2024-03-13 03:45:43.018564 python_115-0.0.4.9/p115/util/concurrent.py
--rw-r--r--   0        0        0     7697 2024-01-28 11:38:07.841565 python_115-0.0.4.9/p115/util/download.py
--rw-r--r--   0        0        0    15006 2024-02-09 07:55:14.302447 python_115-0.0.4.9/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.4.9/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.4.9/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.4.9/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.4.9/p115/util/path.py
--rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.4.9/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.4.9/p115/util/response.py
--rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.4.9/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.4.9/p115/util/text.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.4.9/p115/util/urlopen.py
--rw-r--r--   0        0        0     1251 2024-03-26 07:24:29.271688 python_115-0.0.4.9/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.4.9/readme.md
--rw-r--r--   0        0        0    35866 1970-01-01 00:00:00.000000 python_115-0.0.4.9/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5/LICENSE
+-rw-r--r--   0        0        0   252566 2024-04-02 11:10:02.509209 python_115-0.0.5/p115/__init__.py
+-rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5/p115/__main__.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5/p115/py.typed
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5/p115/util/_init_mimetypes.py
+-rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5/p115/util/cipher.py
+-rw-r--r--   0        0        0     5670 2024-04-02 11:03:33.575384 python_115-0.0.5/p115/util/concurrent.py
+-rw-r--r--   0        0        0    11725 2024-04-02 11:03:58.269419 python_115-0.0.5/p115/util/download.py
+-rw-r--r--   0        0        0    14936 2024-04-02 07:02:17.355689 python_115-0.0.5/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5/p115/util/path.py
+-rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5/p115/util/response.py
+-rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5/p115/util/text.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1249 2024-04-02 11:10:23.041470 python_115-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5/readme.md
+-rw-r--r--   0        0        0    35864 1970-01-01 00:00:00.000000 python_115-0.0.5/PKG-INFO
```

### Comparing `python_115-0.0.4.9/LICENSE` & `python_115-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.4.9/p115/__init__.py` & `python_115-0.0.5/p115/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 ]
 
 import errno
 
 from abc import ABC, abstractmethod
 from asyncio import get_running_loop, run_coroutine_threadsafe, run, to_thread
 from binascii import b2a_hex
-from collections import deque
+from collections import deque, ChainMap
 from collections.abc import (
     AsyncIterator, Awaitable, Callable, Iterable, Iterator, ItemsView, KeysView, Mapping, 
     MutableMapping, Sequence, ValuesView, 
 )
-from concurrent.futures import Future
+from concurrent.futures import Future, ThreadPoolExecutor
 from copy import deepcopy
 from contextlib import asynccontextmanager
 from datetime import date, datetime
 from email.utils import formatdate
 from functools import cached_property, partial, update_wrapper
 from hashlib import md5, sha1, file_digest
 from hmac import digest as hmac_digest
@@ -60,14 +60,15 @@
 
 # NOTE: OR use `pyqrcode` instead
 import qrcode # type: ignore
 
 from .exception import AuthenticationError, LoginError
 from .util.args import argcount
 from .util.cipher import P115RSACipher, P115ECDHCipher, MD5_SALT
+from .util.download import DownloadTask
 from .util.file import bio_chunk_iter, bio_skip_bytes, get_filesize, HTTPFileReader, RequestsFileReader, SupportsRead, SupportsWrite, SupportsGetUrl
 from .util.iter import asyncify_iter
 from .util.path import basename, commonpath, dirname, escape, joins, normpath, splits, unescape
 from .util.property import funcproperty
 from .util.response import get_content_length, get_filename, is_range_request
 from .util.text import cookies_str_to_dict, posix_glob_translate_iter, to_base64
 from .util.urlopen import urlopen
@@ -241,14 +242,38 @@
         if "async_session" in self.__dict__:
             cookiejar2 = self.async_session.cookie_jar
             cookiejar2.clear()
             cookiejar2.update_cookies(cookiejar, URL("http://.115.com"))
         cookies = cookiejar.get_dict()
         self.__dict__["cookie"] = "; ".join(f"{key}={cookies[key]}" for key in ("UID", "CID", "SEID"))
 
+    @property
+    def headers(self, /) -> MappingProxyType:
+        return MappingProxyType(self.session.headers)
+
+    def update_headers(self, headers, /):
+        sync_request_headers = self.session.headers
+        if isinstance(headers, Mapping):
+            try:
+                headers = headers.items()
+            except (AttributeError, TypeError):
+                headers = ((k, headers[k]) for k in headers)
+        for k, v in headers:
+            if v is None:
+                try:
+                    del sync_request_headers[k]
+                except KeyError:
+                    pass
+            else:
+                sync_request_headers[k] = v
+        if "async_session" in self.__dict__:
+            async_request_headers = self.async_session.headers
+            async_request_headers.clear()
+            async_request_headers.update(sync_request_headers) # type: ignore
+
     def login_with_qrcode(
         self, 
         /, 
         app: str = "web", 
         **request_kwargs, 
     ) -> dict:
         """用二维码登录
@@ -725,43 +750,43 @@
                 # 用某字段排序：
                 # - 文件名："file_name"
                 # - 文件大小："file_size"
                 # - 文件种类："file_type"
                 # - 修改时间："user_utime"
                 # - 创建时间："user_ptime"
                 # - 上次打开时间："user_otime"
-            - show_dir: 0 | 1 = 1 # 此参数值必须为 1
 
             - aid: int | str = 1
             - code: int | str = <default>
-            - count_folders: 0 | 1 = <default>
+            - count_folders: 0 | 1 = 1
             - custom_order: int | str = <default>
             - fc_mix: 0 | 1 = <default> # 是否文件夹置顶，0 为置顶
             - format: str = "json"
             - is_q: 0 | 1 = <default>
             - is_share: 0 | 1 = <default>
             - natsort: 0 | 1 = <default>
-            - record_open_time: 0 | 1 = <default>
+            - record_open_time: 0 | 1 = 1
             - scid: int | str = <default>
+            - show_dir: 0 | 1 = 1
             - snap: 0 | 1 = <default>
-            - star: 0 | 1 = <default>
             - source: str = <default>
+            - star: 0 | 1 = <default>
             - suffix: str = <default>
             - type: int | str = <default>
                 # 文件类型：
                 # - 所有: 0
                 # - 文档: 1
                 # - 图片: 2
                 # - 音频: 3
                 # - 视频: 4
                 # - 压缩包: 5
                 # - 应用: 6
         """
         api = "https://webapi.115.com/files"
-        payload = {"cid": 0, "limit": 32, "offset": 0, "asc": 1, "o": "file_name", "show_dir": 1, **payload}
+        payload = {"aid": 1, "asc": 1, "cid": 0, "count_folders": 1, "limit": 32, "o": "file_name", "offset": 0, "record_open_time": 1, "show_dir": 1, **payload}
         return self.request(api, params=payload, async_=async_, **request_kwargs)
 
     def fs_files2(
         self, 
         payload: dict = {}, 
         /, 
         async_: bool = False, 
@@ -778,43 +803,43 @@
                 # 用某字段排序：
                 # - 文件名："file_name"
                 # - 文件大小："file_size"
                 # - 文件种类："file_type"
                 # - 修改时间："user_utime"
                 # - 创建时间："user_ptime"
                 # - 上次打开时间："user_otime"
-            - show_dir: 0 | 1 = 1 # 此参数值必须为 1
 
             - aid: int | str = 1
             - code: int | str = <default>
-            - count_folders: 0 | 1 = <default>
+            - count_folders: 0 | 1 = 1
             - custom_order: int | str = <default>
             - fc_mix: 0 | 1 = <default> # 是否文件夹置顶，0 为置顶
             - format: str = "json"
             - is_q: 0 | 1 = <default>
             - is_share: 0 | 1 = <default>
             - natsort: 0 | 1 = <default>
-            - record_open_time: 0 | 1 = <default>
+            - record_open_time: 0 | 1 = 1
             - scid: int | str = <default>
+            - show_dir: 0 | 1 = 1
             - snap: 0 | 1 = <default>
-            - star: 0 | 1 = <default>
             - source: str = <default>
+            - star: 0 | 1 = <default>
             - suffix: str = <default>
             - type: int | str = <default>
                 # 文件类型：
                 # - 所有: 0
                 # - 文档: 1
                 # - 图片: 2
                 # - 音频: 3
                 # - 视频: 4
                 # - 压缩包: 5
                 # - 应用: 6
         """
         api = "https://aps.115.com/natsort/files.php"
-        payload = {"cid": 0, "limit": 32, "offset": 0, "asc": 1, "o": "file_name", "show_dir": 1, **payload}
+        payload = {"aid": 1, "asc": 1, "cid": 0, "count_folders": 1, "limit": 32, "o": "file_name", "offset": 0, "record_open_time": 1, "show_dir": 1, **payload}
         return self.request(api, params=payload, async_=async_, **request_kwargs)
 
     def fs_files_edit(
         self, 
         payload: list | dict, 
         /, 
         async_: bool = False, 
@@ -3788,14 +3813,15 @@
         """
         """
         if size <= 0:
             return b""
         return self.read_bytes(url, offset, offset+size, headers=headers, **request_kwargs)
 
 
+# TODO: 使用 id 而不是 path
 class P115PathBase(Generic[P115FSType], Mapping, PathLike[str]):
     fs: P115FSType
     path: str
 
     def __init__(
         self, 
         /, 
@@ -3906,24 +3932,22 @@
 
     def download(
         self, 
         /, 
         local_dir: bytes | str | PathLike = "", 
         pid: Optional[int] = None, 
         no_root: bool = False, 
-        write_mode: Literal["", "x", "w", "a"] = "w", 
-        download: Optional[Callable[[str, SupportsWrite[bytes], Unpack[HeadersKeyword]], Any]] = None, 
+        write_mode: Literal["a", "w", "x", "i"] = "a", 
     ):
         return self.fs.download_tree(
             self, 
             local_dir, 
             pid=pid, 
             no_root=no_root, 
             write_mode=write_mode, 
-            download=download, 
         )
 
     def exists(self, /) -> bool:
         return self.fs.exists(self)
 
     def get_url(self, /, headers: Optional[Mapping] = None) -> str:
         return self.fs.get_url(self, headers=headers)
@@ -3977,22 +4001,24 @@
         self, 
         /, 
         topdown: bool = True, 
         min_depth: int = 0, 
         max_depth: int = 1, 
         predicate: Optional[Callable[[Self], Optional[bool]]] = None, 
         onerror: Optional[bool] = None, 
+        **kwargs, 
     ) -> Iterator[Self]:
         return self.fs.iter(
             self, 
             topdown=topdown, 
             min_depth=min_depth, 
             max_depth=max_depth, 
             predicate=predicate, 
             onerror=onerror, 
+            **kwargs, 
         )
 
     def join(self, *names: str) -> Self:
         if not names:
             return self
         return type(self)(self.fs, joinpath(self.path, joins(names)))
 
@@ -4001,22 +4027,22 @@
             return self
         path = self.path
         path_new = normpath(joinpath(path, *paths))
         if path == path_new:
             return self
         return type(self)(self.fs, path_new)
 
-    def listdir(self, /) -> list[str]:
-        return self.fs.listdir(self)
+    def listdir(self, /, **kwargs) -> list[str]:
+        return self.fs.listdir(self, **kwargs)
 
-    def listdir_attr(self, /) -> list[dict]:
-        return self.fs.listdir_attr(self)
+    def listdir_attr(self, /, **kwargs) -> list[dict]:
+        return self.fs.listdir_attr(self, **kwargs)
 
-    def listdir_path(self, /) -> list[Self]:
-        return self.fs.listdir_path(self)
+    def listdir_path(self, /, **kwargs) -> list[Self]:
+        return self.fs.listdir_path(self, **kwargs)
 
     def match(
         self, 
         /, 
         path_pattern: str, 
         ignore_case: bool = False, 
         allow_escaped_slash: bool = True, 
@@ -4339,90 +4365,97 @@
         elif attr["is_directory"]:
             self.__dict__.update(cid=attr["id"], path=self.get_path(id_or_path, pid))
             return attr["id"]
         else:
             raise NotADirectoryError(
                 errno.ENOTDIR, f"{id_or_path!r} (in {pid!r}) is not a directory")
 
-    # TODO: 增加功能，返回一个 Future 对象，可以获取下载进度，可随时取消
     def download(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         local_path_or_file: bytes | str | PathLike | SupportsWrite[bytes] = "", 
         pid: Optional[int] = None, 
-        write_mode: Literal["", "x", "w", "a"] = "w", 
-        download: Optional[Callable[[str, SupportsWrite[bytes], Unpack[HeadersKeyword]], Any]] = None, 
-    ):
-        if hasattr(local_path_or_file, "write"):
-            file = local_path_or_file
-        else:
-            local_path = fspath(local_path_or_file)
-            mode: str = write_mode
-            if mode:
-                mode += "b"
-            elif ospath.lexists(local_path):
-                return
-            else:
-                mode = "wb"
-            if local_path:
-                file = open(local_path, mode)
-            else:
-                file = open(self.attr(id_or_path, pid)["name"], mode)
-        file = cast(SupportsWrite[bytes], file)
-        url = self.get_url(id_or_path, pid)
-        if download:
-            download(url, file, headers=self.client.session.headers)
+        write_mode: Literal["a", "w", "x", "i"] = "a", 
+        submit = None, 
+    ) -> Optional[DownloadTask]:
+        if not hasattr(local_path_or_file, "write"):
+            if not local_path_or_file:
+                local_path_or_file = self.attr(id_or_path, pid)["name"]
+            if ospath.lexists(local_path_or_file): # type: ignore
+                if write_mode == "x":
+                    raise FileExistsError(
+                        errno.EEXIST, 
+                        f"local path already exists: {local_path_or_file!r}", 
+                    )
+                elif write_mode == "i":
+                    return None
+        kwargs = {"resume": write_mode == "a", "headers": self.client.session.headers}
+        if submit is not None:
+            kwargs["submit"] = submit
+        task = DownloadTask.create_task(
+            lambda: self.get_url(id_or_path, pid), 
+            local_path_or_file, 
+            **kwargs, 
+        )
+        if submit is None:
+            task.run_wait()
         else:
-            with self.client.open(url) as fsrc:
-                copyfileobj(fsrc, file)
+            task.run()
+        return task
 
-    # TODO: 增加功能，返回一个 Future 对象，可以获取已完成和未完成的列表，每个任务的进度，可随时取消
     def download_tree(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         local_dir: bytes | str | PathLike = "", 
         pid: Optional[int] = None, 
+        write_mode: Literal["i", "x", "w", "a"] = "a", 
+        submit = None, 
         no_root: bool = False, 
-        write_mode: Literal["", "x", "w", "a"] = "w", 
-        download: Optional[Callable[[str, SupportsWrite[bytes], Unpack[HeadersKeyword]], Any]] = None, 
-    ):
+        predicate: Optional[Callable[[P115PathType], bool]] = None, 
+        onerror: Optional[Callable[[BaseException], Any]] = None, 
+    ) -> Iterator[DownloadTask]:
         local_dir = fsdecode(local_dir)
         if local_dir:
             makedirs(local_dir, exist_ok=True)
         attr = self.attr(id_or_path, pid)
         if attr["is_directory"]:
             if not no_root:
                 local_dir = ospath.join(local_dir, attr["name"])
                 if local_dir:
                     makedirs(local_dir, exist_ok=True)
-            for subattr in self.listdir_attr(attr["id"]):
-                if subattr["is_directory"]:
-                    self.download_tree(
-                        subattr["id"], 
-                        ospath.join(local_dir, subattr["name"]), 
-                        no_root=True, 
-                        write_mode=write_mode, 
-                        download=download, 
-                    )
-                else:
-                    self.download(
-                        subattr["id"], 
-                        ospath.join(local_dir, subattr["name"]), 
+            pathes = self.listdir_path(attr["id"])
+        else:
+            pathes = [type(self).path_class(self, **attr)]
+        for subpath in filter(predicate, pathes):
+            if subpath["is_directory"]:
+                yield from self.download_tree(
+                    subpath["id"], 
+                    ospath.join(local_dir, subpath["name"]), 
+                    write_mode=write_mode, 
+                    submit=submit, 
+                    no_root=True, 
+                    predicate=predicate, 
+                    onerror=onerror, 
+                )
+            else:
+                try:
+                    task = self.download(
+                        subpath["id"], 
+                        ospath.join(local_dir, subpath["name"]), 
                         write_mode=write_mode, 
-                        download=download, 
+                        submit=submit, 
                     )
-        else:
-            self.download(
-                attr["id"], 
-                ospath.join(local_dir, attr["name"]), 
-                write_mode=write_mode, 
-                download=download, 
-            )
+                    if task is not None:
+                        yield task
+                except KeyboardInterrupt:
+                    raise
+                except BaseException as exc:
+                    onerror and onerror(exc)
 
     def exists(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> bool:
@@ -4680,24 +4713,25 @@
         /, 
         pid: Optional[int] = None, 
         topdown: bool = True, 
         min_depth: int = 0, 
         max_depth: int = 1, 
         predicate: Optional[Callable[[P115PathType], Optional[bool]]] = None, 
         onerror: Optional[bool] = None, 
+        **kwargs, 
     ) -> Iterator[P115PathType]:
         if not max_depth:
             return
         if min_depth > 0:
             min_depth -= 1
         if max_depth > 0:
             max_depth -= 1
         path_class = type(self).path_class
         try:
-            for path in self.listdir_path(top, pid):
+            for path in self.listdir_path(top, pid, **kwargs):
                 path = cast(P115PathType, path)
                 yield_me = min_depth <= 0
                 if yield_me and predicate:
                     pred = predicate(path)
                     if pred is None:
                         continue
                     yield_me = pred 
@@ -4721,33 +4755,72 @@
                 raise
 
     def listdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
+        full_path: bool = False, 
+        **kwargs, 
     ) -> list[str]:
-        return [attr["name"] for attr in self.iterdir(id_or_path, pid)]
+        if full_path:
+            return [attr["path"] for attr in self.iterdir(id_or_path, pid, **kwargs)]
+        else:
+            return [attr["name"] for attr in self.iterdir(id_or_path, pid, **kwargs)]
 
     def listdir_attr(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
+        **kwargs, 
     ) -> list[M]:
-        return list(self.iterdir(id_or_path, pid))
+        return list(self.iterdir(id_or_path, pid, **kwargs))
 
     def listdir_path(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
+        **kwargs, 
     ) -> list[P115PathType]:
         path_class = type(self).path_class
-        return [path_class(self, **attr) for attr in self.iterdir(id_or_path, pid)]
+        return [path_class(self, **attr) for attr in self.iterdir(id_or_path, pid, **kwargs)]
+
+    def dictdir(
+        self, 
+        id_or_path: IDOrPathType = "", 
+        /, 
+        pid: Optional[int] = None, 
+        full_path: bool = False, 
+        **kwargs, 
+    ) -> dict[int, str]:
+        if full_path:
+            return {attr["id"]: attr["path"] for attr in self.iterdir(id_or_path, pid, **kwargs)}
+        else:
+            return {attr["id"]: attr["name"] for attr in self.iterdir(id_or_path, pid, **kwargs)}
+
+    def dictdir_attr(
+        self, 
+        id_or_path: IDOrPathType = "", 
+        /, 
+        pid: Optional[int] = None, 
+        **kwargs, 
+    ) -> dict[int, M]:
+        return {attr["id"]: attr for attr in self.iterdir(id_or_path, pid, **kwargs)}
+
+    def dictdir_path(
+        self, 
+        id_or_path: IDOrPathType = "", 
+        /, 
+        pid: Optional[int] = None, 
+        **kwargs, 
+    ) -> dict[int, P115PathType]:
+        path_class = type(self).path_class
+        return {attr["id"]: path_class(self, **attr) for attr in self.iterdir(id_or_path, pid, **kwargs)}
 
     def open(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         mode: str = "r", 
         buffering: Optional[int] = None, 
@@ -4843,16 +4916,17 @@
         return self.glob(pattern, dirname, ignore_case=ignore_case, allow_escaped_slash=allow_escaped_slash)
 
     def scandir(
         self, 
         id_or_path: IDOrPathType, 
         /, 
         pid: Optional[int] = None, 
+        **kwargs, 
     ) -> Iterator[P115PathType]:
-        return iter(self.listdir_path(id_or_path, pid))
+        return iter(self.listdir_path(id_or_path, pid, **kwargs))
 
     def stat(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
     ) -> stat_result:
@@ -4866,29 +4940,30 @@
         /, 
         pid: Optional[int] = None, 
         topdown: bool = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
         onerror: None | bool | Callable = None, 
         _top: str = "", 
+        **kwargs, 
     ) -> Iterator[tuple[str, list[str], list[str]]]:
         if not max_depth:
             return
         if min_depth > 0:
             min_depth -= 1
         if max_depth > 0:
             max_depth -= 1
         yield_me = min_depth <= 0
         try:
             if not _top:
                 _top = self.get_path(top, pid)
             dirs: list[str] = []
             files: list[str] = []
             attrs: list[M] = []
-            for attr in self.listdir_attr(top, pid):
+            for attr in self.listdir_attr(top, pid, **kwargs):
                 if attr["is_directory"]:
                     attrs.append(attr)
                     dirs.append(attr["name"])
                 else:
                     files.append(attr["name"])
             if yield_me and topdown:
                 yield _top, dirs, files
@@ -4915,28 +4990,29 @@
         /, 
         pid: Optional[int] = None, 
         topdown: bool = True, 
         min_depth: int = 0, 
         max_depth: int = -1, 
         onerror: None | bool | Callable = None, 
         _top: str = "", 
+        **kwargs, 
     ) -> Iterator[tuple[str, list[P115PathType], list[P115PathType]]]:
         if not max_depth:
             return
         if min_depth > 0:
             min_depth -= 1
         if max_depth > 0:
             max_depth -= 1
         yield_me = min_depth <= 0
         try:
             if not _top:
                 _top = self.get_path(top, pid)
             dirs: list[P115PathType] = []
             files: list[P115PathType] = []
-            for path in self.listdir_path(top, pid):
+            for path in self.listdir_path(top, pid, **kwargs):
                 (dirs if path["is_directory"] else files).append(path)
             if yield_me and topdown:
                 yield _top, dirs, files
             for path in dirs:
                 yield from self.walk_path(
                     path["id"], 
                     topdown=topdown, 
@@ -5064,31 +5140,40 @@
             errors=errors, 
             newline=newline, 
         ))
         return self
 
 
 class P115FileSystem(P115FileSystemBase[dict, P115Path]):
-    path_to_id: MutableMapping[str, int]
-    id_to_utime: MutableMapping[int, float]
-    pid_to_attrs: MutableMapping[int, dict]
+    id_to_children: Optional[MutableMapping[int, dict]]
+    path_to_id: Optional[MutableMapping[str, int]]
+    get_version: Optional[Callable]
     path_class = P115Path
 
     def __init__(
         self, 
         /, 
         client: P115Client, 
+        id_to_children: Optional[MutableMapping[int, dict]] = None, 
+        path_to_id: Optional[MutableMapping[str, int]] = None, 
+        get_version: Optional[Callable] = lambda attr: attr.get("mtime", 0), 
     ):
+        if id_to_children is not None:
+            id_to_children = {}
+        if type(path_to_id) is dict:
+            path_to_id["/"] = 0
+        elif path_to_id is not None:
+            path_to_id = ChainMap(path_to_id, {"/": 0})
         self.__dict__.update(
             client = client, 
             cid = 0, 
             path = "/", 
-            path_to_id = {"/": 0}, 
-            id_to_utime = {}, 
-            pid_to_attrs = {}, 
+            path_to_id = path_to_id, 
+            id_to_children = id_to_children, 
+            get_version = get_version, 
         )
 
     def __delitem__(self, id_or_path: IDOrPathType, /):
         self.rmtree(id_or_path)
 
     def __len__(self, /) -> int:
         return self.get_directory_capacity(self.cid)
@@ -5110,48 +5195,57 @@
         file: None | str | bytes | bytearray | memoryview | PathLike = None, 
         /, 
     ):
         if file is None:
             return self.touch(id_or_path)
         elif isinstance(file, PathLike):
             if ospath.isdir(file):
-                return self.upload_tree(file, id_or_path, no_root=True, overwrite_or_ignore=True)
+                return list(self.upload_tree(file, id_or_path, no_root=True, overwrite_or_ignore=True))
             else:
-                 return self.upload(file, id_or_path, overwrite_or_ignore=True)
+                return self.upload(file, id_or_path, overwrite_or_ignore=True)
         elif isinstance(file, str):
             return self.write_text(id_or_path, file)
         else:
             return self.write_bytes(id_or_path, file)
 
     @classmethod
-    def login(cls, /, cookie=None, app: str = "web") -> Self:
-        return cls(P115Client(cookie, login_app=app))
+    def login(
+        cls, 
+        /, 
+        cookie = None, 
+        app: str = "web", 
+        **kwargs, 
+    ) -> Self:
+        kwargs["client"] = P115Client(cookie, login_app=app)
+        return cls(**kwargs)
 
     @check_response
     def _copy(self, id: int, pid: int = 0, /) -> dict:
         return self.client.fs_copy(id, pid)
 
     @check_response
     def _delete(self, id: int, /) -> dict:
         return self.client.fs_delete(id)
 
-    @check_response
     def _files(
         self, 
         /, 
         id: int = 0, 
         limit: int = 32, 
         offset: int = 0, 
     ) -> dict:
-        return self.client.fs_files({
+        resp = check_response(self.client.fs_files({
             "cid": id, 
             "limit": limit, 
             "offset": offset, 
             "show_dir": 1, 
-        })
+        }))
+        if id and int(resp["path"][-1]["cid"]) != id:
+            raise NotADirectoryError(errno.ENOTDIR, f"{id} is not a directory")
+        return resp
 
     @check_response
     def _info(self, id: int, /) -> dict:
         return self.client.fs_info({"file_id": id})
 
     @check_response
     def _mkdir(self, name: str, pid: int = 0, /) -> dict:
@@ -5178,126 +5272,199 @@
             try:
                 file.seek(0, 1)
             except:
                 pass
             else:
                 resp = self.client.upload_file(file, name, pid)
                 name = resp["data"]["file_name"]
-                return self._attr_path([name], pid)
+                try:
+                    return self._attr_path([name], pid)
+                except FileNotFoundError:
+                    self._files(pid, 1)
+                    return self._attr_path([name], pid)
         resp = check_response(self.client.upload_file_sample)(file, name, pid)
         id = int(resp["data"]["file_id"])
-        return self._attr(id)
+        try:
+            return self._attr(id)
+        except FileNotFoundError:
+            self._files(pid, 1)
+            return self._attr(id)
 
     def _clear_cache(self, attr: dict, /):
-        pid_to_attrs = self.pid_to_attrs
+        id_to_children = self.id_to_children
+        if id_to_children is None:
+            return
         id = attr["id"]
         pid = attr["parent_id"]
         if id:
             try:
-                pid_to_attrs[pid].pop(id, None)
+                id_to_children[pid]["children"].pop(id, None)
             except:
                 pass
         if attr["is_directory"]:
+            path_to_id = self.path_to_id
+            if path_to_id is None:
+                pop_path = None
+            else:
+                def pop_path(path):
+                    try:
+                        del path_to_id[path]
+                    except:
+                        pass
             startswith = str.startswith
-            pop = self.path_to_id.pop
             dq = deque((id,))
             get, put = dq.popleft, dq.append
             while dq:
-                cache = pid_to_attrs.pop(get(), None)
-                if cache:
-                    for subid, subattr in cache.items():
-                        pop(subattr["path"], None)
+                cid = get()
+                try:
+                    cache = id_to_children[cid]
+                    del id_to_children[cid]
+                except KeyError:
+                    pass
+                else:
+                    for subid, subattr in cache["children"].items():
+                        if pop_path is not None:
+                            pop_path(subattr["path"])
                         if subattr["is_directory"]:
                             put(subid)
-            dirname = attr["path"]
-            pop(dirname, None)
-            dirname += "/"
-            for k in tuple(k for k in self.path_to_id if startswith(k, dirname)):
-                pop(k, None)
+            if path_to_id is not None and pop_path is not None:
+                dirname = attr["path"]
+                pop_path(dirname)
+                dirname += "/"
+                for k in tuple(k for k in path_to_id if startswith(k, dirname)):
+                    pop_path(k)
 
     def _update_cache_path(self, attr: dict, new_attr: dict, /):
-        pid_to_attrs = self.pid_to_attrs
+        id_to_children = self.id_to_children
+        if id_to_children is None:
+            return
         id = attr["id"]
         opid = attr["parent_id"]
         npid = new_attr["parent_id"]
         if id and opid != npid:
             try:
-                pid_to_attrs[opid].pop(id, None)
+                id_to_children[opid]["children"].pop(id, None)
             except:
                 pass
             try:
-                pid_to_attrs[npid][id] = new_attr
+                id_to_children[npid]["children"][id] = new_attr
             except:
                 pass
         if attr["is_directory"]:
-            startswith = str.startswith
             path_to_id = self.path_to_id
-            pop = path_to_id.pop
+            if path_to_id is None:
+                pop_path = None
+            else:
+                def pop_path(path):
+                    try:
+                        del path_to_id[path]
+                    except:
+                        pass
+            startswith = str.startswith
             old_path = attr["path"]
             new_path = new_attr["path"]
-            pop(old_path, None)
-            path_to_id[new_path] = id
+            if pop_path is not None:
+                pop_path(old_path)
+            if path_to_id is not None:
+                path_to_id[new_path] = id
             old_path += "/"
             new_path += "/"
             len_old_path = len(old_path)
             dq = deque((id,))
             get, put = dq.popleft, dq.append
             while dq:
-                cache = pid_to_attrs.pop(get(), None)
-                if cache:
-                    for subid, subattr in cache.items():
+                cid = get()
+                try:
+                    cache = id_to_children[cid]
+                    del id_to_children[cid]
+                except KeyError:
+                    pass
+                else:
+                    for subid, subattr in cache["children"].items():
                         subpath = subattr["path"]
                         if startswith(subpath, old_path):
                             new_subpath = subattr["path"] = new_path + subpath[len_old_path:]
-                            pop(subpath, None)
-                            path_to_id[new_subpath] = subid
+                            if pop_path is not None:
+                                pop_path(subpath)
+                            if path_to_id is not None:
+                                path_to_id[new_subpath] = subid
                         if subattr["is_directory"]:
                             put(subid)
-            for k in tuple(k for k in self.path_to_id if startswith(k, old_path)):
-                pop(k, None)
+            if path_to_id is not None and pop_path is not None:
+                for k in tuple(k for k in path_to_id if startswith(k, old_path)):
+                    pop_path(k)
 
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         pid: Optional[int] = None, 
+        refresh: bool = False, 
     ) -> Iterator[dict]:
-        attr = self.attr(id_or_path, pid)
-        if not attr["is_directory"]:
-            raise NotADirectoryError(errno.ENOTDIR, f"{attr['path']!r} (id={attr['id']!r}) is not a directory")
-        id = attr["id"]
-        utime = attr["utime"].timestamp()
-        if utime > self.id_to_utime.get(id, -1):
+        id_to_children = self.id_to_children
+        get_version = self.get_version
+        if id_to_children is None and isinstance(id_or_path, int):
+            id = id_or_path
+            version = None
+        else:
+            attr = self.attr(id_or_path, pid)
+            if not attr["is_directory"]:
+                raise NotADirectoryError(errno.ENOTDIR, f"{attr['path']!r} (id={attr['id']!r}) is not a directory")
+            id = attr["id"]
+            version = get_version and get_version(attr)
+        if id_to_children is None:
+            pid_attrs = None
+        else:
+            pid_attrs = id_to_children.get(id)
+        if (
+            refresh or 
+            pid_attrs is None or 
+            "version" not in pid_attrs or
+            version != pid_attrs["version"]
+        ):
             pagesize = 1 << 10
             def iterdir():
                 get_files = self._files
                 path_to_id = self.path_to_id
                 resp = get_files(id, limit=pagesize)
                 dirname = joins(("", *(a["name"] for a in resp["path"][1:])))
-                path_to_id[dirname] = id
+                if path_to_id is not None:
+                    path_to_id[dirname] = id
                 lastest_update = datetime.now()
                 count = resp["count"]
                 for attr in resp["data"]:
                     attr = normalize_info(attr, lastest_update=lastest_update)
                     path = attr["path"] = joinpath(dirname, escape(attr["name"]))
-                    path_to_id[path] = attr["id"]
+                    if path_to_id is not None:
+                        path_to_id[path] = attr["id"]
+                    if id_to_children is not None:
+                        try:
+                            id_to_children[attr["id"]].update(attr)
+                        except KeyError:
+                            id_to_children[attr["id"]] = {"attr": attr}
                     yield attr
                 for offset in range(pagesize, count, 1 << 10):
                     resp = get_files(id, limit=pagesize, offset=offset)
                     lastest_update = datetime.now()
                     if resp["count"] != count:
-                        raise RuntimeError("detected count changes during iteration")
+                        raise RuntimeError(f"{id} detected count changes during iteration")
                     for attr in resp["data"]:
                         attr = normalize_info(attr, lastest_update=lastest_update)
                         path = attr["path"] = joinpath(dirname, escape(attr["name"]))
-                        path_to_id[path] = attr["id"]
+                        if path_to_id is not None:
+                            path_to_id[path] = attr["id"]
                         yield attr
-            self.pid_to_attrs[id] = {a["id"]: a for a in iterdir()}
-            self.id_to_utime[id] = utime
-        return iter(self.pid_to_attrs[id].values())
+            children = {a["id"]: a for a in iterdir()}
+            if id_to_children is not None:
+                attrs = id_to_children[id] = {"attr": attr, "children": children}
+                if get_version is not None:
+                    attrs["version"] = version
+        else:
+            children = pid_attrs["children"]
+        return iter(children.values())
 
     def _attr(self, id: int, /) -> dict:
         if id == 0:
             lastest_update = datetime.now()
             return {
                 "id": 0, 
                 "parent_id": 0, 
@@ -5306,34 +5473,52 @@
                 "is_directory": True, 
                 "lastest_update": lastest_update, 
                 "etime": lastest_update, 
                 "utime": lastest_update, 
                 "ptime": datetime.fromtimestamp(0), 
                 "open_time": lastest_update, 
             }
+        id_to_children = self.id_to_children
+        get_version = self.get_version
+        if id_to_children is None:
+            attrs = None
+        else:
+            attrs = id_to_children.get(id)
+        if attrs and "attr" in attrs and get_version is None:
+            return attrs["attr"]
         try:
             data = self._info(id)["data"][0]
         except OSError as e:
             raise FileNotFoundError(errno.ENOENT, f"no such id: {id!r}") from e
         attr = normalize_info(data, lastest_update=datetime.now())
-        pid_to_attrs = self.pid_to_attrs
-        try:
-            pid = attr["parent_id"]
-            attr_old = pid_to_attrs[pid][id]
-            if attr_old["mtime"] == attr["mtime"]:
-                attr_old.update(attr)
-                return attr_old
-        except KeyError:
-            pass
-        path = attr["path"] = joins((*(a["name"] for a in self._dir_get_ancestors(pid)), attr["name"]))
-        self.path_to_id[path] = id
-        try:
-            pid_to_attrs[pid][id] = attr
-        except KeyError:
-            pid_to_attrs[pid] = {id: attr}
+        if id_to_children is not None:
+            if get_version is None:
+                version = None
+            else:
+                version = get_version(attr)
+            if not attrs or "attr" not in attrs or version != attrs.get("version"):
+                pid = attr["parent_id"]
+                if pid:
+                    path = joins((*(a["name"] for a in self._dir_get_ancestors(pid)), attr["name"]))
+                else:
+                    path = "/" + escape(attr["name"])
+                path_to_id = self.path_to_id
+                if path_to_id is not None:
+                    path_to_id[path] = id
+                attr["path"] = path
+                if attrs is None:
+                    id_to_children[id] = {"attr": attr}
+                    if pid not in id_to_children:
+                        id_to_children[pid] = {}
+                    id_to_children.setdefault(pid, {})[id] = attr
+                else:
+                    attrs.pop("version", None)
+                    attrs["attr"].update(attr)
+            else:
+                attrs["attr"].update(attr)
         return attr
 
     def _attr_path(
         self, 
         path: str | PathLike[str] | Sequence[str], 
         /, 
         pid: Optional[int] = None, 
@@ -5343,23 +5528,26 @@
         if pid is None:
             pid = self.cid
         if not path or path == ".":
             return self._attr(pid)
         patht = self.get_patht(path, pid)
         fullpath = joins(patht)
         path_to_id = self.path_to_id
-        if fullpath in path_to_id:
+        if path_to_id is not None and fullpath in path_to_id:
             id = path_to_id[fullpath]
             try:
                 attr = self._attr(id)
                 if attr["path"] == fullpath:
                     return attr
             except FileNotFoundError:
                 pass
-            path_to_id.pop(fullpath, None)
+            try:
+                del path_to_id[fullpath]
+            except:
+                pass
         attr = self._attr(pid)
         for name in patht[len(self.get_patht(pid)):]:
             if not attr["is_directory"]:
                 raise NotADirectoryError(
                     errno.ENOTDIR, f"`pid` does not point to a directory: {pid!r}")
             for attr in self.listdir_attr(pid):
                 if attr["name"] == name:
@@ -5489,14 +5677,15 @@
     def copytree(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType = "", 
         pid: Optional[int] = None, 
         overwrite_or_ignore: Optional[bool] = None, 
+        **kwargs, 
     ) -> Optional[dict]:
         src_attr = self.attr(src_path, pid)
         src_id = src_attr["id"]
         if not src_attr["is_directory"]:
             return self.copy(
                 src_id, 
                 dst_path, 
@@ -5546,15 +5735,15 @@
                     f"destination is not directory: {src_fullpath!r} -> {dst_fullpath!r}", 
                 )
             elif overwrite_or_ignore is None:
                 raise FileExistsError(
                     errno.EEXIST, 
                     f"destination already exists: {src_fullpath!r} -> {dst_fullpath!r}", 
                 )
-        for attr in self.listdir_attr(src_id):
+        for attr in self.listdir_attr(src_id, **kwargs):
             if attr["is_directory"]:
                 self.copytree(
                     attr["id"], 
                     [attr["name"]], 
                     dst_id, 
                     overwrite_or_ignore=overwrite_or_ignore, 
                 )
@@ -5784,14 +5973,15 @@
             }
         if delid == 0:
             return None
         self._delete(delid)
         self._clear_cache(pattr)
         return attr
 
+    # TODO: 支持 dst_path 从 src_path 开始的相对路径
     def rename(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
         pid: Optional[int] = None, 
         replace: bool = False, 
@@ -6046,57 +6236,58 @@
                     return attr
                 self._delete(attr["id"])
         return self._upload(fio, name, pid)
 
     # TODO: 为了提升速度，之后会支持多线程上传，以及直接上传不做检查
     # TODO: 增加功能，可以多线程上传或异步上传，返回 Future 对象，可以获取每个上传任务的进度，并且可以随时取消
     # TODO: 增加断言，可以选择不上传某些文件
+    # TODO: 增加参数，as_task=False，将任务提交到上传队列，返回task对象，可以随时取消，也可以操作调度的 executor
     def upload_tree(
         self, 
         /, 
         local_path: str | PathLike[str] = ".", 
         path: IDOrPathType = "", 
         pid: Optional[int] = None, 
         no_root: bool = False, 
         overwrite_or_ignore: Optional[bool] = None, 
-    ) -> dict:
+    ) -> Iterator[dict]:
         try:
             attr = self.attr(path, pid)
         except FileNotFoundError:
             if isinstance(path, int):
                 raise ValueError(f"no such id: {path!r}")
             attr = self.makedirs(path, pid, exist_ok=True)
         else:
             if not attr["is_directory"]:
                 raise NotADirectoryError(errno.ENOTDIR, f"{attr['path']!r} (id={attr['id']!r}) is not a directory")
         pid = attr["id"]
         try:
             it = scandir(local_path or ".")
         except NotADirectoryError:
-            return self.upload(
+            yield self.upload(
                 local_path, 
                 [ospath.basename(local_path)], 
                 pid=pid, 
                 overwrite_or_ignore=overwrite_or_ignore, 
             )
         else:
             if not no_root:
                 attr = self.makedirs(ospath.basename(local_path), pid, exist_ok=True)
                 pid = attr["parent_id"]
             for entry in it:
                 if entry.is_dir():
-                    self.upload_tree(
+                    yield from self.upload_tree(
                         entry.path, 
                         entry.name, 
                         pid=pid, 
                         no_root=True, 
                         overwrite_or_ignore=overwrite_or_ignore, 
                     )
                 else:
-                    self.upload(
+                    yield self.upload(
                         entry.path, 
                         entry.name, 
                         pid=pid, 
                         overwrite_or_ignore=overwrite_or_ignore, 
                     )
             return attr
 
@@ -6145,15 +6336,15 @@
 class P115ShareFileSystem(P115FileSystemBase[MappingProxyType, P115SharePath]):
     share_link: str
     share_code: str
     receive_code: str
     user_id: int
     path_to_id: MutableMapping[str, int]
     id_to_attr: MutableMapping[int, MappingProxyType]
-    pid_to_attrs: MutableMapping[int, tuple[MappingProxyType]]
+    id_to_children: MutableMapping[int, tuple[MappingProxyType]]
     full_loaded: bool
     path_class = P115SharePath
 
     def __init__(self, /, client: P115Client, share_link: str):
         m = CRE_SHARE_LINK.search(share_link)
         if m is None:
             raise ValueError("not a valid 115 share link")
@@ -6162,15 +6353,15 @@
             cid=0, 
             path="/", 
             share_link=share_link, 
             share_code=m["share_code"], 
             receive_code= m["receive_code"] or "", 
             path_to_id={"/": 0}, 
             id_to_attr={}, 
-            pid_to_attrs={}, 
+            id_to_children={}, 
             full_loaded=False, 
         )
         self.__dict__["user_id"] = int(self.sharedata["userinfo"]["user_id"])
 
     def __repr__(self, /) -> str:
         cls = type(self)
         module = cls.__module__
@@ -6179,15 +6370,21 @@
             name = module + "." + name
         return f"<{name}(client={self.client!r}, share_link={self.share_link!r}, cid={self.cid!r}, path={self.path!r}) at {hex(id(self))}>"
 
     def __setattr__(self, attr, val, /) -> Never:
         raise TypeError("can't set attribute")
 
     @classmethod
-    def login(cls, /, share_link: str, cookie=None, app: str = "web") -> Self:
+    def login(
+        cls, 
+        /, 
+        share_link: str, 
+        cookie = None, 
+        app: str = "web", 
+    ) -> Self:
         return cls(P115Client(cookie, login_app=app), share_link)
 
     def set_receive_code(self, code: str, /):
         self.__dict__["receive_code"] = code
 
     @check_response
     def _files(
@@ -6342,15 +6539,15 @@
                     pass
         else:
             attr = self.attr(id_or_path, pid)
             if not attr["is_directory"]:
                 raise NotADirectoryError(errno.ENOTDIR, f"{attr['path']!r} (id={attr['id']!r}) is not a directory")
             id = attr["id"]
         try:
-            return iter(self.pid_to_attrs[id])
+            return iter(self.id_to_children[id])
         except KeyError:
             dirname = attr["path"]
             def iterdir():
                 page_size = 1 << 10
                 get_files = self._files
                 path_to_id = self.path_to_id
                 data = get_files(id, page_size)["data"]
@@ -6360,15 +6557,15 @@
                     yield MappingProxyType(attr)
                 for offset in range(page_size, data["count"], page_size):
                     data = get_files(id, page_size, offset)["data"]
                     for attr in map(normalize_info, data["list"]):
                         path = attr["path"] = joinpath(dirname, escape(attr["name"]))
                         path_to_id[path] = attr["id"]
                         yield MappingProxyType(attr)
-            t = self.pid_to_attrs[id] = tuple(iterdir())
+            t = self.id_to_children[id] = tuple(iterdir())
             self.id_to_attr.update((attr["id"], attr) for attr in t)
             return iter(t)
 
     def receive(self, ids: int | str | Iterable[int | str], /, cid: int = 0):
         if isinstance(ids, int):
             ids = str(ids)
         elif isinstance(ids, Iterable):
@@ -6547,15 +6744,15 @@
 # TODO: 参考zipfile的接口设计 namelist filelist
 # TODO: 当文件特别多时，可以用 zipfile 等模块来读取文件列表
 class P115ZipFileSystem(P115FileSystemBase[MappingProxyType, P115ZipPath]):
     file_id: Optional[int]
     pick_code: str
     path_to_id: MutableMapping[str, int]
     id_to_attr: MutableMapping[int, MappingProxyType]
-    pid_to_attrs: MutableMapping[int, tuple[MappingProxyType]]
+    id_to_children: MutableMapping[int, tuple[MappingProxyType]]
     full_loaded: bool
     path_class = P115ZipPath
 
     def __init__(
         self, 
         /, 
         client: P115Client, 
@@ -6575,26 +6772,32 @@
             client=client, 
             cid=0, 
             path="/", 
             pick_code=pick_code, 
             file_id=file_id, 
             path_to_id={"/": 0}, 
             id_to_attr={}, 
-            pid_to_attrs={}, 
+            id_to_children={}, 
             full_loaded=False, 
             _nextid=count(1).__next__, 
         )
         if file_id is None:
             self.__dict__["create_time"] = datetime.fromtimestamp(0)
 
     def __setattr__(self, attr, val, /) -> Never:
         raise TypeError("can't set attribute")
 
     @classmethod
-    def login(cls, /, id_or_pickcode: int | str, cookie=None, app: str = "web") -> Self:
+    def login(
+        cls, 
+        /, 
+        id_or_pickcode: int | str, 
+        cookie = None, 
+        app: str = "web", 
+    ) -> Self:
         return cls(P115Client(cookie, login_app=app), id_or_pickcode)
 
     @check_response
     def _files(
         self, 
         /, 
         path: str = "", 
@@ -6729,15 +6932,15 @@
         if not attr["is_directory"]:
             raise NotADirectoryError(
                 errno.ENOTDIR, 
                 f"{attr['path']!r} (id={attr['id']!r}) is not a directory", 
             )
         id = attr["id"]
         try:
-            return iter(self.pid_to_attrs[id])
+            return iter(self.id_to_children[id])
         except KeyError:
             nextid = self.__dict__["_nextid"]
             dirname = attr["path"]
             def iterdir():
                 get_files = self._files
                 path_to_id = self.path_to_id
                 data = get_files(dirname)["data"]
@@ -6751,15 +6954,15 @@
                     data = get_files(dirname, next_marker)["data"]
                     for attr in map(normalize_info, data["list"]):
                         path = joinpath(dirname, escape(attr["name"]))
                         attr.update(id=nextid(), parent_id=id, path=path)
                         path_to_id[path] = attr["id"]
                         yield MappingProxyType(attr)
                     next_marker = data["next_marker"]
-            t = self.pid_to_attrs[id] = tuple(iterdir())
+            t = self.id_to_children[id] = tuple(iterdir())
             self.id_to_attr.update((attr["id"], attr) for attr in t)
             return iter(t)
 
 
 class P115Offline:
     __slots__ = "client",
 
@@ -7126,15 +7329,15 @@
         })
 
     @check_response
     def update(self, /, share_code: str, **payload) -> dict:
         return self.client.share_update({"share_code": share_code, **payload})
 
 
-# TODO 可以关闭缓存，每次拉取最新的数据
+# TODO upload_tree 多线程和进度条，并且为每一个上传返回一个 task，可重试
 # TODO 能及时处理文件已不存在
 # TODO 为各个fs接口添加额外的请求参数
 # TODO 115中多个文件可以在同一目录下同名，如何处理
 # TODO 上传如果失败，因为名字问题，则尝试用uuid名字，上传成功后，再进行改名，如果成功，删除原来的文件，不成功，则删掉上传的文件（如果上传了的话）
 # TODO 如果压缩包尚未解压，则使用 zipfile 之类的模块，去模拟文件系统
 # TODO 支持传入作为缓存的 MutableMapping
 # TODO 调用 getcwd 时需要获取最新的名字
```

### Comparing `python_115-0.0.4.9/p115/util/_init_mimetypes.py` & `python_115-0.0.5/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.4.9/p115/util/cipher.py` & `python_115-0.0.5/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.4.9/p115/util/concurrent.py` & `python_115-0.0.5/p115/util/concurrent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__all__ = ["thread_batch", "thread_pool_batch", "async_batch", "as_thread"]
+__all__ = ["thread_batch", "thread_pool_batch", "async_batch", "as_thread", "run_thread"]
 
-from asyncio import CancelledError, Semaphore, TaskGroup
+from asyncio import CancelledError, Semaphore as AsyncSemaphore, TaskGroup
 from collections.abc import Callable, Coroutine, Iterable
 from concurrent.futures import Future, ThreadPoolExecutor
 from functools import partial, update_wrapper
 from inspect import isawaitable
 from queue import Queue
-from threading import Event, Lock, Thread
+from threading import Event, Lock, Semaphore, Thread
 from typing import cast, Any, Optional, TypeVar
 
 from .args import argcount
 
 
 T = TypeVar("T")
 V = TypeVar("V")
@@ -103,15 +103,15 @@
         pool.shutdown(False, cancel_futures=True)
 
 
 async def async_batch(
     work: Callable[[T], Coroutine[None, None, V]] | Callable[[T, Callable], Coroutine[None, None, V]], 
     tasks: Iterable[T], 
     callback: Optional[Callable[[V], Any]] = None, 
-    sema: Optional[Semaphore] = None, 
+    sema: Optional[AsyncSemaphore] = None, 
 ):
     ac = argcount(work)
     if ac < 1:
         raise TypeError(f"{work!r} should accept a positional argument as task")
     with_submit = ac > 1
     async def works(task):
         try:
@@ -139,25 +139,48 @@
     async with TaskGroup() as tg:
         create_task = tg.create_task
         for task in tasks:
             submit(task)
 
 
 def as_thread(
-    func: Optional[Callable[..., V]] = None, 
+    func: Optional[Callable] = None, 
     /, 
+    lock = None, 
     **thread_init_kwds, 
 ):
     if func is None:
         return partial(as_thread, **thread_init_kwds)
-    def wrapper(*args, **kwds) -> Future[V]: 
-        def asfuture(): 
-            try: 
-                fu.set_result(func(*args, **kwds))
-            except BaseException as e:
-                fu.set_exception(e)
+    if isinstance(lock, int):
+        lock = Semaphore(lock)
+    def wrapper(*args, **kwds) -> Future[V]:
+        if lock is None:
+            def asfuture():
+                try: 
+                    fu.set_result(func(*args, **kwds))
+                except BaseException as e:
+                    fu.set_exception(e)
+        else:
+            def asfuture():
+                with lock:
+                    try: 
+                        fu.set_result(func(*args, **kwds))
+                    except BaseException as e:
+                        fu.set_exception(e)
         fu: Future[V] = Future()
-        thread = fu.thread = Thread(target=asfuture, **thread_init_kwds)
+        thread = fu.thread = Thread(target=asfuture, **thread_init_kwds) # type: ignore
         thread.start()
         return fu
     return update_wrapper(wrapper, func)
 
+
+def run_thread(
+    func: Optional[Callable] = None, 
+    /, 
+    *args, 
+    **kwargs, 
+):
+    if func is None:
+        f = as_thread(None, *args, **kwargs)
+        return lambda func, *args, **kwargs: f(func)(*args, **kwargs)
+    return as_thread(func)(*args, **kwargs)
+
```

### Comparing `python_115-0.0.4.9/p115/util/download.py` & `python_115-0.0.5/p115/util/urlopen.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,88 +1,172 @@
 #!/usr/bin/env python3
-# encoding: utf-8
+# coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__all__ = ["download", "requests_download"]
+__all__ = ["urlopen", "download"]
 
 if __name__ == "__main__":
     from argparse import ArgumentParser
 
     parser = ArgumentParser(description="python url downloader")
     parser.add_argument("url", nargs="?", help="URL(s) to be downloaded (one URL per line), if omitted, read from stdin")
     parser.add_argument("-d", "--savedir", default="", help="path to the downloaded file")
     parser.add_argument("-r", "--resume", action="store_true", help="skip downloaded data")
     parser.add_argument("-hs", "--headers", help="dictionary of HTTP Headers to send with")
-    parser.add_argument("-rq", "--use-requests", action="store_true", help="use `requests` module")
     args = parser.parse_args()
 
-# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Range_requests
-# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-Ranges
-# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Range
-# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/206
-# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/ETag
-# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Range
-# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/If-Range
-# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-Encoding
-# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Encoding
-
 import errno
 
-from collections.abc import Callable, Generator
+from collections.abc import Callable, Generator, Mapping, Sequence
+from copy import copy
+from http.client import HTTPResponse
 from inspect import isgenerator
+from json import dumps
 from os import fsdecode, fstat, makedirs, PathLike
 from os.path import abspath, dirname, isdir, join as joinpath
 from shutil import COPY_BUFSIZE # type: ignore
+from ssl import SSLContext, _create_unverified_context
 from typing import cast, Any, Optional
-
-from requests import Response, Session
+from urllib.error import HTTPError
+from urllib.parse import urlencode, urlsplit
+from urllib.request import build_opener, HTTPSHandler, OpenerDirector, Request
 
 if __name__ == "__main__":
     from sys import path
     path.insert(0, dirname(dirname(__file__)))
     from util.file import bio_skip_bytes, SupportsRead, SupportsWrite # type: ignore
-    from util.iter import cut_iter # type: ignore
     from util.response import get_filename, get_length, is_chunked, is_range_request # type: ignore
     from util.text import headers_str_to_dict # type: ignore
-    from util.urlopen import urlopen # type: ignore
     del path[0]
 else:
     from .file import bio_skip_bytes, SupportsRead, SupportsWrite
-    from .iter import cut_iter
     from .response import get_filename, get_length, is_chunked, is_range_request
     from .text import headers_str_to_dict
-    from .urlopen import urlopen
 
 
-if "__del__" not in Response.__dict__:
-    setattr(Response, "__del__", Response.close)
-if "__del__" not in Session.__dict__:
-    setattr(Session, "__del__", Session.close)
+if "__del__" not in HTTPResponse.__dict__:
+    setattr(HTTPResponse, "__del__", HTTPResponse.close)
+
+
+def urlopen(
+    url: str | Request, 
+    params: Optional[str | Mapping | Sequence[tuple[Any, Any]]] = None, 
+    data: Optional[bytes | str | Mapping | Sequence[tuple[Any, Any]]] = None, 
+    json: Any = None, 
+    headers: dict[str, str] = {"User-agent": ""}, 
+    method: str = "GET", 
+    timeout: Optional[int | float] = None, 
+    proxy: Optional[tuple[str, str]] = None, 
+    opener: OpenerDirector = build_opener(HTTPSHandler(context=_create_unverified_context())), 
+    context: Optional[SSLContext] = None, 
+    origin: Optional[str] = None, 
+) -> HTTPResponse:
+    if isinstance(url, str) and not urlsplit(url).scheme:
+        if origin:
+            if not url.startswith("/"):
+                url = "/" + url
+            url = origin + url
+    if params:
+        if not isinstance(params, str):
+            params = urlencode(params)
+    params = cast(Optional[str], params)
+    if json is not None:
+        if isinstance(json, bytes):
+            data = json
+        else:
+            data = dumps(json).encode("utf-8")
+        headers = {**headers, "Content-type": "application/json"}
+    elif data is not None:
+        if isinstance(data, bytes):
+            pass
+        elif isinstance(data, str):
+            data = data.encode("utf-8")
+        else:
+            data = urlencode(data).encode("latin-1")
+    data = cast(Optional[bytes], data)
+    if isinstance(url, Request):
+        req = url
+        if params:
+            req.full_url += "?&"["?" in req.full_url] + params
+        if headers:
+            for key, val in headers.items():
+                req.add_header(key, val)
+        if data is not None:
+            req.data = data
+        req.method = method.upper()
+    else:
+        if params:
+            url += "?&"["?" in url] + params
+        req = Request(url, data, headers=headers, method=method.upper())
+    if proxy:
+        req.set_proxy(*proxy)
+    if context:
+        opener = build_opener(HTTPSHandler(context=context))
+    if timeout is None:
+        return opener.open(req)
+    else:
+        return opener.open(req, timeout=timeout)
 
 
 def download(
     url: str, 
     file: bytes | str | PathLike | SupportsWrite[bytes] = "", 
     resume: bool = False, 
     chunksize: int = COPY_BUFSIZE, 
     headers: Optional[dict[str, str]] = None, 
     make_reporthook: Optional[Callable[[Optional[int]], Callable[[int], Any] | Generator[int, Any, Any]]] = None, 
-    urlopen: Callable = urlopen, 
+    **urlopen_kwargs, 
 ) -> str | SupportsWrite[bytes]:
-    """
+    """Download a URL into a file.
+
+    Example::
+
+        1. use `make_reporthook` to show progress:
+
+            You can use the following function to show progress for the download task
+
+            .. code: python
+
+                from time import perf_counter
+
+                def progress(total=None):
+                    read_num = 0
+                    start_t = perf_counter()
+                    while True:
+                        read_num += yield
+                        speed = read_num / 1024 / 1024 / (perf_counter() - start_t)
+                        print(f"\r\x1b[K{read_num} / {total} | {speed:.2f} MB/s", end="", flush=True)
+
+            Or use the following function for more real-time speed
+
+            .. code: python
+
+                from collections import deque
+                from time import perf_counter
+    
+                def progress(total=None):
+                    dq = deque(maxlen=64)
+                    read_num = 0
+                    dq.append((read_num, perf_counter()))
+                    while True:
+                        read_num += yield
+                        cur_t = perf_counter()
+                        speed = (read_num - dq[0][0]) / 1024 / 1024 / (cur_t - dq[0][1])
+                        print(f"\r\x1b[K{read_num} / {total} | {speed:.2f} MB/s", end="", flush=True)
+                        dq.append((read_num, cur_t))
     """
     if headers:
-        headers = {**headers, "Accept-Encoding": "identity"}
+        headers = {**headers, "Accept-encoding": "identity"}
     else:
-        headers = {"Accept-Encoding": "identity"}
+        headers = {"Accept-encoding": "identity"}
 
     if chunksize <= 0:
         chunksize = COPY_BUFSIZE
 
-    resp = urlopen(url, headers=headers)
+    resp: HTTPResponse = urlopen(url, headers=headers, **urlopen_kwargs)
     length = get_length(resp)
     if length == 0 and is_chunked(resp):
         length = None
 
     fdst: SupportsWrite[bytes]
     if hasattr(file, "write"):
         file = fdst = cast(SupportsWrite[bytes], file)
@@ -101,67 +185,53 @@
         try:
             filesize = fstat(fdst.fileno()).st_size # type: ignore
         except (AttributeError, OSError):
             pass
         else:
             if filesize == length:
                 return file
+            if filesize and is_range_request(resp):
+                if filesize == length:
+                    return file
             elif length is not None and filesize > length:
                 raise OSError(errno.EIO, f"file {file!r} is larger than url {url!r}: {filesize} > {length} (in bytes)")
-    elif length == 0:
-        return file
 
     if make_reporthook:
         reporthook = make_reporthook(length)
         if isgenerator(reporthook):
             next(reporthook)
             reporthook = reporthook.send
         reporthook = cast(Callable[[int], Any], reporthook)
     else:
         reporthook = None
 
-    if filesize and is_range_request(resp):
-        resp.close()
-        resp = urlopen(url, headers={**headers, "Range": "bytes=%d-" % filesize})
-        if not is_range_request(resp):
-            raise OSError(errno.EIO, f"range request failed: {url!r}")
-
-    with resp:
-        fsrc_read = resp.read
-        fdst_write = fdst.write
+    try:
         if filesize:
             if is_range_request(resp):
+                resp.close()
+                resp = urlopen(url, headers={**headers, "Range": "bytes=%d-" % filesize}, **urlopen_kwargs)
+                if not is_range_request(resp):
+                    raise OSError(errno.EIO, f"range request failed: {url!r}")
                 if reporthook:
                     reporthook(filesize)
-            else:
+            elif resume:
                 bio_skip_bytes(resp, filesize, callback=reporthook)
 
+        fsrc_read = resp.read 
+        fdst_write = fdst.write
         while (chunk := fsrc_read(chunksize)):
             fdst_write(chunk)
             if reporthook:
                 reporthook(len(chunk))
+    finally:
+        resp.close()
 
     return file
 
 
-def requests_download(
-    url: str, 
-    urlopen: Callable = Session().get, 
-    **kwargs, 
-) -> str | SupportsWrite[bytes]:
-    """
-    """
-    def urlopen_wrapper(url, headers):
-        resp = urlopen(url, headers=headers, stream=True)
-        resp.raise_for_status()
-        resp.read = resp.raw.read
-        return resp
-    return download(url, urlopen=urlopen_wrapper, **kwargs)
-
-
 if __name__ == "__main__":
     from collections import deque
     from time import perf_counter
 
     def progress(total=None):
         dq: deque[tuple[int, float]] = deque(maxlen=64)
         read_num = 0
@@ -183,30 +253,25 @@
     else:
         from sys import stdin
         urls = (l.removesuffix("\n") for l in stdin)
     savedir = args.savedir
     if savedir:
         makedirs(savedir, exist_ok=True)
 
-    if args.use_requests:
-        downloader: Callable = requests_download
-    else:
-        downloader = download
-
     try:
         headers = args.headers
         if headers is not None:
             headers = headers_str_to_dict(headers)
         for url in urls:
             if not url:
                 continue
             try:
-                file = downloader(
+                file = download(
                     url, 
-                    file=savedir, 
+                    savedir, 
                     resume=args.resume, 
                     make_reporthook=progress, 
                     headers=headers, 
                 )
                 print(f"\r\x1b[K\x1b[1;32mDOWNLOADED\x1b[0m \x1b[4;34m{url!r}\x1b[0m\n |_ ⏬ \x1b[4;34m{file!r}\x1b[0m")
             except BaseException as e:
                 print(f"\r\x1b[K\x1b[1;31mERROR\x1b[0m \x1b[4;34m{url!r}\x1b[0m\n  |_ 🙅 \x1b[1;31m{type(e).__qualname__}\x1b[0m: {e}")
```

### Comparing `python_115-0.0.4.9/p115/util/file.py` & `python_115-0.0.5/p115/util/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __all__ = [
     "SupportsRead", "SupportsWrite", "SupportsGetUrl", 
-    "bio_chunk_iter", "bio_skip_bytes", "get_filesize", "HTTPFileReader", "RequestsFileReader"
+    "bio_chunk_iter", "bio_skip_iter", "bio_skip_bytes", "get_filesize", 
+    "HTTPFileReader", "RequestsFileReader", 
 ]
 
 import errno
 
 from collections.abc import Callable, Iterator, Mapping
 from functools import cached_property, partial
 from http.client import HTTPResponse
@@ -67,68 +68,69 @@
     elif size < 0:
         while (chunk := read(chunksize)):
             yield chunk
             if callback:
                 callback(len(chunk))
 
 
-def bio_skip_bytes(
+def bio_skip_iter(
     bio: BytesReadable, 
     size: int = -1, 
     chunksize: int = COPY_BUFSIZE, 
-    callback: Optional[Callable[[int], Any]] = None, 
-) -> BytesReadable:
+) -> Iterator[int]:
     if size == 0:
-        return bio
+        return
     if chunksize <= 0:
         chunksize = COPY_BUFSIZE
     try:
         if size > 0:
             pos = bio.seek(size, 1) # type: ignore
         else:
             pos = bio.seek(0, 2) # type: ignore
-        if callback:
-            callback(pos)
+        yield pos
     except Exception:
         if hasattr(bio, "readinto"):
             readinto = bio.readinto
             buf = bytearray(chunksize)
             if size > 0:
                 while size >= chunksize:
-                    length = readinto(buf)
-                    if callback:
-                        callback(length)
+                    yield (length := readinto(buf))
                     if length < chunksize:
                         break
                     size -= chunksize
                 if size:
                     del buf[size:]
-                    length = readinto(buf)
-                    if callback:
-                        callback(length)
+                    yield readinto(buf)
             else:
                 while (length := readinto(buf)):
-                    if callback:
-                        callback(length)
+                    yield length
         else:
             read = bio.read
             if size > 0:
                 while size:
                     readsize = min(chunksize, size)
                     chunk = read(readsize)
-                    length = len(chunk)
-                    if callback:
-                        callback(length)
+                    yield (length := len(chunk))
                     if length < readsize:
                         break
                     size -= readsize
             else:
                 while (chunk := read(chunksize)):
-                    if callback:
-                        callback(len(chunk))
+                    yield len(chunk)
+
+
+def bio_skip_bytes(
+    bio: BytesReadable, 
+    size: int = -1, 
+    chunksize: int = COPY_BUFSIZE, 
+    callback: Optional[Callable[[int], Any]] = None, 
+) -> BytesReadable:
+    for length in bio_skip_iter(bio, size, chunksize):
+        if callback:
+            callback(length)
     return bio
 
 
 def get_filesize(file, /, dont_read: bool = True) -> int:
     if isinstance(file, (bytes, str, PathLike)):
         return stat(file).st_size
     curpos = 0
```

### Comparing `python_115-0.0.4.9/p115/util/hash.py` & `python_115-0.0.5/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.4.9/p115/util/ignore.py` & `python_115-0.0.5/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.4.9/p115/util/iter.py` & `python_115-0.0.5/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.4.9/p115/util/path.py` & `python_115-0.0.5/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.4.9/p115/util/property.py` & `python_115-0.0.5/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.4.9/p115/util/response.py` & `python_115-0.0.5/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.4.9/p115/util/retry.py` & `python_115-0.0.5/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.4.9/p115/util/text.py` & `python_115-0.0.5/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.4.9/p115/util/urlopen.py` & `python_115-0.0.5/p115/util/download.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,172 +1,196 @@
 #!/usr/bin/env python3
-# coding: utf-8
+# encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__all__ = ["urlopen", "download"]
+__all__ = ["DownloadTask", "download_iter", "download", "requests_download"]
 
 if __name__ == "__main__":
     from argparse import ArgumentParser
 
     parser = ArgumentParser(description="python url downloader")
     parser.add_argument("url", nargs="?", help="URL(s) to be downloaded (one URL per line), if omitted, read from stdin")
     parser.add_argument("-d", "--savedir", default="", help="path to the downloaded file")
     parser.add_argument("-r", "--resume", action="store_true", help="skip downloaded data")
     parser.add_argument("-hs", "--headers", help="dictionary of HTTP Headers to send with")
+    parser.add_argument("-rq", "--use-requests", action="store_true", help="use `requests` module")
     args = parser.parse_args()
 
+# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Range_requests
+# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-Ranges
+# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Range
+# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/206
+# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/ETag
+# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Range
+# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/If-Range
+# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-Encoding
+# NOTE https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Encoding
+
 import errno
 
-from collections.abc import Callable, Generator, Mapping, Sequence
-from copy import copy
-from http.client import HTTPResponse
+from collections.abc import Callable, Generator, Iterator
 from inspect import isgenerator
-from json import dumps
 from os import fsdecode, fstat, makedirs, PathLike
 from os.path import abspath, dirname, isdir, join as joinpath
 from shutil import COPY_BUFSIZE # type: ignore
-from ssl import SSLContext, _create_unverified_context
-from typing import cast, Any, Optional
-from urllib.error import HTTPError
-from urllib.parse import urlencode, urlsplit
-from urllib.request import build_opener, HTTPSHandler, OpenerDirector, Request
+from threading import Event
+from typing import cast, Any, NamedTuple, Never, Optional, Self
+
+from requests import Response, Session
 
 if __name__ == "__main__":
     from sys import path
     path.insert(0, dirname(dirname(__file__)))
-    from util.file import bio_skip_bytes, SupportsRead, SupportsWrite # type: ignore
+    from util.concurrent import run_thread # type: ignore
+    from util.file import bio_skip_iter, SupportsRead, SupportsWrite # type: ignore
+    from util.iter import cut_iter # type: ignore
     from util.response import get_filename, get_length, is_chunked, is_range_request # type: ignore
     from util.text import headers_str_to_dict # type: ignore
+    from util.urlopen import urlopen # type: ignore
     del path[0]
 else:
-    from .file import bio_skip_bytes, SupportsRead, SupportsWrite
+    from .concurrent import run_thread
+    from .file import bio_skip_iter, SupportsRead, SupportsWrite
+    from .iter import cut_iter
     from .response import get_filename, get_length, is_chunked, is_range_request
     from .text import headers_str_to_dict
+    from .urlopen import urlopen
 
 
-if "__del__" not in HTTPResponse.__dict__:
-    setattr(HTTPResponse, "__del__", HTTPResponse.close)
+if "__del__" not in Response.__dict__:
+    setattr(Response, "__del__", Response.close)
+if "__del__" not in Session.__dict__:
+    setattr(Session, "__del__", Session.close)
+
+
+class DownloadProgress(NamedTuple):
+    total: int
+    downloaded: int
+    skipped: int
+    last_incr: int = 0
+    extra: Any = None
+
+
+class DownloadTask:
+
+    def __init__(self, /, gen, submit=run_thread):
+        if not callable(submit):
+            submit = submit.submit
+        self._submit = submit
+        self._state = "PENDING"
+        self._gen = gen
+        self._done_event = Event()
+
+    def __repr__(self, /) -> str:
+        return f"<{type(self).__qualname__} :: state={self.state!r} progress={self.progress!r}>"
+
+    @classmethod
+    def create_task(
+        cls, 
+        /, 
+        *args, 
+        submit=run_thread, 
+        **kwargs, 
+    ) -> Self:
+        return cls(download_iter(*args, **kwargs), submit=submit)
+
+    @property
+    def closed(self, /) -> bool:
+        return self._state in ("CANCELED", "FAILED", "FINISHED")
+
+    @property
+    def progress(self, /) -> Optional[DownloadProgress]:
+        return self.__dict__.get("_progress")
+
+    @property
+    def result(self, /):
+        self._done_event.wait()
+        return self._result
+
+    @result.setter
+    def result(self, val, /):
+        self._result = val
+        self._done_event.set()
+
+    @property
+    def state(self, /) -> str:
+        return self._state
 
+    def close(self, /):
+        if self._state in ("CANCELED", "FAILED", "FINISHED"):
+            pass
+        else:
+            state = self._state
+            self._state = "CANCELED"
+            if state != "RUNNING":
+                self.run()
+
+    def pause(self, /):
+        if self._state in ("PAUSED", "RUNNING"):
+            self._state = "PAUSED"
+        else:
+            raise RuntimeError(f"can't pause when state={self._state!r}")
 
-def urlopen(
-    url: str | Request, 
-    params: Optional[str | Mapping | Sequence[tuple[Any, Any]]] = None, 
-    data: Optional[bytes | str | Mapping | Sequence[tuple[Any, Any]]] = None, 
-    json: Any = None, 
-    headers: dict[str, str] = {"User-agent": ""}, 
-    method: str = "GET", 
-    timeout: Optional[int | float] = None, 
-    proxy: Optional[tuple[str, str]] = None, 
-    opener: OpenerDirector = build_opener(HTTPSHandler(context=_create_unverified_context())), 
-    context: Optional[SSLContext] = None, 
-    origin: Optional[str] = None, 
-) -> HTTPResponse:
-    if isinstance(url, str) and not urlsplit(url).scheme:
-        if origin:
-            if not url.startswith("/"):
-                url = "/" + url
-            url = origin + url
-    if params:
-        if not isinstance(params, str):
-            params = urlencode(params)
-    params = cast(Optional[str], params)
-    if json is not None:
-        if isinstance(json, bytes):
-            data = json
+    def _run(self, /):
+        if self._state in ("PENDING", "PAUSED"):
+            self._state = "RUNNING"
         else:
-            data = dumps(json).encode("utf-8")
-        headers = {**headers, "Content-type": "application/json"}
-    elif data is not None:
-        if isinstance(data, bytes):
-            pass
-        elif isinstance(data, str):
-            data = data.encode("utf-8")
+            raise RuntimeError(f"can't run when state={self._state!r}")
+        gen = self._gen
+        try:
+            while self._state == "RUNNING":
+                self._progress = next(gen)
+        except KeyboardInterrupt:
+            raise
+        except StopIteration as exc:
+            self._state = "FINISHED"
+            self.result = exc.value
+        except BaseException as exc:
+            self._state = "FAILED"
+            self.result = exc
         else:
-            data = urlencode(data).encode("latin-1")
-    data = cast(Optional[bytes], data)
-    if isinstance(url, Request):
-        req = url
-        if params:
-            req.full_url += "?&"["?" in req.full_url] + params
-        if headers:
-            for key, val in headers.items():
-                req.add_header(key, val)
-        if data is not None:
-            req.data = data
-        req.method = method.upper()
-    else:
-        if params:
-            url += "?&"["?" in url] + params
-        req = Request(url, data, headers=headers, method=method.upper())
-    if proxy:
-        req.set_proxy(*proxy)
-    if context:
-        opener = build_opener(HTTPSHandler(context=context))
-    if timeout is None:
-        return opener.open(req)
-    else:
-        return opener.open(req, timeout=timeout)
+            if self._state == "CANCELED":
+                try:
+                    gen.close()
+                finally:
+                    self.result = None
+
+    def run(self, /):
+        return self._submit(self._run)
+
+    def run_wait(self, /):
+        if not self._done_event.is_set():
+            if self._state == "RUNNING":
+                self._done_event.wait()
+            else:
+                self._run()
 
 
-def download(
-    url: str, 
+def download_iter(
+    url: str | Callable[[], str], 
     file: bytes | str | PathLike | SupportsWrite[bytes] = "", 
     resume: bool = False, 
     chunksize: int = COPY_BUFSIZE, 
     headers: Optional[dict[str, str]] = None, 
-    make_reporthook: Optional[Callable[[Optional[int]], Callable[[int], Any] | Generator[int, Any, Any]]] = None, 
-    **urlopen_kwargs, 
-) -> str | SupportsWrite[bytes]:
-    """Download a URL into a file.
-
-    Example::
-
-        1. use `make_reporthook` to show progress:
-
-            You can use the following function to show progress for the download task
-
-            .. code: python
-
-                from time import perf_counter
-
-                def progress(total=None):
-                    read_num = 0
-                    start_t = perf_counter()
-                    while True:
-                        read_num += yield
-                        speed = read_num / 1024 / 1024 / (perf_counter() - start_t)
-                        print(f"\r\x1b[K{read_num} / {total} | {speed:.2f} MB/s", end="", flush=True)
-
-            Or use the following function for more real-time speed
-
-            .. code: python
-
-                from collections import deque
-                from time import perf_counter
-    
-                def progress(total=None):
-                    dq = deque(maxlen=64)
-                    read_num = 0
-                    dq.append((read_num, perf_counter()))
-                    while True:
-                        read_num += yield
-                        cur_t = perf_counter()
-                        speed = (read_num - dq[0][0]) / 1024 / 1024 / (cur_t - dq[0][1])
-                        print(f"\r\x1b[K{read_num} / {total} | {speed:.2f} MB/s", end="", flush=True)
-                        dq.append((read_num, cur_t))
+    urlopen: Callable = urlopen, 
+) -> Iterator[DownloadProgress]:
+    """
     """
+    if not isinstance(url, str):
+        url = url()
+
     if headers:
-        headers = {**headers, "Accept-encoding": "identity"}
+        headers = {**headers, "Accept-Encoding": "identity"}
     else:
-        headers = {"Accept-encoding": "identity"}
+        headers = {"Accept-Encoding": "identity"}
 
     if chunksize <= 0:
         chunksize = COPY_BUFSIZE
 
-    resp: HTTPResponse = urlopen(url, headers=headers, **urlopen_kwargs)
+    resp = urlopen(url, headers=headers)
     length = get_length(resp)
     if length == 0 and is_chunked(resp):
         length = None
 
     fdst: SupportsWrite[bytes]
     if hasattr(file, "write"):
         file = fdst = cast(SupportsWrite[bytes], file)
@@ -176,60 +200,100 @@
             file = joinpath(file, get_filename(resp, "download"))
         try:
             fdst = open(file, "ab" if resume else "wb")
         except FileNotFoundError:
             makedirs(dirname(file), exist_ok=True)
             fdst = open(file, "ab" if resume else "wb")
 
+    extra = {"url": url, "file": file, "resume": resume}
+
     filesize = 0
     if resume:
         try:
             filesize = fstat(fdst.fileno()).st_size # type: ignore
         except (AttributeError, OSError):
             pass
         else:
             if filesize == length:
-                return file
-            if filesize and is_range_request(resp):
-                if filesize == length:
-                    return file
+                yield DownloadProgress(length, 0, length, length, extra)
+                return
             elif length is not None and filesize > length:
                 raise OSError(errno.EIO, f"file {file!r} is larger than url {url!r}: {filesize} > {length} (in bytes)")
+    elif length == 0:
+        yield DownloadProgress(0, 0, 0, 0, extra)
+        return
+
+    if filesize and is_range_request(resp):
+        resp.close()
+        resp = urlopen(url, headers={**headers, "Range": "bytes=%d-" % filesize})
+        if not is_range_request(resp):
+            raise OSError(errno.EIO, f"range request failed: {url!r}")
+
+    yield DownloadProgress(length, 0, 0, 0, extra)
+
+    length_downloaded = 0
+    length_skipped = 0
+    with resp:
+        fsrc_read = resp.read
+        fdst_write = fdst.write
+        if filesize:
+            if is_range_request(resp):
+                length_skipped = filesize
+                yield DownloadProgress(length, 0, length_skipped, length_skipped, extra)
+            else:
+                for skiplen in bio_skip_iter(resp, filesize):
+                    length_skipped += skiplen
+                    yield DownloadProgress(length, 0, length_skipped, skiplen, extra)
 
+        while (chunk := fsrc_read(chunksize)):
+            downlen = fdst_write(chunk)
+            length_downloaded += downlen
+            yield DownloadProgress(length, length_downloaded, length_skipped, downlen, extra)
+
+
+def download(
+    url: str | Callable[[], str], 
+    file: bytes | str | PathLike | SupportsWrite[bytes] = "", 
+    resume: bool = False, 
+    chunksize: int = COPY_BUFSIZE, 
+    headers: Optional[dict[str, str]] = None, 
+    urlopen: Callable = urlopen, 
+    make_reporthook: Optional[Callable[[Optional[int]], Callable[[int], Any] | Generator[int, Any, Any]]] = None, 
+):
+    """
+    """
+    gen = download_iter(url, file, resume=resume, chunksize=chunksize, headers=headers, urlopen=urlopen)
     if make_reporthook:
-        reporthook = make_reporthook(length)
+        progress = next(gen)
+        reporthook = make_reporthook(progress.total)
         if isgenerator(reporthook):
             next(reporthook)
             reporthook = reporthook.send
         reporthook = cast(Callable[[int], Any], reporthook)
+        reporthook(progress.last_incr)
     else:
         reporthook = None
 
-    try:
-        if filesize:
-            if is_range_request(resp):
-                resp.close()
-                resp = urlopen(url, headers={**headers, "Range": "bytes=%d-" % filesize}, **urlopen_kwargs)
-                if not is_range_request(resp):
-                    raise OSError(errno.EIO, f"range request failed: {url!r}")
-                if reporthook:
-                    reporthook(filesize)
-            elif resume:
-                bio_skip_bytes(resp, filesize, callback=reporthook)
+    for progress in gen:
+        reporthook and reporthook(progress.last_incr)
 
-        fsrc_read = resp.read 
-        fdst_write = fdst.write
-        while (chunk := fsrc_read(chunksize)):
-            fdst_write(chunk)
-            if reporthook:
-                reporthook(len(chunk))
-    finally:
-        resp.close()
 
-    return file
+def requests_download(
+    url: str | Callable[[], str], 
+    urlopen: Callable = Session().get, 
+    **kwargs, 
+):
+    """
+    """
+    def urlopen_wrapper(url, headers):
+        resp = urlopen(url, headers=headers, stream=True)
+        resp.raise_for_status()
+        resp.read = resp.raw.read
+        return resp
+    return download(url, urlopen=urlopen_wrapper, **kwargs)
 
 
 if __name__ == "__main__":
     from collections import deque
     from time import perf_counter
 
     def progress(total=None):
@@ -253,25 +317,30 @@
     else:
         from sys import stdin
         urls = (l.removesuffix("\n") for l in stdin)
     savedir = args.savedir
     if savedir:
         makedirs(savedir, exist_ok=True)
 
+    if args.use_requests:
+        downloader: Callable = requests_download
+    else:
+        downloader = download
+
     try:
         headers = args.headers
         if headers is not None:
             headers = headers_str_to_dict(headers)
         for url in urls:
             if not url:
                 continue
             try:
-                file = download(
+                file = downloader(
                     url, 
-                    savedir, 
+                    file=savedir, 
                     resume=args.resume, 
                     make_reporthook=progress, 
                     headers=headers, 
                 )
                 print(f"\r\x1b[K\x1b[1;32mDOWNLOADED\x1b[0m \x1b[4;34m{url!r}\x1b[0m\n |_ ⏬ \x1b[4;34m{file!r}\x1b[0m")
             except BaseException as e:
                 print(f"\r\x1b[K\x1b[1;31mERROR\x1b[0m \x1b[4;34m{url!r}\x1b[0m\n  |_ 🙅 \x1b[1;31m{type(e).__qualname__}\x1b[0m: {e}")
```

### Comparing `python_115-0.0.4.9/pyproject.toml` & `python_115-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.4.9"
+version = "0.0.5"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.4.9/readme.md` & `python_115-0.0.5/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.4.9/PKG-INFO` & `python_115-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.4.9
+Version: 0.0.5
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

