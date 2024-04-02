# Comparing `tmp/imagekitio-4.0.0.tar.gz` & `tmp/imagekitio-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imagekitio-4.0.0.tar", last modified: Fri Feb  9 06:44:33 2024, max compression
+gzip compressed data, was "imagekitio-4.0.1.tar", last modified: Tue Apr  2 11:55:40 2024, max compression
```

## Comparing `imagekitio-4.0.0.tar` & `imagekitio-4.0.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:33.802516 imagekitio-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-09 06:44:11.000000 imagekitio-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    49535 2024-02-09 06:44:33.798516 imagekitio-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    49139 2024-02-09 06:44:11.000000 imagekitio-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:33.790516 imagekitio-4.0.0/imagekitio/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:33.790516 imagekitio-4.0.0/imagekitio/constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/constants/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/constants/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/constants/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/constants/supported_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/constants/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:33.790516 imagekitio-4.0.0/imagekitio/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/exceptions/BadRequestException.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/exceptions/ConflictException.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/exceptions/ForbiddenException.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/exceptions/InternalServerException.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/exceptions/NotFoundException.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/exceptions/PartialSuccessException.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/exceptions/TooManyRequestsException.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/exceptions/UnauthorizedException.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/exceptions/UnknownException.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37166 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:33.794516 imagekitio-4.0.0/imagekitio/models/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/CopyFileRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/CopyFolderRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/CreateCustomMetadataFieldsRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/CreateFolderRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/CustomMetaDataTypeEnum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/CustomMetadataFieldsSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/DeleteFolderRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/ListAndSearchFileRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/MoveFileRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/MoveFolderRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/RenameFileRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/UpdateCustomMetadataFieldsRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/UpdateFileRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/UploadFileRequestOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:33.798516 imagekitio-4.0.0/imagekitio/models/results/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/AITags.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/BulkDeleteFileResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/CustomMetadataFieldsResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/CustomMetadataFieldsResultWithResponseMetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/CustomMetadataSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/EmbeddedMetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/FileResult.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/FileResultWithResponseMetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/FolderResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/GetBulkJobStatusResult.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/GetMetadataResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/ListCustomMetadataFieldsResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/ListFileResult.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/MetadataExif.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/MetadataExifExif.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/MetadataExifGPS.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/MetadataExifImage.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/MetadataExifInteroperability.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/MetadataExifThumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/PurgeCacheResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/PurgeCacheStatusResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/RenameFileResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/ResponseMetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/ResponseMetadataResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/TagsResult.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/UploadFileResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/VersionInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/models/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:33.798516 imagekitio-4.0.0/imagekitio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/utils/calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-02-09 06:44:11.000000 imagekitio-4.0.0/imagekitio/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:33.790516 imagekitio-4.0.0/imagekitio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    49535 2024-02-09 06:44:33.000000 imagekitio-4.0.0/imagekitio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-02-09 06:44:33.000000 imagekitio-4.0.0/imagekitio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 06:44:33.000000 imagekitio-4.0.0/imagekitio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-09 06:44:33.000000 imagekitio-4.0.0/imagekitio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-09 06:44:33.000000 imagekitio-4.0.0/imagekitio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 06:44:33.802516 imagekitio-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-09 06:44:11.000000 imagekitio-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:33.798516 imagekitio-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:11.000000 imagekitio-4.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 06:44:33.798516 imagekitio-4.0.0/tests/dummy_data/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-09 06:44:11.000000 imagekitio-4.0.0/tests/dummy_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-02-09 06:44:11.000000 imagekitio-4.0.0/tests/dummy_data/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-09 06:44:11.000000 imagekitio-4.0.0/tests/dummy_data/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-02-09 06:44:11.000000 imagekitio-4.0.0/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-02-09 06:44:11.000000 imagekitio-4.0.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    35697 2024-02-09 06:44:11.000000 imagekitio-4.0.0/tests/test_custom_metadata_fields_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)   550898 2024-02-09 06:44:11.000000 imagekitio-4.0.0/tests/test_files_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    20838 2024-02-09 06:44:11.000000 imagekitio-4.0.0/tests/test_folder_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    16145 2024-02-09 06:44:11.000000 imagekitio-4.0.0/tests/test_generate_url.py
--rw-r--r--   0 runner    (1001) docker     (127)    11201 2024-02-09 06:44:11.000000 imagekitio-4.0.0/tests/test_models_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    12294 2024-02-09 06:44:11.000000 imagekitio-4.0.0/tests/test_tags_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-09 06:44:11.000000 imagekitio-4.0.0/tests/test_utils_calculation.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-02-09 06:44:11.000000 imagekitio-4.0.0/tests/test_utils_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-02-09 06:44:11.000000 imagekitio-4.0.0/tests/test_utils_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:40.918028 imagekitio-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-02 11:55:18.000000 imagekitio-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    49535 2024-04-02 11:55:40.918028 imagekitio-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    49139 2024-04-02 11:55:18.000000 imagekitio-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:40.906028 imagekitio-4.0.1/imagekitio/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:40.910028 imagekitio-4.0.1/imagekitio/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/constants/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/constants/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/constants/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/constants/supported_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/constants/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:40.910028 imagekitio-4.0.1/imagekitio/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/exceptions/BadRequestException.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/exceptions/ConflictException.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/exceptions/ForbiddenException.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/exceptions/InternalServerException.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/exceptions/NotFoundException.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/exceptions/PartialSuccessException.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/exceptions/TooManyRequestsException.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/exceptions/UnauthorizedException.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/exceptions/UnknownException.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37166 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:40.910028 imagekitio-4.0.1/imagekitio/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/CopyFileRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/CopyFolderRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/CreateCustomMetadataFieldsRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/CreateFolderRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/CustomMetaDataTypeEnum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/CustomMetadataFieldsSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/DeleteFolderRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/ListAndSearchFileRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/MoveFileRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/MoveFolderRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/RenameFileRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/UpdateCustomMetadataFieldsRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/UpdateFileRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/UploadFileRequestOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:40.914028 imagekitio-4.0.1/imagekitio/models/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/AITags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/BulkDeleteFileResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/CustomMetadataFieldsResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/CustomMetadataFieldsResultWithResponseMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/CustomMetadataSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/EmbeddedMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/FileResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/FileResultWithResponseMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/FolderResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/GetBulkJobStatusResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/GetMetadataResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/ListCustomMetadataFieldsResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/ListFileResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/MetadataExif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/MetadataExifExif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/MetadataExifGPS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/MetadataExifImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/MetadataExifInteroperability.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/MetadataExifThumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/PurgeCacheResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/PurgeCacheStatusResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/RenameFileResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/ResponseMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/ResponseMetadataResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/TagsResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/UploadFileResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/VersionInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/models/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9137 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:40.914028 imagekitio-4.0.1/imagekitio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/utils/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-04-02 11:55:18.000000 imagekitio-4.0.1/imagekitio/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:40.906028 imagekitio-4.0.1/imagekitio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    49535 2024-04-02 11:55:40.000000 imagekitio-4.0.1/imagekitio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-02 11:55:40.000000 imagekitio-4.0.1/imagekitio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:55:40.000000 imagekitio-4.0.1/imagekitio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 11:55:40.000000 imagekitio-4.0.1/imagekitio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 11:55:40.000000 imagekitio-4.0.1/imagekitio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 11:55:40.918028 imagekitio-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-02 11:55:18.000000 imagekitio-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:40.918028 imagekitio-4.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:18.000000 imagekitio-4.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:40.918028 imagekitio-4.0.1/tests/dummy_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 11:55:18.000000 imagekitio-4.0.1/tests/dummy_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-02 11:55:18.000000 imagekitio-4.0.1/tests/dummy_data/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-02 11:55:18.000000 imagekitio-4.0.1/tests/dummy_data/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-02 11:55:18.000000 imagekitio-4.0.1/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-02 11:55:18.000000 imagekitio-4.0.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35697 2024-04-02 11:55:18.000000 imagekitio-4.0.1/tests/test_custom_metadata_fields_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)   550898 2024-04-02 11:55:18.000000 imagekitio-4.0.1/tests/test_files_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20838 2024-04-02 11:55:18.000000 imagekitio-4.0.1/tests/test_folder_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19858 2024-04-02 11:55:18.000000 imagekitio-4.0.1/tests/test_generate_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11201 2024-04-02 11:55:18.000000 imagekitio-4.0.1/tests/test_models_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12294 2024-04-02 11:55:18.000000 imagekitio-4.0.1/tests/test_tags_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-02 11:55:18.000000 imagekitio-4.0.1/tests/test_utils_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-02 11:55:18.000000 imagekitio-4.0.1/tests/test_utils_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-02 11:55:18.000000 imagekitio-4.0.1/tests/test_utils_utils.py
```

### Comparing `imagekitio-4.0.0/LICENSE` & `imagekitio-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/PKG-INFO` & `imagekitio-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imagekitio
-Version: 4.0.0
+Version: 4.0.1
 Summary: Python wrapper for the ImageKit API
 Home-page: https://github.com/imagekit-developer/imagekit-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `imagekitio-4.0.0/README.md` & `imagekitio-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/client.py` & `imagekitio-4.0.1/imagekitio/client.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/constants/defaults.py` & `imagekitio-4.0.1/imagekitio/constants/defaults.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,7 +12,8 @@
     SDK_VERSION = "python-3.2.0"
     TRANSFORMATION_PARAMETER = "tr"
     CHAIN_TRANSFORM_DELIMITER = ":"
     TRANSFORM_DELIMITER = ","
     TRANSFORM_KEY_VALUE_DELIMITER = "-"
     SIGNATURE_PARAMETER = "ik-s"
     TIMESTAMP_PARAMETER = "ik-t"
+    IGNORE_CHARACTERS = '~@#$&()*!+=:;,?/\''
```

### Comparing `imagekitio-4.0.0/imagekitio/constants/errors.py` & `imagekitio-4.0.1/imagekitio/constants/errors.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/constants/files.py` & `imagekitio-4.0.1/imagekitio/constants/files.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/constants/supported_transform.py` & `imagekitio-4.0.1/imagekitio/constants/supported_transform.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/file.py` & `imagekitio-4.0.1/imagekitio/file.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/CreateCustomMetadataFieldsRequestOptions.py` & `imagekitio-4.0.1/imagekitio/models/CreateCustomMetadataFieldsRequestOptions.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/CustomMetadataFieldsSchema.py` & `imagekitio-4.0.1/imagekitio/models/CustomMetadataFieldsSchema.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/ListAndSearchFileRequestOptions.py` & `imagekitio-4.0.1/imagekitio/models/ListAndSearchFileRequestOptions.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/UpdateCustomMetadataFieldsRequestOptions.py` & `imagekitio-4.0.1/imagekitio/models/UpdateCustomMetadataFieldsRequestOptions.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/UpdateFileRequestOptions.py` & `imagekitio-4.0.1/imagekitio/models/UpdateFileRequestOptions.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/UploadFileRequestOptions.py` & `imagekitio-4.0.1/imagekitio/models/UploadFileRequestOptions.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/BulkDeleteFileResult.py` & `imagekitio-4.0.1/imagekitio/models/results/BulkDeleteFileResult.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/CustomMetadataFieldsResult.py` & `imagekitio-4.0.1/imagekitio/models/results/CustomMetadataFieldsResult.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/CustomMetadataFieldsResultWithResponseMetadata.py` & `imagekitio-4.0.1/imagekitio/models/results/CustomMetadataFieldsResultWithResponseMetadata.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/CustomMetadataSchema.py` & `imagekitio-4.0.1/imagekitio/models/results/CustomMetadataSchema.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/FileResult.py` & `imagekitio-4.0.1/imagekitio/models/results/FileResult.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/FileResultWithResponseMetadata.py` & `imagekitio-4.0.1/imagekitio/models/results/FileResultWithResponseMetadata.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/FolderResult.py` & `imagekitio-4.0.1/imagekitio/models/results/FolderResult.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/GetBulkJobStatusResult.py` & `imagekitio-4.0.1/imagekitio/models/results/GetBulkJobStatusResult.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/GetMetadataResult.py` & `imagekitio-4.0.1/imagekitio/models/results/GetMetadataResult.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/ListCustomMetadataFieldsResult.py` & `imagekitio-4.0.1/imagekitio/models/results/ListCustomMetadataFieldsResult.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/MetadataExif.py` & `imagekitio-4.0.1/imagekitio/models/results/MetadataExif.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/MetadataExifExif.py` & `imagekitio-4.0.1/imagekitio/models/results/MetadataExifExif.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/MetadataExifImage.py` & `imagekitio-4.0.1/imagekitio/models/results/MetadataExifImage.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/MetadataExifThumbnail.py` & `imagekitio-4.0.1/imagekitio/models/results/MetadataExifThumbnail.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/TagsResult.py` & `imagekitio-4.0.1/imagekitio/models/results/TagsResult.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/models/results/UploadFileResult.py` & `imagekitio-4.0.1/imagekitio/models/results/UploadFileResult.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/resource.py` & `imagekitio-4.0.1/imagekitio/resource.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/url.py` & `imagekitio-4.0.1/imagekitio/url.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import hashlib
 import hmac
 import sys
 from datetime import datetime as dt
 from typing import Any, Dict, List
-from urllib.parse import ParseResult, urlparse, urlunparse, parse_qsl, urlencode
+from urllib.parse import ParseResult, urlparse, urlunparse, parse_qsl, urlencode, quote, unquote
 
 from .constants.defaults import Default
 from .constants.supported_transform import SUPPORTED_TRANS
 from .utils.formatter import camel_dict_to_snake_dict, flatten_dict
 
 from .constants.errors import ERRORS
 
@@ -138,15 +138,15 @@
         if url_endpoint[-1] != "/":
             url_endpoint += "/"
 
         if expiry_timestamp < 1:
             expiry_timestamp = Default.DEFAULT_TIMESTAMP.value
 
         replaced_url = url.replace(url_endpoint, "") + str(expiry_timestamp)
-
+        replaced_url = Url.encode_string_if_required(replaced_url)
         signature = hmac.new(
             key=private_key.encode(), msg=replaced_url.encode(), digestmod=hashlib.sha1
         )
         return signature.hexdigest()
 
     @staticmethod
     def is_valid_trans_options(options: Dict[str, Any]) -> bool:
@@ -207,7 +207,25 @@
                         )
 
             parsed_transforms.append(
                 Default.TRANSFORM_DELIMITER.value.join(parsed_transform_step)
             )
 
         return Default.CHAIN_TRANSFORM_DELIMITER.value.join(parsed_transforms)
+
+    @staticmethod
+    def encodeURI(url_str):
+        # https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/encodeURI
+        if "?" in url_str:
+            # here we are not encoding query parameters as it is allready encoded
+            encoded_url = quote(url_str.split('?')[0], safe=Default.IGNORE_CHARACTERS.value)+"?"+url_str.split('?')[1]
+        else:
+            encoded_url = quote(url_str, safe=Default.IGNORE_CHARACTERS.value)
+        return encoded_url
+
+    @staticmethod
+    def has_more_than_ascii(s):
+        return any(ord(char) > 127 for char in s)
+        
+    @staticmethod
+    def encode_string_if_required(s):
+        return Url.encodeURI(s) if Url.has_more_than_ascii(s) else s
```

### Comparing `imagekitio-4.0.0/imagekitio/utils/calculation.py` & `imagekitio-4.0.1/imagekitio/utils/calculation.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/utils/formatter.py` & `imagekitio-4.0.1/imagekitio/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio/utils/utils.py` & `imagekitio-4.0.1/imagekitio/utils/utils.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/imagekitio.egg-info/PKG-INFO` & `imagekitio-4.0.1/imagekitio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imagekitio
-Version: 4.0.0
+Version: 4.0.1
 Summary: Python wrapper for the ImageKit API
 Home-page: https://github.com/imagekit-developer/imagekit-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `imagekitio-4.0.0/imagekitio.egg-info/SOURCES.txt` & `imagekitio-4.0.1/imagekitio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/setup.py` & `imagekitio-4.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements/requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 setuptools.setup(
     name="imagekitio",
-    version="4.0.0",
+    version="4.0.1",
     description="Python wrapper for the ImageKit API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=install_requires,
     url="https://github.com/imagekit-developer/imagekit-python",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `imagekitio-4.0.0/tests/dummy_data/file.py` & `imagekitio-4.0.1/tests/dummy_data/file.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/tests/helpers.py` & `imagekitio-4.0.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/tests/test_client.py` & `imagekitio-4.0.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/tests/test_custom_metadata_fields_ops.py` & `imagekitio-4.0.1/tests/test_custom_metadata_fields_ops.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/tests/test_files_ops.py` & `imagekitio-4.0.1/tests/test_files_ops.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/tests/test_folder_ops.py` & `imagekitio-4.0.1/tests/test_folder_ops.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/tests/test_generate_url.py` & `imagekitio-4.0.1/tests/test_generate_url.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 from imagekitio.client import ImageKit
 from imagekitio.constants.defaults import Default
-
+from imagekitio.url import Url
 
 class TestGenerateURL(unittest.TestCase):
     def setUp(self) -> None:
         self.client = ImageKit(
             private_key="private_key_test",
             public_key="public_key_test",
             url_endpoint="https://test-domain.com/test-endpoint",
@@ -322,14 +322,98 @@
             ],
             "signed": True,
             "expire_seconds": 100,
         }
         url = self.client.url(options)
         self.assertIn("ik-t", url)
 
+    def test_url_signed_with_diacritic_in_filename(self):
+        url = "https://test-domain.com/test-endpoint/test_é_path_alt.jpg"
+        encodedUrl = Url.encode_string_if_required(url)
+        self.assertEqual(
+            encodedUrl,
+            "https://test-domain.com/test-endpoint/test_%C3%A9_path_alt.jpg",
+        )
+        signature = Url.get_signature("private_key_test", url, "https://test-domain.com/test-endpoint", 9999999999)
+        options = {
+            "path": "/test_é_path_alt.jpg",
+            "signed": True,
+        }
+        url = self.client.url(options)
+        self.assertEqual(
+            url,
+            "https://test-domain.com/test-endpoint/test_é_path_alt.jpg?ik-s="+signature,
+        )
+
+    def test_url_signed_with_diacritic_in_filename_and_path(self):
+        url = "https://test-domain.com/test-endpoint/aéb/test_é_path_alt.jpg"
+        encodedUrl = Url.encode_string_if_required(url)
+        self.assertEqual(
+            encodedUrl,
+            "https://test-domain.com/test-endpoint/a%C3%A9b/test_%C3%A9_path_alt.jpg",
+        )
+        signature = Url.get_signature("private_key_test", url, "https://test-domain.com/test-endpoint", 9999999999)
+        options = {
+            "path": "/aéb/test_é_path_alt.jpg",
+            "signed": True,
+        }
+        url = self.client.url(options)
+        self.assertEqual(
+            url,
+            "https://test-domain.com/test-endpoint/aéb/test_é_path_alt.jpg?ik-s="+signature,
+        )
+
+    def test_url_signed_with_diacritic_in_filename_path_transforamtion_in_path(self):
+        url = "https://test-domain.com/test-endpoint/tr:l-text,i-Imagekité,fs-50,l-end/aéb/test_é_path_alt.jpg"
+        encodedUrl = Url.encode_string_if_required(url)
+        self.assertEqual(
+            encodedUrl,
+            "https://test-domain.com/test-endpoint/tr:l-text,i-Imagekit%C3%A9,fs-50,l-end/a%C3%A9b/test_%C3%A9_path_alt.jpg",
+        )
+        signature = Url.get_signature("private_key_test", url, "https://test-domain.com/test-endpoint", 9999999999)
+        options = {
+            "path": "/aéb/test_é_path_alt.jpg",
+            "transformation": [
+                {
+                    "raw": "l-text,i-Imagekité,fs-50,l-end"
+                },
+            ],
+            "signed": True,
+             "transformation_position": "path"
+        }
+        url = self.client.url(options)
+        self.assertEqual(
+            url,
+            "https://test-domain.com/test-endpoint/tr:l-text,i-Imagekité,fs-50,l-end/aéb/test_é_path_alt.jpg?ik-s="+signature,
+        )
+
+    def test_url_signed_with_diacritic_in_filename_path_transforamtion_in_query(self):
+        url = "https://test-domain.com/test-endpoint/aéb/test_é_path_alt.jpg?tr=l-text%2Ci-Imagekit%C3%A9%2Cfs-50%2Cl-end"
+        encodedUrl = Url.encode_string_if_required(url)
+        self.assertEqual(
+            encodedUrl,
+            "https://test-domain.com/test-endpoint/a%C3%A9b/test_%C3%A9_path_alt.jpg?tr=l-text%2Ci-Imagekit%C3%A9%2Cfs-50%2Cl-end",
+        )
+        signature = Url.get_signature("private_key_test", url, "https://test-domain.com/test-endpoint", 9999999999)
+        options = {
+            "path": "/aéb/test_é_path_alt.jpg",
+            "transformation": [
+                {
+                    "raw": "l-text,i-Imagekité,fs-50,l-end"
+                },
+            ],
+            "signed": True,
+             "transformation_position": "query"
+        }
+        url = self.client.url(options)
+        self.assertEqual(
+            url,
+            "https://test-domain.com/test-endpoint/aéb/test_é_path_alt.jpg?tr=l-text%2Ci-Imagekit%C3%A9%2Cfs-50%2Cl-end&ik-s="+signature,
+        )
+
     def test_generate_url_with_path_and_src_uses_path(self):
         """
         In case when both path and src fields are provided, the `path` should be preferred
         """
         options = {
             "path": "/default-image.jpg",
             "src": "https://ik.imagekit.io/ldt7znpgpjs/test_YhNhoRxWt.jpg",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `imagekitio-4.0.0/tests/test_models_results.py` & `imagekitio-4.0.1/tests/test_models_results.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/tests/test_tags_ops.py` & `imagekitio-4.0.1/tests/test_tags_ops.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/tests/test_utils_calculation.py` & `imagekitio-4.0.1/tests/test_utils_calculation.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/tests/test_utils_formatter.py` & `imagekitio-4.0.1/tests/test_utils_formatter.py`

 * *Files identical despite different names*

### Comparing `imagekitio-4.0.0/tests/test_utils_utils.py` & `imagekitio-4.0.1/tests/test_utils_utils.py`

 * *Files identical despite different names*

