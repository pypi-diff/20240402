# Comparing `tmp/yunxiao-0.4.9.tar.gz` & `tmp/yunxiao-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.4.9.tar", last modified: Fri Mar 29 06:58:08 2024, max compression
+gzip compressed data, was "yunxiao-0.5.0.tar", last modified: Tue Apr  2 06:42:52 2024, max compression
```

## Comparing `yunxiao-0.4.9.tar` & `yunxiao-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 06:58:08.338245 yunxiao-0.4.9/
--rw-rw-rw-   0        0        0      509 2024-03-29 06:58:08.337246 yunxiao-0.4.9/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-02-29 10:36:23.000000 yunxiao-0.4.9/README.md
--rw-rw-rw-   0        0        0     1853 2024-03-28 10:02:07.000000 yunxiao-0.4.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 06:58:08.338245 yunxiao-0.4.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-29 06:58:08.325250 yunxiao-0.4.9/yunxiao/
--rw-rw-rw-   0        0        0       53 2024-02-29 10:36:23.000000 yunxiao-0.4.9/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    36396 2024-03-29 06:55:31.000000 yunxiao-0.4.9/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2024-03-29 06:58:08.336245 yunxiao-0.4.9/yunxiao.egg-info/
--rw-rw-rw-   0        0        0      509 2024-03-29 06:58:08.000000 yunxiao-0.4.9/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2024-03-29 06:58:08.000000 yunxiao-0.4.9/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 06:58:08.000000 yunxiao-0.4.9/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-29 06:58:08.000000 yunxiao-0.4.9/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-29 06:58:08.000000 yunxiao-0.4.9/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 06:42:52.940063 yunxiao-0.5.0/
+-rw-rw-rw-   0        0        0      509 2024-04-02 06:42:52.939063 yunxiao-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-02-29 10:36:23.000000 yunxiao-0.5.0/README.md
+-rw-rw-rw-   0        0        0     1944 2024-04-02 06:42:43.000000 yunxiao-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 06:42:52.940063 yunxiao-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 06:42:52.925162 yunxiao-0.5.0/yunxiao/
+-rw-rw-rw-   0        0        0       53 2024-02-29 10:36:23.000000 yunxiao-0.5.0/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    35501 2024-04-02 06:32:17.000000 yunxiao-0.5.0/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:42:52.938048 yunxiao-0.5.0/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0      509 2024-04-02 06:42:52.000000 yunxiao-0.5.0/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-04-02 06:42:52.000000 yunxiao-0.5.0/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 06:42:52.000000 yunxiao-0.5.0/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-02 06:42:52.000000 yunxiao-0.5.0/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-02 06:42:52.000000 yunxiao-0.5.0/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.4.9/pyproject.toml` & `yunxiao-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.4.9"
+version = "0.5.0"
 description = "An API SDK tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "sqkkyzx", email = "admin@sqkkyzx.com"},
 ]
 
 dependencies = ["requests"]
@@ -15,14 +15,15 @@
 [tool.poetry.dependencies]
 python = "^3.12"
 
 [tool.poetry.publish]
 repository = "pypi"
 
 [tool.poetry.changelog]
+"0.5.0" = "新增: '订单组详情'端点;\n改进: '账户明细'端点更改函数名"
 "0.4.9" = "新增: '账户明细'端点;\n改进: 尝试将会话重用"
 "0.4.8" = "修复: 因域名造成的远程服务不存在问题"
 "0.4.7" = "新增: 查询课消明细"
 "0.4.6" = "修复: 修复"
 "0.4.5" = "改进: 将token和cookie保存在对象内部，移除V3"
 "0.4.4" = "修复：回退到requests"
 "0.4.3" = "改进：使用支持http2的httpx模块替换requests\n移除：移除了预设的时间值"
```

### Comparing `yunxiao-0.4.9/yunxiao/yunxiao.py` & `yunxiao-0.5.0/yunxiao/yunxiao.py`

 * *Files 1% similar despite different names*

```diff
@@ -802,39 +802,28 @@
                 "confirmStatusList": [],
                 "phone": ""
             }
         )
 
     # 查询收支明细-账户明细
     @loop_pages()
-    def payments_query_record(self, page, size, startdate: str = "", enddate: str = "",
-                              display_invalid_order: bool = True, types: tuple = ()):
-        """
-        列出指定操作日期范围的所有订单记录
-        :param size: 分页查询，每页数量
-        :param page: 分页查询，起始页码
-        :param types: 收支类型：**0** 收费 **1** 转课 **2** 退费
-        :param display_invalid_order: 是否展示已作废订单
-        :param enddate: YY-MM-DD
-        :param startdate: YY-MM-DD
-        :return:
-        """
-
+    def payments_account_record(self, page, size, startdate: str = "", enddate: str = "", displayInvalidOrder=False,
+                                typeList: tuple = (), paymentAccountCustomIds: tuple = ()):
         return self.request(
             method="post",
             url=f"https://{self.host}/api/cs-pc-report/cs-report/reports/findPaymentAccountCustomRecord",
             json={
                 "_t_": timestamp(),
-                "paymentAccountCustomIds": [],
                 "page": {"pageNum": page, "pageSize": size},
                 "campusIds": self.campus,
                 "startTime": startdate,
                 "endTime": enddate,
-                "displayInvalidOrder": display_invalid_order,
-                "typeList": list(types)
+                "paymentAccountCustomIds": list(paymentAccountCustomIds),
+                "typeList": list(typeList),
+                "displayInvalidOrder": displayInvalidOrder
             }
         )
 
     # 取得收据信息
     def payments_query_receipt(self, orderinfo_id: int, payment_groupid: int) -> dict:
         """
         取得收据信息。
@@ -848,14 +837,25 @@
             params={
                 "orderInfoId": orderinfo_id,
                 "paymentGroupId": payment_groupid,
                 "_t_": timestamp()
             }
         )["data"]
 
+    # 查询指定订单组详情（APP接口）
+    def order_group_detil(self, orderinfo_id):
+        return self.request(
+            method="get",
+            url=f"https://{self.host}/apics-edu/orderInfo/get",
+            params={
+                "orderInfoId": orderinfo_id,
+                "_t_": timestamp()
+            }
+        )["data"]
+
     # 查询签单业绩
     @loop_pages("achievementBelongerDetailItems")
     def payments_query_achievements_datarange(self, page, size, startdate: str = "", enddate: str = "",
                                               teacher_ids: tuple = (), order_types: tuple = ()):
         """
         查询业绩归属，根据日期
         :param order_types: **0** 收费 **1** 转课 **2** 退费 **3** 结转
@@ -889,26 +889,7 @@
     # 查询招生来源
     def comefroms_query(self):
         return self.request(
             method="get",
             url=f"https://{self.host}/api/cs-crm/customField/get",
             params={"_t_": timestamp(), "customFieldId": "26118419"}
         )["data"]["selectItemList"]
-
-    @loop_pages()
-    def findPaymentAccountCustomRecord(self, page, size, startdate: str = "", enddate: str = "",
-                                       displayInvalidOrder=False, typeList: tuple = (),
-                                       paymentAccountCustomIds: tuple = ()):
-        return self.request(
-            method="post",
-            url=f"https://{self.host}/api/cs-pc-report/cs-report/reports/findPaymentAccountCustomRecord",
-            json={
-                "_t_": timestamp(),
-                "page": {"pageNum": page, "pageSize": size},
-                "campusIds": self.campus,
-                "startTime": startdate,
-                "endTime": enddate,
-                "paymentAccountCustomIds": list(paymentAccountCustomIds),
-                "typeList": list(typeList),
-                "displayInvalidOrder": displayInvalidOrder
-            }
-        )
```

