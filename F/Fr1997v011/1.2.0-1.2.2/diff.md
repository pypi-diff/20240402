# Comparing `tmp/Fr1997v011-1.2.0.tar.gz` & `tmp/Fr1997v011-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.2.0.tar", last modified: Sat Mar  9 07:58:06 2024, max compression
+gzip compressed data, was "Fr1997v011-1.2.2.tar", last modified: Tue Apr  2 02:58:55 2024, max compression
```

## Comparing `Fr1997v011-1.2.0.tar` & `Fr1997v011-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-09 07:58:06.010475 Fr1997v011-1.2.0/
-drwxrwxrwx   0        0        0        0 2024-03-09 07:58:06.002962 Fr1997v011-1.2.0/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-03-09 07:58:05.000000 Fr1997v011-1.2.0/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-03-09 07:58:05.000000 Fr1997v011-1.2.0/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-09 07:58:05.000000 Fr1997v011-1.2.0/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-09 07:58:05.000000 Fr1997v011-1.2.0/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-03-09 07:58:05.000000 Fr1997v011-1.2.0/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.2.0/LICENSE
--rw-rw-rw-   0        0        0      182 2024-03-09 07:58:06.009469 Fr1997v011-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-03-05 07:02:57.000000 Fr1997v011-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-09 07:58:06.003962 Fr1997v011-1.2.0/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.2.0/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-09 07:58:06.005962 Fr1997v011-1.2.0/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2023-10-09 02:29:18.000000 Fr1997v011-1.2.0/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   123673 2024-03-09 07:58:03.000000 Fr1997v011-1.2.0/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-03-09 07:58:06.007963 Fr1997v011-1.2.0/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.2.0/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-03-09 07:58:06.010475 Fr1997v011-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-03-09 07:58:03.000000 Fr1997v011-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 02:58:55.138230 Fr1997v011-1.2.2/
+drwxrwxrwx   0        0        0        0 2024-04-02 02:58:55.128719 Fr1997v011-1.2.2/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-04-02 02:58:55.000000 Fr1997v011-1.2.2/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-04-02 02:58:55.000000 Fr1997v011-1.2.2/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 02:58:55.000000 Fr1997v011-1.2.2/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-02 02:58:55.000000 Fr1997v011-1.2.2/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-04-02 02:58:55.000000 Fr1997v011-1.2.2/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-04-02 02:58:55.136230 Fr1997v011-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-03-26 06:16:58.000000 Fr1997v011-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 02:58:55.129719 Fr1997v011-1.2.2/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.2.2/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 02:58:55.132719 Fr1997v011-1.2.2/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2023-10-09 02:29:18.000000 Fr1997v011-1.2.2/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   126840 2024-04-02 02:58:52.000000 Fr1997v011-1.2.2/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-04-02 02:58:55.135230 Fr1997v011-1.2.2/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.2.2/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 02:58:55.138230 Fr1997v011-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-04-02 02:56:58.000000 Fr1997v011-1.2.2/setup.py
```

### Comparing `Fr1997v011-1.2.0/LICENSE` & `Fr1997v011-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.2.0/README.md` & `Fr1997v011-1.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.1.9.tar.gz
+pip install dist/Fr1997v011-1.2.1.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.2.0/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.2.2/fr1997_mode/mode_func/all_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import redis
 import pymysql
 import random
 import hashlib
 import requests
 import ctypes
 import struct
+import base64
 import memcache  # pip install python-memcached
 from elasticsearch import Elasticsearch  # ES
 from concurrent.futures import ThreadPoolExecutor  # 线程次
 from pypinyin import pinyin, Style  # 汉字转拼音
 
 import execjs  # pip install PyExecJS
 from urllib import parse  # 三位
@@ -34,15 +35,15 @@
 """
 
 """
     配置文件
         所有配置在这个地方读取 
         使用内存缓存机制 memcache
         没有读取到内存中的配置，这个包相当于不能用
-    
+    pip3 cache purge
     pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple Fr1997v011==1.1.9
 """
 
 
 # 存储内存数据
 def cache_set(key, data, save_time=None):
     mc = memcache.Client(['127.0.0.1:11211'], debug=True)
@@ -841,14 +842,31 @@
                 'last_up': int(file_info.st_mtime),
                 'created': int(file_info.st_ctime),
                 'is_directory': os.path.isdir(file_path),
                 'is_file': os.path.isfile(file_path),
             })
         return all_file_info
 
+    # dict 多重数据结构提取web链接
+    def dict_web_url(self, data):
+        links = []
+
+        if isinstance(data, dict):
+            for value in data.values():
+                links.extend(self.dict_web_url(value))
+        elif isinstance(data, list):
+            for item in data:
+                links.extend(self.dict_web_url(item))
+        elif isinstance(data, str):
+            # 使用正则表达式查找所有链接
+            found_links = re.findall(r'https?://\S+', data)
+            links.extend(found_links)
+
+        return links
+
 
 # 采集
 class SpiderJike:
     # >>>>----------------       spider_func         ----------------<<<<<
     # ai api2d 余额查询
     @staticmethod
     def ai_api2d_token_count():
@@ -1070,14 +1088,25 @@
 
         # 视频下载地址
         try:
             download_addr_url_list = res_data['video']['download_addr']['url_list']
         except:
             download_addr_url_list = []
 
+        # mp3 url
+        try:
+            mp3_url_list = res_data['music']['play_url']['url_list']
+
+            if '.mp3' in res_data['music']['play_url']['url_list'][0]:
+                pass
+            else:
+                mp3_url_list = []
+        except:
+            mp3_url_list = []
+
         # author_head
         author_head = res_data['author']['avatar_thumb']['url_list'][0]
         base_ret_data['video_id'] = res_data["aweme_id"]
         base_ret_data['v_id'] = v_id
         base_ret_data['title'] = desc
         base_ret_data['video_cover'] = cover_img
 
@@ -1092,14 +1121,15 @@
         base_ret_data['create_date'] = create_time
         base_ret_data['release_time'] = release_time
         base_ret_data['nickname'] = nickname
         base_ret_data['author_head'] = author_head
         base_ret_data['describe'] = describe
 
         base_ret_data['download_addr_url_list'] = download_addr_url_list
+        base_ret_data['mp3_url_list'] = mp3_url_list
 
         if tp == 'django_video_info':
             return {
                 "video_id": res_data["aweme_id"],
                 "v_id": v_id,
                 'video_description': desc,
                 'video_cover': cover_img,
@@ -1362,15 +1392,15 @@
             data_data = response.json
             user_detail = data_data.get('user')
 
             data_json = self.analysis_douyin_user(user_detail)  # 数据获取
             return data_json
 
     # 【api】 视频详情
-    def api_douyin_video(self, video_id):
+    def api_douyin_video(self, video_id, use_proxies=1):
         cookies = mode_pro.ttwid_cookie_tt(get_cache=1)
         headers = {
             "authority": "www.douyin.com",
             "pragma": "no-cache",
             "cache-control": "no-cache",
             "accept": "application/json, text/plain, */*",
             "user-agent": config_dict['base_ua'],
@@ -1378,15 +1408,18 @@
             "accept-language": "zh-CN,zh;q=0.9",
             'cookie': f'msToken={mode_pro.get_douyin_token(107)};odin_tt=;passport_csrf_token=1;{random.choice(cookies)}'
         }
 
         url = f'https://www.douyin.com/aweme/v1/web/aweme/detail/?device_platform=webapp&aid=6383&channel=channel_pc_web&aweme_id={video_id}&pc_client_type=1&version_code=190500&version_name=19.5.0'
         url = mode_pro.get_xbogus_new_gbk(url, config_dict['base_ua'])
         try:
-            response = HttpJike.get(url=url, headers=headers, proxies=HttpJike.proxies_choose())
+            if use_proxies:
+                response = HttpJike.get(url=url, headers=headers, proxies=HttpJike.proxies_choose())
+            else:
+                response = HttpJike.get(url=url, headers=headers)
             if response.status_code == 200:
                 data_data = response.json
 
                 # 是否存在
                 if '因作品权限或已被删除，无法观看，去看看其他作品吧' in str(data_data):
                     return {'aweme_type': 1, 'is_alive': 0, 'err': 'del'}
 
@@ -1536,17 +1569,17 @@
         return save_data
 
     # 【数据解析】 用户详情
     def analysis_douyin_user(self, res_data):
         aweme_count = res_data['aweme_count']
         follower_count = res_data['follower_count']
         nickname = res_data['nickname']
-        unique_id = res_data.get('unique_id','')
+        unique_id = res_data.get('unique_id', '')
         if len(unique_id) == 0:
-            unique_id = res_data.get('short_id','')
+            unique_id = res_data.get('short_id', '')
         user_id = res_data['uid']
         total_favorited = res_data['total_favorited']
         author_head = res_data['avatar_168x168']['url_list'][0]
         introduction = mode_text.word_change(res_data['signature'])
         # 用户类型 1=个人  2=黄V  3=蓝V  4=注销  5=未知
         user_type = 5
         organization = ''
@@ -1947,14 +1980,30 @@
                     fields = list(save_data[0].keys())
                     placeholders = ', '.join(f'%({i})s' for i in fields)
                     fields_str = ','.join(fields)
                     sql_inserts = f"INSERT ignore INTO {table} ({fields_str}) values({placeholders})"
                     n = cursor.executemany(sql_inserts, save_data)
                     conn.commit()
                     return n
+                elif method == 'insert_creat_all' or method == 'isc':
+                    pass
+                    # # 根据索引插入或更新 没有索引最后 没有更新默认
+                    # key = kwargs.get('key')
+                    # if key in None:
+                    #
+                    # update_key = []
+                    #
+                    # fields = list(save_data[0].keys())
+                    # placeholders = ', '.join(f'%({i})s' for i in fields)
+                    # fields_str = ','.join(fields)
+                    # sql_inserts = f"INSERT INTO {table} ({fields_str}) values({placeholders}) on DUPLICATE {key} update"
+                    # return sql_inserts
+                    # # n = cursor.executemany(sql_inserts, save_data)
+                    # # conn.commit()
+                    # # return n
                 elif method == 'table_exist' or method == 'te':
                     # 查询 表是否存在
                     return cursor.execute(sql_table_exist)
                 elif method == 'create_table' or method == 'tc':  # 创建一个表
                     table_exist = cursor.execute(sql_table_exist)
                     if table_exist:
                         del_and_create = kwargs.get('del_and_create', 0)
@@ -2061,15 +2110,14 @@
         response = es.search(
             index=table,
             body=body
         )
         _shards = response.get('_shards')
         if _shards:
             successful = _shards.get('successful')
-            print(successful)
             if successful > 0:
                 value = response.get('hits')['total']['value']
                 hits_list = response.get('hits')['hits']
                 print(f'总个数:{value} 取出:{len(hits_list)}')
                 if ret_num == 0:
                     return hits_list
                 else:
@@ -2099,15 +2147,14 @@
         response = es.search(
             index=table,
             body=body
         )
         _shards = response.get('_shards')
         if _shards:
             successful = _shards.get('successful')
-            print(successful)
             if successful > 0:
                 value = response.get('hits')['total']['value']
                 hits_list = response.get('hits')['hits']
                 print(f'总个数:{value} 取出:{len(hits_list)}')
                 if ret_num == 0:
                     return hits_list
                 else:
@@ -2375,15 +2422,15 @@
                     "track_total_hits": 'true',
                 }
                 response = es.search(index=table, body=body)
                 if response:
                     _shards = response.get('_shards')
                     if _shards:
                         successful = _shards.get('successful')
-                        if successful == 1:
+                        if successful > 0:
                             # 数据集
                             hits_list = response.get('hits')['hits']
                             print('本次取出符合条件的总数:', len(hits_list))
 
                             for index_x, i in enumerate(hits_list):
                                 _s = i['_source']
                                 _id = i['_id']
@@ -3177,15 +3224,14 @@
 
     # 获取信息
     def get_myself_info(self):
         return self.fr1997_config_dict
 
     # 获取出生年龄等信息
     def get_age_info(self):
-        print(self.fr1997_config_dict)
         name = self.fr1997_config_dict['name']
         return name
 
 
 mode_feishu = Feishu()  # 飞书app api
 mode_time = TimeJike()  # 时间处理
 mode_text = TextJike()  # 文本处理
@@ -3196,7 +3242,40 @@
 mode_pros = ModeStatic()  # 其它函数
 mode_cos = Cos()  # cos
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
 
 mode_pro = ModeFunc()  # main
 
+# def fast_douyin_video_text():
+#     text = 'https://www.douyin.com/search/%E8%B6%B3%E7%90%83?modal_id=7105766792102038821&type=video'
+#     video_id = mode_douyin.get_video_id(text)  # 获取video_id
+#     video_info = mode_douyin.api_douyin_video(video_id, use_proxies=1)
+#
+#     """
+#         如果视频详细自带 mp3格式可以直接转
+#     """
+#
+#     if video_info:
+#         print(video_info)
+#         mp3_url_list = video_info['mp3_url_list']
+#         print(mp3_url_list)
+#
+#         if mp3_url_list:
+#             mp3_url = mp3_url_list[0]
+#             print(mp3_url_list)
+#
+#         #     headers = {
+#         #         'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36 Edg/122.0.0.0',
+#         #     }
+#         #     mp3_url_bs64 = base64.b64encode(mp3_url.encode()).decode()
+#         #     response_text = requests.get(url=f'http://49.234.188.96:7677/hello/{mp3_url_bs64}', headers=headers)
+#         #     print(response_text.text)
+#         # else:
+#         #     wav_url = video_info['download_addr_url_list'][0]
+#         #     print(wav_url)
+#         #     # response = requests.get(wav_url)
+#         #     # print(response.content)
+#
+#
+# fast_douyin_video_text()
+
```

