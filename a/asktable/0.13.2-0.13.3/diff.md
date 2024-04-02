# Comparing `tmp/asktable-0.13.2-py3-none-any.whl.zip` & `tmp/asktable-0.13.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,34 +1,34 @@
-Zip file size: 26717 bytes, number of entries: 32
+Zip file size: 26749 bytes, number of entries: 32
 -rw-r--r--  2.0 unx       86 b- defN 24-Apr-01 06:18 asktable/__init__.py
 -rw-r--r--  2.0 unx     2180 b- defN 24-Apr-01 06:16 asktable/api.py
 -rw-r--r--  2.0 unx     1667 b- defN 24-Apr-01 06:16 asktable/cli.py
 -rw-r--r--  2.0 unx     1220 b- defN 24-Apr-01 06:16 asktable/client.py
 -rw-r--r--  2.0 unx       41 b- defN 24-Apr-01 06:16 asktable/exceptions.py
 -rw-r--r--  2.0 unx      875 b- defN 24-Apr-01 06:44 asktable/log.py
 -rw-r--r--  2.0 unx     1492 b- defN 24-Apr-01 06:16 asktable/upload.py
 -rw-r--r--  2.0 unx      152 b- defN 24-Apr-01 06:16 asktable/models/__init__.py
 -rw-r--r--  2.0 unx     2588 b- defN 24-Apr-01 06:16 asktable/models/base.py
 -rw-r--r--  2.0 unx     2769 b- defN 24-Apr-01 06:16 asktable/models/chat.py
--rw-r--r--  2.0 unx     6395 b- defN 24-Apr-01 06:16 asktable/models/datasource.py
+-rw-r--r--  2.0 unx     6371 b- defN 24-Apr-02 12:05 asktable/models/datasource.py
 -rw-r--r--  2.0 unx     1264 b- defN 24-Apr-01 06:16 asktable/models/message.py
 -rw-r--r--  2.0 unx      878 b- defN 24-Apr-01 06:16 asktable/models/run.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-08 14:27 atcommon/__init__.py
 -rw-r--r--  2.0 unx     3352 b- defN 24-Mar-20 07:26 atcommon/tools.py
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-01 09:46 atcommon/version.py
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-02 12:06 atcommon/version.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-31 13:33 atcommon/exceptions/__init__.py
 -rw-r--r--  2.0 unx     1060 b- defN 24-Apr-01 06:16 atcommon/exceptions/client.py
 -rw-r--r--  2.0 unx       95 b- defN 24-Apr-01 06:16 atcommon/exceptions/server.py
--rw-r--r--  2.0 unx     1889 b- defN 24-Mar-11 05:37 atcommon/exceptions/server_base.py
+-rw-r--r--  2.0 unx     1979 b- defN 24-Apr-01 13:45 atcommon/exceptions/server_base.py
 -rw-r--r--  2.0 unx      589 b- defN 24-Apr-01 06:16 atcommon/exceptions/server_plugins.py
 -rw-r--r--  2.0 unx      466 b- defN 24-Apr-01 06:16 atcommon/models/__init__.py
 -rw-r--r--  2.0 unx      731 b- defN 24-Jan-20 03:26 atcommon/models/base.py
 -rw-r--r--  2.0 unx     2344 b- defN 24-Apr-01 06:16 atcommon/models/bi.py
 -rw-r--r--  2.0 unx     1069 b- defN 24-Apr-01 06:16 atcommon/models/chat.py
 -rw-r--r--  2.0 unx      682 b- defN 24-Apr-01 06:16 atcommon/models/datasource.py
 -rw-r--r--  2.0 unx    21682 b- defN 24-Apr-01 06:28 atcommon/models/meta.py
--rw-r--r--  2.0 unx     8285 b- defN 24-Apr-01 09:46 asktable-0.13.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-01 09:46 asktable-0.13.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 24-Apr-01 09:46 asktable-0.13.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 24-Apr-01 09:46 asktable-0.13.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2557 b- defN 24-Apr-01 09:46 asktable-0.13.2.dist-info/RECORD
-32 files, 66581 bytes uncompressed, 22637 bytes compressed:  66.0%
+-rw-r--r--  2.0 unx     8309 b- defN 24-Apr-02 12:06 asktable-0.13.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 12:06 asktable-0.13.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 24-Apr-02 12:06 asktable-0.13.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 24-Apr-02 12:06 asktable-0.13.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2557 b- defN 24-Apr-02 12:06 asktable-0.13.3.dist-info/RECORD
+32 files, 66671 bytes uncompressed, 22669 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -75,23 +75,23 @@
 
 Filename: atcommon/models/datasource.py
 Comment: 
 
 Filename: atcommon/models/meta.py
 Comment: 
 
-Filename: asktable-0.13.2.dist-info/METADATA
+Filename: asktable-0.13.3.dist-info/METADATA
 Comment: 
 
-Filename: asktable-0.13.2.dist-info/WHEEL
+Filename: asktable-0.13.3.dist-info/WHEEL
 Comment: 
 
-Filename: asktable-0.13.2.dist-info/entry_points.txt
+Filename: asktable-0.13.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: asktable-0.13.2.dist-info/top_level.txt
+Filename: asktable-0.13.3.dist-info/top_level.txt
 Comment: 
 
-Filename: asktable-0.13.2.dist-info/RECORD
+Filename: asktable-0.13.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## asktable/models/datasource.py

```diff
@@ -118,18 +118,18 @@
 
         if not id:
             raise ValueError("No ID or Name provided")
         # 通过资源ID来获取
         return self.api.send(endpoint=f"{self.endpoint}/{id}", method="GET")
 
     @convert_to_object(cls=DataSourceClientModel)
-    def register(self, ds_type, ds_access_config, ds_name=None):
+    def register(self, type, access_config, name=None):
         data = {
-            "type": ds_type, "name": ds_name,
-            "access_config": ds_access_config
+            "type": type, "name": name,
+            "access_config": access_config
         }
         return self.api.send(endpoint=self.endpoint, method="POST",
                              data=data)
 
     def upload_file_to_oss(self, local_file_path):
         oss_info = self.create_upload_params()['oss']
         file_name = os.path.basename(local_file_path)
@@ -157,20 +157,20 @@
 
         if direct_to_oss:
             url = self.upload_file_to_oss(local_file_path)
         else:
             url = self.upload_file_to_server(local_file_path)
 
         if file_ext == '.csv':
-            return self.register(ds_type="csv", ds_access_config={
+            return self.register(type="csv", ds_access_config={
                 "location_type": "http",
                 "location_url": url,
             })
         elif file_ext in ['.xls', '.xlsx']:
-            return self.register(ds_type="excel", ds_access_config={
+            return self.register(type="excel", ds_access_config={
                 "location_type": "http",
                 "location_url": url,
             })
         else:
             raise UnsupportedFileType(f"File type {file_ext} not supported")
 
     # def signed_url(self, url):
```

## atcommon/version.py

```diff
@@ -1 +1 @@
-VERSION="0.13.2"
+VERSION="0.13.3"
```

## atcommon/exceptions/server_base.py

```diff
@@ -98,7 +98,12 @@
     message = "Prompt too long"
 
 
 class InvalidStrucQuery(InternalError):
     code = 3002
     message = "Invalid query syntax"
 
+
+class LLMServiceError(InternalError):
+    code = 3003
+    message = "LLM service error"
+
```

## Comparing `asktable-0.13.2.dist-info/METADATA` & `asktable-0.13.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asktable
-Version: 0.13.2
+Version: 0.13.3
 Summary: AskTable SDK
 Home-page: https://asktable.com/
 Author: lele
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: tabulate
 Requires-Dist: pybase62
@@ -59,28 +59,29 @@
 以下示例使用命令行CLI方式演示。
 
 ### 注册数据源
 
 1. 注册 MySQL 数据源，这个地址必须是 AskTable Server可访问的
     ```python
     at.datasources.register(
-        ds_type="mysql",
-        ds_access_config={
+        type="mysql",
+        access_config={
             "host": "localhost",
             "port": 3306,
             "user": "root",
-            "password": ""
+            "password": "",
+            "db": "test"  # 可选
         }
     )
     ```
 2. 注册一个可下载的文件(Excel或CSV)
     ```python
     at.datasources.register(
-        ds_type="csv",
-        ds_access_config={
+        type="csv",
+        access_config={
             "location_url": "https://example.com/path/to/myfile.csv",
             "location_type": "http",
         }
     )
     ```
 
 3. 上传并注册一个本地的文件（Excel或CSV）
```

## Comparing `asktable-0.13.2.dist-info/RECORD` & `asktable-0.13.3.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 asktable/client.py,sha256=pfj9w1I5-0I78_maqds6pzS2OJmO7G8h_siwR09kUCw,1220
 asktable/exceptions.py,sha256=HUys_aPowtoLqjO4XhANXBQCUUpty1zLxV4fWPqBkLc,41
 asktable/log.py,sha256=CIRsQtXMB24sD5fFsUn2hxlEVJB33Ej8TIQKyET2pQ8,875
 asktable/upload.py,sha256=ZctBvZtKnBZWucRXzvdp25zBNGz3eQ6PAfdhzLzfMUU,1492
 asktable/models/__init__.py,sha256=LDrDHxIjYwQN-fLW4BKMkuogEUcDfLxMYtlEkq0Xzfk,152
 asktable/models/base.py,sha256=vDe19yuK6SJglgRlz8Gq9qKg_x1Cxs2tK82VKeJ3UCI,2588
 asktable/models/chat.py,sha256=Z-2p_crBI5HwljcIxtRNV46_FfsVmNc5oRrwq3dNigE,2769
-asktable/models/datasource.py,sha256=RsyR4pp_BowzYy9x8loK4mGfr1fzuHICEi9KIAapVKw,6395
+asktable/models/datasource.py,sha256=nLKmyA8mQ832ulT7mvc6B6MfNoepOU7T-qSQ6QeTqqA,6371
 asktable/models/message.py,sha256=4bIt5VTBXvH5iQYb5_LoOIIbbNEkjmUsLfkjx4Il7-M,1264
 asktable/models/run.py,sha256=xf4oNReawEmQk0rmYn-uWPu_zkZD7ws1-77bOfUWYTw,878
 atcommon/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 atcommon/tools.py,sha256=s0C_ti20oi8HfeSuEn5Oo5hLY7Jjo0tlzi8hAcpyXyg,3352
-atcommon/version.py,sha256=NS1t7ZG209bf7LDUCxa8i-J9cnNUQBQuYWGdpzVi_-U,16
+atcommon/version.py,sha256=umQ1GgcfOyyJ-ctVYlUvRVGZ-30oMBO1-F5sIgF_OB0,16
 atcommon/exceptions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 atcommon/exceptions/client.py,sha256=WaVggqCBVXKC7d9iTZsNfFg1uj0jgzuYUbWrHy8mBME,1060
 atcommon/exceptions/server.py,sha256=BSlYmdfDasoAq6oK9fyGhws3EBPII_hkHpx_JQmMdAY,95
-atcommon/exceptions/server_base.py,sha256=1sQfYYvxfGQatSk59BNFqf91FhMoZG2n3UcunX2eAhA,1889
+atcommon/exceptions/server_base.py,sha256=Bae0oZrN30QJozYY8sq4BwGYJA75Berq7h7z2Db6XhY,1979
 atcommon/exceptions/server_plugins.py,sha256=MqQgXsGHUn0JB3EAos1vlf8SLjUMNGXAY7lcBKSA_8c,589
 atcommon/models/__init__.py,sha256=QDsebmmUAHCKrMs789lDMt9HU9DR0kH-TGnE1CtW9kU,466
 atcommon/models/base.py,sha256=UVM9dKL22-k4k44H6DYQeNIe35vJ1Vg0ppGDZiVDiIU,731
 atcommon/models/bi.py,sha256=77HEtXOEj2tJwXe34s5Shsu4LWDihxAols8Rcz5cOFU,2344
 atcommon/models/chat.py,sha256=Si_eo8H8h_NtIOc76qhXoYcHp_tPMavud2sEnUXEejo,1069
 atcommon/models/datasource.py,sha256=WXYeAYpk_kLNp0sEDs0MJhAogn8VSjGuS7nenRpbCV0,682
 atcommon/models/meta.py,sha256=koGi9LvRdBskdblTtgbUpbF2lIThEbCVr-v27vZ_2JA,21682
-asktable-0.13.2.dist-info/METADATA,sha256=U4bSW3OZcA5moUWOGVi4YD-jwd9pTWbUpwYYM7uR06g,8285
-asktable-0.13.2.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
-asktable-0.13.2.dist-info/entry_points.txt,sha256=OS7zXFo5f2wYttNLFf6EScGBaN_2XtYbV_Fl_C3RhY8,47
-asktable-0.13.2.dist-info/top_level.txt,sha256=j_dz8lioIJZMGAy7UUdXv0ytGGhh8HFsGhSXaULxT4M,18
-asktable-0.13.2.dist-info/RECORD,,
+asktable-0.13.3.dist-info/METADATA,sha256=YZff2_vOv11ZSZmLwJyOcOGLxZYJES2iVOeIH7Z2J4U,8309
+asktable-0.13.3.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
+asktable-0.13.3.dist-info/entry_points.txt,sha256=OS7zXFo5f2wYttNLFf6EScGBaN_2XtYbV_Fl_C3RhY8,47
+asktable-0.13.3.dist-info/top_level.txt,sha256=j_dz8lioIJZMGAy7UUdXv0ytGGhh8HFsGhSXaULxT4M,18
+asktable-0.13.3.dist-info/RECORD,,
```

