# Comparing `tmp/wechatpayv3-1.2.8.tar.gz` & `tmp/wechatpayv3-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wechatpayv3-1.2.8.tar", last modified: Sun Dec  5 00:52:41 2021, max compression
+gzip compressed data, was "wechatpayv3-1.2.9.tar", last modified: Sun Dec  5 06:44:50 2021, max compression
```

## Comparing `wechatpayv3-1.2.8.tar` & `wechatpayv3-1.2.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2021-12-05 00:52:41.814546 wechatpayv3-1.2.8/
--rw-rw-rw-   0        0        0     1090 2021-08-15 06:33:57.000000 wechatpayv3-1.2.8/LICENSE
--rw-rw-rw-   0        0        0       17 2021-04-14 14:01:29.000000 wechatpayv3-1.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0    34484 2021-12-05 00:52:41.812548 wechatpayv3-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    33918 2021-12-03 01:31:34.000000 wechatpayv3-1.2.8/README.md
--rw-rw-rw-   0        0        0       42 2021-12-05 00:52:41.815546 wechatpayv3-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0      839 2021-12-05 00:49:31.000000 wechatpayv3-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-12-05 00:52:41.785546 wechatpayv3-1.2.8/wechatpayv3/
--rw-rw-rw-   0        0        0     9397 2021-11-23 05:07:43.000000 wechatpayv3-1.2.8/wechatpayv3/__init__.py
--rw-rw-rw-   0        0        0     5126 2021-11-19 09:11:25.000000 wechatpayv3-1.2.8/wechatpayv3/apply4subject.py
--rw-rw-rw-   0        0        0     6793 2021-11-19 09:11:42.000000 wechatpayv3-1.2.8/wechatpayv3/applyment.py
--rw-rw-rw-   0        0        0     3543 2021-11-04 14:11:53.000000 wechatpayv3-1.2.8/wechatpayv3/businesscircle.py
--rw-rw-rw-   0        0        0     7124 2021-11-23 05:07:57.000000 wechatpayv3-1.2.8/wechatpayv3/complaint.py
--rw-rw-rw-   0        0        0     9517 2021-11-20 01:53:12.000000 wechatpayv3-1.2.8/wechatpayv3/core.py
--rw-rw-rw-   0        0        0     4137 2021-11-29 08:38:17.000000 wechatpayv3-1.2.8/wechatpayv3/ecommerce.py
--rw-rw-rw-   0        0        0     3945 2021-11-19 09:12:07.000000 wechatpayv3-1.2.8/wechatpayv3/goldplan.py
--rw-rw-rw-   0        0        0    49969 2021-12-05 00:47:07.000000 wechatpayv3-1.2.8/wechatpayv3/marketing.py
--rw-rw-rw-   0        0        0     2042 2021-09-17 01:10:30.000000 wechatpayv3-1.2.8/wechatpayv3/media.py
--rw-rw-rw-   0        0        0     1351 2021-11-19 09:24:44.000000 wechatpayv3-1.2.8/wechatpayv3/merchantrisk.py
--rw-rw-rw-   0        0        0     9859 2021-11-04 14:12:07.000000 wechatpayv3-1.2.8/wechatpayv3/parking.py
--rw-rw-rw-   0        0        0    23818 2021-11-04 02:22:51.000000 wechatpayv3-1.2.8/wechatpayv3/payscore.py
--rw-rw-rw-   0        0        0    25781 2021-11-19 02:17:50.000000 wechatpayv3-1.2.8/wechatpayv3/profitsharing.py
--rw-rw-rw-   0        0        0     6134 2021-11-22 01:30:55.000000 wechatpayv3-1.2.8/wechatpayv3/smartguide.py
--rw-rw-rw-   0        0        0    17585 2021-11-04 14:12:15.000000 wechatpayv3-1.2.8/wechatpayv3/transaction.py
--rw-rw-rw-   0        0        0      298 2021-09-15 02:45:47.000000 wechatpayv3-1.2.8/wechatpayv3/type.py
--rw-rw-rw-   0        0        0     3941 2021-10-03 03:21:32.000000 wechatpayv3-1.2.8/wechatpayv3/utils.py
-drwxrwxrwx   0        0        0        0 2021-12-05 00:52:41.806552 wechatpayv3-1.2.8/wechatpayv3.egg-info/
--rw-rw-rw-   0        0        0    34484 2021-12-05 00:52:41.000000 wechatpayv3-1.2.8/wechatpayv3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      658 2021-12-05 00:52:41.000000 wechatpayv3-1.2.8/wechatpayv3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-05 00:52:41.000000 wechatpayv3-1.2.8/wechatpayv3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2021-12-05 00:52:41.000000 wechatpayv3-1.2.8/wechatpayv3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-12-05 00:52:41.000000 wechatpayv3-1.2.8/wechatpayv3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-12-05 06:44:50.109809 wechatpayv3-1.2.9/
+-rw-rw-rw-   0        0        0     1090 2021-08-15 06:33:57.000000 wechatpayv3-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0       17 2021-04-14 14:01:29.000000 wechatpayv3-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    34484 2021-12-05 06:44:50.106810 wechatpayv3-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    33918 2021-12-03 01:31:34.000000 wechatpayv3-1.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2021-12-05 06:44:50.110810 wechatpayv3-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      839 2021-12-05 06:41:08.000000 wechatpayv3-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-12-05 06:44:50.080818 wechatpayv3-1.2.9/wechatpayv3/
+-rw-rw-rw-   0        0        0     9397 2021-11-23 05:07:43.000000 wechatpayv3-1.2.9/wechatpayv3/__init__.py
+-rw-rw-rw-   0        0        0     5126 2021-11-19 09:11:25.000000 wechatpayv3-1.2.9/wechatpayv3/apply4subject.py
+-rw-rw-rw-   0        0        0     6793 2021-11-19 09:11:42.000000 wechatpayv3-1.2.9/wechatpayv3/applyment.py
+-rw-rw-rw-   0        0        0     3543 2021-11-04 14:11:53.000000 wechatpayv3-1.2.9/wechatpayv3/businesscircle.py
+-rw-rw-rw-   0        0        0     7124 2021-11-23 05:07:57.000000 wechatpayv3-1.2.9/wechatpayv3/complaint.py
+-rw-rw-rw-   0        0        0     9517 2021-11-20 01:53:12.000000 wechatpayv3-1.2.9/wechatpayv3/core.py
+-rw-rw-rw-   0        0        0     4137 2021-11-29 08:38:17.000000 wechatpayv3-1.2.9/wechatpayv3/ecommerce.py
+-rw-rw-rw-   0        0        0     3945 2021-11-19 09:12:07.000000 wechatpayv3-1.2.9/wechatpayv3/goldplan.py
+-rw-rw-rw-   0        0        0    49969 2021-12-05 00:47:07.000000 wechatpayv3-1.2.9/wechatpayv3/marketing.py
+-rw-rw-rw-   0        0        0     2042 2021-09-17 01:10:30.000000 wechatpayv3-1.2.9/wechatpayv3/media.py
+-rw-rw-rw-   0        0        0     1351 2021-11-19 09:24:44.000000 wechatpayv3-1.2.9/wechatpayv3/merchantrisk.py
+-rw-rw-rw-   0        0        0     9859 2021-11-04 14:12:07.000000 wechatpayv3-1.2.9/wechatpayv3/parking.py
+-rw-rw-rw-   0        0        0    23818 2021-11-04 02:22:51.000000 wechatpayv3-1.2.9/wechatpayv3/payscore.py
+-rw-rw-rw-   0        0        0    25917 2021-12-05 06:43:17.000000 wechatpayv3-1.2.9/wechatpayv3/profitsharing.py
+-rw-rw-rw-   0        0        0     6134 2021-11-22 01:30:55.000000 wechatpayv3-1.2.9/wechatpayv3/smartguide.py
+-rw-rw-rw-   0        0        0    17585 2021-11-04 14:12:15.000000 wechatpayv3-1.2.9/wechatpayv3/transaction.py
+-rw-rw-rw-   0        0        0      298 2021-09-15 02:45:47.000000 wechatpayv3-1.2.9/wechatpayv3/type.py
+-rw-rw-rw-   0        0        0     3941 2021-10-03 03:21:32.000000 wechatpayv3-1.2.9/wechatpayv3/utils.py
+drwxrwxrwx   0        0        0        0 2021-12-05 06:44:50.101807 wechatpayv3-1.2.9/wechatpayv3.egg-info/
+-rw-rw-rw-   0        0        0    34484 2021-12-05 06:44:49.000000 wechatpayv3-1.2.9/wechatpayv3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2021-12-05 06:44:49.000000 wechatpayv3-1.2.9/wechatpayv3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-12-05 06:44:49.000000 wechatpayv3-1.2.9/wechatpayv3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2021-12-05 06:44:49.000000 wechatpayv3-1.2.9/wechatpayv3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2021-12-05 06:44:49.000000 wechatpayv3-1.2.9/wechatpayv3.egg-info/top_level.txt
```

### Comparing `wechatpayv3-1.2.8/LICENSE` & `wechatpayv3-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/PKG-INFO` & `wechatpayv3-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wechatpayv3
-Version: 1.2.8
+Version: 1.2.9
 Summary: 微信支付 API v3 Python SDK(python sdk for wechatpay v3)
 Home-page: https://github.com/minibear2021/wechatpayv3
 Author: minibear
 License: MIT
 Keywords: python sdk wechatpay api v3 微信支付
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wechatpayv3-1.2.8/README.md` & `wechatpayv3-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/setup.py` & `wechatpayv3-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf8") as f:
     long_description = f.read()
 
 setup(
     name="wechatpayv3",
-    version="1.2.8",
+    version="1.2.9",
     author="minibear",
     description="微信支付 API v3 Python SDK(python sdk for wechatpay v3)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     keywords="python sdk wechatpay api v3 微信支付",
     url="https://github.com/minibear2021/wechatpayv3",
```

### Comparing `wechatpayv3-1.2.8/wechatpayv3/__init__.py` & `wechatpayv3-1.2.9/wechatpayv3/__init__.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3/apply4subject.py` & `wechatpayv3-1.2.9/wechatpayv3/apply4subject.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3/applyment.py` & `wechatpayv3-1.2.9/wechatpayv3/applyment.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3/businesscircle.py` & `wechatpayv3-1.2.9/wechatpayv3/businesscircle.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3/complaint.py` & `wechatpayv3-1.2.9/wechatpayv3/complaint.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3/core.py` & `wechatpayv3-1.2.9/wechatpayv3/core.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3/ecommerce.py` & `wechatpayv3-1.2.9/wechatpayv3/ecommerce.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3/goldplan.py` & `wechatpayv3-1.2.9/wechatpayv3/goldplan.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3/marketing.py` & `wechatpayv3-1.2.9/wechatpayv3/marketing.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3/media.py` & `wechatpayv3-1.2.9/wechatpayv3/media.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3/merchantrisk.py` & `wechatpayv3-1.2.9/wechatpayv3/merchantrisk.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3/parking.py` & `wechatpayv3-1.2.9/wechatpayv3/parking.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3/payscore.py` & `wechatpayv3-1.2.9/wechatpayv3/payscore.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3/profitsharing.py` & `wechatpayv3-1.2.9/wechatpayv3/profitsharing.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,36 +6,38 @@
 def profitsharing_order(self, transaction_id, out_order_no, receivers, unfreeze_unsplit,
                         appid=None, sub_appid=None, sub_mchid=None):
     """请求分账
     :param transaction_id: 微信支付订单号，示例值：'4208450740201411110007820472'
     :param out_order_no: 商户分账单号，只能是数字、大小写字母_-|*@，示例值：'P20150806125346'
     :param receivers: 分账接收方列表，最多可有50个分账接收方，示例值：{{'type':'MERCHANT_ID', 'account':'86693852', 'amount':888, 'description':'分给商户A'}}
     :param unfreeze_unsplit: 是否解冻剩余未分资金，示例值：True, False
-    :param appid: 应用ID，可不填，默认传入初始化时的appid，示例值：'wx1234567890abcdef'    
+    :param appid: 应用ID，可不填，默认传入初始化时的appid，示例值：'wx1234567890abcdef'
     :param sub_appid: (服务商模式)子商户应用ID，示例值：'wxd678efh567hg6999'
     :param sub_mchid: (服务商模式)子商户的商户号，由微信支付生成并下发。示例值：'1900000109'
     """
     params = {}
     if transaction_id:
         params.update({'transaction_id': transaction_id})
     else:
         raise Exception('transaction_id is not assigned')
     if out_order_no:
         params.update({'out_order_no': out_order_no})
     else:
         raise Exception('out_order_no is not assigned')
-    if unfreeze_unsplit:
+    if isinstance(unfreeze_unsplit, bool):
         params.update({'unfreeze_unsplit': unfreeze_unsplit})
     else:
         raise Exception('unfreeze_unsplit is not assigned')
     if receivers:
         params.update({'receivers': receivers})
     else:
         raise Exception('receivers is not assigned')
-    params.update({'appid': appid if appid else self._core._appid})
+    if params.get('receivers').get('name'):
+        params['receivers']['name'] = self._core.encrypt(params['receivers']['name'])
+    params.update({'appid': appid if appid else self._appid})
     if self._partner_mode:
         if sub_appid:
             params.update({'sub_appid': sub_appid})
         if sub_mchid:
             params.update({'sub_mchid': sub_mchid})
         else:
             raise Exception('sub_mchid is not assigned.')
@@ -269,15 +271,15 @@
     """连锁品牌请求分账
     :param brand_mchid: 品牌主商户号，示例值：'1900000108'
     :param sub_mchid: 子商户的商户号，由微信支付生成并下发。示例值：'1900000109'
     :param transaction_id: 微信支付订单号，示例值：'4208450740201411110007820472'
     :param out_order_no: 商户分账单号，只能是数字、大小写字母_-|*@，示例值：'P20150806125346'
     :param receivers: 分账接收方列表，最多可有50个分账接收方，示例值：{{'type':'MERCHANT_ID', 'account':'86693852', 'amount':888, 'description':'分给商户A'}}
     :param finish: 是否完成分账，示例值：True, False
-    :param appid: 应用ID，可不填，默认传入初始化时的appid，示例值：'wx1234567890abcdef'    
+    :param appid: 应用ID，可不填，默认传入初始化时的appid，示例值：'wx1234567890abcdef'
     :param sub_appid: 子商户应用ID，示例值：'wxd678efh567hg6999'
     """
     params = {}
     if brand_mchid:
         params.update({'brand_mchid': brand_mchid})
     else:
         raise Exception('brand_mchid is not assigned')
```

### Comparing `wechatpayv3-1.2.8/wechatpayv3/smartguide.py` & `wechatpayv3-1.2.9/wechatpayv3/smartguide.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3/transaction.py` & `wechatpayv3-1.2.9/wechatpayv3/transaction.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3/utils.py` & `wechatpayv3-1.2.9/wechatpayv3/utils.py`

 * *Files identical despite different names*

### Comparing `wechatpayv3-1.2.8/wechatpayv3.egg-info/PKG-INFO` & `wechatpayv3-1.2.9/wechatpayv3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wechatpayv3
-Version: 1.2.8
+Version: 1.2.9
 Summary: 微信支付 API v3 Python SDK(python sdk for wechatpay v3)
 Home-page: https://github.com/minibear2021/wechatpayv3
 Author: minibear
 License: MIT
 Keywords: python sdk wechatpay api v3 微信支付
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wechatpayv3-1.2.8/wechatpayv3.egg-info/SOURCES.txt` & `wechatpayv3-1.2.9/wechatpayv3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

