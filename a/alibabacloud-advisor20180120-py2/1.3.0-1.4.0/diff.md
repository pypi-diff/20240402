# Comparing `tmp/alibabacloud_advisor20180120_py2-1.3.0.tar.gz` & `tmp/alibabacloud_advisor20180120_py2-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_advisor20180120_py2-1.3.0.tar", last modified: Mon Feb 26 03:51:24 2024, max compression
+gzip compressed data, was "dist/alibabacloud_advisor20180120_py2-1.4.0.tar", last modified: Tue Apr  2 15:54:40 2024, max compression
```

## Comparing `alibabacloud_advisor20180120_py2-1.3.0.tar` & `alibabacloud_advisor20180120_py2-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 03:51:24.000000 alibabacloud_advisor20180120_py2-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      213 2024-02-26 03:51:23.000000 alibabacloud_advisor20180120_py2-1.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-26 03:51:23.000000 alibabacloud_advisor20180120_py2-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-02-26 03:51:23.000000 alibabacloud_advisor20180120_py2-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2508 2024-02-26 03:51:24.000000 alibabacloud_advisor20180120_py2-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2024-02-26 03:51:23.000000 alibabacloud_advisor20180120_py2-1.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2024-02-26 03:51:23.000000 alibabacloud_advisor20180120_py2-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 03:51:24.000000 alibabacloud_advisor20180120_py2-1.3.0/alibabacloud_advisor20180120/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-26 03:51:23.000000 alibabacloud_advisor20180120_py2-1.3.0/alibabacloud_advisor20180120/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16040 2024-02-26 03:51:23.000000 alibabacloud_advisor20180120_py2-1.3.0/alibabacloud_advisor20180120/client.py
--rw-r--r--   0 root         (0) root         (0)    71269 2024-02-26 03:51:23.000000 alibabacloud_advisor20180120_py2-1.3.0/alibabacloud_advisor20180120/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 03:51:24.000000 alibabacloud_advisor20180120_py2-1.3.0/alibabacloud_advisor20180120_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2508 2024-02-26 03:51:24.000000 alibabacloud_advisor20180120_py2-1.3.0/alibabacloud_advisor20180120_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2024-02-26 03:51:24.000000 alibabacloud_advisor20180120_py2-1.3.0/alibabacloud_advisor20180120_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 03:51:24.000000 alibabacloud_advisor20180120_py2-1.3.0/alibabacloud_advisor20180120_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-02-26 03:51:24.000000 alibabacloud_advisor20180120_py2-1.3.0/alibabacloud_advisor20180120_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-26 03:51:24.000000 alibabacloud_advisor20180120_py2-1.3.0/alibabacloud_advisor20180120_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-26 03:51:24.000000 alibabacloud_advisor20180120_py2-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2935 2024-02-26 03:51:23.000000 alibabacloud_advisor20180120_py2-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)      314 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2508 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/alibabacloud_advisor20180120/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/alibabacloud_advisor20180120/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20800 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/alibabacloud_advisor20180120/client.py
+-rw-r--r--   0 root         (0) root         (0)   102313 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/alibabacloud_advisor20180120/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/alibabacloud_advisor20180120_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2508 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/alibabacloud_advisor20180120_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/alibabacloud_advisor20180120_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/alibabacloud_advisor20180120_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/alibabacloud_advisor20180120_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/alibabacloud_advisor20180120_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2935 2024-04-02 15:54:40.000000 alibabacloud_advisor20180120_py2-1.4.0/setup.py
```

### Comparing `alibabacloud_advisor20180120_py2-1.3.0/LICENSE` & `alibabacloud_advisor20180120_py2-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_advisor20180120_py2-1.3.0/PKG-INFO` & `alibabacloud_advisor20180120_py2-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_advisor20180120_py2
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud Intelligent Advisor (20180120) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_advisor20180120_py2-1.3.0/README-CN.md` & `alibabacloud_advisor20180120_py2-1.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_advisor20180120_py2-1.3.0/README.md` & `alibabacloud_advisor20180120_py2-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_advisor20180120_py2-1.3.0/alibabacloud_advisor20180120/client.py` & `alibabacloud_advisor20180120_py2-1.4.0/alibabacloud_advisor20180120/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -212,14 +212,110 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_advisor_resources(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_advisor_resources_with_options(request, runtime)
 
+    def describe_cost_check_advices_with_options(self, tmp_req, runtime):
+        UtilClient.validate_model(tmp_req)
+        request = advisor_20180120_models.DescribeCostCheckAdvicesShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.region_ids):
+            request.region_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.region_ids, 'RegionIds', 'json')
+        if not UtilClient.is_unset(tmp_req.resource_ids):
+            request.resource_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resource_ids, 'ResourceIds', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.check_id):
+            query['CheckId'] = request.check_id
+        if not UtilClient.is_unset(request.language):
+            query['Language'] = request.language
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_ids_shrink):
+            query['RegionIds'] = request.region_ids_shrink
+        if not UtilClient.is_unset(request.resource_ids_shrink):
+            query['ResourceIds'] = request.resource_ids_shrink
+        if not UtilClient.is_unset(request.resource_name):
+            query['ResourceName'] = request.resource_name
+        if not UtilClient.is_unset(request.severity):
+            query['Severity'] = request.severity
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeCostCheckAdvices',
+            version='2018-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            advisor_20180120_models.DescribeCostCheckAdvicesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_cost_check_advices(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_cost_check_advices_with_options(request, runtime)
+
+    def describe_cost_check_results_with_options(self, tmp_req, runtime):
+        UtilClient.validate_model(tmp_req)
+        request = advisor_20180120_models.DescribeCostCheckResultsShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.check_ids):
+            request.check_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.check_ids, 'CheckIds', 'json')
+        if not UtilClient.is_unset(tmp_req.region_ids):
+            request.region_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.region_ids, 'RegionIds', 'json')
+        if not UtilClient.is_unset(tmp_req.resource_ids):
+            request.resource_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.resource_ids, 'ResourceIds', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.check_ids_shrink):
+            query['CheckIds'] = request.check_ids_shrink
+        if not UtilClient.is_unset(request.group_by):
+            query['GroupBy'] = request.group_by
+        if not UtilClient.is_unset(request.product):
+            query['Product'] = request.product
+        if not UtilClient.is_unset(request.region_ids_shrink):
+            query['RegionIds'] = request.region_ids_shrink
+        if not UtilClient.is_unset(request.resource_ids_shrink):
+            query['ResourceIds'] = request.resource_ids_shrink
+        if not UtilClient.is_unset(request.resource_name):
+            query['ResourceName'] = request.resource_name
+        if not UtilClient.is_unset(request.severity):
+            query['Severity'] = request.severity
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeCostCheckResults',
+            version='2018-01-20',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            advisor_20180120_models.DescribeCostCheckResultsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def describe_cost_check_results(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_cost_check_results_with_options(request, runtime)
+
     def get_history_advices_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.language):
             query['Language'] = request.language
```

### Comparing `alibabacloud_advisor20180120_py2-1.3.0/alibabacloud_advisor20180120/models.py` & `alibabacloud_advisor20180120_py2-1.4.0/alibabacloud_advisor20180120/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1187,14 +1187,790 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeAdvisorResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeCostCheckAdvicesRequest(TeaModel):
+    def __init__(self, check_id=None, language=None, page_number=None, page_size=None, region_ids=None,
+                 resource_ids=None, resource_name=None, severity=None):
+        self.check_id = check_id  # type: str
+        self.language = language  # type: str
+        self.page_number = page_number  # type: int
+        self.page_size = page_size  # type: int
+        self.region_ids = region_ids  # type: list[str]
+        self.resource_ids = resource_ids  # type: list[str]
+        self.resource_name = resource_name  # type: str
+        self.severity = severity  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeCostCheckAdvicesRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.check_id is not None:
+            result['CheckId'] = self.check_id
+        if self.language is not None:
+            result['Language'] = self.language
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_ids is not None:
+            result['RegionIds'] = self.region_ids
+        if self.resource_ids is not None:
+            result['ResourceIds'] = self.resource_ids
+        if self.resource_name is not None:
+            result['ResourceName'] = self.resource_name
+        if self.severity is not None:
+            result['Severity'] = self.severity
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CheckId') is not None:
+            self.check_id = m.get('CheckId')
+        if m.get('Language') is not None:
+            self.language = m.get('Language')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionIds') is not None:
+            self.region_ids = m.get('RegionIds')
+        if m.get('ResourceIds') is not None:
+            self.resource_ids = m.get('ResourceIds')
+        if m.get('ResourceName') is not None:
+            self.resource_name = m.get('ResourceName')
+        if m.get('Severity') is not None:
+            self.severity = m.get('Severity')
+        return self
+
+
+class DescribeCostCheckAdvicesShrinkRequest(TeaModel):
+    def __init__(self, check_id=None, language=None, page_number=None, page_size=None, region_ids_shrink=None,
+                 resource_ids_shrink=None, resource_name=None, severity=None):
+        self.check_id = check_id  # type: str
+        self.language = language  # type: str
+        self.page_number = page_number  # type: int
+        self.page_size = page_size  # type: int
+        self.region_ids_shrink = region_ids_shrink  # type: str
+        self.resource_ids_shrink = resource_ids_shrink  # type: str
+        self.resource_name = resource_name  # type: str
+        self.severity = severity  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeCostCheckAdvicesShrinkRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.check_id is not None:
+            result['CheckId'] = self.check_id
+        if self.language is not None:
+            result['Language'] = self.language
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_ids_shrink is not None:
+            result['RegionIds'] = self.region_ids_shrink
+        if self.resource_ids_shrink is not None:
+            result['ResourceIds'] = self.resource_ids_shrink
+        if self.resource_name is not None:
+            result['ResourceName'] = self.resource_name
+        if self.severity is not None:
+            result['Severity'] = self.severity
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CheckId') is not None:
+            self.check_id = m.get('CheckId')
+        if m.get('Language') is not None:
+            self.language = m.get('Language')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionIds') is not None:
+            self.region_ids_shrink = m.get('RegionIds')
+        if m.get('ResourceIds') is not None:
+            self.resource_ids_shrink = m.get('ResourceIds')
+        if m.get('ResourceName') is not None:
+            self.resource_name = m.get('ResourceName')
+        if m.get('Severity') is not None:
+            self.severity = m.get('Severity')
+        return self
+
+
+class DescribeCostCheckAdvicesResponseBodyDataAdviceListTags(TeaModel):
+    def __init__(self, tag_key=None, tag_value=None):
+        self.tag_key = tag_key  # type: str
+        self.tag_value = tag_value  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeCostCheckAdvicesResponseBodyDataAdviceListTags, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.tag_key is not None:
+            result['TagKey'] = self.tag_key
+        if self.tag_value is not None:
+            result['TagValue'] = self.tag_value
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('TagValue') is not None:
+            self.tag_value = m.get('TagValue')
+        return self
+
+
+class DescribeCostCheckAdvicesResponseBodyDataAdviceList(TeaModel):
+    def __init__(self, aliyun_id=None, content=None, end_time=None, gmt_deleted=None, product=None, region_id=None,
+                 resource_id=None, resource_name=None, severity=None, start_time=None, tags=None, url=None, user_name=None,
+                 zone_id=None):
+        self.aliyun_id = aliyun_id  # type: long
+        self.content = content  # type: str
+        self.end_time = end_time  # type: long
+        self.gmt_deleted = gmt_deleted  # type: long
+        self.product = product  # type: str
+        self.region_id = region_id  # type: str
+        self.resource_id = resource_id  # type: str
+        self.resource_name = resource_name  # type: str
+        self.severity = severity  # type: str
+        self.start_time = start_time  # type: long
+        self.tags = tags  # type: list[DescribeCostCheckAdvicesResponseBodyDataAdviceListTags]
+        self.url = url  # type: str
+        self.user_name = user_name  # type: str
+        self.zone_id = zone_id  # type: str
+
+    def validate(self):
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeCostCheckAdvicesResponseBodyDataAdviceList, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.aliyun_id is not None:
+            result['AliyunId'] = self.aliyun_id
+        if self.content is not None:
+            result['Content'] = self.content
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.gmt_deleted is not None:
+            result['GmtDeleted'] = self.gmt_deleted
+        if self.product is not None:
+            result['Product'] = self.product
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_id is not None:
+            result['ResourceId'] = self.resource_id
+        if self.resource_name is not None:
+            result['ResourceName'] = self.resource_name
+        if self.severity is not None:
+            result['Severity'] = self.severity
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        result['Tags'] = []
+        if self.tags is not None:
+            for k in self.tags:
+                result['Tags'].append(k.to_map() if k else None)
+        if self.url is not None:
+            result['Url'] = self.url
+        if self.user_name is not None:
+            result['UserName'] = self.user_name
+        if self.zone_id is not None:
+            result['ZoneId'] = self.zone_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AliyunId') is not None:
+            self.aliyun_id = m.get('AliyunId')
+        if m.get('Content') is not None:
+            self.content = m.get('Content')
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('GmtDeleted') is not None:
+            self.gmt_deleted = m.get('GmtDeleted')
+        if m.get('Product') is not None:
+            self.product = m.get('Product')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceId') is not None:
+            self.resource_id = m.get('ResourceId')
+        if m.get('ResourceName') is not None:
+            self.resource_name = m.get('ResourceName')
+        if m.get('Severity') is not None:
+            self.severity = m.get('Severity')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        self.tags = []
+        if m.get('Tags') is not None:
+            for k in m.get('Tags'):
+                temp_model = DescribeCostCheckAdvicesResponseBodyDataAdviceListTags()
+                self.tags.append(temp_model.from_map(k))
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        if m.get('UserName') is not None:
+            self.user_name = m.get('UserName')
+        if m.get('ZoneId') is not None:
+            self.zone_id = m.get('ZoneId')
+        return self
+
+
+class DescribeCostCheckAdvicesResponseBodyData(TeaModel):
+    def __init__(self, advice_list=None, check_id=None, page_number=None, page_size=None, total_count=None):
+        self.advice_list = advice_list  # type: list[DescribeCostCheckAdvicesResponseBodyDataAdviceList]
+        self.check_id = check_id  # type: str
+        self.page_number = page_number  # type: int
+        self.page_size = page_size  # type: int
+        self.total_count = total_count  # type: int
+
+    def validate(self):
+        if self.advice_list:
+            for k in self.advice_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeCostCheckAdvicesResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['AdviceList'] = []
+        if self.advice_list is not None:
+            for k in self.advice_list:
+                result['AdviceList'].append(k.to_map() if k else None)
+        if self.check_id is not None:
+            result['CheckId'] = self.check_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.advice_list = []
+        if m.get('AdviceList') is not None:
+            for k in m.get('AdviceList'):
+                temp_model = DescribeCostCheckAdvicesResponseBodyDataAdviceList()
+                self.advice_list.append(temp_model.from_map(k))
+        if m.get('CheckId') is not None:
+            self.check_id = m.get('CheckId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribeCostCheckAdvicesResponseBody(TeaModel):
+    def __init__(self, code=None, data=None, message=None, request_id=None, success=None):
+        self.code = code  # type: str
+        self.data = data  # type: DescribeCostCheckAdvicesResponseBodyData
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+        self.success = success  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(DescribeCostCheckAdvicesResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = DescribeCostCheckAdvicesResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class DescribeCostCheckAdvicesResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeCostCheckAdvicesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeCostCheckAdvicesResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeCostCheckAdvicesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeCostCheckResultsRequest(TeaModel):
+    def __init__(self, check_ids=None, group_by=None, product=None, region_ids=None, resource_ids=None,
+                 resource_name=None, severity=None):
+        self.check_ids = check_ids  # type: list[str]
+        self.group_by = group_by  # type: str
+        self.product = product  # type: str
+        self.region_ids = region_ids  # type: list[str]
+        self.resource_ids = resource_ids  # type: list[str]
+        self.resource_name = resource_name  # type: str
+        self.severity = severity  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeCostCheckResultsRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.check_ids is not None:
+            result['CheckIds'] = self.check_ids
+        if self.group_by is not None:
+            result['GroupBy'] = self.group_by
+        if self.product is not None:
+            result['Product'] = self.product
+        if self.region_ids is not None:
+            result['RegionIds'] = self.region_ids
+        if self.resource_ids is not None:
+            result['ResourceIds'] = self.resource_ids
+        if self.resource_name is not None:
+            result['ResourceName'] = self.resource_name
+        if self.severity is not None:
+            result['Severity'] = self.severity
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CheckIds') is not None:
+            self.check_ids = m.get('CheckIds')
+        if m.get('GroupBy') is not None:
+            self.group_by = m.get('GroupBy')
+        if m.get('Product') is not None:
+            self.product = m.get('Product')
+        if m.get('RegionIds') is not None:
+            self.region_ids = m.get('RegionIds')
+        if m.get('ResourceIds') is not None:
+            self.resource_ids = m.get('ResourceIds')
+        if m.get('ResourceName') is not None:
+            self.resource_name = m.get('ResourceName')
+        if m.get('Severity') is not None:
+            self.severity = m.get('Severity')
+        return self
+
+
+class DescribeCostCheckResultsShrinkRequest(TeaModel):
+    def __init__(self, check_ids_shrink=None, group_by=None, product=None, region_ids_shrink=None,
+                 resource_ids_shrink=None, resource_name=None, severity=None):
+        self.check_ids_shrink = check_ids_shrink  # type: str
+        self.group_by = group_by  # type: str
+        self.product = product  # type: str
+        self.region_ids_shrink = region_ids_shrink  # type: str
+        self.resource_ids_shrink = resource_ids_shrink  # type: str
+        self.resource_name = resource_name  # type: str
+        self.severity = severity  # type: int
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeCostCheckResultsShrinkRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.check_ids_shrink is not None:
+            result['CheckIds'] = self.check_ids_shrink
+        if self.group_by is not None:
+            result['GroupBy'] = self.group_by
+        if self.product is not None:
+            result['Product'] = self.product
+        if self.region_ids_shrink is not None:
+            result['RegionIds'] = self.region_ids_shrink
+        if self.resource_ids_shrink is not None:
+            result['ResourceIds'] = self.resource_ids_shrink
+        if self.resource_name is not None:
+            result['ResourceName'] = self.resource_name
+        if self.severity is not None:
+            result['Severity'] = self.severity
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CheckIds') is not None:
+            self.check_ids_shrink = m.get('CheckIds')
+        if m.get('GroupBy') is not None:
+            self.group_by = m.get('GroupBy')
+        if m.get('Product') is not None:
+            self.product = m.get('Product')
+        if m.get('RegionIds') is not None:
+            self.region_ids_shrink = m.get('RegionIds')
+        if m.get('ResourceIds') is not None:
+            self.resource_ids_shrink = m.get('ResourceIds')
+        if m.get('ResourceName') is not None:
+            self.resource_name = m.get('ResourceName')
+        if m.get('Severity') is not None:
+            self.severity = m.get('Severity')
+        return self
+
+
+class DescribeCostCheckResultsResponseBodyDataViewGroupCheckItems(TeaModel):
+    def __init__(self, advice_count=None, advice_resource_count=None, category=None, check_id=None, check_name=None,
+                 current_cost=None, description=None, expected_saving_cost=None, optimized_cost=None, product=None,
+                 severity=None, summary=None, tips=None):
+        self.advice_count = advice_count  # type: int
+        self.advice_resource_count = advice_resource_count  # type: int
+        self.category = category  # type: str
+        self.check_id = check_id  # type: str
+        self.check_name = check_name  # type: str
+        self.current_cost = current_cost  # type: float
+        self.description = description  # type: str
+        self.expected_saving_cost = expected_saving_cost  # type: float
+        self.optimized_cost = optimized_cost  # type: float
+        self.product = product  # type: str
+        self.severity = severity  # type: int
+        self.summary = summary  # type: str
+        self.tips = tips  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeCostCheckResultsResponseBodyDataViewGroupCheckItems, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.advice_count is not None:
+            result['AdviceCount'] = self.advice_count
+        if self.advice_resource_count is not None:
+            result['AdviceResourceCount'] = self.advice_resource_count
+        if self.category is not None:
+            result['Category'] = self.category
+        if self.check_id is not None:
+            result['CheckId'] = self.check_id
+        if self.check_name is not None:
+            result['CheckName'] = self.check_name
+        if self.current_cost is not None:
+            result['CurrentCost'] = self.current_cost
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.expected_saving_cost is not None:
+            result['ExpectedSavingCost'] = self.expected_saving_cost
+        if self.optimized_cost is not None:
+            result['OptimizedCost'] = self.optimized_cost
+        if self.product is not None:
+            result['Product'] = self.product
+        if self.severity is not None:
+            result['Severity'] = self.severity
+        if self.summary is not None:
+            result['Summary'] = self.summary
+        if self.tips is not None:
+            result['Tips'] = self.tips
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AdviceCount') is not None:
+            self.advice_count = m.get('AdviceCount')
+        if m.get('AdviceResourceCount') is not None:
+            self.advice_resource_count = m.get('AdviceResourceCount')
+        if m.get('Category') is not None:
+            self.category = m.get('Category')
+        if m.get('CheckId') is not None:
+            self.check_id = m.get('CheckId')
+        if m.get('CheckName') is not None:
+            self.check_name = m.get('CheckName')
+        if m.get('CurrentCost') is not None:
+            self.current_cost = m.get('CurrentCost')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('ExpectedSavingCost') is not None:
+            self.expected_saving_cost = m.get('ExpectedSavingCost')
+        if m.get('OptimizedCost') is not None:
+            self.optimized_cost = m.get('OptimizedCost')
+        if m.get('Product') is not None:
+            self.product = m.get('Product')
+        if m.get('Severity') is not None:
+            self.severity = m.get('Severity')
+        if m.get('Summary') is not None:
+            self.summary = m.get('Summary')
+        if m.get('Tips') is not None:
+            self.tips = m.get('Tips')
+        return self
+
+
+class DescribeCostCheckResultsResponseBodyDataViewGroup(TeaModel):
+    def __init__(self, check_items=None, group_code=None, group_count=None, group_expected_saving_cost=None,
+                 group_name=None):
+        self.check_items = check_items  # type: list[DescribeCostCheckResultsResponseBodyDataViewGroupCheckItems]
+        self.group_code = group_code  # type: str
+        self.group_count = group_count  # type: int
+        self.group_expected_saving_cost = group_expected_saving_cost  # type: float
+        self.group_name = group_name  # type: str
+
+    def validate(self):
+        if self.check_items:
+            for k in self.check_items:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeCostCheckResultsResponseBodyDataViewGroup, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['CheckItems'] = []
+        if self.check_items is not None:
+            for k in self.check_items:
+                result['CheckItems'].append(k.to_map() if k else None)
+        if self.group_code is not None:
+            result['GroupCode'] = self.group_code
+        if self.group_count is not None:
+            result['GroupCount'] = self.group_count
+        if self.group_expected_saving_cost is not None:
+            result['GroupExpectedSavingCost'] = self.group_expected_saving_cost
+        if self.group_name is not None:
+            result['GroupName'] = self.group_name
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.check_items = []
+        if m.get('CheckItems') is not None:
+            for k in m.get('CheckItems'):
+                temp_model = DescribeCostCheckResultsResponseBodyDataViewGroupCheckItems()
+                self.check_items.append(temp_model.from_map(k))
+        if m.get('GroupCode') is not None:
+            self.group_code = m.get('GroupCode')
+        if m.get('GroupCount') is not None:
+            self.group_count = m.get('GroupCount')
+        if m.get('GroupExpectedSavingCost') is not None:
+            self.group_expected_saving_cost = m.get('GroupExpectedSavingCost')
+        if m.get('GroupName') is not None:
+            self.group_name = m.get('GroupName')
+        return self
+
+
+class DescribeCostCheckResultsResponseBodyData(TeaModel):
+    def __init__(self, advice_resource_count=None, group_by=None, normal_count=None, resource_count=None,
+                 total_count=None, view_group=None, warning_count=None):
+        self.advice_resource_count = advice_resource_count  # type: int
+        self.group_by = group_by  # type: str
+        self.normal_count = normal_count  # type: int
+        self.resource_count = resource_count  # type: int
+        self.total_count = total_count  # type: int
+        self.view_group = view_group  # type: list[DescribeCostCheckResultsResponseBodyDataViewGroup]
+        self.warning_count = warning_count  # type: int
+
+    def validate(self):
+        if self.view_group:
+            for k in self.view_group:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeCostCheckResultsResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.advice_resource_count is not None:
+            result['AdviceResourceCount'] = self.advice_resource_count
+        if self.group_by is not None:
+            result['GroupBy'] = self.group_by
+        if self.normal_count is not None:
+            result['NormalCount'] = self.normal_count
+        if self.resource_count is not None:
+            result['ResourceCount'] = self.resource_count
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        result['ViewGroup'] = []
+        if self.view_group is not None:
+            for k in self.view_group:
+                result['ViewGroup'].append(k.to_map() if k else None)
+        if self.warning_count is not None:
+            result['WarningCount'] = self.warning_count
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AdviceResourceCount') is not None:
+            self.advice_resource_count = m.get('AdviceResourceCount')
+        if m.get('GroupBy') is not None:
+            self.group_by = m.get('GroupBy')
+        if m.get('NormalCount') is not None:
+            self.normal_count = m.get('NormalCount')
+        if m.get('ResourceCount') is not None:
+            self.resource_count = m.get('ResourceCount')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        self.view_group = []
+        if m.get('ViewGroup') is not None:
+            for k in m.get('ViewGroup'):
+                temp_model = DescribeCostCheckResultsResponseBodyDataViewGroup()
+                self.view_group.append(temp_model.from_map(k))
+        if m.get('WarningCount') is not None:
+            self.warning_count = m.get('WarningCount')
+        return self
+
+
+class DescribeCostCheckResultsResponseBody(TeaModel):
+    def __init__(self, code=None, data=None, message=None, request_id=None, success=None):
+        self.code = code  # type: str
+        self.data = data  # type: DescribeCostCheckResultsResponseBodyData
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+        self.success = success  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(DescribeCostCheckResultsResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = DescribeCostCheckResultsResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class DescribeCostCheckResultsResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeCostCheckResultsResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeCostCheckResultsResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeCostCheckResultsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetHistoryAdvicesRequest(TeaModel):
     def __init__(self, end_date=None, language=None, page_num=None, page_size=None, product=None, reverse=None,
                  severity=None, start_date=None):
         self.end_date = end_date  # type: str
         self.language = language  # type: str
         self.page_num = page_num  # type: int
         self.page_size = page_size  # type: int
```

### Comparing `alibabacloud_advisor20180120_py2-1.3.0/alibabacloud_advisor20180120_py2.egg-info/PKG-INFO` & `alibabacloud_advisor20180120_py2-1.4.0/alibabacloud_advisor20180120_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-advisor20180120-py2
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud Intelligent Advisor (20180120) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_advisor20180120_py2-1.3.0/setup.py` & `alibabacloud_advisor20180120_py2-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_advisor20180120_py2.
 
-Created on 26/02/2024
+Created on 02/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_advisor20180120"
 NAME = "alibabacloud_advisor20180120_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Intelligent Advisor (20180120) SDK Library for Python2"
```

