# Comparing `tmp/txdpy-7.5.4.tar.gz` & `tmp/txdpy-7.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\86186\Desktop\?????\txdpy\txdpy\dist\.tmp-69rbhw23\txdpy-7.5.4.tar", last modified: Thu Mar 21 04:48:37 2024, max compression
+gzip compressed data, was "C:\Users\86186\Desktop\?????\txdpy\txdpy\dist\.tmp-axa54got\txdpy-7.6.5.tar", last modified: Tue Apr  2 01:39:48 2024, max compression
```

## Comparing `txdpy-7.5.4.tar` & `txdpy-7.6.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 04:48:37.000000 txdpy-7.5.4/
--rw-rw-rw-   0        0        0       71 2024-03-21 04:48:37.000000 txdpy-7.5.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-03-21 04:48:37.000000 txdpy-7.5.4/setup.cfg
--rw-rw-rw-   0        0        0      346 2024-03-21 04:48:25.000000 txdpy-7.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-21 04:48:37.000000 txdpy-7.5.4/txdpy/
--rw-rw-rw-   0        0        0    39935 2024-03-20 06:17:21.000000 txdpy-7.5.4/txdpy/URLjoin.py
--rw-rw-rw-   0        0        0     2736 2024-03-20 06:17:21.000000 txdpy-7.5.4/txdpy/__init__.py
--rw-rw-rw-   0        0        0    26828 2024-03-21 04:44:52.000000 txdpy-7.5.4/txdpy/bk_179.py
--rw-rw-rw-   0        0        0     3854 2024-03-20 06:17:21.000000 txdpy-7.5.4/txdpy/easyreq.py
--rw-rw-rw-   0        0        0     3245 2024-03-20 06:17:21.000000 txdpy-7.5.4/txdpy/excel_easy.py
--rw-rw-rw-   0        0        0     2472 2024-03-20 06:17:21.000000 txdpy-7.5.4/txdpy/get_key.py
--rw-rw-rw-   0        0        0     1715 2024-03-20 06:17:21.000000 txdpy-7.5.4/txdpy/list_processing.py
--rw-rw-rw-   0        0        0     1515 2024-03-20 06:17:21.000000 txdpy-7.5.4/txdpy/lookup.py
--rw-rw-rw-   0        0        0     2674 2024-03-20 06:17:21.000000 txdpy-7.5.4/txdpy/progress_display.py
--rw-rw-rw-   0        0        0     6469 2024-03-20 06:17:21.000000 txdpy-7.5.4/txdpy/pytmysql.py
--rw-rw-rw-   0        0        0    11803 2024-03-20 06:48:51.000000 txdpy-7.5.4/txdpy/read_data.py
--rw-rw-rw-   0        0        0     3002 2024-03-20 06:17:21.000000 txdpy-7.5.4/txdpy/requests_operation.py
--rw-rw-rw-   0        0        0     2031 2024-03-20 06:17:21.000000 txdpy-7.5.4/txdpy/selenium_Firefox.py
--rw-rw-rw-   0        0        0      933 2024-03-20 06:17:21.000000 txdpy-7.5.4/txdpy/str_category.py
--rw-rw-rw-   0        0        0      742 2024-03-20 06:17:21.000000 txdpy-7.5.4/txdpy/text_similar.py
--rw-rw-rw-   0        0        0      623 2024-03-20 06:17:21.000000 txdpy-7.5.4/txdpy/translate.py
-drwxrwxrwx   0        0        0        0 2024-03-21 04:48:37.000000 txdpy-7.5.4/txdpy.egg-info/
--rw-rw-rw-   0        0        0       71 2024-03-21 04:48:37.000000 txdpy-7.5.4/txdpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2024-03-21 04:48:37.000000 txdpy-7.5.4/txdpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 04:48:37.000000 txdpy-7.5.4/txdpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2024-03-21 04:48:37.000000 txdpy-7.5.4/txdpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-21 04:48:37.000000 txdpy-7.5.4/txdpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 01:39:48.000000 txdpy-7.6.5/
+-rw-rw-rw-   0        0        0       71 2024-04-02 01:39:48.000000 txdpy-7.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-02 01:39:48.000000 txdpy-7.6.5/setup.cfg
+-rw-rw-rw-   0        0        0      360 2024-04-02 01:17:18.000000 txdpy-7.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 01:39:48.000000 txdpy-7.6.5/txdpy/
+-rw-rw-rw-   0        0        0    39935 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/URLjoin.py
+-rw-rw-rw-   0        0        0     2781 2024-03-25 09:27:18.000000 txdpy-7.6.5/txdpy/__init__.py
+-rw-rw-rw-   0        0        0    27547 2024-03-28 06:02:54.000000 txdpy-7.6.5/txdpy/bk_179.py
+-rw-rw-rw-   0        0        0     3854 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/easyreq.py
+-rw-rw-rw-   0        0        0     3232 2024-04-02 01:15:36.000000 txdpy-7.6.5/txdpy/excel_easy.py
+-rw-rw-rw-   0        0        0     2472 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/get_key.py
+-rw-rw-rw-   0        0        0     1715 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/list_processing.py
+-rw-rw-rw-   0        0        0     1515 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/lookup.py
+-rw-rw-rw-   0        0        0     2850 2024-03-22 06:06:06.000000 txdpy-7.6.5/txdpy/progress_display.py
+-rw-rw-rw-   0        0        0     6469 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/pytmysql.py
+-rw-rw-rw-   0        0        0    11803 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/read_data.py
+-rw-rw-rw-   0        0        0     3002 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/requests_operation.py
+-rw-rw-rw-   0        0        0     2031 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/selenium_Firefox.py
+-rw-rw-rw-   0        0        0      933 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/str_category.py
+-rw-rw-rw-   0        0        0      774 2024-03-26 02:45:24.000000 txdpy-7.6.5/txdpy/text_similar.py
+-rw-rw-rw-   0        0        0      623 2024-03-21 05:24:55.000000 txdpy-7.6.5/txdpy/translate.py
+drwxrwxrwx   0        0        0        0 2024-04-02 01:39:48.000000 txdpy-7.6.5/txdpy.egg-info/
+-rw-rw-rw-   0        0        0       71 2024-04-02 01:39:48.000000 txdpy-7.6.5/txdpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2024-04-02 01:39:48.000000 txdpy-7.6.5/txdpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 01:39:48.000000 txdpy-7.6.5/txdpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2024-04-02 01:39:48.000000 txdpy-7.6.5/txdpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-02 01:39:48.000000 txdpy-7.6.5/txdpy.egg-info/top_level.txt
```

### Comparing `txdpy-7.5.4/txdpy/URLjoin.py` & `txdpy-7.6.5/txdpy/URLjoin.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.5.4/txdpy/__init__.py` & `txdpy-7.6.5/txdpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __all__ = ['urljoin', 'headers_dict', 'PyMySQL', 'rl', 'si', 'liduel', 'param_dict',
            'is_num', 'is_Sletter', 'is_Bletter', 'is_letter', 'is_num_letter', 'is_chinese',
            'get_chinese', 'get_letter', 'get_Bletter', 'get_Sletter', 'get_Sletter', 'get_num', 'get_middle',
            'get_num_letter', 'webptablesl', 'req', 'dow_file', 'list_dupl', 'selenium_firefox', 'get_ssq','is_ssq',
            'excel_into_mysql', 'prurar_code', 'convert_pc', 'convert_kl', 'delete_flase_empty', 'txdavg', 'txdmin',
            'txdperc', 'QueryScoreRank', 'timer', 'exenla', 'getexcelth', 'prvadepl', 'read_excel',
            'ExtractEnrollmentLabels', 'sortedlbys', 'UpdateName', 'optstr','progbar','text_similar'
-           'Recognit_Data_Process','gen_excel','translate','ReadData','get_ms_name','get_code_name'
+           'Recognit_Data_Process','gen_excel','translate','ReadData','get_ms_name','get_code_name','unify_keys'
            # 'PyBloomFilter'
            ]
 
 from .URLjoin import urljoin
 from .requests_operation import headers_dict
 from .requests_operation import param_dict
 from .requests_operation import webptablesl
@@ -53,13 +53,14 @@
 from .bk_179 import prvadepl
 from .bk_179 import ExtractEnrollmentLabels
 from .bk_179 import UpdateName
 from .bk_179 import sortedlbys
 from .bk_179 import optstr
 from .bk_179 import get_ms_name
 from .bk_179 import get_code_name
+from .bk_179 import unify_keys
 from .excel_easy import read_excel
 from .excel_easy import gen_excel
 from .translate import translate
 from .read_data import ReadData
 from .progress_display import progbar
 from .text_similar import text_similar
```

### Comparing `txdpy-7.5.4/txdpy/bk_179.py` & `txdpy-7.6.5/txdpy/bk_179.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,23 +350,24 @@
 def exenla(major,maispb=False,return_string=False):
     """
     :param major:专业名称
     :param maispb:是否查找匹配标签
     :param return_string:返回字符串
     :return: 专业名称中的标签
     """
-    bqs={'招生标签':set([v for v in
-              ['联合培养', '中外合作', '校企合作', '国家专项', '高职本科', '地方专项', '高校专项', '联合办学',
-               '精准扶贫',
-               '少数民族', '民族班', '少民', '闽台', '优师', '公费', '订单', '双语', '定向', '预科'] if
-              v in major]),
-    '匹配标签': set([v for v in
-                       [] if
-                       v in major])
+    bqs={'招生标签':list(set([v for v in
+              ['联合培养', '中外合作', '校企合作', '国家专项', '高职本科', '地方专项', '高校专项', '联合办学','精准扶贫','少数民族', '民族班', '少民', '闽台', '优师', '公费', '订单', '双语', '定向', '预科']
+                if v in major and f'非{v}' not in major])),
+    '匹配标签': list(set([v for v in
+                       ['师范','苏区专项']
+                    if v in major and f'非{v}' not in major]))
      }
+    zhonhwaihezuo=re.search('中.合作',major)
+    if zhonhwaihezuo and '中外合作' not in bqs['招生标签']:
+        bqs['招生标签'].append('中外合作')
     if return_string:
         return '、'.join(bqs['招生标签'])
     return bqs if maispb else bqs['招生标签']
 
 #获取表头中字段名称索引，表头以列表形式传入
 def getexcelth(rowdatas0,ht):
     """
@@ -408,32 +409,33 @@
         :param major:专业名称
         :param batch:批次
         :param school_name:学校名称，学校名称中有“职业”关键字优先在职业本科查找专业名称信息
         :return:专业名称、专业名称逻辑代码、二级大类、二级大类逻辑代码、一级大类、一级大类逻辑代码
         """
         major_name = get_ms_name(major)[0]
         if '专科' in batch:
-            cengci = '专科'
+            return self.data.get('专科' + '_' + major_name, [None] * 6)
         else:
+            major_name = '本科预科班' if '预科' in major_name else major_name
+            mana = self.data.get('本科' + '_' + major_name)
+            if mana:
+                return mana
             if '职业' in school_name:
-                cengci = '职业本科'
-            else:
-                cengci = '本科'
-        major_name = '本科预科班' if '预科' in major_name else major_name
-        return self.data.get(cengci + '_' + major_name, [None] * 6)
+                return self.data.get('职业本科' + '_' + major_name, [None] * 6)
+        return [None] * 6
 
 #对列表中的多个列表以第某个元素进行排序
 def sortedlbys(lists,i,reverse=False):
     """
     :param lists:数据列表
     :param i:一维数据中基准索引
     :param reverse:排序方式，默认False，有小到大
     :return:排序后的数据列表
     """
-    sorted_lists = sorted(lists, key=lambda x: x[i], reverse=True)
+    sorted_lists = sorted(lists, key=lambda x: x[i], reverse=reverse)
     return sorted_lists
 
 class UpdateName():
     """
     更新院校名称和专业名称
     """
     def __init__(self):
@@ -521,8 +523,21 @@
     """
     判断是否为学校名称
     """
     re_string=re.search('([\u4e00-\u9fa5]+)',optstr(string))
     if re_string:
         re_string=re_string.group(1)
         if re_string.endswith('大学') or re_string.endswith('学院') or re_string.endswith('学校') or re_string.endswith('分校'):
-            return True
+            return True
+
+def unify_keys(ks):
+    """
+    统一表头字段名称
+    """
+    key_dict={x[0]: x[1] for x in ReadData('读取数据时表头字段统一化参考表').data[1:]}
+    for i,k1 in enumerate(ks):
+        for k2,ys in key_dict.items():
+            for y in ys.split(','):
+                if y==k1:
+                    ks[i]=k2
+                    break
+    return ks
```

### Comparing `txdpy-7.5.4/txdpy/easyreq.py` & `txdpy-7.6.5/txdpy/easyreq.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.5.4/txdpy/excel_easy.py` & `txdpy-7.6.5/txdpy/excel_easy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os.path
 from .pytmysql import PyMySQL
 import xlrd,xlsxwriter
 from .bk_179 import optstr
+from file_ls import ls
 from tqdm import tqdm
 
 def excel_into_mysql(file:str,host:str, password:str, database:str,bm:str,th_a=1,stat:int=0,port:int=3306, user:str='root',auto_add_key:bool=True):
     """
     :param file: 文件路径
     :param host: mysql地址
     :param password: mysql密码
@@ -72,21 +73,19 @@
 def read_excel(file_path,sheet_index=0):
     """
     :param file_path:文件路径或路径下第一个文件
     :param sheet_index:工作表索引默认第一个
     return:表格数据
     """
     if not file_path.endswith('.xlsx'):
-        file_paths=file_ls(file_path)
+        file_paths=ls(file_path)
         for path in file_paths:
             if path.endswith('.xlsx'):
                 file_path=path
                 break
+    from openpyxl import load_workbook
+    workbook = load_workbook(filename=file_path)
+    worksheet = workbook.worksheets[sheet_index]
     datas = []
-    import xlrd
-    # 打开Excel文件并获取工作表
-    workbook = xlrd.open_workbook(file_path)
-    worksheet = workbook.sheet_by_index(sheet_index)
-    # 遍历每一行数据
-    for i in range(worksheet.nrows):
-        datas.append([prvadepl(v) if type(v)==float else v for v in worksheet.row_values(i)])
+    for row in worksheet.iter_rows():
+        datas.append([prvadepl(cell.value) if isinstance(cell.value, float) else cell.value for cell in row])
     return datas
```

### Comparing `txdpy-7.5.4/txdpy/get_key.py` & `txdpy-7.6.5/txdpy/get_key.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.5.4/txdpy/list_processing.py` & `txdpy-7.6.5/txdpy/list_processing.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.5.4/txdpy/lookup.py` & `txdpy-7.6.5/txdpy/lookup.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.5.4/txdpy/progress_display.py` & `txdpy-7.6.5/txdpy/progress_display.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,21 +10,23 @@
     """
     监控任务进度
     :param ls: 可遍历对象
     """
     if isinstance(ls, collections.abc.Iterator):
         ls = [l for l in ls]#解决迭代对象
     len_ls=len(ls)
+    if not len_ls:
+        return
     decpla=len(str(len_ls))
     start_time=time()
     i=0
     for l in ls:
         if i != 0:
             already_use_time = (time()-start_time) or 0.000000001#已使用时间
-            remain_tasks=len_ls-i#剩余任务
+            remain_tasks = len_ls - i  # 剩余任务
             estimate_remain_time=already_use_time/i*remain_tasks#预估剩余时间
         else:
             i += 1
             yield l
             continue
         print("\033[92m"+
               f'总任务数：{len_ls}，'
@@ -36,14 +38,16 @@
               f'速度：{save_speed_decimal(i/already_use_time)}条/秒，'
               f'当前时间：{format_duration1(time())}，'
               f'预估完成时间：{format_duration1(time()+estimate_remain_time)}'
               +"\033[0m")
         i+=1
         yield l
     already_use_time = time() - start_time  # 已使用时间
+    remain_tasks = len_ls - i  # 剩余任务
+    estimate_remain_time = already_use_time / i * remain_tasks  # 预估剩余时间
     print("\033[92m" +
           f'总任务数：{len_ls}，'
           f'当前已完成任务数：{i}，'
           f'剩余任务数{remain_tasks}，'
           f'进度：{round(i * 100 / len_ls, decpla)}%，'
           f'已用时间：{format_duration2(already_use_time)}，'
           f'预估剩余时间：{format_duration2(estimate_remain_time)}，'
```

### Comparing `txdpy-7.5.4/txdpy/pytmysql.py` & `txdpy-7.6.5/txdpy/pytmysql.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.5.4/txdpy/read_data.py` & `txdpy-7.6.5/txdpy/read_data.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.5.4/txdpy/requests_operation.py` & `txdpy-7.6.5/txdpy/requests_operation.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.5.4/txdpy/selenium_Firefox.py` & `txdpy-7.6.5/txdpy/selenium_Firefox.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.5.4/txdpy/str_category.py` & `txdpy-7.6.5/txdpy/str_category.py`

 * *Files identical despite different names*

### Comparing `txdpy-7.5.4/txdpy/text_similar.py` & `txdpy-7.6.5/txdpy/text_similar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-import requests
+import requests,json
+from time import sleep
 
-def text_similar(text_1, text_2):
-    params = {"grant_type": "client_credentials", "client_id": "7eb6Ee3o8FLh9ce3ATX1MA1S",
+params = {"grant_type": "client_credentials", "client_id": "7eb6Ee3o8FLh9ce3ATX1MA1S",
               "client_secret": "O44grcUdKtKSXXAMTkgpoDamFeweeGy7"}
-    access_token = str(
-        requests.post("https://aip.baidubce.com/oauth/2.0/token", params=params).json().get("access_token"))
+access_token = str(
+    requests.post("https://aip.baidubce.com/oauth/2.0/token", params=params).json().get("access_token"))
 
+def text_similar(text_1, text_2):
+    sleep(.5)
     url = "https://aip.baidubce.com/rpc/2.0/nlp/v2/simnet?charset=&access_token=" + access_token
     payload = json.dumps({
         "text_1": text_1,
         "text_2": text_2
     })
     response = requests.request("POST", url, headers={'Content-Type': 'application/json', 'Accept': 'application/json'},
                                 data=payload)
```

### Comparing `txdpy-7.5.4/txdpy/translate.py` & `txdpy-7.6.5/txdpy/translate.py`

 * *Files identical despite different names*

