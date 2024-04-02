# Comparing `tmp/ip_check-1.5.0-py3-none-any.whl.zip` & `tmp/ip_check-1.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 33868 bytes, number of entries: 23
+Zip file size: 34001 bytes, number of entries: 23
 -rw-rw-r--  2.0 unx      383 b- defN 24-Mar-19 08:00 ipcheck/__init__.py
--rw-rw-r--  2.0 unx     6297 b- defN 24-Apr-01 02:03 ipcheck/geoinfo.py
+-rw-rw-r--  2.0 unx     6609 b- defN 24-Apr-02 02:06 ipcheck/geoinfo.py
 -rw-rw-r--  2.0 unx    10424 b- defN 24-Mar-27 01:44 ipcheck/main.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Mar-14 08:04 ipcheck/app/__init__.py
 -rw-rw-r--  2.0 unx      726 b- defN 24-Mar-14 08:04 ipcheck/app/base_config.py
 -rw-rw-r--  2.0 unx      388 b- defN 24-Mar-14 08:04 ipcheck/app/common_config.py
 -rw-rw-r--  2.0 unx     6052 b- defN 24-Mar-25 07:07 ipcheck/app/config.py
 -rw-rw-r--  2.0 unx     1773 b- defN 24-Mar-19 08:00 ipcheck/app/default_config.py
 -rw-rw-r--  2.0 unx     1841 b- defN 24-Mar-27 06:11 ipcheck/app/gen_ip_utils.py
@@ -12,14 +12,14 @@
 -rw-rw-r--  2.0 unx     2546 b- defN 24-Mar-14 08:04 ipcheck/app/rtt_test.py
 -rw-rw-r--  2.0 unx      223 b- defN 24-Mar-14 08:04 ipcheck/app/rtt_test_config.py
 -rw-rw-r--  2.0 unx     5565 b- defN 24-Mar-19 08:00 ipcheck/app/speed_test.py
 -rw-rw-r--  2.0 unx      223 b- defN 24-Mar-14 08:04 ipcheck/app/speed_test_config.py
 -rw-rw-r--  2.0 unx     2585 b- defN 24-Apr-01 02:04 ipcheck/app/utils.py
 -rw-rw-r--  2.0 unx     3796 b- defN 24-Mar-27 03:30 ipcheck/app/valid_test.py
 -rw-rw-r--  2.0 unx      303 b- defN 24-Mar-14 08:04 ipcheck/app/valid_test_config.py
--rw-rw-r--  2.0 unx    35148 b- defN 24-Apr-01 02:25 ip_check-1.5.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     5235 b- defN 24-Apr-01 02:25 ip_check-1.5.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-01 02:25 ip_check-1.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      201 b- defN 24-Apr-01 02:25 ip_check-1.5.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-01 02:25 ip_check-1.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1864 b- defN 24-Apr-01 02:25 ip_check-1.5.0.dist-info/RECORD
-23 files, 87135 bytes uncompressed, 30858 bytes compressed:  64.6%
+-rw-rw-r--  2.0 unx    35148 b- defN 24-Apr-02 02:12 ip_check-1.5.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5266 b- defN 24-Apr-02 02:12 ip_check-1.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-02 02:12 ip_check-1.5.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      201 b- defN 24-Apr-02 02:12 ip_check-1.5.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-02 02:12 ip_check-1.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1864 b- defN 24-Apr-02 02:12 ip_check-1.5.1.dist-info/RECORD
+23 files, 87478 bytes uncompressed, 30991 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -45,26 +45,26 @@
 
 Filename: ipcheck/app/valid_test.py
 Comment: 
 
 Filename: ipcheck/app/valid_test_config.py
 Comment: 
 
-Filename: ip_check-1.5.0.dist-info/LICENSE
+Filename: ip_check-1.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: ip_check-1.5.0.dist-info/METADATA
+Filename: ip_check-1.5.1.dist-info/METADATA
 Comment: 
 
-Filename: ip_check-1.5.0.dist-info/WHEEL
+Filename: ip_check-1.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: ip_check-1.5.0.dist-info/entry_points.txt
+Filename: ip_check-1.5.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ip_check-1.5.0.dist-info/top_level.txt
+Filename: ip_check-1.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ip_check-1.5.0.dist-info/RECORD
+Filename: ip_check-1.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipcheck/geoinfo.py

```diff
@@ -13,16 +13,16 @@
 
 GEO2CITY_DB_NAME = 'GeoLite2-City.mmdb'
 GEO2ASN_DB_NAME = 'GeoLite2-ASN.mmdb'
 GEO2CITY_DB_PATH = os.path.join(os.path.dirname(__file__), GEO2CITY_DB_NAME)
 GEO2ASN_DB_PATH = os.path.join(os.path.dirname(__file__), GEO2ASN_DB_NAME)
 GEO_CONFIG_PATH = os.path.join(os.path.dirname(__file__), 'geo.ini')
 GEO_DEFAULT_CONFIG = '''[common]
-# 下载使用代理
-proxy = host:port
+# 下载使用代理,格式为 protocal://host:port, 如: socks5://127.0.0.1:1080
+proxy =
 # asn 数据库下载地址
 db_asn_url = xxxx
 # city 数据库下载地址
 db_city_url = yyyy
 '''
 
 def download_geo_db(url :str, path:str, proxy=None):
@@ -133,19 +133,26 @@
         path = GEO2ASN_DB_PATH
     if path:
         download_geo_db(url, path, proxy)
     else:
         print('请输入包含{} 或 {} 的url'.format(GEO2CITY_DB_NAME, GEO2ASN_DB_NAME))
 
 def parse_geo_config():
+    def get_option_safely(section: str, option: str, default_value=None):
+        nonlocal parser
+        if parser.has_option(section, option):
+            return parser.get(section, option)
+        else:
+            return default_value
+
     parser = configparser.ConfigParser()
     parser.read(GEO_CONFIG_PATH, 'utf-8')
-    db_asn_url = parser.get('common', 'db_asn_url')
-    db_city_url = parser.get('common', 'db_city_url')
-    proxy = parser.get('common', 'proxy')
+    db_asn_url = get_option_safely('common', 'db_asn_url')
+    db_city_url = get_option_safely('common', 'db_city_url')
+    proxy = get_option_safely('common', 'proxy')
     return db_asn_url, db_city_url, proxy
 
 def check_or_gen_def_config():
     if not os.path.exists(GEO_CONFIG_PATH):
         print('警告: 配置文件不存在，正在生成默认配置... ...')
         write_file(GEO_DEFAULT_CONFIG, GEO_CONFIG_PATH)
         print('配置文件已生成位于 {}, 请按需要修改！'.format(GEO_CONFIG_PATH))
```

## Comparing `ip_check-1.5.0.dist-info/LICENSE` & `ip_check-1.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ip_check-1.5.0.dist-info/METADATA` & `ip_check-1.5.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: ip-check
-Version: 1.5.0
+Version: 1.5.1
 Summary: Powerful cdn network speed test utils.
 Author: nobitaqaq
 Author-email: xiaoleigs@gmail.com
 Keywords: cdn,speed test,network speed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geoip2
 Requires-Dist: ipaddress (~=1.0.23)
 Requires-Dist: requests
+Requires-Dist: requests[socks]
 Requires-Dist: tcppinglib (~=2.0.3)
 Requires-Dist: tqdm
 Requires-Dist: urllib3 (~=1.26.15)
 
 # ip-check
 
 高效的cdn 测速工具，用于ip 优选。
```

## Comparing `ip_check-1.5.0.dist-info/RECORD` & `ip_check-1.5.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ipcheck/__init__.py,sha256=mjRHWAo73u50fxwseCRsTdvj9pPNZuTmsKW8Qpj-cNk,383
-ipcheck/geoinfo.py,sha256=ZFOOiXahWy97noLuaB-mrrpXIIC0j3F85H8xX8QPQgY,6297
+ipcheck/geoinfo.py,sha256=s90kPWJfrJQB1AT5zOfhcunH9h_HD5FQ6FyDfY1baJ0,6609
 ipcheck/main.py,sha256=qKfWwjWhUiNC6ZBM4ijPMZlpzBoOArl7qU3riVOiZoA,10424
 ipcheck/app/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ipcheck/app/base_config.py,sha256=PxNW4PXHagvULNc9FgDwMtu7aCn91RYx2SqBYd4-nd4,726
 ipcheck/app/common_config.py,sha256=s5WjPy45UhxBgymYgZRaQugaSvxBM-96_PXUUa7Pc9U,388
 ipcheck/app/config.py,sha256=_vvb-xuD7R2rR6wqEVWCBDtOeIuf-bMlZiexKu7RmZo,6052
 ipcheck/app/default_config.py,sha256=7OP6pibA78-xkmVGZ4kLsmWzV8fKRff8bCXd9sceFPU,1773
 ipcheck/app/gen_ip_utils.py,sha256=8jOj7jpn8M2-eMxd6SrdZyuH4_xUwYTtY3ji-MWKkjY,1841
@@ -11,13 +11,13 @@
 ipcheck/app/rtt_test.py,sha256=d1_iC3OFeqBAFqqHBdRN_IH5jlRgtd5USn0vV0_CM8M,2546
 ipcheck/app/rtt_test_config.py,sha256=PK7M7uLst4Zi3v2DgKA8rfpZsXIRnwfTxYa12bPDeb8,223
 ipcheck/app/speed_test.py,sha256=b_YGCGIZOhwD1A1MpjUFb9CHYFKlLwodT9S7ZHYGzdg,5565
 ipcheck/app/speed_test_config.py,sha256=Ji1jUEqSjAIqkzUzeE1BBHPfoJ2E-JeG36DJiHJ3CYA,223
 ipcheck/app/utils.py,sha256=kyWjI6bARGJHlJUmkU1ZQ2wwchl98XLMd87UzZDvdPE,2585
 ipcheck/app/valid_test.py,sha256=UDA1mU7JTV0mwk0vYzjW0Y069jtArGVhv9lx3SRVAGQ,3796
 ipcheck/app/valid_test_config.py,sha256=46CI8Qs8Ldfn43tfQZs_71H8d78AunJTc1kb7ib15ug,303
-ip_check-1.5.0.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
-ip_check-1.5.0.dist-info/METADATA,sha256=A34KjZR_VqlMzvAhL7JK7Ggd90BY0Y0BxvAe-c7H8uc,5235
-ip_check-1.5.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-ip_check-1.5.0.dist-info/entry_points.txt,sha256=LbstGY5z6sejWLCwyd9pTq4qRdfCsligLhJHjwp-Pd0,201
-ip_check-1.5.0.dist-info/top_level.txt,sha256=24binHFMOV_-4WIWZrtgRz4y7uY3vUxlJBq2UXMMfvY,8
-ip_check-1.5.0.dist-info/RECORD,,
+ip_check-1.5.1.dist-info/LICENSE,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
+ip_check-1.5.1.dist-info/METADATA,sha256=ZuTULQYpYZkJKqVIcGD9kN47Vg0km68t_dynFN0iMRU,5266
+ip_check-1.5.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+ip_check-1.5.1.dist-info/entry_points.txt,sha256=LbstGY5z6sejWLCwyd9pTq4qRdfCsligLhJHjwp-Pd0,201
+ip_check-1.5.1.dist-info/top_level.txt,sha256=24binHFMOV_-4WIWZrtgRz4y7uY3vUxlJBq2UXMMfvY,8
+ip_check-1.5.1.dist-info/RECORD,,
```

