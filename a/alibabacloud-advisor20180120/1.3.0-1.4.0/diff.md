# Comparing `tmp/alibabacloud_advisor20180120-1.3.0.tar.gz` & `tmp/alibabacloud_advisor20180120-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_advisor20180120-1.3.0.tar", last modified: Mon Feb 26 03:51:50 2024, max compression
+gzip compressed data, was "dist/alibabacloud_advisor20180120-1.4.0.tar", last modified: Tue Apr  2 15:55:15 2024, max compression
```

## Comparing `alibabacloud_advisor20180120-1.3.0.tar` & `alibabacloud_advisor20180120-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      210 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2441 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1111 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1196 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/alibabacloud_advisor20180120/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/alibabacloud_advisor20180120/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37249 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/alibabacloud_advisor20180120/client.py
--rw-r--r--   0 root         (0) root         (0)    70724 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/alibabacloud_advisor20180120/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/alibabacloud_advisor20180120.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2441 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/alibabacloud_advisor20180120.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/alibabacloud_advisor20180120.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/alibabacloud_advisor20180120.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/alibabacloud_advisor20180120.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/alibabacloud_advisor20180120.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2643 2024-02-26 03:51:50.000000 alibabacloud_advisor20180120-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1111 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/alibabacloud_advisor20180120/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/alibabacloud_advisor20180120/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48129 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/alibabacloud_advisor20180120/client.py
+-rw-r--r--   0 root         (0) root         (0)   101452 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/alibabacloud_advisor20180120/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/alibabacloud_advisor20180120.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/alibabacloud_advisor20180120.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/alibabacloud_advisor20180120.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/alibabacloud_advisor20180120.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/alibabacloud_advisor20180120.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/alibabacloud_advisor20180120.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2643 2024-04-02 15:55:15.000000 alibabacloud_advisor20180120-1.4.0/setup.py
```

### Comparing `alibabacloud_advisor20180120-1.3.0/LICENSE` & `alibabacloud_advisor20180120-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_advisor20180120-1.3.0/PKG-INFO` & `alibabacloud_advisor20180120-1.4.0/alibabacloud_advisor20180120.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_advisor20180120
-Version: 1.3.0
+Name: alibabacloud-advisor20180120
+Version: 1.4.0
 Summary: Alibaba Cloud Intelligent Advisor (20180120) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_advisor20180120-1.3.0/README-CN.md` & `alibabacloud_advisor20180120-1.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_advisor20180120-1.3.0/README.md` & `alibabacloud_advisor20180120-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_advisor20180120-1.3.0/alibabacloud_advisor20180120/client.py` & `alibabacloud_advisor20180120-1.4.0/alibabacloud_advisor20180120/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -479,14 +479,234 @@
     async def describe_advisor_resources_async(
         self,
         request: advisor_20180120_models.DescribeAdvisorResourcesRequest,
     ) -> advisor_20180120_models.DescribeAdvisorResourcesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_advisor_resources_with_options_async(request, runtime)
 
+    def describe_cost_check_advices_with_options(
+        self,
+        tmp_req: advisor_20180120_models.DescribeCostCheckAdvicesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> advisor_20180120_models.DescribeCostCheckAdvicesResponse:
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
+    async def describe_cost_check_advices_with_options_async(
+        self,
+        tmp_req: advisor_20180120_models.DescribeCostCheckAdvicesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> advisor_20180120_models.DescribeCostCheckAdvicesResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_cost_check_advices(
+        self,
+        request: advisor_20180120_models.DescribeCostCheckAdvicesRequest,
+    ) -> advisor_20180120_models.DescribeCostCheckAdvicesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_cost_check_advices_with_options(request, runtime)
+
+    async def describe_cost_check_advices_async(
+        self,
+        request: advisor_20180120_models.DescribeCostCheckAdvicesRequest,
+    ) -> advisor_20180120_models.DescribeCostCheckAdvicesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_cost_check_advices_with_options_async(request, runtime)
+
+    def describe_cost_check_results_with_options(
+        self,
+        tmp_req: advisor_20180120_models.DescribeCostCheckResultsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> advisor_20180120_models.DescribeCostCheckResultsResponse:
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
+    async def describe_cost_check_results_with_options_async(
+        self,
+        tmp_req: advisor_20180120_models.DescribeCostCheckResultsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> advisor_20180120_models.DescribeCostCheckResultsResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_cost_check_results(
+        self,
+        request: advisor_20180120_models.DescribeCostCheckResultsRequest,
+    ) -> advisor_20180120_models.DescribeCostCheckResultsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_cost_check_results_with_options(request, runtime)
+
+    async def describe_cost_check_results_async(
+        self,
+        request: advisor_20180120_models.DescribeCostCheckResultsRequest,
+    ) -> advisor_20180120_models.DescribeCostCheckResultsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_cost_check_results_with_options_async(request, runtime)
+
     def get_history_advices_with_options(
         self,
         request: advisor_20180120_models.GetHistoryAdvicesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> advisor_20180120_models.GetHistoryAdvicesResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_advisor20180120-1.3.0/alibabacloud_advisor20180120/models.py` & `alibabacloud_advisor20180120-1.4.0/alibabacloud_advisor20180120/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1354,14 +1354,900 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeAdvisorResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeCostCheckAdvicesRequest(TeaModel):
+    def __init__(
+        self,
+        check_id: str = None,
+        language: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        region_ids: List[str] = None,
+        resource_ids: List[str] = None,
+        resource_name: str = None,
+        severity: str = None,
+    ):
+        self.check_id = check_id
+        self.language = language
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_ids = region_ids
+        self.resource_ids = resource_ids
+        self.resource_name = resource_name
+        self.severity = severity
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        check_id: str = None,
+        language: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        region_ids_shrink: str = None,
+        resource_ids_shrink: str = None,
+        resource_name: str = None,
+        severity: str = None,
+    ):
+        self.check_id = check_id
+        self.language = language
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_ids_shrink = region_ids_shrink
+        self.resource_ids_shrink = resource_ids_shrink
+        self.resource_name = resource_name
+        self.severity = severity
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        tag_key: str = None,
+        tag_value: str = None,
+    ):
+        self.tag_key = tag_key
+        self.tag_value = tag_value
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TagKey') is not None:
+            self.tag_key = m.get('TagKey')
+        if m.get('TagValue') is not None:
+            self.tag_value = m.get('TagValue')
+        return self
+
+
+class DescribeCostCheckAdvicesResponseBodyDataAdviceList(TeaModel):
+    def __init__(
+        self,
+        aliyun_id: int = None,
+        content: str = None,
+        end_time: int = None,
+        gmt_deleted: int = None,
+        product: str = None,
+        region_id: str = None,
+        resource_id: str = None,
+        resource_name: str = None,
+        severity: str = None,
+        start_time: int = None,
+        tags: List[DescribeCostCheckAdvicesResponseBodyDataAdviceListTags] = None,
+        url: str = None,
+        user_name: str = None,
+        zone_id: str = None,
+    ):
+        self.aliyun_id = aliyun_id
+        self.content = content
+        self.end_time = end_time
+        self.gmt_deleted = gmt_deleted
+        self.product = product
+        self.region_id = region_id
+        self.resource_id = resource_id
+        self.resource_name = resource_name
+        self.severity = severity
+        self.start_time = start_time
+        self.tags = tags
+        self.url = url
+        self.user_name = user_name
+        self.zone_id = zone_id
+
+    def validate(self):
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        advice_list: List[DescribeCostCheckAdvicesResponseBodyDataAdviceList] = None,
+        check_id: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        total_count: int = None,
+    ):
+        self.advice_list = advice_list
+        self.check_id = check_id
+        self.page_number = page_number
+        self.page_size = page_size
+        self.total_count = total_count
+
+    def validate(self):
+        if self.advice_list:
+            for k in self.advice_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        code: str = None,
+        data: DescribeCostCheckAdvicesResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeCostCheckAdvicesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        check_ids: List[str] = None,
+        group_by: str = None,
+        product: str = None,
+        region_ids: List[str] = None,
+        resource_ids: List[str] = None,
+        resource_name: str = None,
+        severity: int = None,
+    ):
+        self.check_ids = check_ids
+        self.group_by = group_by
+        self.product = product
+        self.region_ids = region_ids
+        self.resource_ids = resource_ids
+        self.resource_name = resource_name
+        self.severity = severity
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        check_ids_shrink: str = None,
+        group_by: str = None,
+        product: str = None,
+        region_ids_shrink: str = None,
+        resource_ids_shrink: str = None,
+        resource_name: str = None,
+        severity: int = None,
+    ):
+        self.check_ids_shrink = check_ids_shrink
+        self.group_by = group_by
+        self.product = product
+        self.region_ids_shrink = region_ids_shrink
+        self.resource_ids_shrink = resource_ids_shrink
+        self.resource_name = resource_name
+        self.severity = severity
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        advice_count: int = None,
+        advice_resource_count: int = None,
+        category: str = None,
+        check_id: str = None,
+        check_name: str = None,
+        current_cost: float = None,
+        description: str = None,
+        expected_saving_cost: float = None,
+        optimized_cost: float = None,
+        product: str = None,
+        severity: int = None,
+        summary: str = None,
+        tips: str = None,
+    ):
+        self.advice_count = advice_count
+        self.advice_resource_count = advice_resource_count
+        self.category = category
+        self.check_id = check_id
+        self.check_name = check_name
+        self.current_cost = current_cost
+        self.description = description
+        self.expected_saving_cost = expected_saving_cost
+        self.optimized_cost = optimized_cost
+        self.product = product
+        self.severity = severity
+        self.summary = summary
+        self.tips = tips
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        check_items: List[DescribeCostCheckResultsResponseBodyDataViewGroupCheckItems] = None,
+        group_code: str = None,
+        group_count: int = None,
+        group_expected_saving_cost: float = None,
+        group_name: str = None,
+    ):
+        self.check_items = check_items
+        self.group_code = group_code
+        self.group_count = group_count
+        self.group_expected_saving_cost = group_expected_saving_cost
+        self.group_name = group_name
+
+    def validate(self):
+        if self.check_items:
+            for k in self.check_items:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        advice_resource_count: int = None,
+        group_by: str = None,
+        normal_count: int = None,
+        resource_count: int = None,
+        total_count: int = None,
+        view_group: List[DescribeCostCheckResultsResponseBodyDataViewGroup] = None,
+        warning_count: int = None,
+    ):
+        self.advice_resource_count = advice_resource_count
+        self.group_by = group_by
+        self.normal_count = normal_count
+        self.resource_count = resource_count
+        self.total_count = total_count
+        self.view_group = view_group
+        self.warning_count = warning_count
+
+    def validate(self):
+        if self.view_group:
+            for k in self.view_group:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        code: str = None,
+        data: DescribeCostCheckResultsResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+        success: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeCostCheckResultsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         end_date: str = None,
         language: str = None,
         page_num: int = None,
         page_size: int = None,
```

### Comparing `alibabacloud_advisor20180120-1.3.0/alibabacloud_advisor20180120.egg-info/PKG-INFO` & `alibabacloud_advisor20180120-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-advisor20180120
-Version: 1.3.0
+Name: alibabacloud_advisor20180120
+Version: 1.4.0
 Summary: Alibaba Cloud Intelligent Advisor (20180120) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_advisor20180120-1.3.0/setup.py` & `alibabacloud_advisor20180120-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_advisor20180120.
 
-Created on 26/02/2024
+Created on 02/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_advisor20180120"
 NAME = "alibabacloud_advisor20180120" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Intelligent Advisor (20180120) SDK Library for Python"
```

