# Comparing `tmp/pixelbin-3.2.0.tar.gz` & `tmp/pixelbin-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelbin-3.2.0.tar", max compression
+gzip compressed data, was "pixelbin-4.0.0.tar", max compression
```

## Comparing `pixelbin-3.2.0.tar` & `pixelbin-4.0.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1065 2022-05-27 05:55:59.335216 pixelbin-3.2.0/LICENSE
--rw-r--r--   0        0        0    11665 2023-10-31 10:53:15.064641 pixelbin-3.2.0/README.md
--rw-r--r--   0        0        0    82339 2024-03-14 06:57:44.199719 pixelbin-3.2.0/documentation/platform/ASSETS.md
--rw-r--r--   0        0        0     3705 2023-10-31 10:53:15.065715 pixelbin-3.2.0/documentation/platform/ORGANIZATION.md
--rw-r--r--   0        0        0      247 2023-06-08 10:09:17.344691 pixelbin-3.2.0/documentation/platform/README.md
--rw-r--r--   0        0        0      167 2022-05-27 05:55:59.312424 pixelbin-3.2.0/pixelbin/__init__.py
--rw-r--r--   0        0        0        0 2022-05-27 06:01:25.401889 pixelbin-3.2.0/pixelbin/common/__init__.py
--rw-r--r--   0        0        0     3709 2023-05-12 08:24:33.227089 pixelbin-3.2.0/pixelbin/common/aiohttp_helper.py
--rw-r--r--   0        0        0      165 2022-05-27 06:01:25.402704 pixelbin-3.2.0/pixelbin/common/constants.py
--rw-r--r--   0        0        0      276 2022-05-27 05:55:59.314728 pixelbin-3.2.0/pixelbin/common/date_helper.py
--rw-r--r--   0        0        0     1241 2022-11-08 19:12:32.304888 pixelbin-3.2.0/pixelbin/common/exceptions.py
--rw-r--r--   0        0        0     2733 2022-05-27 06:01:25.403240 pixelbin-3.2.0/pixelbin/common/utils.py
--rw-r--r--   0        0        0      272 2022-05-27 06:01:25.403508 pixelbin-3.2.0/pixelbin/platform/OAuthClient.py
--rw-r--r--   0        0        0    64214 2024-03-14 06:57:44.200126 pixelbin-3.2.0/pixelbin/platform/PixelbinClient.py
--rw-r--r--   0        0        0     1164 2022-05-27 06:01:25.404202 pixelbin-3.2.0/pixelbin/platform/PixelbinConfig.py
--rw-r--r--   0        0        0     2289 2023-05-12 08:24:33.227557 pixelbin-3.2.0/pixelbin/platform/PlatformAPIClient.py
--rw-r--r--   0        0        0        0 2022-05-27 05:55:59.316752 pixelbin-3.2.0/pixelbin/platform/__init__.py
--rw-r--r--   0        0        0      319 2023-06-08 10:09:17.345977 pixelbin-3.2.0/pixelbin/platform/enums.py
--rw-r--r--   0        0        0      345 2023-02-03 06:42:04.215978 pixelbin-3.2.0/pixelbin/platform/models/AddCredentialsRequest.py
--rw-r--r--   0        0        0      297 2023-02-03 06:42:04.216164 pixelbin-3.2.0/pixelbin/platform/models/AddCredentialsResponse.py
--rw-r--r--   0        0        0      392 2023-02-03 06:42:04.216350 pixelbin-3.2.0/pixelbin/platform/models/AddPresetRequest.py
--rw-r--r--   0        0        0      446 2023-02-03 06:42:04.216479 pixelbin-3.2.0/pixelbin/platform/models/AddPresetResponse.py
--rw-r--r--   0        0        0      466 2022-11-08 19:12:32.305375 pixelbin-3.2.0/pixelbin/platform/models/AppOrgDetails.py
--rw-r--r--   0        0        0      650 2022-05-27 05:55:59.317908 pixelbin-3.2.0/pixelbin/platform/models/AppSchema.py
--rw-r--r--   0        0        0     3007 2024-03-14 06:57:44.200677 pixelbin-3.2.0/pixelbin/platform/models/AssetsValidator.py
--rw-r--r--   0        0        0      240 2022-05-27 05:55:59.318322 pixelbin-3.2.0/pixelbin/platform/models/BaseSchema.py
--rw-r--r--   0        0        0      331 2022-05-27 05:55:59.318534 pixelbin-3.2.0/pixelbin/platform/models/CreateFolderRequest.py
--rw-r--r--   0        0        0      630 2023-02-03 06:42:04.217084 pixelbin-3.2.0/pixelbin/platform/models/Credentials.py
--rw-r--r--   0        0        0      286 2023-02-03 06:42:04.217347 pixelbin-3.2.0/pixelbin/platform/models/CredentialsItem.py
--rw-r--r--   0        0        0      592 2023-02-03 06:42:04.217573 pixelbin-3.2.0/pixelbin/platform/models/DeleteCredentialsResponse.py
--rw-r--r--   0        0        0      321 2022-05-27 05:55:59.318746 pixelbin-3.2.0/pixelbin/platform/models/DeleteMultipleFilesRequest.py
--rw-r--r--   0        0        0      349 2022-05-27 05:55:59.318959 pixelbin-3.2.0/pixelbin/platform/models/Delimiter.py
--rw-r--r--   0        0        0      287 2022-05-27 05:55:59.319154 pixelbin-3.2.0/pixelbin/platform/models/ErrorSchema.py
--rw-r--r--   0        0        0      732 2022-05-27 05:55:59.319473 pixelbin-3.2.0/pixelbin/platform/models/FileUploadRequest.py
--rw-r--r--   0        0        0      898 2023-10-31 10:53:15.067734 pixelbin-3.2.0/pixelbin/platform/models/FilesResponse.py
--rw-r--r--   0        0        0      424 2022-05-27 05:55:59.319957 pixelbin-3.2.0/pixelbin/platform/models/FoldersResponse.py
--rw-r--r--   0        0        0      481 2023-02-03 06:42:04.217778 pixelbin-3.2.0/pixelbin/platform/models/GetAncestorsResponse.py
--rw-r--r--   0        0        0      384 2023-02-03 06:42:04.218175 pixelbin-3.2.0/pixelbin/platform/models/GetFilesWithConstraintsItem.py
--rw-r--r--   0        0        0      528 2023-02-03 06:42:04.218367 pixelbin-3.2.0/pixelbin/platform/models/GetFilesWithConstraintsRequest.py
--rw-r--r--   0        0        0      461 2023-02-03 06:42:04.218564 pixelbin-3.2.0/pixelbin/platform/models/GetPresetsResponse.py
--rw-r--r--   0        0        0      318 2023-06-08 10:09:17.346152 pixelbin-3.2.0/pixelbin/platform/models/GetTransformationContextSuccessResponse.py
--rw-r--r--   0        0        0      442 2022-05-27 05:55:59.320141 pixelbin-3.2.0/pixelbin/platform/models/ListFilesResponse.py
--rw-r--r--   0        0        0      590 2022-05-27 05:55:59.320346 pixelbin-3.2.0/pixelbin/platform/models/OrganizationDetailSchema.py
--rw-r--r--   0        0        0      270 2022-11-08 19:12:32.305605 pixelbin-3.2.0/pixelbin/platform/models/OrganizationValidator.py
--rw-r--r--   0        0        0      326 2022-05-27 05:55:59.320885 pixelbin-3.2.0/pixelbin/platform/models/PresignedUrl.py
--rw-r--r--   0        0        0      328 2024-03-14 06:57:44.200854 pixelbin-3.2.0/pixelbin/platform/models/PresignedUrlV2.py
--rw-r--r--   0        0        0      736 2022-05-27 05:55:59.321142 pixelbin-3.2.0/pixelbin/platform/models/SignedUploadRequest.py
--rw-r--r--   0        0        0      785 2024-03-14 06:57:44.201014 pixelbin-3.2.0/pixelbin/platform/models/SignedUploadRequestV2.py
--rw-r--r--   0        0        0      352 2022-05-27 05:55:59.321384 pixelbin-3.2.0/pixelbin/platform/models/SignedUploadResponse.py
--rw-r--r--   0        0        0      358 2024-03-14 06:57:44.201162 pixelbin-3.2.0/pixelbin/platform/models/SignedUploadV2Response.py
--rw-r--r--   0        0        0      583 2022-05-27 05:55:59.321727 pixelbin-3.2.0/pixelbin/platform/models/TransformationModuleResponse.py
--rw-r--r--   0        0        0      474 2022-05-27 05:55:59.321995 pixelbin-3.2.0/pixelbin/platform/models/TransformationModulesResponse.py
--rw-r--r--   0        0        0      317 2023-06-08 10:09:17.346323 pixelbin-3.2.0/pixelbin/platform/models/TransformationValidator.py
--rw-r--r--   0        0        0      299 2023-02-03 06:42:04.218752 pixelbin-3.2.0/pixelbin/platform/models/UpdateCredentialsRequest.py
--rw-r--r--   0        0        0      625 2023-10-31 10:53:15.068539 pixelbin-3.2.0/pixelbin/platform/models/UpdateFileRequest.py
--rw-r--r--   0        0        0      294 2022-05-27 05:55:59.322486 pixelbin-3.2.0/pixelbin/platform/models/UpdateFolderRequest.py
--rw-r--r--   0        0        0      294 2023-02-03 06:42:04.219019 pixelbin-3.2.0/pixelbin/platform/models/UpdatePresetRequest.py
--rw-r--r--   0        0        0      846 2023-10-31 10:53:15.069046 pixelbin-3.2.0/pixelbin/platform/models/UploadResponse.py
--rw-r--r--   0        0        0      730 2022-05-27 05:55:59.323111 pixelbin-3.2.0/pixelbin/platform/models/UrlUploadRequest.py
--rw-r--r--   0        0        0     2588 2024-03-14 06:57:44.201768 pixelbin-3.2.0/pixelbin/platform/models/__init__.py
--rw-r--r--   0        0        0      542 2022-05-27 05:55:59.323718 pixelbin-3.2.0/pixelbin/platform/models/exploreFolderResponse.py
--rw-r--r--   0        0        0      670 2023-10-31 10:53:15.069355 pixelbin-3.2.0/pixelbin/platform/models/exploreItem.py
--rw-r--r--   0        0        0      440 2022-05-27 05:55:59.325358 pixelbin-3.2.0/pixelbin/platform/models/exploreResponse.py
--rw-r--r--   0        0        0      411 2022-05-27 05:55:59.325644 pixelbin-3.2.0/pixelbin/platform/models/folderItem.py
--rw-r--r--   0        0        0      466 2022-05-27 05:55:59.325929 pixelbin-3.2.0/pixelbin/platform/models/page.py
--rw-r--r--   0        0        0        0 2022-05-27 06:01:25.404488 pixelbin-3.2.0/pixelbin/utils/__init__.py
--rw-r--r--   0        0        0     1566 2023-10-31 10:53:15.069846 pixelbin-3.2.0/pixelbin/utils/security.py
--rw-r--r--   0        0        0    12533 2024-01-17 07:14:19.029529 pixelbin-3.2.0/pixelbin/utils/url.py
--rw-r--r--   0        0        0      762 2024-03-14 06:57:44.202003 pixelbin-3.2.0/pyproject.toml
--rw-r--r--   0        0        0    12869 2024-03-14 06:58:36.730601 pixelbin-3.2.0/setup.py
--rw-r--r--   0        0        0    12531 2024-03-14 06:58:36.731777 pixelbin-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-05-27 05:55:59.335216 pixelbin-4.0.0/LICENSE
+-rw-r--r--   0        0        0    11718 2024-04-02 07:18:47.494966 pixelbin-4.0.0/README.md
+-rw-r--r--   0        0        0    82339 2024-03-14 06:57:44.199719 pixelbin-4.0.0/documentation/platform/ASSETS.md
+-rw-r--r--   0        0        0     3705 2023-10-31 10:53:15.065715 pixelbin-4.0.0/documentation/platform/ORGANIZATION.md
+-rw-r--r--   0        0        0      247 2023-06-08 10:09:17.344691 pixelbin-4.0.0/documentation/platform/README.md
+-rw-r--r--   0        0        0      167 2022-05-27 05:55:59.312424 pixelbin-4.0.0/pixelbin/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-27 06:01:25.401889 pixelbin-4.0.0/pixelbin/common/__init__.py
+-rw-r--r--   0        0        0     3709 2023-05-12 08:24:33.227089 pixelbin-4.0.0/pixelbin/common/aiohttp_helper.py
+-rw-r--r--   0        0        0      165 2022-05-27 06:01:25.402704 pixelbin-4.0.0/pixelbin/common/constants.py
+-rw-r--r--   0        0        0      276 2022-05-27 05:55:59.314728 pixelbin-4.0.0/pixelbin/common/date_helper.py
+-rw-r--r--   0        0        0     1241 2022-11-08 19:12:32.304888 pixelbin-4.0.0/pixelbin/common/exceptions.py
+-rw-r--r--   0        0        0     2733 2022-05-27 06:01:25.403240 pixelbin-4.0.0/pixelbin/common/utils.py
+-rw-r--r--   0        0        0      272 2022-05-27 06:01:25.403508 pixelbin-4.0.0/pixelbin/platform/OAuthClient.py
+-rw-r--r--   0        0        0    64214 2024-03-14 06:57:44.200126 pixelbin-4.0.0/pixelbin/platform/PixelbinClient.py
+-rw-r--r--   0        0        0     1164 2022-05-27 06:01:25.404202 pixelbin-4.0.0/pixelbin/platform/PixelbinConfig.py
+-rw-r--r--   0        0        0     2289 2023-05-12 08:24:33.227557 pixelbin-4.0.0/pixelbin/platform/PlatformAPIClient.py
+-rw-r--r--   0        0        0        0 2022-05-27 05:55:59.316752 pixelbin-4.0.0/pixelbin/platform/__init__.py
+-rw-r--r--   0        0        0      319 2023-06-08 10:09:17.345977 pixelbin-4.0.0/pixelbin/platform/enums.py
+-rw-r--r--   0        0        0      345 2023-02-03 06:42:04.215978 pixelbin-4.0.0/pixelbin/platform/models/AddCredentialsRequest.py
+-rw-r--r--   0        0        0      297 2023-02-03 06:42:04.216164 pixelbin-4.0.0/pixelbin/platform/models/AddCredentialsResponse.py
+-rw-r--r--   0        0        0      392 2023-02-03 06:42:04.216350 pixelbin-4.0.0/pixelbin/platform/models/AddPresetRequest.py
+-rw-r--r--   0        0        0      446 2023-02-03 06:42:04.216479 pixelbin-4.0.0/pixelbin/platform/models/AddPresetResponse.py
+-rw-r--r--   0        0        0      466 2022-11-08 19:12:32.305375 pixelbin-4.0.0/pixelbin/platform/models/AppOrgDetails.py
+-rw-r--r--   0        0        0      650 2022-05-27 05:55:59.317908 pixelbin-4.0.0/pixelbin/platform/models/AppSchema.py
+-rw-r--r--   0        0        0     3007 2024-03-14 06:57:44.200677 pixelbin-4.0.0/pixelbin/platform/models/AssetsValidator.py
+-rw-r--r--   0        0        0      240 2022-05-27 05:55:59.318322 pixelbin-4.0.0/pixelbin/platform/models/BaseSchema.py
+-rw-r--r--   0        0        0      331 2022-05-27 05:55:59.318534 pixelbin-4.0.0/pixelbin/platform/models/CreateFolderRequest.py
+-rw-r--r--   0        0        0      630 2023-02-03 06:42:04.217084 pixelbin-4.0.0/pixelbin/platform/models/Credentials.py
+-rw-r--r--   0        0        0      286 2023-02-03 06:42:04.217347 pixelbin-4.0.0/pixelbin/platform/models/CredentialsItem.py
+-rw-r--r--   0        0        0      592 2023-02-03 06:42:04.217573 pixelbin-4.0.0/pixelbin/platform/models/DeleteCredentialsResponse.py
+-rw-r--r--   0        0        0      321 2022-05-27 05:55:59.318746 pixelbin-4.0.0/pixelbin/platform/models/DeleteMultipleFilesRequest.py
+-rw-r--r--   0        0        0      349 2022-05-27 05:55:59.318959 pixelbin-4.0.0/pixelbin/platform/models/Delimiter.py
+-rw-r--r--   0        0        0      287 2022-05-27 05:55:59.319154 pixelbin-4.0.0/pixelbin/platform/models/ErrorSchema.py
+-rw-r--r--   0        0        0      732 2022-05-27 05:55:59.319473 pixelbin-4.0.0/pixelbin/platform/models/FileUploadRequest.py
+-rw-r--r--   0        0        0      898 2023-10-31 10:53:15.067734 pixelbin-4.0.0/pixelbin/platform/models/FilesResponse.py
+-rw-r--r--   0        0        0      424 2022-05-27 05:55:59.319957 pixelbin-4.0.0/pixelbin/platform/models/FoldersResponse.py
+-rw-r--r--   0        0        0      481 2023-02-03 06:42:04.217778 pixelbin-4.0.0/pixelbin/platform/models/GetAncestorsResponse.py
+-rw-r--r--   0        0        0      384 2023-02-03 06:42:04.218175 pixelbin-4.0.0/pixelbin/platform/models/GetFilesWithConstraintsItem.py
+-rw-r--r--   0        0        0      528 2023-02-03 06:42:04.218367 pixelbin-4.0.0/pixelbin/platform/models/GetFilesWithConstraintsRequest.py
+-rw-r--r--   0        0        0      461 2023-02-03 06:42:04.218564 pixelbin-4.0.0/pixelbin/platform/models/GetPresetsResponse.py
+-rw-r--r--   0        0        0      318 2023-06-08 10:09:17.346152 pixelbin-4.0.0/pixelbin/platform/models/GetTransformationContextSuccessResponse.py
+-rw-r--r--   0        0        0      442 2022-05-27 05:55:59.320141 pixelbin-4.0.0/pixelbin/platform/models/ListFilesResponse.py
+-rw-r--r--   0        0        0      590 2022-05-27 05:55:59.320346 pixelbin-4.0.0/pixelbin/platform/models/OrganizationDetailSchema.py
+-rw-r--r--   0        0        0      270 2022-11-08 19:12:32.305605 pixelbin-4.0.0/pixelbin/platform/models/OrganizationValidator.py
+-rw-r--r--   0        0        0      326 2022-05-27 05:55:59.320885 pixelbin-4.0.0/pixelbin/platform/models/PresignedUrl.py
+-rw-r--r--   0        0        0      328 2024-03-14 06:57:44.200854 pixelbin-4.0.0/pixelbin/platform/models/PresignedUrlV2.py
+-rw-r--r--   0        0        0      736 2022-05-27 05:55:59.321142 pixelbin-4.0.0/pixelbin/platform/models/SignedUploadRequest.py
+-rw-r--r--   0        0        0      785 2024-03-14 06:57:44.201014 pixelbin-4.0.0/pixelbin/platform/models/SignedUploadRequestV2.py
+-rw-r--r--   0        0        0      352 2022-05-27 05:55:59.321384 pixelbin-4.0.0/pixelbin/platform/models/SignedUploadResponse.py
+-rw-r--r--   0        0        0      358 2024-03-14 06:57:44.201162 pixelbin-4.0.0/pixelbin/platform/models/SignedUploadV2Response.py
+-rw-r--r--   0        0        0      583 2022-05-27 05:55:59.321727 pixelbin-4.0.0/pixelbin/platform/models/TransformationModuleResponse.py
+-rw-r--r--   0        0        0      474 2022-05-27 05:55:59.321995 pixelbin-4.0.0/pixelbin/platform/models/TransformationModulesResponse.py
+-rw-r--r--   0        0        0      317 2023-06-08 10:09:17.346323 pixelbin-4.0.0/pixelbin/platform/models/TransformationValidator.py
+-rw-r--r--   0        0        0      299 2023-02-03 06:42:04.218752 pixelbin-4.0.0/pixelbin/platform/models/UpdateCredentialsRequest.py
+-rw-r--r--   0        0        0      625 2023-10-31 10:53:15.068539 pixelbin-4.0.0/pixelbin/platform/models/UpdateFileRequest.py
+-rw-r--r--   0        0        0      294 2022-05-27 05:55:59.322486 pixelbin-4.0.0/pixelbin/platform/models/UpdateFolderRequest.py
+-rw-r--r--   0        0        0      294 2023-02-03 06:42:04.219019 pixelbin-4.0.0/pixelbin/platform/models/UpdatePresetRequest.py
+-rw-r--r--   0        0        0      846 2023-10-31 10:53:15.069046 pixelbin-4.0.0/pixelbin/platform/models/UploadResponse.py
+-rw-r--r--   0        0        0      730 2022-05-27 05:55:59.323111 pixelbin-4.0.0/pixelbin/platform/models/UrlUploadRequest.py
+-rw-r--r--   0        0        0     2588 2024-03-14 06:57:44.201768 pixelbin-4.0.0/pixelbin/platform/models/__init__.py
+-rw-r--r--   0        0        0      542 2022-05-27 05:55:59.323718 pixelbin-4.0.0/pixelbin/platform/models/exploreFolderResponse.py
+-rw-r--r--   0        0        0      670 2023-10-31 10:53:15.069355 pixelbin-4.0.0/pixelbin/platform/models/exploreItem.py
+-rw-r--r--   0        0        0      440 2022-05-27 05:55:59.325358 pixelbin-4.0.0/pixelbin/platform/models/exploreResponse.py
+-rw-r--r--   0        0        0      411 2022-05-27 05:55:59.325644 pixelbin-4.0.0/pixelbin/platform/models/folderItem.py
+-rw-r--r--   0        0        0      466 2022-05-27 05:55:59.325929 pixelbin-4.0.0/pixelbin/platform/models/page.py
+-rw-r--r--   0        0        0        0 2022-05-27 06:01:25.404488 pixelbin-4.0.0/pixelbin/utils/__init__.py
+-rw-r--r--   0        0        0     1488 2024-04-02 07:18:47.495248 pixelbin-4.0.0/pixelbin/utils/security.py
+-rw-r--r--   0        0        0    12533 2024-01-17 07:14:19.029529 pixelbin-4.0.0/pixelbin/utils/url.py
+-rw-r--r--   0        0        0      762 2024-04-02 07:18:47.495496 pixelbin-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0    12923 2024-04-02 07:18:52.597634 pixelbin-4.0.0/setup.py
+-rw-r--r--   0        0        0    12584 2024-04-02 07:18:52.598709 pixelbin-4.0.0/PKG-INFO
```

### Comparing `pixelbin-3.2.0/LICENSE` & `pixelbin-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/README.md` & `pixelbin-4.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,34 +49,34 @@
 
 ## Security Utils
 
 ### For generating Signed URLs
 
 Generate a signed PixelBin url
 
-| Parameter                  | Description                                          | Example                                                                                    |
-| -------------------------- | ---------------------------------------------------- | ------------------------------------------------------------------------------------------ |
-| `url` (string)             | A valid Pixelbin URL to be signed                    | `https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg` |
-| `expiry_seconds` (int)     | Number of seconds the signed URL should be valid for | `20`                                                                                       |
-| `token_id` (int or string) | ID of the token used for signing                     | `42`                                                                                       |
-| `token` (string)           | Value of the token used for signing                  | `dummy-token`                                                                              |
+| Parameter              | Description                                          | Example                                                                                    |
+| ---------------------- | ---------------------------------------------------- | ------------------------------------------------------------------------------------------ |
+| `url` (string)         | A valid Pixelbin URL to be signed                    | `https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg` |
+| `expiry_seconds` (int) | Number of seconds the signed URL should be valid for | `20`                                                                                       |
+| `access_key` (string)  | Access key of the token used for signing             | `6227274d-92c9-4b74-bef8-2528542516d8`                                                     |
+| `token` (string)       | Value of the token used for signing                  | `dummy-token`                                                                              |
 
 Example:
 
 ```python
 from pixelbin.utils.security import sign_url
 
 signed_url = sign_url(
     "https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg", # url
     20, # expiry_seconds
-    42, # token_id
+    "6227274d-92c9-4b74-bef8-2528542516d8", # access_key
     "dummy-token", # token
 );
 # signed_url
-# https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg?pbs=8eb6a00af74e57967a42316e4de238aa88d92961649764fad1832c1bff101f25&pbe=1695635915&pbt=1
+# https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg?pbs=8eb6a00af74e57967a42316e4de238aa88d92961649764fad1832c1bff101f25&pbe=1695635915&pbt=6227274d-92c9-4b74-bef8-2528542516d8
 ```
 
 Usage with custom domain url
 
 ```python
 from pixelbin.utils.security import sign_url
 
@@ -194,15 +194,15 @@
 #     "baseUrl": "https://xyz.designify.media",
 #     "wrkr": False,
 #     "workerPath": "",
 #     "options": {}
 # }
 ```
 
-````python
+```python
 workerUrl =
     "https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/wrkr/resize:h100,w:200/folder/image.jpeg";
 
 obj = url_to_obj(workerUrl)
 # obj
 # {
 #     "cloudName": "your-cloud-name",
@@ -211,14 +211,15 @@
 #     "transformations": [],
 #     "filePath": "",
 #     "worker": True,
 #     "workerPath": "resize:h100,w:200/folder/image.jpeg",
 #     "baseUrl": "https://cdn.pixelbin.io"
 #     "options": {}
 # }
+```
 
 ### obj_to_url
 
 Converts the extracted url obj to a Pixelbin url.
 
 | Property                   | Description                                          | Example                               |
 | -------------------------- | ---------------------------------------------------- | ------------------------------------- |
@@ -227,15 +228,15 @@
 | `version` (string)         | CDN API version                                      | `v2`                                  |
 | `transformations` (array)  | Extracted transformations from the URL               | `[{ "plugin": "t", "name": "flip" }]` |
 | `filePath` (string)        | Path to the file on Pixelbin storage                 | `/path/to/image.jpeg`                 |
 | `baseUrl` (string)         | Base URL                                             | `https://cdn.pixelbin.io/`            |
 | `isCustomDomain` (boolean) | Indicates if the URL is for a custom domain          | `False`                               |
 | `worker` (boolean)         | Indicates if the URL is a URL Translation Worker URL | `False`                               |
 | `workerPath` (string)      | Input path to a URL Translation Worker               | `resize:w200,h400/folder/image.jpeg`  |
-| `options` (Object)         | Query parameters added, such as "dpr" and "f_auto"   | `{ "dpr": 2.0, "f_auto": True }`    |
+| `options` (Object)         | Query parameters added, such as "dpr" and "f_auto"   | `{ "dpr": 2.0, "f_auto": True }`      |
 
 ```python
 from pixelbin.utils.url import obj_to_url
 
 obj = {
     cloudName: "your-cloud-name",
     zone: "z-slug",
@@ -266,15 +267,15 @@
     ],
     filePath: "path/to/image.jpeg",
     baseUrl: "https://cdn.pixelbin.io",
 }
 url = obj_to_url(obj) # obj is as shown above
 # url
 # https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg?dpr=2.0&f_auto=true
-````
+```
 
 Usage with custom domain
 
 ```python
 from pixelbin.utils.url import obj_to_url
 
 obj = {
```

### Comparing `pixelbin-3.2.0/documentation/platform/ASSETS.md` & `pixelbin-4.0.0/documentation/platform/ASSETS.md`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/documentation/platform/ORGANIZATION.md` & `pixelbin-4.0.0/documentation/platform/ORGANIZATION.md`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/common/aiohttp_helper.py` & `pixelbin-4.0.0/pixelbin/common/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/common/exceptions.py` & `pixelbin-4.0.0/pixelbin/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/common/utils.py` & `pixelbin-4.0.0/pixelbin/common/utils.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/PixelbinClient.py` & `pixelbin-4.0.0/pixelbin/platform/PixelbinClient.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/PixelbinConfig.py` & `pixelbin-4.0.0/pixelbin/platform/PixelbinConfig.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/PlatformAPIClient.py` & `pixelbin-4.0.0/pixelbin/platform/PlatformAPIClient.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/AppSchema.py` & `pixelbin-4.0.0/pixelbin/platform/models/AppSchema.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/AssetsValidator.py` & `pixelbin-4.0.0/pixelbin/platform/models/AssetsValidator.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/Credentials.py` & `pixelbin-4.0.0/pixelbin/platform/models/Credentials.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/DeleteCredentialsResponse.py` & `pixelbin-4.0.0/pixelbin/platform/models/DeleteCredentialsResponse.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/FileUploadRequest.py` & `pixelbin-4.0.0/pixelbin/platform/models/FileUploadRequest.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/FilesResponse.py` & `pixelbin-4.0.0/pixelbin/platform/models/FilesResponse.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/GetFilesWithConstraintsRequest.py` & `pixelbin-4.0.0/pixelbin/platform/models/GetFilesWithConstraintsRequest.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/OrganizationDetailSchema.py` & `pixelbin-4.0.0/pixelbin/platform/models/OrganizationDetailSchema.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/SignedUploadRequest.py` & `pixelbin-4.0.0/pixelbin/platform/models/SignedUploadRequest.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/SignedUploadRequestV2.py` & `pixelbin-4.0.0/pixelbin/platform/models/SignedUploadRequestV2.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/TransformationModuleResponse.py` & `pixelbin-4.0.0/pixelbin/platform/models/TransformationModuleResponse.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/UpdateFileRequest.py` & `pixelbin-4.0.0/pixelbin/platform/models/UpdateFileRequest.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/UploadResponse.py` & `pixelbin-4.0.0/pixelbin/platform/models/UploadResponse.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/UrlUploadRequest.py` & `pixelbin-4.0.0/pixelbin/platform/models/UrlUploadRequest.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/__init__.py` & `pixelbin-4.0.0/pixelbin/platform/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/exploreFolderResponse.py` & `pixelbin-4.0.0/pixelbin/platform/models/exploreFolderResponse.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/platform/models/exploreItem.py` & `pixelbin-4.0.0/pixelbin/platform/models/exploreItem.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pixelbin/utils/security.py` & `pixelbin-4.0.0/pixelbin/utils/security.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Union
 import time
 import hmac
 import hashlib
 from urllib import parse
 from ..common.exceptions import (
     PixelbinIllegalArgumentError,
 )
@@ -11,25 +10,24 @@
 def hmac_sha256(key: str, message: str):
     return hmac.new(key.encode(), message.encode(), hashlib.sha256).hexdigest()
 
 
 def generate_signature(url_path: str, expiry_timestamp: int, key: str):
     if url_path.startswith("/"):
         url_path = url_path[1:]
-    url_path = parse.quote(url_path)
     signature = hmac_sha256(key, f"{url_path}{expiry_timestamp}")
     return signature
 
 
-def sign_url(url: str, expiry_seconds: int, token_id: Union[int, str], token: str):
+def sign_url(url: str, expiry_seconds: int, access_key: str, token: str):
     if not isinstance(expiry_seconds, int):
         raise PixelbinIllegalArgumentError("expiry_seconds must be an integer")
 
-    if not isinstance(token_id, (int, str)):
-        raise PixelbinIllegalArgumentError("token_id must be an integer or string")
+    if not isinstance(access_key, (int, str)):
+        raise PixelbinIllegalArgumentError("access_key must be a string")
 
     if not isinstance(token, str):
         raise PixelbinIllegalArgumentError("token must be a string")
 
     url_parts = parse.urlparse(url)
     url_path = url_parts.path
     url_query = parse.parse_qs(url_parts.query)
@@ -39,12 +37,12 @@
 
     expiry_timestamp = int(time.time()) + expiry_seconds
 
     signature = generate_signature(url_path, expiry_timestamp, token)
 
     url_query["pbs"] = signature
     url_query["pbe"] = expiry_timestamp
-    url_query["pbt"] = token_id
+    url_query["pbt"] = access_key
 
     url_parts = url_parts._replace(query=parse.urlencode(url_query, doseq=True))
 
     return parse.urlunparse(url_parts)
```

### Comparing `pixelbin-3.2.0/pixelbin/utils/url.py` & `pixelbin-4.0.0/pixelbin/utils/url.py`

 * *Files identical despite different names*

### Comparing `pixelbin-3.2.0/pyproject.toml` & `pixelbin-4.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pixelbin"
-version = "3.2.0"
+version = "4.0.0"
 description = "Pixelbin SDK for Python"
 authors = ["Pixelbin <dev@pixelbin.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pixelbin-dev/pixelbin-python-sdk"
 repository = "https://github.com/pixelbin-dev/pixelbin-python-sdk"
 keywords = ["Pixelbin"]
```

### Comparing `pixelbin-3.2.0/setup.py` & `pixelbin-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
  'marshmallow>=3.15.0,<4.0.0',
  'pytest>=7.2.2,<8.0.0',
  'pytz>=2022.1,<2023.0',
  'ujson>=5.2.0,<6.0.0']
 
 setup_kwargs = {
     'name': 'pixelbin',
-    'version': '3.2.0',
+    'version': '4.0.0',
     'description': 'Pixelbin SDK for Python',
-    'long_description': '# Pixelbin Backend SDK for Python\n\nPixelbin Backend SDK for python helps you integrate the core Pixelbin features with your application.\n\n## Getting Started\n\nGetting started with Pixelbin Backend SDK for Python\n\n### Installation\n\n```\npip install pixelbin\n```\n\n---\n\n### Usage\n\n#### Quick Example\n\n```python\nimport asyncio\n\nfrom pixelbin import PixelbinClient, PixelbinConfig\n\n# create client with your API_TOKEN\nconfig = PixelbinConfig({\n    "domain": "https://api.pixelbin.io",\n    "apiSecret": "API_TOKEN",\n})\n\n# Create a pixelbin instance\npixelbin:PixelbinClient = PixelbinClient(config=config)\n\n# Sync method call\ntry:\n    result = pixelbin.assets.listFiles()\n    print(result)\nexcept Exception as e:\n    print(e)\n\n# Async method call\ntry:\n    result = asyncio.get_event_loop().run_until_complete(pixelbin.assets.listFilesAsync())\n    print(result)\nexcept Exception as e:\n    print(e)\n```\n\n## Security Utils\n\n### For generating Signed URLs\n\nGenerate a signed PixelBin url\n\n| Parameter                  | Description                                          | Example                                                                                    |\n| -------------------------- | ---------------------------------------------------- | ------------------------------------------------------------------------------------------ |\n| `url` (string)             | A valid Pixelbin URL to be signed                    | `https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg` |\n| `expiry_seconds` (int)     | Number of seconds the signed URL should be valid for | `20`                                                                                       |\n| `token_id` (int or string) | ID of the token used for signing                     | `42`                                                                                       |\n| `token` (string)           | Value of the token used for signing                  | `dummy-token`                                                                              |\n\nExample:\n\n```python\nfrom pixelbin.utils.security import sign_url\n\nsigned_url = sign_url(\n    "https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg", # url\n    20, # expiry_seconds\n    42, # token_id\n    "dummy-token", # token\n);\n# signed_url\n# https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg?pbs=8eb6a00af74e57967a42316e4de238aa88d92961649764fad1832c1bff101f25&pbe=1695635915&pbt=1\n```\n\nUsage with custom domain url\n\n```python\nfrom pixelbin.utils.security import sign_url\n\nsigned_url = sign_url(\n    "https://test.example.com/v2/original/__playground/playground-default.jpeg", # url\n    30, # expirySeconds\n    22, # tokenId\n    "dummy-token", # token\n);\n# signedUrl\n# https://test.example.com/v2/original/__playground/playground-default.jpeg?pbs=1aef31c1e0ecd8a875b1d3184f324327f4ab4bce419d81d1eb1a818ee5f2e3eb&pbe=1695705975&pbt=22\n```\n\n## URL Utils\n\nPixelbin provides url utilities to construct and deconstruct Pixelbin urls.\n\n### url_to_obj\n\nDeconstruct a pixelbin url\n\n| parameter               | description                                                        | example                                                                                               |\n| ----------------------- | ------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------- |\n| `url` (string)          | A valid Pixelbin URL                                               | `https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg` |\n| `opts` (Object)         | Options for the conversion                                         | Default: `{ isCustomDomain: False }`                                                                  |\n| `opts.is_custom_domain` | Indicates if the URL belongs to a custom domain (default: `False`) |\n\n**Returns**:\n\n| Property                  | Description                                          | Example                               |\n| ------------------------- | ---------------------------------------------------- | ------------------------------------- |\n| `baseURL` (string)        | Base path of the URL                                 | `https://cdn.pixelbin.io`             |\n| `filePath` (string)       | Path to the file on Pixelbin storage                 | `/path/to/image.jpeg`                 |\n| `version` (string)        | Version of the URL                                   | `v2`                                  |\n| `cloudName` (string)      | Cloud name from the URL                              | `your-cloud-name`                     |\n| `transformations` (array) | A list of transformation objects                     | `[{ "plugin": "t", "name": "flip" }]` |\n| `zone` (string)           | Zone slug from the URL                               | `z-slug`                              |\n| `pattern` (string)        | Transformation pattern extracted from the URL        | `t.resize(h:100,w:200)~t.flip()`      |\n| `worker` (boolean)        | Indicates if the URL is a URL Translation Worker URL | `False`                               |\n| `workerPath` (string)     | Input path to a URL Translation Worker               | `resize:w200,h400/folder/image.jpeg`  |\n| `options` (Object)        | Query parameters added, such as "dpr" and "f_auto"   | `{ dpr: 2.5, f_auto: True}`           |\n\nExample:\n\n```python\nfrom pixelbin.utils.url import url_to_obj\n\npixelbinUrl = "https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg?dpr=2.0&f_auto=true"\nobj = url_to_obj(pixelbinUrl)\n# obj\n# {\n#     "cloudName": "your-cloud-name",\n#     "zone": "z-slug",\n#     "version": "v2",\n#     "options": {\n#         "dpr": 2.0,\n#         "f_auto": True,\n#     },\n#     "transformations": [\n#         {\n#             "plugin": "t",\n#             "name": "resize",\n#             "values": [\n#                 {\n#                     "key": "h",\n#                     "value": "100"\n#                 },\n#                 {\n#                     "key": "w",\n#                     "value": "200"\n#                 }\n#             ]\n#         },\n#         {\n#             "plugin": "t",\n#             "name": "flip",\n#         }\n#     ],\n#     "filePath": "path/to/image.jpeg",\n#     "baseUrl": "https://cdn.pixelbin.io"\n# }\n```\n\n```python\nfrom pixelbin.utils.url import url_to_obj\n\ncustomDomainUrl =\n    "https://xyz.designify.media/v2/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg";\nobj = url_to_obj(customDomainUrl, opts={ is_custom_domain: True })\n# obj\n# {\n#     "zone": "z-slug",\n#     "version": "v2",\n#     "transformations": [\n#         {\n#             "plugin": "t",\n#             "name": "resize",\n#             "values": [\n#                 {\n#                     "key": "h",\n#                     "value": "100"\n#                 },\n#                 {\n#                     "key": "w",\n#                     "value": "200"\n#                 }\n#             ]\n#         },\n#         {\n#             "plugin": "t",\n#             "name": "flip",\n#         }\n#     ],\n#     "filePath": "path/to/image.jpeg",\n#     "baseUrl": "https://xyz.designify.media",\n#     "wrkr": False,\n#     "workerPath": "",\n#     "options": {}\n# }\n```\n\n````python\nworkerUrl =\n    "https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/wrkr/resize:h100,w:200/folder/image.jpeg";\n\nobj = url_to_obj(workerUrl)\n# obj\n# {\n#     "cloudName": "your-cloud-name",\n#     "zone": "z-slug",\n#     "version": "v2",\n#     "transformations": [],\n#     "filePath": "",\n#     "worker": True,\n#     "workerPath": "resize:h100,w:200/folder/image.jpeg",\n#     "baseUrl": "https://cdn.pixelbin.io"\n#     "options": {}\n# }\n\n### obj_to_url\n\nConverts the extracted url obj to a Pixelbin url.\n\n| Property                   | Description                                          | Example                               |\n| -------------------------- | ---------------------------------------------------- | ------------------------------------- |\n| `cloudName` (string)       | The cloudname extracted from the URL                 | `your-cloud-name`                     |\n| `zone` (string)            | 6 character zone slug                                | `z-slug`                              |\n| `version` (string)         | CDN API version                                      | `v2`                                  |\n| `transformations` (array)  | Extracted transformations from the URL               | `[{ "plugin": "t", "name": "flip" }]` |\n| `filePath` (string)        | Path to the file on Pixelbin storage                 | `/path/to/image.jpeg`                 |\n| `baseUrl` (string)         | Base URL                                             | `https://cdn.pixelbin.io/`            |\n| `isCustomDomain` (boolean) | Indicates if the URL is for a custom domain          | `False`                               |\n| `worker` (boolean)         | Indicates if the URL is a URL Translation Worker URL | `False`                               |\n| `workerPath` (string)      | Input path to a URL Translation Worker               | `resize:w200,h400/folder/image.jpeg`  |\n| `options` (Object)         | Query parameters added, such as "dpr" and "f_auto"   | `{ "dpr": 2.0, "f_auto": True }`    |\n\n```python\nfrom pixelbin.utils.url import obj_to_url\n\nobj = {\n    cloudName: "your-cloud-name",\n    zone: "z-slug",\n    version: "v2",\n    options: {\n        dpr: 2.0,\n        f_auto: True,\n    },\n    transformations: [\n        {\n            plugin: "t",\n            name: "resize",\n            values: [\n                {\n                    key: "h",\n                    value: "100",\n                },\n                {\n                    key: "w",\n                    value: "200",\n                },\n            ],\n        },\n        {\n            plugin: "t",\n            name: "flip",\n        },\n    ],\n    filePath: "path/to/image.jpeg",\n    baseUrl: "https://cdn.pixelbin.io",\n}\nurl = obj_to_url(obj) # obj is as shown above\n# url\n# https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg?dpr=2.0&f_auto=true\n````\n\nUsage with custom domain\n\n```python\nfrom pixelbin.utils.url import obj_to_url\n\nobj = {\n    zone: "z-slug",\n    version: "v2",\n    transformations: [\n        {\n            plugin: "t",\n            name: "resize",\n            values: [\n                {\n                    key: "h",\n                    value: "100",\n                },\n                {\n                    key: "w",\n                    value: "200",\n                },\n            ],\n        },\n        {\n            plugin: "t",\n            name: "flip",\n        },\n    ],\n    filePath: "path/to/image.jpeg",\n    baseUrl: "https://xyz.designify.media",\n    isCustomDomain: True,\n};\nurl = Pixelbin.utils.objToUrl(obj); # obj is as shown above\n# url\n# https://xyz.designify.media/v2/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg\n```\n\nUsage with URL Translation Worker\n\n```python\nfrom pixelbin.utils.url import obj_to_url\n\nobj = {\n    cloudName: "your-cloud-name",\n    zone: "z-slug",\n    version: "v2",\n    transformations: [],\n    filePath: "",\n    worker: True,\n    workerPath: "resize:h100,w:200/folder/image.jpeg",\n    baseUrl: "https://cdn.pixelbin.io",\n};\nurl = Pixelbin.utils.objToUrl(obj); # obj is as shown above\n# url\n# https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/wrkr/resize:h100,w:200/folder/image.jpeg\n```\n\n## Documentation\n\n-   [API docs](documentation/platform/README.md)\n',
+    'long_description': '# Pixelbin Backend SDK for Python\n\nPixelbin Backend SDK for python helps you integrate the core Pixelbin features with your application.\n\n## Getting Started\n\nGetting started with Pixelbin Backend SDK for Python\n\n### Installation\n\n```\npip install pixelbin\n```\n\n---\n\n### Usage\n\n#### Quick Example\n\n```python\nimport asyncio\n\nfrom pixelbin import PixelbinClient, PixelbinConfig\n\n# create client with your API_TOKEN\nconfig = PixelbinConfig({\n    "domain": "https://api.pixelbin.io",\n    "apiSecret": "API_TOKEN",\n})\n\n# Create a pixelbin instance\npixelbin:PixelbinClient = PixelbinClient(config=config)\n\n# Sync method call\ntry:\n    result = pixelbin.assets.listFiles()\n    print(result)\nexcept Exception as e:\n    print(e)\n\n# Async method call\ntry:\n    result = asyncio.get_event_loop().run_until_complete(pixelbin.assets.listFilesAsync())\n    print(result)\nexcept Exception as e:\n    print(e)\n```\n\n## Security Utils\n\n### For generating Signed URLs\n\nGenerate a signed PixelBin url\n\n| Parameter              | Description                                          | Example                                                                                    |\n| ---------------------- | ---------------------------------------------------- | ------------------------------------------------------------------------------------------ |\n| `url` (string)         | A valid Pixelbin URL to be signed                    | `https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg` |\n| `expiry_seconds` (int) | Number of seconds the signed URL should be valid for | `20`                                                                                       |\n| `access_key` (string)  | Access key of the token used for signing             | `6227274d-92c9-4b74-bef8-2528542516d8`                                                     |\n| `token` (string)       | Value of the token used for signing                  | `dummy-token`                                                                              |\n\nExample:\n\n```python\nfrom pixelbin.utils.security import sign_url\n\nsigned_url = sign_url(\n    "https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg", # url\n    20, # expiry_seconds\n    "6227274d-92c9-4b74-bef8-2528542516d8", # access_key\n    "dummy-token", # token\n);\n# signed_url\n# https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg?pbs=8eb6a00af74e57967a42316e4de238aa88d92961649764fad1832c1bff101f25&pbe=1695635915&pbt=6227274d-92c9-4b74-bef8-2528542516d8\n```\n\nUsage with custom domain url\n\n```python\nfrom pixelbin.utils.security import sign_url\n\nsigned_url = sign_url(\n    "https://test.example.com/v2/original/__playground/playground-default.jpeg", # url\n    30, # expirySeconds\n    22, # tokenId\n    "dummy-token", # token\n);\n# signedUrl\n# https://test.example.com/v2/original/__playground/playground-default.jpeg?pbs=1aef31c1e0ecd8a875b1d3184f324327f4ab4bce419d81d1eb1a818ee5f2e3eb&pbe=1695705975&pbt=22\n```\n\n## URL Utils\n\nPixelbin provides url utilities to construct and deconstruct Pixelbin urls.\n\n### url_to_obj\n\nDeconstruct a pixelbin url\n\n| parameter               | description                                                        | example                                                                                               |\n| ----------------------- | ------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------- |\n| `url` (string)          | A valid Pixelbin URL                                               | `https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg` |\n| `opts` (Object)         | Options for the conversion                                         | Default: `{ isCustomDomain: False }`                                                                  |\n| `opts.is_custom_domain` | Indicates if the URL belongs to a custom domain (default: `False`) |\n\n**Returns**:\n\n| Property                  | Description                                          | Example                               |\n| ------------------------- | ---------------------------------------------------- | ------------------------------------- |\n| `baseURL` (string)        | Base path of the URL                                 | `https://cdn.pixelbin.io`             |\n| `filePath` (string)       | Path to the file on Pixelbin storage                 | `/path/to/image.jpeg`                 |\n| `version` (string)        | Version of the URL                                   | `v2`                                  |\n| `cloudName` (string)      | Cloud name from the URL                              | `your-cloud-name`                     |\n| `transformations` (array) | A list of transformation objects                     | `[{ "plugin": "t", "name": "flip" }]` |\n| `zone` (string)           | Zone slug from the URL                               | `z-slug`                              |\n| `pattern` (string)        | Transformation pattern extracted from the URL        | `t.resize(h:100,w:200)~t.flip()`      |\n| `worker` (boolean)        | Indicates if the URL is a URL Translation Worker URL | `False`                               |\n| `workerPath` (string)     | Input path to a URL Translation Worker               | `resize:w200,h400/folder/image.jpeg`  |\n| `options` (Object)        | Query parameters added, such as "dpr" and "f_auto"   | `{ dpr: 2.5, f_auto: True}`           |\n\nExample:\n\n```python\nfrom pixelbin.utils.url import url_to_obj\n\npixelbinUrl = "https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg?dpr=2.0&f_auto=true"\nobj = url_to_obj(pixelbinUrl)\n# obj\n# {\n#     "cloudName": "your-cloud-name",\n#     "zone": "z-slug",\n#     "version": "v2",\n#     "options": {\n#         "dpr": 2.0,\n#         "f_auto": True,\n#     },\n#     "transformations": [\n#         {\n#             "plugin": "t",\n#             "name": "resize",\n#             "values": [\n#                 {\n#                     "key": "h",\n#                     "value": "100"\n#                 },\n#                 {\n#                     "key": "w",\n#                     "value": "200"\n#                 }\n#             ]\n#         },\n#         {\n#             "plugin": "t",\n#             "name": "flip",\n#         }\n#     ],\n#     "filePath": "path/to/image.jpeg",\n#     "baseUrl": "https://cdn.pixelbin.io"\n# }\n```\n\n```python\nfrom pixelbin.utils.url import url_to_obj\n\ncustomDomainUrl =\n    "https://xyz.designify.media/v2/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg";\nobj = url_to_obj(customDomainUrl, opts={ is_custom_domain: True })\n# obj\n# {\n#     "zone": "z-slug",\n#     "version": "v2",\n#     "transformations": [\n#         {\n#             "plugin": "t",\n#             "name": "resize",\n#             "values": [\n#                 {\n#                     "key": "h",\n#                     "value": "100"\n#                 },\n#                 {\n#                     "key": "w",\n#                     "value": "200"\n#                 }\n#             ]\n#         },\n#         {\n#             "plugin": "t",\n#             "name": "flip",\n#         }\n#     ],\n#     "filePath": "path/to/image.jpeg",\n#     "baseUrl": "https://xyz.designify.media",\n#     "wrkr": False,\n#     "workerPath": "",\n#     "options": {}\n# }\n```\n\n```python\nworkerUrl =\n    "https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/wrkr/resize:h100,w:200/folder/image.jpeg";\n\nobj = url_to_obj(workerUrl)\n# obj\n# {\n#     "cloudName": "your-cloud-name",\n#     "zone": "z-slug",\n#     "version": "v2",\n#     "transformations": [],\n#     "filePath": "",\n#     "worker": True,\n#     "workerPath": "resize:h100,w:200/folder/image.jpeg",\n#     "baseUrl": "https://cdn.pixelbin.io"\n#     "options": {}\n# }\n```\n\n### obj_to_url\n\nConverts the extracted url obj to a Pixelbin url.\n\n| Property                   | Description                                          | Example                               |\n| -------------------------- | ---------------------------------------------------- | ------------------------------------- |\n| `cloudName` (string)       | The cloudname extracted from the URL                 | `your-cloud-name`                     |\n| `zone` (string)            | 6 character zone slug                                | `z-slug`                              |\n| `version` (string)         | CDN API version                                      | `v2`                                  |\n| `transformations` (array)  | Extracted transformations from the URL               | `[{ "plugin": "t", "name": "flip" }]` |\n| `filePath` (string)        | Path to the file on Pixelbin storage                 | `/path/to/image.jpeg`                 |\n| `baseUrl` (string)         | Base URL                                             | `https://cdn.pixelbin.io/`            |\n| `isCustomDomain` (boolean) | Indicates if the URL is for a custom domain          | `False`                               |\n| `worker` (boolean)         | Indicates if the URL is a URL Translation Worker URL | `False`                               |\n| `workerPath` (string)      | Input path to a URL Translation Worker               | `resize:w200,h400/folder/image.jpeg`  |\n| `options` (Object)         | Query parameters added, such as "dpr" and "f_auto"   | `{ "dpr": 2.0, "f_auto": True }`      |\n\n```python\nfrom pixelbin.utils.url import obj_to_url\n\nobj = {\n    cloudName: "your-cloud-name",\n    zone: "z-slug",\n    version: "v2",\n    options: {\n        dpr: 2.0,\n        f_auto: True,\n    },\n    transformations: [\n        {\n            plugin: "t",\n            name: "resize",\n            values: [\n                {\n                    key: "h",\n                    value: "100",\n                },\n                {\n                    key: "w",\n                    value: "200",\n                },\n            ],\n        },\n        {\n            plugin: "t",\n            name: "flip",\n        },\n    ],\n    filePath: "path/to/image.jpeg",\n    baseUrl: "https://cdn.pixelbin.io",\n}\nurl = obj_to_url(obj) # obj is as shown above\n# url\n# https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg?dpr=2.0&f_auto=true\n```\n\nUsage with custom domain\n\n```python\nfrom pixelbin.utils.url import obj_to_url\n\nobj = {\n    zone: "z-slug",\n    version: "v2",\n    transformations: [\n        {\n            plugin: "t",\n            name: "resize",\n            values: [\n                {\n                    key: "h",\n                    value: "100",\n                },\n                {\n                    key: "w",\n                    value: "200",\n                },\n            ],\n        },\n        {\n            plugin: "t",\n            name: "flip",\n        },\n    ],\n    filePath: "path/to/image.jpeg",\n    baseUrl: "https://xyz.designify.media",\n    isCustomDomain: True,\n};\nurl = Pixelbin.utils.objToUrl(obj); # obj is as shown above\n# url\n# https://xyz.designify.media/v2/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg\n```\n\nUsage with URL Translation Worker\n\n```python\nfrom pixelbin.utils.url import obj_to_url\n\nobj = {\n    cloudName: "your-cloud-name",\n    zone: "z-slug",\n    version: "v2",\n    transformations: [],\n    filePath: "",\n    worker: True,\n    workerPath: "resize:h100,w:200/folder/image.jpeg",\n    baseUrl: "https://cdn.pixelbin.io",\n};\nurl = Pixelbin.utils.objToUrl(obj); # obj is as shown above\n# url\n# https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/wrkr/resize:h100,w:200/folder/image.jpeg\n```\n\n## Documentation\n\n-   [API docs](documentation/platform/README.md)\n',
     'author': 'Pixelbin',
     'author_email': 'dev@pixelbin.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/pixelbin-dev/pixelbin-python-sdk',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pixelbin-3.2.0/PKG-INFO` & `pixelbin-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelbin
-Version: 3.2.0
+Version: 4.0.0
 Summary: Pixelbin SDK for Python
 Home-page: https://github.com/pixelbin-dev/pixelbin-python-sdk
 License: MIT
 Keywords: Pixelbin
 Author: Pixelbin
 Author-email: dev@pixelbin.io
 Requires-Python: >=3.8,<4.0
@@ -73,34 +73,34 @@
 
 ## Security Utils
 
 ### For generating Signed URLs
 
 Generate a signed PixelBin url
 
-| Parameter                  | Description                                          | Example                                                                                    |
-| -------------------------- | ---------------------------------------------------- | ------------------------------------------------------------------------------------------ |
-| `url` (string)             | A valid Pixelbin URL to be signed                    | `https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg` |
-| `expiry_seconds` (int)     | Number of seconds the signed URL should be valid for | `20`                                                                                       |
-| `token_id` (int or string) | ID of the token used for signing                     | `42`                                                                                       |
-| `token` (string)           | Value of the token used for signing                  | `dummy-token`                                                                              |
+| Parameter              | Description                                          | Example                                                                                    |
+| ---------------------- | ---------------------------------------------------- | ------------------------------------------------------------------------------------------ |
+| `url` (string)         | A valid Pixelbin URL to be signed                    | `https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg` |
+| `expiry_seconds` (int) | Number of seconds the signed URL should be valid for | `20`                                                                                       |
+| `access_key` (string)  | Access key of the token used for signing             | `6227274d-92c9-4b74-bef8-2528542516d8`                                                     |
+| `token` (string)       | Value of the token used for signing                  | `dummy-token`                                                                              |
 
 Example:
 
 ```python
 from pixelbin.utils.security import sign_url
 
 signed_url = sign_url(
     "https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg", # url
     20, # expiry_seconds
-    42, # token_id
+    "6227274d-92c9-4b74-bef8-2528542516d8", # access_key
     "dummy-token", # token
 );
 # signed_url
-# https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg?pbs=8eb6a00af74e57967a42316e4de238aa88d92961649764fad1832c1bff101f25&pbe=1695635915&pbt=1
+# https://cdn.pixelbin.io/v2/dummy-cloudname/original/__playground/playground-default.jpeg?pbs=8eb6a00af74e57967a42316e4de238aa88d92961649764fad1832c1bff101f25&pbe=1695635915&pbt=6227274d-92c9-4b74-bef8-2528542516d8
 ```
 
 Usage with custom domain url
 
 ```python
 from pixelbin.utils.security import sign_url
 
@@ -218,15 +218,15 @@
 #     "baseUrl": "https://xyz.designify.media",
 #     "wrkr": False,
 #     "workerPath": "",
 #     "options": {}
 # }
 ```
 
-````python
+```python
 workerUrl =
     "https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/wrkr/resize:h100,w:200/folder/image.jpeg";
 
 obj = url_to_obj(workerUrl)
 # obj
 # {
 #     "cloudName": "your-cloud-name",
@@ -235,14 +235,15 @@
 #     "transformations": [],
 #     "filePath": "",
 #     "worker": True,
 #     "workerPath": "resize:h100,w:200/folder/image.jpeg",
 #     "baseUrl": "https://cdn.pixelbin.io"
 #     "options": {}
 # }
+```
 
 ### obj_to_url
 
 Converts the extracted url obj to a Pixelbin url.
 
 | Property                   | Description                                          | Example                               |
 | -------------------------- | ---------------------------------------------------- | ------------------------------------- |
@@ -251,15 +252,15 @@
 | `version` (string)         | CDN API version                                      | `v2`                                  |
 | `transformations` (array)  | Extracted transformations from the URL               | `[{ "plugin": "t", "name": "flip" }]` |
 | `filePath` (string)        | Path to the file on Pixelbin storage                 | `/path/to/image.jpeg`                 |
 | `baseUrl` (string)         | Base URL                                             | `https://cdn.pixelbin.io/`            |
 | `isCustomDomain` (boolean) | Indicates if the URL is for a custom domain          | `False`                               |
 | `worker` (boolean)         | Indicates if the URL is a URL Translation Worker URL | `False`                               |
 | `workerPath` (string)      | Input path to a URL Translation Worker               | `resize:w200,h400/folder/image.jpeg`  |
-| `options` (Object)         | Query parameters added, such as "dpr" and "f_auto"   | `{ "dpr": 2.0, "f_auto": True }`    |
+| `options` (Object)         | Query parameters added, such as "dpr" and "f_auto"   | `{ "dpr": 2.0, "f_auto": True }`      |
 
 ```python
 from pixelbin.utils.url import obj_to_url
 
 obj = {
     cloudName: "your-cloud-name",
     zone: "z-slug",
@@ -290,15 +291,15 @@
     ],
     filePath: "path/to/image.jpeg",
     baseUrl: "https://cdn.pixelbin.io",
 }
 url = obj_to_url(obj) # obj is as shown above
 # url
 # https://cdn.pixelbin.io/v2/your-cloud-name/z-slug/t.resize(h:100,w:200)~t.flip()/path/to/image.jpeg?dpr=2.0&f_auto=true
-````
+```
 
 Usage with custom domain
 
 ```python
 from pixelbin.utils.url import obj_to_url
 
 obj = {
```

