# Comparing `tmp/b2sdk-1.9.0.tar.gz` & `tmp/b2sdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sdk-1.9.0.tar", last modified: Mon Jun  7 22:23:57 2021, max compression
+gzip compressed data, was "b2sdk-2.0.0.tar", last modified: Tue Apr  2 12:02:25 2024, max compression
```

## Comparing `b2sdk-1.9.0.tar` & `b2sdk-2.0.0.tar`

### file list

```diff
@@ -1,327 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.402168 b2sdk-1.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.370168 b2sdk-1.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      697 2021-06-07 22:23:51.000000 b2sdk-1.9.0/.github/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (121)      241 2021-06-07 22:23:51.000000 b2sdk-1.9.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (121)      721 2021-06-07 22:23:51.000000 b2sdk-1.9.0/.github/no-response.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.370168 b2sdk-1.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2021-06-07 22:23:51.000000 b2sdk-1.9.0/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2905 2021-06-07 22:23:51.000000 b2sdk-1.9.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-06-07 22:23:51.000000 b2sdk-1.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      592 2021-06-07 22:23:51.000000 b2sdk-1.9.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     7781 2021-06-07 22:23:51.000000 b2sdk-1.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     3161 2021-06-07 22:23:51.000000 b2sdk-1.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2021-06-07 22:23:51.000000 b2sdk-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-06-07 22:23:51.000000 b2sdk-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3073 2021-06-07 22:23:57.402168 b2sdk-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2021-06-07 22:23:51.000000 b2sdk-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-06-07 22:23:51.000000 b2sdk-1.9.0/README.release.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk/
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk/_pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (121)      516 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/_pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      382 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/_pyinstaller/hook-b2sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk/_v2/
--rw-r--r--   0 runner    (1001) docker     (121)     8550 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5200 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/_v2/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk/account_info/
--rw-r--r--   0 runner    (1001) docker     (121)      369 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11920 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/abstract.py
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     4306 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (121)    21789 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/sqlite_account_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     4176 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/stub.py
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/test_upload_url_concurrency.py
--rw-r--r--   0 runner    (1001) docker     (121)     3545 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/account_info/upload_url_pool.py
--rw-r--r--   0 runner    (1001) docker     (121)    20530 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    17096 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/b2http.py
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/bounded_queue_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)    44096 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/bucket.py
--rw-r--r--   0 runner    (1001) docker     (121)     3064 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     7027 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/download_dest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk/encryption/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11557 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/encryption/setting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/encryption/types.py
--rw-r--r--   0 runner    (1001) docker     (121)    15966 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)    13787 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (121)     8901 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/file_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk/large_file/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/large_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1463 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/large_file/part.py
--rw-r--r--   0 runner    (1001) docker     (121)     4632 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/large_file/services.py
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/large_file/unfinished_large_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     5776 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/progress.py
--rw-r--r--   0 runner    (1001) docker     (121)    46815 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/raw_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    65343 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/raw_simulator.py
--rw-r--r--   0 runner    (1001) docker     (121)    20284 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk/stream/
--rw-r--r--   0 runner    (1001) docker     (121)      570 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/stream/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5261 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/stream/chained.py
--rw-r--r--   0 runner    (1001) docker     (121)     2384 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/stream/hashing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3145 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/stream/progress.py
--rw-r--r--   0 runner    (1001) docker     (121)     2325 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/stream/range.py
--rw-r--r--   0 runner    (1001) docker     (121)     2374 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/stream/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.378168 b2sdk-1.9.0/b2sdk/sync/
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15187 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/action.py
--rw-r--r--   0 runner    (1001) docker     (121)     3967 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/encryption_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     2971 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)    14288 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/folder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2034 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/folder_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2786 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/path.py
--rw-r--r--   0 runner    (1001) docker     (121)    17536 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3862 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/policy_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    11137 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/report.py
--rw-r--r--   0 runner    (1001) docker     (121)     9100 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/scan_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)    15571 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.378168 b2sdk-1.9.0/b2sdk/transfer/
--rw-r--r--   0 runner    (1001) docker     (121)      575 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.378168 b2sdk-1.9.0/b2sdk/transfer/emerge/
--rw-r--r--   0 runner    (1001) docker     (121)      300 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4913 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/emerger.py
--rw-r--r--   0 runner    (1001) docker     (121)    22537 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.378168 b2sdk-1.9.0/b2sdk/transfer/emerge/planner/
--rw-r--r--   0 runner    (1001) docker     (121)      308 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/planner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5317 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/planner/part_definition.py
--rw-r--r--   0 runner    (1001) docker     (121)    29454 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/planner/planner.py
--rw-r--r--   0 runner    (1001) docker     (121)     3546 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/planner/upload_subpart.py
--rw-r--r--   0 runner    (1001) docker     (121)     2742 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/emerge/write_intent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.378168 b2sdk-1.9.0/b2sdk/transfer/inbound/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5584 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/download_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.378168 b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/
--rw-r--r--   0 runner    (1001) docker     (121)      312 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2493 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/abstract.py
--rw-r--r--   0 runner    (1001) docker     (121)    14733 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/range.py
--rw-r--r--   0 runner    (1001) docker     (121)     2984 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/simple.py
--rw-r--r--   0 runner    (1001) docker     (121)     2397 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/inbound/file_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.382168 b2sdk-1.9.0/b2sdk/transfer/outbound/
--rw-r--r--   0 runner    (1001) docker     (121)      302 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11309 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/copy_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2792 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/copy_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     2076 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/large_file_upload_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/outbound_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/progress_reporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     9769 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/upload_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     6964 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/transfer/outbound/upload_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    12435 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.382168 b2sdk-1.9.0/b2sdk/v0/
--rw-r--r--   0 runner    (1001) docker     (121)      670 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v0/account_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      964 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v0/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v0/bucket.py
--rw-r--r--   0 runner    (1001) docker     (121)      930 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v0/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     7265 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v0/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.382168 b2sdk-1.9.0/b2sdk/v1/
--rw-r--r--   0 runner    (1001) docker     (121)      965 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5891 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/account_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3972 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/bucket.py
--rw-r--r--   0 runner    (1001) docker     (121)      533 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     4116 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/file_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.382168 b2sdk-1.9.0/b2sdk/v1/sync/
--rw-r--r--   0 runner    (1001) docker     (121)      448 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3946 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/encryption_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     3838 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/file_to_path_translator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2092 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/folder.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/folder_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     7122 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/scan_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     5171 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/v1/sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     7031 2021-06-07 22:23:51.000000 b2sdk-1.9.0/b2sdk/version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.374168 b2sdk-1.9.0/b2sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3073 2021-06-07 22:23:57.000000 b2sdk-1.9.0/b2sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8254 2021-06-07 22:23:57.000000 b2sdk-1.9.0/b2sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-07 22:23:57.000000 b2sdk-1.9.0/b2sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-06-07 22:23:57.000000 b2sdk-1.9.0/b2sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      317 2021-06-07 22:23:57.000000 b2sdk-1.9.0/b2sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-06-07 22:23:57.000000 b2sdk-1.9.0/b2sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.382168 b2sdk-1.9.0/contrib/
--rwxr-xr-x   0 runner    (1001) docker     (121)      486 2021-06-07 22:23:51.000000 b2sdk-1.9.0/contrib/color-b2-logs.sh
--rw-r--r--   0 runner    (1001) docker     (121)      711 2021-06-07 22:23:51.000000 b2sdk-1.9.0/contrib/debug_logs.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.386168 b2sdk-1.9.0/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/bash_completion.md
--rw-r--r--   0 runner    (1001) docker     (121)     4561 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/markup-test.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)       84 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/render_sqlite_account_info_schema.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.386168 b2sdk-1.9.0/doc/source/
--rw-r--r--   0 runner    (1001) docker     (121)    20807 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/advanced.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.386168 b2sdk-1.9.0/doc/source/api/
--rw-r--r--   0 runner    (1001) docker     (121)     4401 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/account_info.rst
--rw-r--r--   0 runner    (1001) docker     (121)      150 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      147 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/bucket.rst
--rw-r--r--   0 runner    (1001) docker     (121)      548 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/cache.rst
--rw-r--r--   0 runner    (1001) docker     (121)      356 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/data_classes.rst
--rw-r--r--   0 runner    (1001) docker     (121)      659 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/download_dest.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.386168 b2sdk-1.9.0/doc/source/api/encryption/
--rw-r--r--   0 runner    (1001) docker     (121)      410 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/encryption/setting.rst
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/encryption/types.rst
--rw-r--r--   0 runner    (1001) docker     (121)      323 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/enums.rst
--rw-r--r--   0 runner    (1001) docker     (121)      194 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/exception.rst
--rw-r--r--   0 runner    (1001) docker     (121)      895 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/file_lock.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/internal/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/b2http.rst
--rw-r--r--   0 runner    (1001) docker     (121)      164 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/cache.rst
--rw-r--r--   0 runner    (1001) docker     (121)      227 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/download_dest.rst
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/raw_api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      227 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/raw_simulator.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/session.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/internal/stream/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/stream/chained.rst
--rw-r--r--   0 runner    (1001) docker     (121)      214 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/stream/hashing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      249 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/stream/progress.rst
--rw-r--r--   0 runner    (1001) docker     (121)      215 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/stream/range.rst
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/stream/wrapper.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/internal/sync/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/action.rst
--rw-r--r--   0 runner    (1001) docker     (121)      201 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/exception.rst
--rw-r--r--   0 runner    (1001) docker     (121)      183 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/folder.rst
--rw-r--r--   0 runner    (1001) docker     (121)      211 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/folder_parser.rst
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/path.rst
--rw-r--r--   0 runner    (1001) docker     (121)      183 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/policy.rst
--rw-r--r--   0 runner    (1001) docker     (121)      215 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/policy_manager.rst
--rw-r--r--   0 runner    (1001) docker     (121)      211 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/scan_policies.rst
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/sync/sync.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.366168 b2sdk-1.9.0/doc/source/api/internal/transfer/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/download_manager.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/downloader/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/downloader/abstract.rst
--rw-r--r--   0 runner    (1001) docker     (121)      292 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/downloader/parallel.rst
--rw-r--r--   0 runner    (1001) docker     (121)      291 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/downloader/range.rst
--rw-r--r--   0 runner    (1001) docker     (121)      282 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/downloader/simple.rst
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/transfer/inbound/file_metadata.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/internal/transfer/outbound/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/transfer/outbound/upload_source.rst
--rw-r--r--   0 runner    (1001) docker     (121)      177 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/internal/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)      668 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/progress.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8407 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/sync.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.366168 b2sdk-1.9.0/doc/source/api/transfer/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/transfer/emerge/
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/transfer/emerge/write_intent.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/api/transfer/outbound/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/transfer/outbound/outbound_source.rst
--rw-r--r--   0 runner    (1001) docker     (121)      516 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6662 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/api_types.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6630 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3357 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/doc/source/dot/
--rw-r--r--   0 runner    (1001) docker     (121)     4994 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/dot/sqlite_account_info_schema.dot
--rw-r--r--   0 runner    (1001) docker     (121)     2229 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      629 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14360 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/quick_start.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3269 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/server_side_encryption.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3740 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/source/tutorial.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)     1052 2021-06-07 22:23:51.000000 b2sdk-1.9.0/doc/sqlite_account_info_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     6410 2021-06-07 22:23:51.000000 b2sdk-1.9.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-06-07 22:23:51.000000 b2sdk-1.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      940 2021-06-07 22:23:57.402168 b2sdk-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4764 2021-06-07 22:23:51.000000 b2sdk-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/test/integration/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      854 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/integration/test_raw_api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.390168 b2sdk-1.9.0/test/static/
--rw-r--r--   0 runner    (1001) docker     (121)      290 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/static/test_licenses.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      288 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/account_info/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/account_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3140 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/account_info/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)    16872 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/account_info/test_account_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/account_info/test_sqlite_account_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/api/
--rw-r--r--   0 runner    (1001) docker     (121)      292 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12505 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/api/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/bucket/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/bucket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    56149 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/bucket/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (121)     4260 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/file_lock/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/file_lock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      624 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/file_lock/test_legal_hold.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/file_version/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/file_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/file_version/test_file_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)      387 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/fixtures/b2http.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/fixtures/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/fixtures/raw_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      836 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/fixtures/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/internal/
--rw-r--r--   0 runner    (1001) docker     (121)      297 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1148 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/internal/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    23009 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/internal/test_emerge_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.394168 b2sdk-1.9.0/test/unit/sync/
--rw-r--r--   0 runner    (1001) docker     (121)      293 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4201 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/sync/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)     2273 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/sync/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     2625 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/sync/test_scan_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)    33498 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/sync/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5675 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.398168 b2sdk-1.9.0/test/unit/v0/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.398168 b2sdk-1.9.0/test/unit/v0/apiver/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/apiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/apiver/apiver_deps.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/apiver/apiver_deps_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/deps.py
--rw-r--r--   0 runner    (1001) docker     (121)      621 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/deps_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)    11722 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_b2http.py
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_bounded_queue_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)    49489 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (121)     6154 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_copy_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_download_dest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_file_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3314 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2039 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (121)     6958 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_raw_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_scan_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     3311 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_session.py
--rw-r--r--   0 runner    (1001) docker     (121)    34022 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_sync_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     6970 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4064 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v0/test_version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.402168 b2sdk-1.9.0/test/unit/v1/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.402168 b2sdk-1.9.0/test/unit/v1/apiver/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/apiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/apiver/apiver_deps.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/apiver/apiver_deps_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)      601 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/deps.py
--rw-r--r--   0 runner    (1001) docker     (121)      621 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/deps_exception.py
--rw-r--r--   0 runner    (1001) docker     (121)    11722 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_b2http.py
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_bounded_queue_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     6196 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_copy_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_download_dest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_file_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3314 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2039 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (121)     6817 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_raw_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_scan_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     3311 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_session.py
--rw-r--r--   0 runner    (1001) docker     (121)    34972 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_sync_report.py
--rw-r--r--   0 runner    (1001) docker     (121)     6970 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4064 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v1/test_version_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.402168 b2sdk-1.9.0/test/unit/v2/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.402168 b2sdk-1.9.0/test/unit/v2/apiver/
--rw-r--r--   0 runner    (1001) docker     (121)      402 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v2/apiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v2/apiver/apiver_deps.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v2/apiver/apiver_deps_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 22:23:57.402168 b2sdk-1.9.0/test/unit/v_all/
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v_all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2992 2021-06-07 22:23:51.000000 b2sdk-1.9.0/test/unit/v_all/test_api.py
+-rw-r--r--   0        0        0    11963 2024-04-02 12:02:17.615899 b2sdk-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2219 2024-04-02 12:02:17.615899 b2sdk-2.0.0/README.md
+lrwxr-xr-x   0        0        0        0 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/LICENSE -> ../LICENSE
+-rw-r--r--   0        0        0      422 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/__init__.py
+-rw-r--r--   0        0        0      319 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/__main__.py
+-rw-r--r--   0        0        0      443 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/__init__.py
+-rw-r--r--   0        0        0      414 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/account_info/__init__.py
+-rw-r--r--   0        0        0    12688 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/account_info/abstract.py
+-rw-r--r--   0        0        0     1381 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/account_info/exception.py
+-rw-r--r--   0        0        0     4400 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/account_info/in_memory.py
+-rw-r--r--   0        0        0    24095 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/account_info/sqlite_account_info.py
+-rw-r--r--   0        0        0     4349 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/account_info/stub.py
+-rw-r--r--   0        0        0     3534 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/account_info/upload_url_pool.py
+-rw-r--r--   0        0        0    26244 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/api.py
+-rw-r--r--   0        0        0     1748 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/api_config.py
+-rw-r--r--   0        0        0     5835 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/application_key.py
+-rw-r--r--   0        0        0    21710 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/b2http.py
+-rw-r--r--   0        0        0     2316 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/bounded_queue_executor.py
+-rw-r--r--   0        0        0    80069 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/bucket.py
+-rw-r--r--   0        0        0     3746 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/cache.py
+-rw-r--r--   0        0        0      340 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/encryption/__init__.py
+-rw-r--r--   0        0        0    12661 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/encryption/setting.py
+-rw-r--r--   0        0        0     1433 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/encryption/types.py
+-rw-r--r--   0        0        0    19632 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/exception.py
+-rw-r--r--   0        0        0    13765 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/file_lock.py
+-rw-r--r--   0        0        0    23877 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/file_version.py
+-rw-r--r--   0        0        0     1997 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/filter.py
+-rw-r--r--   0        0        0     1555 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/http_constants.py
+-rw-r--r--   0        0        0      863 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/included_sources.py
+-rw-r--r--   0        0        0      340 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/large_file/__init__.py
+-rw-r--r--   0        0        0     1496 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/large_file/part.py
+-rw-r--r--   0        0        0     4777 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/large_file/services.py
+-rw-r--r--   0        0        0     2923 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/large_file/unfinished_large_file.py
+-rw-r--r--   0        0        0     7131 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/progress.py
+-rw-r--r--   0        0        0    36052 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/raw_api.py
+-rw-r--r--   0        0        0    76908 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/raw_simulator.py
+-rw-r--r--   0        0        0      341 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/replication/__init__.py
+-rw-r--r--   0        0        0     8707 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/replication/monitoring.py
+-rw-r--r--   0        0        0     7331 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/replication/setting.py
+-rw-r--r--   0        0        0    13198 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/replication/setup.py
+-rw-r--r--   0        0        0      710 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/replication/types.py
+-rw-r--r--   0        0        0    10141 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/requests/LICENSE
+-rw-r--r--   0        0        0      289 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/requests/NOTICE
+-rw-r--r--   0        0        0      232 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/requests/README.md
+-rw-r--r--   0        0        0     3275 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/requests/__init__.py
+-rw-r--r--   0        0        0      868 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/requests/included_source_meta.py
+-rw-r--r--   0        0        0      334 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/scan/__init__.py
+-rw-r--r--   0        0        0     2880 2024-04-02 12:02:17.615899 b2sdk-2.0.0/b2sdk/_internal/scan/exception.py
+-rw-r--r--   0        0        0    15863 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/scan/folder.py
+-rw-r--r--   0        0        0     2021 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/scan/folder_parser.py
+-rw-r--r--   0        0        0     2724 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/scan/path.py
+-rw-r--r--   0        0        0     9060 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/scan/policies.py
+-rw-r--r--   0        0        0     6071 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/scan/report.py
+-rw-r--r--   0        0        0     3935 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/scan/scan.py
+-rw-r--r--   0        0        0    20904 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/session.py
+-rw-r--r--   0        0        0      615 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/stream/__init__.py
+-rw-r--r--   0        0        0      531 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/stream/base.py
+-rw-r--r--   0        0        0     5273 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/stream/chained.py
+-rw-r--r--   0        0        0     2389 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/stream/hashing.py
+-rw-r--r--   0        0        0     3100 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/stream/progress.py
+-rw-r--r--   0        0        0     2597 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/stream/range.py
+-rw-r--r--   0        0        0     2278 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/stream/wrapper.py
+-rw-r--r--   0        0        0      334 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/__init__.py
+-rw-r--r--   0        0        0    18071 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/action.py
+-rw-r--r--   0        0        0     3901 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/encryption_provider.py
+-rw-r--r--   0        0        0      422 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/exception.py
+-rw-r--r--   0        0        0    18364 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/policy.py
+-rw-r--r--   0        0        0     4378 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/policy_manager.py
+-rw-r--r--   0        0        0     6351 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/report.py
+-rw-r--r--   0        0        0    14535 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/sync/sync.py
+-rw-r--r--   0        0        0      620 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/__init__.py
+-rw-r--r--   0        0        0      345 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/__init__.py
+-rw-r--r--   0        0        0    14793 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/emerger.py
+-rw-r--r--   0        0        0      556 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/exception.py
+-rw-r--r--   0        0        0    29077 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/executor.py
+-rw-r--r--   0        0        0      353 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/planner/__init__.py
+-rw-r--r--   0        0        0     5456 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/planner/part_definition.py
+-rw-r--r--   0        0        0    32575 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/planner/planner.py
+-rw-r--r--   0        0        0     3582 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/planner/upload_subpart.py
+-rw-r--r--   0        0        0     8394 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/unbound_write_intent.py
+-rw-r--r--   0        0        0     3229 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/write_intent.py
+-rw-r--r--   0        0        0      346 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/__init__.py
+-rw-r--r--   0        0        0     4399 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/download_manager.py
+-rw-r--r--   0        0        0     9663 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloaded_file.py
+-rw-r--r--   0        0        0      357 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloader/__init__.py
+-rw-r--r--   0        0        0     3921 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloader/abstract.py
+-rw-r--r--   0        0        0    18395 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloader/parallel.py
+-rw-r--r--   0        0        0     3518 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloader/simple.py
+-rw-r--r--   0        0        0     3114 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloader/stats_collector.py
+-rw-r--r--   0        0        0      347 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/__init__.py
+-rw-r--r--   0        0        0    10338 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/copy_manager.py
+-rw-r--r--   0        0        0     3118 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/copy_source.py
+-rw-r--r--   0        0        0     2114 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/large_file_upload_state.py
+-rw-r--r--   0        0        0     1804 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/outbound_source.py
+-rw-r--r--   0        0        0     1625 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/progress_reporter.py
+-rw-r--r--   0        0        0     9583 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/upload_manager.py
+-rw-r--r--   0        0        0    13100 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/upload_source.py
+-rw-r--r--   0        0        0      560 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/transfer/transfer_manager.py
+-rw-r--r--   0        0        0    14788 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1561 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/docs.py
+-rw-r--r--   0        0        0     1643 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/escape.py
+-rw-r--r--   0        0        0      948 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0     1186 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/http_date.py
+-rw-r--r--   0        0        0     1660 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/range_.py
+-rw-r--r--   0        0        0     3546 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/thread_pool.py
+-rw-r--r--   0        0        0      561 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/utils/typing.py
+-rw-r--r--   0        0        0     6873 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_internal/version_utils.py
+-rw-r--r--   0        0        0      551 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_pyinstaller/__init__.py
+-rw-r--r--   0        0        0      417 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_pyinstaller/hook-b2sdk.py
+-rw-r--r--   0        0        0    12389 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_v3/__init__.py
+-rw-r--r--   0        0        0     7083 2024-04-02 12:02:17.619899 b2sdk-2.0.0/b2sdk/_v3/exception.py
+-rw-r--r--   0        0        0      705 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v0/__init__.py
+-rw-r--r--   0        0        0     2035 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v0/account_info.py
+-rw-r--r--   0        0        0      999 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v0/api.py
+-rw-r--r--   0        0        0     1078 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v0/bucket.py
+-rw-r--r--   0        0        0      969 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v0/exception.py
+-rw-r--r--   0        0        0     7245 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v0/sync.py
+-rw-r--r--   0        0        0     1351 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/__init__.py
+-rw-r--r--   0        0        0     5908 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/account_info.py
+-rw-r--r--   0        0        0     8348 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/api.py
+-rw-r--r--   0        0        0     1927 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/b2http.py
+-rw-r--r--   0        0        0    13668 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/bucket.py
+-rw-r--r--   0        0        0      530 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/cache.py
+-rw-r--r--   0        0        0     6787 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/download_dest.py
+-rw-r--r--   0        0        0     1580 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/exception.py
+-rw-r--r--   0        0        0     2218 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/file_metadata.py
+-rw-r--r--   0        0        0     7019 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/file_version.py
+-rw-r--r--   0        0        0      334 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/replication/__init__.py
+-rw-r--r--   0        0        0     1148 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/replication/monitoring.py
+-rw-r--r--   0        0        0     2596 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/session.py
+-rw-r--r--   0        0        0      505 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/__init__.py
+-rw-r--r--   0        0        0     3869 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/encryption_provider.py
+-rw-r--r--   0        0        0     3849 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/file.py
+-rw-r--r--   0        0        0     2816 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/file_to_path_translator.py
+-rw-r--r--   0        0        0     2318 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/folder.py
+-rw-r--r--   0        0        0      738 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/folder_parser.py
+-rw-r--r--   0        0        0      846 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/report.py
+-rw-r--r--   0        0        0     6929 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/scan_policies.py
+-rw-r--r--   0        0        0     5387 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v1/sync/sync.py
+-rw-r--r--   0        0        0     1356 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/__init__.py
+-rw-r--r--   0        0        0      454 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/_compat.py
+-rw-r--r--   0        0        0      494 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/account_info.py
+-rw-r--r--   0        0        0     2235 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/api.py
+-rw-r--r--   0        0        0      803 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/b2http.py
+-rw-r--r--   0        0        0     3086 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/bucket.py
+-rw-r--r--   0        0        0      812 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/exception.py
+-rw-r--r--   0        0        0     2902 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/file_version.py
+-rw-r--r--   0        0        0     1339 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/large_file.py
+-rw-r--r--   0        0        0     2751 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/raw_api.py
+-rw-r--r--   0        0        0     3704 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/raw_simulator.py
+-rw-r--r--   0        0        0     1523 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/session.py
+-rw-r--r--   0        0        0      369 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/sync.py
+-rw-r--r--   0        0        0      584 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/transfer.py
+-rw-r--r--   0        0        0     1033 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/utils.py
+-rw-r--r--   0        0        0     1612 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/v2/version_utils.py
+-rw-r--r--   0        0        0      767 2024-04-02 12:02:17.623899 b2sdk-2.0.0/b2sdk/version.py
+-rw-r--r--   0        0        0     4285 2024-04-02 12:02:25.727878 b2sdk-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3288 1970-01-01 00:00:00.000000 b2sdk-2.0.0/PKG-INFO
```

### Comparing `b2sdk-1.9.0/PKG-INFO` & `b2sdk-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: b2sdk
-Version: 1.9.0
+Version: 2.0.0
 Summary: Backblaze B2 SDK
-Home-page: https://github.com/Backblaze/b2-sdk-python
-Author: Backblaze, Inc.
-Author-email: support@backblaze.com
-License: MIT
 Keywords: backblaze b2 cloud storage
-Platform: UNKNOWN
+Author-Email: Backblaze Inc <support@backblaze.com>
+License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Project-URL: Homepage, https://github.com/Backblaze/b2-sdk-python
+Requires-Python: >=3.7
+Requires-Dist: importlib-metadata>=3.3.0; python_version < "3.8"
+Requires-Dist: logfury<2.0.0,>=1.0.1
+Requires-Dist: requests<3.0.0,>=2.9.1
+Requires-Dist: typing-extensions>=4.7.1; python_version < "3.12"
 Description-Content-Type: text/markdown
-Provides-Extra: doc
-License-File: LICENSE
 
 # B2 Python SDK
 &nbsp;[![Continuous Integration](https://github.com/Backblaze/b2-sdk-python/workflows/Continuous%20Integration/badge.svg)](https://github.com/Backblaze/b2-sdk-python/actions?query=workflow%3A%22Continuous+Integration%22)&nbsp;[![License](https://img.shields.io/pypi/l/b2sdk.svg?label=License)](https://pypi.python.org/pypi/b2)&nbsp;[![python versions](https://img.shields.io/pypi/pyversions/b2sdk.svg?label=python%20versions)](https://pypi.python.org/pypi/b2sdk)&nbsp;[![PyPI version](https://img.shields.io/pypi/v/b2sdk.svg?label=PyPI%20version)](https://pypi.python.org/pypi/b2sdk)&nbsp;[![Docs](https://readthedocs.org/projects/b2-sdk-python/badge/?version=master)](https://b2-sdk-python.readthedocs.io/en/master/)
 
 
 
 This repository contains a client library and a few handy utilities for easy access to all of the capabilities of B2 Cloud Storage.
@@ -47,19 +49,17 @@
 - we increase MAJOR version when we make incompatible API changes
 - we increase MINOR version when we add functionality in a backwards-compatible manner, and
 - we increase PATCH version when we make backwards-compatible bug fixes (unless someone relies on the undocumented behavior of a fixed bug)
 
 Therefore when setting up b2sdk as a dependency, please make sure to match the version appropriately, for example you could put this in your `requirements.txt` to make sure your code is compatible with the `b2sdk` version your user will get from pypi:
 
 ```
-b2sdk>=0.0.0,<1.0.0
+b2sdk>=2,<3
 ```
 
 # Release History
 
 Please refer to the [changelog](CHANGELOG.md).
 
 # Developer Info
 
 Please see our [contributing guidelines](CONTRIBUTING.md).
-
-
```

### Comparing `b2sdk-1.9.0/README.md` & `b2sdk-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 - we increase MAJOR version when we make incompatible API changes
 - we increase MINOR version when we add functionality in a backwards-compatible manner, and
 - we increase PATCH version when we make backwards-compatible bug fixes (unless someone relies on the undocumented behavior of a fixed bug)
 
 Therefore when setting up b2sdk as a dependency, please make sure to match the version appropriately, for example you could put this in your `requirements.txt` to make sure your code is compatible with the `b2sdk` version your user will get from pypi:
 
 ```
-b2sdk>=0.0.0,<1.0.0
+b2sdk>=2,<3
 ```
 
 # Release History
 
 Please refer to the [changelog](CHANGELOG.md).
 
 # Developer Info
```

### Comparing `b2sdk-1.9.0/b2sdk/_pyinstaller/__init__.py` & `b2sdk-2.0.0/b2sdk/_pyinstaller/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # File: b2sdk/_pyinstaller/__init__.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import os
 
 
 def get_hook_dirs():
     """Get hooks directories for pyinstaller.
```

### Comparing `b2sdk-1.9.0/b2sdk/account_info/abstract.py` & `b2sdk-2.0.0/b2sdk/_internal/account_info/abstract.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 ######################################################################
 #
-# File: b2sdk/account_info/abstract.py
+# File: b2sdk/_internal/account_info/abstract.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
+
 from abc import abstractmethod
-from typing import Optional
 
-from b2sdk.account_info import exception
-from b2sdk.raw_api import ALL_CAPABILITIES
-from b2sdk.utils import B2TraceMetaAbstract, limit_trace_arguments
+from b2sdk._internal.account_info import exception
+from b2sdk._internal.raw_api import ALL_CAPABILITIES
+from b2sdk._internal.utils import B2TraceMetaAbstract, limit_trace_arguments
 
 
 class AbstractAccountInfo(metaclass=B2TraceMetaAbstract):
     """
     Abstract class for a holder for all account-related information
     that needs to be kept between API calls and between invocations of the program.
 
@@ -39,23 +40,32 @@
     @classmethod
     def all_capabilities(cls):
         """
         Return a list of all possible capabilities.
 
         :rtype: list
         """
-        return cls.ALL_CAPABILITIES
+        return ALL_CAPABILITIES
 
     @abstractmethod
     def clear(self):
         """
         Remove all stored information.
         """
 
     @abstractmethod
+    def list_bucket_names_ids(self) -> list[tuple[str, str]]:
+        """
+        List buckets in the cache.
+
+        :return: list of tuples (bucket_name, bucket_id)
+        """
+        pass
+
+    @abstractmethod
     @limit_trace_arguments(only=['self'])
     def refresh_entire_bucket_name_cache(self, name_id_iterable):
         """
         Remove all previous name-to-id mappings and stores new ones.
 
         :param iterable name_id_iterable: an iterable of tuples of the form (name, id)
         """
@@ -69,29 +79,29 @@
         """
 
     @abstractmethod
     def save_bucket(self, bucket):
         """
         Remember the ID for the given bucket name.
 
-        :param b2sdk.v1.Bucket bucket: a Bucket object
+        :param b2sdk.v2.Bucket bucket: a Bucket object
         """
 
     @abstractmethod
     def get_bucket_id_or_none_from_bucket_name(self, bucket_name):
         """
         Look up the bucket ID for the given bucket name.
 
         :param str bucket_name: a bucket name
         :return bucket ID or None:
         :rtype: str, None
         """
 
     @abstractmethod
-    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> Optional[str]:
+    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> str | None:
         """
         Look up the bucket name for the given bucket id.
         """
 
     @abstractmethod
     def clear_bucket_upload_data(self, bucket_id):
         """
@@ -122,18 +132,31 @@
         :rtype: bool
         """
         try:
             return self.get_account_id() == account_id and self.get_realm() == realm
         except exception.MissingAccountData:
             return False
 
+    def is_master_key(self) -> bool:
+        application_key_id = self.get_application_key_id()
+        account_id = self.get_account_id()
+        new_style_master_key_suffix = '0000000000'
+        if account_id == application_key_id:
+            return True  # old style
+        if len(application_key_id
+              ) == (3 + len(account_id) + len(new_style_master_key_suffix)):  # 3 for cluster id
+            # new style
+            if application_key_id.endswith(account_id + new_style_master_key_suffix):
+                return True
+        return False
+
     @abstractmethod
     def get_account_id(self):
         """
-        Return account ID or raises :class:`~b2sdk.v1.exception.MissingAccountData` exception.
+        Return account ID or raises :class:`~b2sdk.v2.exception.MissingAccountData` exception.
 
         :rtype: str
         """
 
     @abstractmethod
     def get_application_key_id(self):
         """
@@ -141,47 +164,47 @@
 
         :rtype: str
         """
 
     @abstractmethod
     def get_account_auth_token(self):
         """
-        Return account_auth_token or raises :class:`~b2sdk.v1.exception.MissingAccountData` exception.
+        Return account_auth_token or raises :class:`~b2sdk.v2.exception.MissingAccountData` exception.
 
         :rtype: str
         """
 
     @abstractmethod
     def get_api_url(self):
         """
-        Return api_url or raises :class:`~b2sdk.v1.exception.MissingAccountData` exception.
+        Return api_url or raises :class:`~b2sdk.v2.exception.MissingAccountData` exception.
 
         :rtype: str
         """
 
     @abstractmethod
     def get_application_key(self):
         """
-        Return application_key or raises :class:`~b2sdk.v1.exception.MissingAccountData` exception.
+        Return application_key or raises :class:`~b2sdk.v2.exception.MissingAccountData` exception.
 
         :rtype: str
         """
 
     @abstractmethod
     def get_download_url(self):
         """
-        Return download_url or raises :class:`~b2sdk.v1.exception.MissingAccountData` exception.
+        Return download_url or raises :class:`~b2sdk.v2.exception.MissingAccountData` exception.
 
         :rtype: str
         """
 
     @abstractmethod
     def get_realm(self):
         """
-        Return realm or raises :class:`~b2sdk.v1.exception.MissingAccountData` exception.
+        Return realm or raises :class:`~b2sdk.v2.exception.MissingAccountData` exception.
 
         :rtype: str
         """
 
     @abstractmethod
     def get_recommended_part_size(self):
         """
@@ -209,15 +232,15 @@
 
         :rtype: dict
         """
 
     @abstractmethod
     def get_s3_api_url(self):
         """
-        Return s3_api_url or raises :class:`~b2sdk.v1.exception.MissingAccountData` exception.
+        Return s3_api_url or raises :class:`~b2sdk.v2.exception.MissingAccountData` exception.
 
         :rtype: str
         """
 
     @limit_trace_arguments(
         only=[
             'self',
@@ -316,15 +339,14 @@
         """
         return (
             ('bucketId' in allowed) and ('bucketName' in allowed) and
             ((allowed['bucketId'] is not None) or (allowed['bucketName'] is None)) and
             ('capabilities' in allowed) and ('namePrefix' in allowed)
         )
 
-    # TODO: make a decorator for set_auth_data()
     @abstractmethod
     def _set_auth_data(
         self, account_id, auth_token, api_url, download_url, recommended_part_size,
         absolute_minimum_part_size, application_key, realm, s3_api_url, allowed, application_key_id
     ):
         """
         Actually store the auth data.  Can assume that 'allowed' is present and valid.
```

### Comparing `b2sdk-1.9.0/b2sdk/account_info/exception.py` & `b2sdk-2.0.0/b2sdk/_internal/account_info/exception.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 ######################################################################
 #
-# File: b2sdk/account_info/exception.py
+# File: b2sdk/_internal/account_info/exception.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from abc import (ABCMeta)
+from abc import ABCMeta
 
 from ..exception import B2Error
 
 
 class AccountInfoError(B2Error, metaclass=ABCMeta):
     """
     Base class for all account info errors.
@@ -26,31 +27,30 @@
     """
 
     def __init__(self, file_name):
         """
         :param file_name: an account info file name
         :type file_name: str
         """
-        super(CorruptAccountInfo, self).__init__()
+        super().__init__()
         self.file_name = file_name
 
     def __str__(self):
-        return 'Account info file (%s) appears corrupted.  Try removing and then re-authorizing the account.' % (
-            self.file_name,
-        )
+        return f'Account info file ({self.file_name}) appears corrupted. ' \
+               f'Try removing and then re-authorizing the account.'
 
 
 class MissingAccountData(AccountInfoError):
     """
     Raised when there is no account info data available.
     """
 
     def __init__(self, key):
         """
         :param key: a key for getting account data
         :type key: str
         """
-        super(MissingAccountData, self).__init__()
+        super().__init__()
         self.key = key
 
     def __str__(self):
-        return 'Missing account data: %s' % (self.key,)
+        return f'Missing account data: {self.key}'
```

### Comparing `b2sdk-1.9.0/b2sdk/account_info/in_memory.py` & `b2sdk-2.0.0/b2sdk/_internal/account_info/in_memory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 ######################################################################
 #
-# File: b2sdk/account_info/in_memory.py
+# File: b2sdk/_internal/account_info/in_memory.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from typing import Optional
+from functools import wraps
 
 from .exception import MissingAccountData
 from .upload_url_pool import UrlPoolAccountInfo
 
-from functools import wraps
-
 
 def _raise_missing_if_result_is_none(function):
     """
     Raise MissingAccountData if function's result is None.
     """
 
     @wraps(function)
@@ -35,20 +34,20 @@
 
 class InMemoryAccountInfo(UrlPoolAccountInfo):
     """
     *AccountInfo* which keeps all data in memory.
     """
 
     def __init__(self, *args, **kwargs):
-        super(InMemoryAccountInfo, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._clear_in_memory_account_fields()
 
     def clear(self):
         self._clear_in_memory_account_fields()
-        return super(InMemoryAccountInfo, self).clear()
+        return super().clear()
 
     def _clear_in_memory_account_fields(self):
         self._account_id = None
         self._application_key_id = None
         self._allowed = None
         self._api_url = None
         self._application_key = None
@@ -78,20 +77,23 @@
 
     def refresh_entire_bucket_name_cache(self, name_id_iterable):
         self._buckets = dict(name_id_iterable)
 
     def get_bucket_id_or_none_from_bucket_name(self, bucket_name):
         return self._buckets.get(bucket_name)
 
-    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> Optional[str]:
+    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> str | None:
         for name, cached_id_ in self._buckets.items():
             if cached_id_ == bucket_id:
                 return name
         return None
 
+    def list_bucket_names_ids(self) -> list[tuple[str, str]]:
+        return [(name, id_) for name, id_ in self._buckets.items()]
+
     def save_bucket(self, bucket):
         self._buckets[bucket.name] = bucket.id_
 
     def remove_bucket_name(self, bucket_name):
         if bucket_name in self._buckets:
             del self._buckets[bucket_name]
```

### Comparing `b2sdk-1.9.0/b2sdk/account_info/sqlite_account_info.py` & `b2sdk-2.0.0/b2sdk/_internal/account_info/sqlite_account_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 ######################################################################
 #
-# File: b2sdk/account_info/sqlite_account_info.py
+# File: b2sdk/_internal/account_info/sqlite_account_info.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import json
 import logging
 import os
+import re
+import sqlite3
 import stat
+import sys
 import threading
-from typing import Optional, List
 
-from .exception import (CorruptAccountInfo, MissingAccountData)
+from .exception import CorruptAccountInfo, MissingAccountData
 from .upload_url_pool import UrlPoolAccountInfo
 
-import sqlite3
-
 logger = logging.getLogger(__name__)
 
 B2_ACCOUNT_INFO_ENV_VAR = 'B2_ACCOUNT_INFO'
-B2_ACCOUNT_INFO_DEFAULT_FILE = '~/.b2_account_info'
+B2_ACCOUNT_INFO_DEFAULT_FILE = os.path.join('~', '.b2_account_info')
+B2_ACCOUNT_INFO_PROFILE_FILE = os.path.join('~', '.b2db-{profile}.sqlite')
+B2_ACCOUNT_INFO_PROFILE_NAME_REGEXP = re.compile(r'[a-zA-Z0-9_\-]{1,64}')
 XDG_CONFIG_HOME_ENV_VAR = 'XDG_CONFIG_HOME'
 
 DEFAULT_ABSOLUTE_MINIMUM_PART_SIZE = 5000000  # this value is used ONLY in migrating db, and in v1 wrapper, it is not
 # meant to be a default for other applications
 
 
 class SqliteAccountInfo(UrlPoolAccountInfo):
@@ -35,69 +38,110 @@
     Store account information in an `sqlite3 <https://www.sqlite.org>`_ database which is
     used to manage concurrent access to the data.
 
     The ``update_done`` table tracks the schema updates that have been
     completed.
     """
 
-    def __init__(self, file_name=None, last_upgrade_to_run=None):
+    def __init__(self, file_name=None, last_upgrade_to_run=None, profile: str | None = None):
         """
         Initialize SqliteAccountInfo.
 
         The exact algorithm used to determine the location of the database file is not API in any sense.
         If the location of the database file is required (for cleanup, etc), do not assume a specific resolution:
         instead, use ``self.filename`` to get the actual resolved location.
 
         SqliteAccountInfo currently checks locations in the following order:
 
+        If ``profile`` arg is provided:
+
+        * ``{B2_ACCOUNT_INFO_PROFILE_FILE}`` if it already exists
+        * ``${XDG_CONFIG_HOME_ENV_VAR}/b2/db-<profile>.sqlite`` on XDG-compatible OSes (Linux, BSD)
+        * ``{B2_ACCOUNT_INFO_PROFILE_FILE}``
+
+        Otherwise:
+
         * ``file_name``, if truthy
         * ``{B2_ACCOUNT_INFO_ENV_VAR}`` env var's value, if set
-        * ``{B2_ACCOUNT_INFO_DEFAULT_FILE}``, if it exists
-        * ``{XDG_CONFIG_HOME_ENV_VAR}/b2/account_info``, if ``{XDG_CONFIG_HOME_ENV_VAR}`` env var is set
+        * ``{B2_ACCOUNT_INFO_DEFAULT_FILE}``, if it already exists
+        * ``${XDG_CONFIG_HOME_ENV_VAR}/b2/account_info`` on XDG-compatible OSes (Linux, BSD)
         * ``{B2_ACCOUNT_INFO_DEFAULT_FILE}``, as default
 
-        If the directory ``{XDG_CONFIG_HOME_ENV_VAR}/b2`` does not exist (and is needed), it is created.
+        If the directory ``${XDG_CONFIG_HOME_ENV_VAR}/b2`` does not exist (and is needed), it is created.
 
         :param str file_name: The sqlite file to use; overrides the default.
         :param int last_upgrade_to_run: For testing only, override the auto-update on the db.
         """
         self.thread_local = threading.local()
 
-        if file_name:
-            user_account_info_path = file_name
-        elif B2_ACCOUNT_INFO_ENV_VAR in os.environ:
-            user_account_info_path = os.environ[B2_ACCOUNT_INFO_ENV_VAR]
-        elif os.path.exists(os.path.expanduser(B2_ACCOUNT_INFO_DEFAULT_FILE)):
-            user_account_info_path = B2_ACCOUNT_INFO_DEFAULT_FILE
-        elif XDG_CONFIG_HOME_ENV_VAR in os.environ:
-            config_home = os.environ[XDG_CONFIG_HOME_ENV_VAR]
-            user_account_info_path = os.path.join(config_home, 'b2', 'account_info')
-            if not os.path.exists(os.path.join(config_home, 'b2')):
-                os.makedirs(os.path.join(config_home, 'b2'), mode=0o755)
-        else:
-            user_account_info_path = B2_ACCOUNT_INFO_DEFAULT_FILE
-
-        self.filename = os.path.expanduser(user_account_info_path)
+        self.filename = self.get_user_account_info_path(file_name=file_name, profile=profile)
         logger.debug('%s file path to use: %s', self.__class__.__name__, self.filename)
 
         self._validate_database(last_upgrade_to_run)
         with self._get_connection() as conn:
             self._create_tables(conn, last_upgrade_to_run)
-        super(SqliteAccountInfo, self).__init__()
+        super().__init__()
 
     # dirty trick to use parameters in the docstring
     if getattr(__init__, '__doc__', None):  # don't break when using `python -oo`
         __init__.__doc__ = __init__.__doc__.format(
             **dict(
                 B2_ACCOUNT_INFO_ENV_VAR=B2_ACCOUNT_INFO_ENV_VAR,
                 B2_ACCOUNT_INFO_DEFAULT_FILE=B2_ACCOUNT_INFO_DEFAULT_FILE,
+                B2_ACCOUNT_INFO_PROFILE_FILE=B2_ACCOUNT_INFO_PROFILE_FILE,
                 XDG_CONFIG_HOME_ENV_VAR=XDG_CONFIG_HOME_ENV_VAR,
             )
         )
 
+    @classmethod
+    def _get_xdg_config_path(cls) -> str | None:
+        """
+        Return XDG config path if the OS is XDG-compatible (Linux, BSD), None otherwise.
+
+        If $XDG_CONFIG_HOME is empty but the OS is XDG compliant, fallback to ~/.config as expected by XDG standard.
+        """
+        xdg_config_home = os.getenv(XDG_CONFIG_HOME_ENV_VAR)
+        if xdg_config_home or sys.platform not in ('win32', 'darwin'):
+            return xdg_config_home or os.path.join(os.path.expanduser('~/.config'))
+        return None
+
+    @classmethod
+    def get_user_account_info_path(cls, file_name: str | None = None, profile: str | None = None):
+        if profile and not B2_ACCOUNT_INFO_PROFILE_NAME_REGEXP.match(profile):
+            raise ValueError(f'Invalid profile name: {profile}')
+
+        profile_file = B2_ACCOUNT_INFO_PROFILE_FILE.format(profile=profile) if profile else None
+        xdg_config_path = cls._get_xdg_config_path()
+
+        if file_name:
+            if profile:
+                raise ValueError('Provide either file_name or profile, not both')
+            user_account_info_path = file_name
+        elif B2_ACCOUNT_INFO_ENV_VAR in os.environ:
+            if profile:
+                raise ValueError(
+                    f'Provide either {B2_ACCOUNT_INFO_ENV_VAR} env var or profile, not both'
+                )
+            user_account_info_path = os.environ[B2_ACCOUNT_INFO_ENV_VAR]
+        elif not profile and os.path.exists(os.path.expanduser(B2_ACCOUNT_INFO_DEFAULT_FILE)):
+            user_account_info_path = B2_ACCOUNT_INFO_DEFAULT_FILE
+        elif profile and os.path.exists(profile_file):
+            user_account_info_path = profile_file
+        elif xdg_config_path:
+            os.makedirs(os.path.join(xdg_config_path, 'b2'), mode=0o755, exist_ok=True)
+
+            file_name = f'db-{profile}.sqlite' if profile else 'account_info'
+            user_account_info_path = os.path.join(xdg_config_path, 'b2', file_name)
+        elif profile:
+            user_account_info_path = profile_file
+        else:
+            user_account_info_path = B2_ACCOUNT_INFO_DEFAULT_FILE
+
+        return os.path.expanduser(user_account_info_path)
+
     def _validate_database(self, last_upgrade_to_run=None):
         """
         Make sure that the database is openable.  Removes the file if it's not.
         """
         # If there is no file there, that's fine.  It will get created when
         # we connect.
         if not os.path.exists(self.filename):
@@ -161,28 +205,32 @@
             return self.thread_local.connection
 
     def _connect(self):
         return sqlite3.connect(self.filename, isolation_level='EXCLUSIVE')
 
     def _create_database(self, last_upgrade_to_run):
         """
-        Make sure that the database is created and sets the file permissions.
+        Make sure that the database is created and has appropriate file permissions.
         This should be done before storing any sensitive data in it.
         """
+        # Prepare a file
+        fd = os.open(
+            self.filename,
+            flags=os.O_RDWR | os.O_CREAT,
+            mode=stat.S_IRUSR | stat.S_IWUSR,
+        )
+        os.close(fd)
         # Create the tables in the database
         conn = self._connect()
         try:
             with conn:
                 self._create_tables(conn, last_upgrade_to_run)
         finally:
             conn.close()
 
-        # Set the file permissions
-        os.chmod(self.filename, stat.S_IRUSR | stat.S_IWUSR)
-
     def _create_tables(self, conn, last_upgrade_to_run):
         conn.execute(
             """
             CREATE TABLE IF NOT EXISTS
             update_done (
                 update_number INT NOT NULL
             );
@@ -324,15 +372,15 @@
                                     s3_api_url
                                 FROM tmp_account;
                                 """,
                     'DROP TABLE tmp_account;',
                 ]
             )
 
-    def _ensure_update(self, update_number, update_commands: List[str]):
+    def _ensure_update(self, update_number, update_commands: list[str]):
         """
         Run the update with the given number if it hasn't been done yet.
 
         Does the update and stores the number as a single transaction,
         so they will always be in sync.
         """
         with self._get_connection() as conn:
@@ -518,15 +566,15 @@
             return ''
         else:
             return result
 
     def _get_account_info_or_raise(self, column_name):
         try:
             with self._get_connection() as conn:
-                cursor = conn.execute('SELECT %s FROM account;' % (column_name,))
+                cursor = conn.execute(f'SELECT {column_name} FROM account;')
                 value = cursor.fetchone()[0]
                 return value
         except Exception as e:
             logger.exception(
                 '_get_account_info_or_raise encountered a problem while trying to retrieve "%s"',
                 column_name
             )
@@ -554,17 +602,22 @@
             conn.execute('DELETE FROM bucket WHERE bucket_name = ?;', (bucket_name,))
 
     def get_bucket_id_or_none_from_bucket_name(self, bucket_name):
         return self._safe_query(
             'SELECT bucket_id FROM bucket WHERE bucket_name = ?;', (bucket_name,)
         )
 
-    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> Optional[str]:
+    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> str | None:
         return self._safe_query('SELECT bucket_name FROM bucket WHERE bucket_id = ?;', (bucket_id,))
 
+    def list_bucket_names_ids(self) -> list[tuple[str, str]]:
+        with self._get_connection() as conn:
+            cursor = conn.execute('SELECT bucket_name, bucket_id FROM bucket;')
+            return cursor.fetchall()
+
     def _safe_query(self, query, params):
         try:
             with self._get_connection() as conn:
                 cursor = conn.execute(query, params)
                 return cursor.fetchone()[0]
         except TypeError:  # TypeError: 'NoneType' object is unsubscriptable
             return None
```

### Comparing `b2sdk-1.9.0/b2sdk/account_info/stub.py` & `b2sdk-2.0.0/b2sdk/_internal/account_info/stub.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ######################################################################
 #
-# File: b2sdk/account_info/stub.py
+# File: b2sdk/_internal/account_info/stub.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from typing import Optional
 import collections
 import threading
 
 from .abstract import AbstractAccountInfo
 
 
 class StubAccountInfo(AbstractAccountInfo):
@@ -69,17 +69,20 @@
 
     def refresh_entire_bucket_name_cache(self, name_id_iterable):
         self.buckets = {}
 
     def get_bucket_id_or_none_from_bucket_name(self, bucket_name):
         return None
 
-    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> Optional[str]:
+    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> str | None:
         return None
 
+    def list_bucket_names_ids(self) -> list[tuple[str, str]]:
+        return list((bucket.bucket_name, bucket.bucket_id) for bucket in self.buckets.values())
+
     def save_bucket(self, bucket):
         self.buckets[bucket.bucket_id] = bucket
 
     def remove_bucket_name(self, bucket_name):
         pass
 
     def take_bucket_upload_url(self, bucket_id):
```

### Comparing `b2sdk-1.9.0/b2sdk/account_info/upload_url_pool.py` & `b2sdk-2.0.0/b2sdk/_internal/account_info/upload_url_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 ######################################################################
 #
-# File: b2sdk/account_info/upload_url_pool.py
+# File: b2sdk/_internal/account_info/upload_url_pool.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from abc import abstractmethod
 import collections
 import threading
+from abc import abstractmethod
 
 from .abstract import AbstractAccountInfo
 
 
-class UploadUrlPool(object):
+class UploadUrlPool:
     """
     For each key (either a bucket id or large file id), hold a pool
     of (url, auth_token) pairs.
 
     .. note:
         This class is thread-safe.
     """
@@ -64,32 +65,32 @@
             if key in self._pool:
                 del self._pool[key]
 
 
 class UrlPoolAccountInfo(AbstractAccountInfo):
     """
     Implement part of :py:class:`AbstractAccountInfo` for upload URL pool management
-    with a simple, key-value storage, such as :py:class:`b2sdk.v1.UploadUrlPool`.
+    with a simple, key-value storage, such as :py:class:`b2sdk.v2.UploadUrlPool`.
     """
     # staticmethod is necessary here to avoid the first argument binding to the first argument (like ``partial(fun, arg)``)
     BUCKET_UPLOAD_POOL_CLASS = staticmethod(
         UploadUrlPool
     )  #: A url pool class to use for small files.
     LARGE_FILE_UPLOAD_POOL_CLASS = staticmethod(
         UploadUrlPool
     )  #: A url pool class to use for large files.
 
     def __init__(self):
-        super(UrlPoolAccountInfo, self).__init__()
+        super().__init__()
         self._reset_upload_pools()
 
     @abstractmethod
     def clear(self):
         self._reset_upload_pools()
-        return super(UrlPoolAccountInfo, self).clear()
+        return super().clear()
 
     def _reset_upload_pools(self):
         self._bucket_uploads = self.BUCKET_UPLOAD_POOL_CLASS()
         self._large_file_uploads = self.LARGE_FILE_UPLOAD_POOL_CLASS()
 
     # bucket upload url
     def put_bucket_upload_url(self, bucket_id, upload_url, upload_auth_token):
```

### Comparing `b2sdk-1.9.0/b2sdk/b2http.py` & `b2sdk-2.0.0/b2sdk/_internal/b2http.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,59 @@
 ######################################################################
 #
-# File: b2sdk/b2http.py
+# File: b2sdk/_internal/b2http.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
+import datetime
 import io
 import json
+import locale
 import logging
 import socket
+import threading
+import time
+from contextlib import contextmanager
+from random import random
+from typing import Any, Callable
+
+try:
+    from typing_extensions import Literal
+except ImportError:
+    from typing import Literal
 
-import arrow
 import requests
-import time
+from requests.adapters import HTTPAdapter
 
-from typing import Any, Dict
+from b2sdk.version import USER_AGENT
 
+from .api_config import DEFAULT_HTTP_API_CONFIG, B2HttpApiConfig
 from .exception import (
-    B2Error, B2RequestTimeoutDuringUpload, BadDateFormat, BrokenPipe, B2ConnectionError,
-    B2RequestTimeout, ClockSkew, ConnectionReset, interpret_b2_error, UnknownError, UnknownHost
+    B2ConnectionError,
+    B2Error,
+    B2RequestTimeout,
+    B2RequestTimeoutDuringUpload,
+    BadDateFormat,
+    BrokenPipe,
+    ClockSkew,
+    ConnectionReset,
+    PotentialS3EndpointPassedAsRealm,
+    UnknownError,
+    UnknownHost,
+    interpret_b2_error,
 )
-from .version import USER_AGENT
+from .requests import NotDecompressingResponse
+from .utils.typing import JSON
 
+LOCALE_LOCK = threading.Lock()
 logger = logging.getLogger(__name__)
 
 
 def _print_exception(e, indent=''):
     """
     Used for debugging to print out nested exception structures.
 
@@ -38,125 +63,40 @@
     print(indent + 'CLASS', type(e))
     for (i, a) in enumerate(e.args):
         print(indent + 'ARG %d: %s' % (i, repr(a)))
         if isinstance(a, Exception):
             _print_exception(a, indent + '        ')
 
 
-def _translate_errors(fcn, post_params=None):
-    """
-    Call the given function, turning any exception raised into the right
-    kind of B2Error.
-
-    :param dict post_params: request parameters
-    """
-    try:
-        response = fcn()
-        if response.status_code not in [200, 206]:
-            # Decode the error object returned by the service
-            error = json.loads(response.content.decode('utf-8')) if response.content else {}
-            raise interpret_b2_error(
-                int(error.get('status', response.status_code)),
-                error.get('code'),
-                error.get('message'),
-                response.headers,
-                post_params,
-            )
-        return response
-
-    except B2Error:
-        raise  # pass through exceptions from just above
-
-    except requests.ConnectionError as e0:
-        e1 = e0.args[0]
-        if isinstance(e1, requests.packages.urllib3.exceptions.MaxRetryError):
-            msg = e1.args[0]
-            if 'nodename nor servname provided, or not known' in msg:
-                # Unknown host, or DNS failing.  In the context of calling
-                # B2, this means that something is down between here and
-                # Backblaze, so we treat it like 503 Service Unavailable.
-                raise UnknownHost()
-        elif isinstance(e1, requests.packages.urllib3.exceptions.ProtocolError):
-            e2 = e1.args[1]
-            if isinstance(e2, socket.error):
-                if len(e2.args) >= 2 and e2.args[1] == 'Broken pipe':
-                    # Broken pipes are usually caused by the service rejecting
-                    # an upload request for cause, so we use a 400 Bad Request
-                    # code.
-                    raise BrokenPipe()
-        raise B2ConnectionError(str(e0))
-
-    except requests.Timeout as e:
-        raise B2RequestTimeout(str(e))
-
-    except Exception as e:
-        text = repr(e)
-
-        # This is a special case to handle when urllib3 doesn't translate
-        # ECONNRESET into something that requests can turn into something
-        # we understand.  The SysCallError is from the optional library
-        # pyOpenSsl, which we don't require, so we can't import it and
-        # catch it explicitly.
-        #
-        # The text from one such error looks like this: SysCallError(104, 'ECONNRESET')
-        if text.startswith('SysCallError'):
-            if 'ECONNRESET' in text:
-                raise ConnectionReset()
-
-        logger.exception('_translate_errors has intercepted an unexpected exception')
-        raise UnknownError(text)
-
-
-def _translate_and_retry(fcn, try_count, post_params=None):
-    """
-    Try calling fcn try_count times, retrying only if
-    the exception is a retryable B2Error.
-
-    :param int try_count: a number of retries
-    :param dict post_params: request parameters
-    """
-    # For all but the last try, catch the exception.
-    wait_time = 1.0
-    for _ in range(try_count - 1):
+@contextmanager
+def setlocale(name):
+    with LOCALE_LOCK:
+        saved = locale.setlocale(locale.LC_ALL)
         try:
-            return _translate_errors(fcn, post_params)
-        except B2Error as e:
-            if not e.should_retry_http():
-                raise
-            logger.debug(str(e), exc_info=True)
-            if e.retry_after_seconds is not None:
-                sleep_duration = e.retry_after_seconds
-                sleep_reason = 'server asked us to'
-            else:
-                sleep_duration = wait_time
-                sleep_reason = 'that is what the default exponential backoff is'
-            logger.info('Pausing thread for %i seconds because %s', sleep_duration, sleep_reason)
-            time.sleep(sleep_duration)
-            wait_time *= 1.5
-
-    # If the last try gets an exception, it will be raised.
-    return _translate_errors(fcn, post_params)
+            yield locale.setlocale(locale.LC_ALL, name)
+        finally:
+            locale.setlocale(locale.LC_ALL, saved)
 
 
-class ResponseContextManager(object):
+class ResponseContextManager:
     """
     A context manager that closes a requests.Response when done.
     """
 
     def __init__(self, response):
         self.response = response
 
     def __enter__(self):
         return self.response
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self.response.close()
+        return None
 
 
-class HttpCallback(object):
+class HttpCallback:
     """
     A callback object that does nothing.  Overrides pre_request
     and/or post_request as desired.
     """
 
     def pre_request(self, method, url, headers):
         """
@@ -200,33 +140,34 @@
         :param response: a response object from the requests library
         """
         # Make a string that uses month numbers instead of month names
         server_date_str = response.headers['Date']
 
         # Convert the server time to a datetime object
         try:
-            server_time = arrow.get(
-                server_date_str, 'ddd, DD MMM YYYY HH:mm:ss ZZZ'
-            )  # this, unlike datetime.datetime.strptime, always uses English locale
-        except arrow.parser.ParserError:
+            with setlocale("C"):
+                server_time = datetime.datetime.strptime(
+                    server_date_str, '%a, %d %b %Y %H:%M:%S %Z'
+                )
+        except ValueError:
             logger.exception('server returned date in an inappropriate format')
             raise BadDateFormat(server_date_str)
 
         # Get the local time
-        local_time = arrow.utcnow()
+        local_time = datetime.datetime.utcnow()
 
         # Check the difference.
         max_allowed = 10 * 60  # ten minutes, in seconds
         skew = local_time - server_time
         skew_seconds = skew.total_seconds()
         if max_allowed < abs(skew_seconds):
             raise ClockSkew(skew_seconds)
 
 
-class B2Http(object):
+class B2Http:
     """
     A wrapper for the requests module.  Provides the operations
     needed to access B2, and handles retrying when the returned
     status is 503 Service Unavailable, 429 Too Many Requests, etc.
 
     The operations supported are:
 
@@ -241,92 +182,190 @@
 
        try:
            response_dict = b2_http.post_json_return_json(url, headers, params)
            ...
        except B2Error as e:
            ...
 
+    Please note that the timeout/retry system, including class-level variables,
+    is not a part of the interface and is subject to change.
     """
 
-    # timeout for HTTP GET/POST requests
-    TIMEOUT = 900  # 15 minutes as server-side copy can take time
+    CONNECTION_TIMEOUT = 3 + 6 + 12 + 24 + 1  # 4 standard tcp retransmissions + 1s latency
+    TIMEOUT = 128
+    TIMEOUT_FOR_COPY = 1200  # 20 minutes as server-side copy can take time
+    TIMEOUT_FOR_UPLOAD = 128
+    TRY_COUNT_DATA = 20
+    TRY_COUNT_DOWNLOAD = 20
+    TRY_COUNT_HEAD = 5
+    TRY_COUNT_OTHER = 5
 
-    def __init__(self, requests_module=None, install_clock_skew_hook=True, user_agent_append=None):
+    def __init__(self, api_config: B2HttpApiConfig = DEFAULT_HTTP_API_CONFIG):
         """
         Initialize with a reference to the requests module, which makes
         it easy to mock for testing.
-
-        :param requests_module: a reference to requests module
-        :param bool install_clock_skew_hook: if True, install a clock skew hook
-        :param str user_agent_append: if provided, the string will be appended to the User-Agent
-        """
-        requests_to_use = requests_module or requests
-        self.user_agent = self._get_user_agent(user_agent_append)
-        self.session = requests_to_use.Session()
+        """
+        self.user_agent = self._get_user_agent(api_config.user_agent_append)
+        self.session = api_config.http_session_factory()
+        if not api_config.decode_content:
+            self.session.adapters.clear()
+            self.session.mount('', NotDecompressingHTTPAdapter())
         self.callbacks = []
-        if install_clock_skew_hook:
+        if api_config.install_clock_skew_hook:
             self.add_callback(ClockSkewHook())
 
     def add_callback(self, callback):
         """
         Add a callback that inherits from HttpCallback.
 
         :param callback: a callback to be added to a chain
         :type callback: callable
         """
         self.callbacks.append(callback)
 
-    def post_content_return_json(self, url, headers, data, try_count=5, post_params=None):
+    def request(
+        self,
+        method: Literal['POST', 'GET', 'HEAD'],
+        url: str,
+        headers: dict[str, str],
+        data: io.BytesIO | bytes | None = None,
+        try_count: int = TRY_COUNT_DATA,
+        params: dict[str, str] | None = None,
+        *,
+        stream: bool = False,
+        _timeout: int | None = None,
+    ) -> requests.Response:
         """
         Use like this:
 
         .. code-block:: python
 
            try:
-               response_dict = b2_http.post_content_return_json(url, headers, data)
+               response_dict = b2_http.request('POST', url, headers, data)
                ...
            except B2Error as e:
                ...
 
-        :param str url: a URL to call
-        :param dict headers: headers to send.
-        :param data: bytes (Python 3) or str (Python 2), or a file-like object, to send
-        :return: a dict that is the decoded JSON
-        :rtype: dict
+        :param method: uppercase HTTP method name
+        :param url: a URL to call
+        :param headers: headers to send.
+        :param data: raw bytes or a file-like object to send
+        :param try_count: a number of retries
+        :param params: a dict that will be converted to query string for GET requests or additional metadata for POST requests
+        :param stream: if True, the response will be streamed
+        :param _timeout: a timeout for the request in seconds if not default
+        :return: final response
+        :raises: B2Error if the request fails
         """
+        method = method.upper()
         request_headers = {**headers, 'User-Agent': self.user_agent}
 
-        # Do the HTTP POST.  This may retry, so each post needs to
-        # rewind the data back to the beginning.
-        def do_post():
-            data.seek(0)
-            self._run_pre_request_hooks('POST', url, request_headers)
-            response = self.session.post(
-                url, headers=request_headers, data=data, timeout=self.TIMEOUT
+        def do_request():
+            # This may retry, so each time we need to rewind the data back to the beginning.
+            if data is not None and not isinstance(data, bytes):
+                data.seek(0)
+            self._run_pre_request_hooks(method, url, request_headers)
+            response = self.session.request(
+                method,
+                url,
+                headers=request_headers,
+                data=data,
+                params=params if method == 'GET' else None,
+                timeout=(self.CONNECTION_TIMEOUT, _timeout or self.TIMEOUT_FOR_UPLOAD),
+                stream=stream,
             )
-            self._run_post_request_hooks('POST', url, request_headers, response)
+            self._run_post_request_hooks(method, url, request_headers, response)
             return response
 
-        try:
-            response = _translate_and_retry(do_post, try_count, post_params)
-        except B2RequestTimeout:
-            # this forces a token refresh, which is necessary if request is still alive
-            # on the server but has terminated for some reason on the client. See #79
-            raise B2RequestTimeoutDuringUpload()
+        return self._translate_and_retry(do_request, try_count, params)
+
+    def request_content_return_json(
+        self,
+        method: Literal['POST', 'GET', 'HEAD'],
+        url: str,
+        headers: dict[str, str],
+        data: io.BytesIO | bytes | None = None,
+        try_count: int = TRY_COUNT_DATA,
+        params: dict[str, str] | None = None,
+        *,
+        _timeout: int | None = None,
+    ) -> JSON:
+        """
+        Use like this:
+
+        .. code-block:: python
+
+           try:
+               response_dict = b2_http.request_content_return_json('POST', url, headers, data)
+               ...
+           except B2Error as e:
+               ...
+
+        :param method: uppercase HTTP method name
+        :param url: a URL to call
+        :param headers: headers to send.
+        :param data: raw bytes or a file-like object to send
+        :return: decoded JSON
+        """
+        response = self.request(
+            method,
+            url,
+            headers={
+                **headers, 'Accept': 'application/json'
+            },
+            data=data,
+            try_count=try_count,
+            params=params,
+            _timeout=_timeout
+        )
 
         # Decode the JSON that came back.  If we've gotten this far,
         # we know we have a status of 200 OK.  In this case, the body
         # of the response is always JSON, so we don't need to handle
         # it being something else.
         try:
             return json.loads(response.content.decode('utf-8'))
         finally:
             response.close()
 
-    def post_json_return_json(self, url, headers, params, try_count=5):
+    def post_content_return_json(
+        self,
+        url: str,
+        headers: dict[str, str],
+        data: bytes | io.IOBase,
+        try_count: int = TRY_COUNT_DATA,
+        post_params: dict[str, str] | None = None,
+        _timeout: int | None = None,
+    ) -> JSON:
+        """
+        Use like this:
+
+        .. code-block:: python
+
+           try:
+               response_dict = b2_http.post_content_return_json(url, headers, data)
+               ...
+           except B2Error as e:
+               ...
+
+        :param str url: a URL to call
+        :param dict headers: headers to send.
+        :param data: a file-like object to send
+        :return: a dict that is the decoded JSON
+        """
+        try:
+            return self.request_content_return_json(
+                'POST', url, headers, data, try_count, post_params, _timeout=_timeout
+            )
+        except B2RequestTimeout:
+            # this forces a token refresh, which is necessary if request is still alive
+            # on the server but has terminated for some reason on the client. See #79
+            raise B2RequestTimeoutDuringUpload()
+
+    def post_json_return_json(self, url, headers, params, try_count: int = TRY_COUNT_OTHER):
         """
         Use like this:
 
         .. code-block:: python
 
            try:
                response_dict = b2_http.post_json_return_json(url, headers, params)
@@ -336,18 +375,35 @@
 
         :param str url: a URL to call
         :param dict headers: headers to send.
         :param dict params: a dict that will be converted to JSON
         :return: the decoded JSON document
         :rtype: dict
         """
-        data = io.BytesIO(json.dumps(params).encode())
-        return self.post_content_return_json(url, headers, data, try_count, params)
 
-    def get_content(self, url, headers, try_count=5):
+        # This is not just b2_copy_file or b2_copy_part, but it would not
+        # be good to find out by analyzing the url.
+        # In the future a more generic system between raw_api and b2http
+        # to indicate the timeouts should be designed.
+        timeout = self.TIMEOUT_FOR_COPY
+
+        data = json.dumps(params).encode()
+        return self.post_content_return_json(
+            url,
+            {
+                **headers,
+                'Content-Type': 'application/json',
+            },
+            data,
+            try_count,
+            params,
+            _timeout=timeout,
+        )
+
+    def get_content(self, url, headers, try_count: int = TRY_COUNT_DOWNLOAD):
         """
         Fetches content from a URL.
 
         Use like this:
 
         .. code-block:: python
 
@@ -363,29 +419,25 @@
             - iter_content()
 
         :param str url: a URL to call
         :param dict headers: headers to send
         :param int try_count: a number or retries
         :return: Context manager that returns an object that supports iter_content()
         """
-        request_headers = {**headers, 'User-Agent': self.user_agent}
-
-        # Do the HTTP GET.
-        def do_get():
-            self._run_pre_request_hooks('GET', url, request_headers)
-            response = self.session.get(
-                url, headers=request_headers, stream=True, timeout=self.TIMEOUT
-            )
-            self._run_post_request_hooks('GET', url, request_headers, response)
-            return response
-
-        response = _translate_and_retry(do_get, try_count, None)
+        response = self.request(
+            'GET', url, headers=headers, try_count=try_count, stream=True, _timeout=self.TIMEOUT
+        )
         return ResponseContextManager(response)
 
-    def head_content(self, url: str, headers: Dict[str, Any], try_count: int = 5) -> Dict[str, Any]:
+    def head_content(
+        self,
+        url: str,
+        headers: dict[str, Any],
+        try_count: int = TRY_COUNT_HEAD,
+    ) -> requests.Response:
         """
         Does a HEAD instead of a GET for the URL.
         The response's content is limited to the headers.
 
         Use like this:
 
         .. code-block:: python
@@ -398,101 +450,176 @@
 
         The response object is only guaranteed to have:
             - headers
 
         :param str url: a URL to call
         :param dict headers: headers to send
         :param int try_count: a number or retries
-        :return: the decoded response
-        :rtype: dict
+        :return: HTTP response
         """
-        request_headers = {**headers, 'User-Agent': self.user_agent}
-
-        # Do the HTTP HEAD.
-        def do_head():
-            self._run_pre_request_hooks('HEAD', url, request_headers)
-            response = self.session.head(
-                url, headers=request_headers, stream=True, timeout=self.TIMEOUT
-            )
-            self._run_post_request_hooks('HEAD', url, request_headers, response)
-            return response
-
-        return _translate_and_retry(do_head, try_count, None)
+        return self.request('HEAD', url, headers=headers, try_count=try_count)
 
     @classmethod
     def _get_user_agent(cls, user_agent_append):
         if user_agent_append:
-            return '%s %s' % (USER_AGENT, user_agent_append)
+            return f'{USER_AGENT} {user_agent_append}'
         return USER_AGENT
 
     def _run_pre_request_hooks(self, method, url, headers):
         for callback in self.callbacks:
             callback.pre_request(method, url, headers)
 
     def _run_post_request_hooks(self, method, url, headers, response):
         for callback in self.callbacks:
             callback.post_request(method, url, headers, response)
 
+    @classmethod
+    def _translate_errors(cls, fcn, post_params=None):
+        """
+        Call the given function, turning any exception raised into the right
+        kind of B2Error.
 
-def test_http():
-    """
-    Run a few tests on error diagnosis.
+        :param dict post_params: request parameters
+        """
+        response = None
+        try:
+            response = fcn()
+            if response.status_code not in (200, 206):
+                # Decode the error object returned by the service
+                try:
+                    error = json.loads(response.content.decode('utf-8')) if response.content else {}
+                    if not isinstance(error, dict):
+                        raise ValueError('json error value is not a dict')
+                except (json.JSONDecodeError, UnicodeDecodeError, ValueError):
+                    logger.error('failed to decode error response: %r', response.content)
+                    # When the user points to an S3 endpoint, he won't receive the JSON error
+                    # he expects. In that case, we can provide at least a hint of "what happened".
+                    # s3 url has the form of e.g. https://s3.us-west-000.backblazeb2.com
+                    if '://s3.' in response.url:
+                        raise PotentialS3EndpointPassedAsRealm(response.content)
+                    error = {
+                        'message': response.content.decode('utf-8', errors='replace'),
+                        'code': 'non_json_response',
+                    }
+                extra_error_keys = error.keys() - ('code', 'status', 'message')
+                if extra_error_keys:
+                    logger.debug(
+                        'received error has extra (unsupported) keys: %s', extra_error_keys
+                    )
+
+                try:
+                    status = int(error.get('status', response.status_code))
+                    if status != response.status_code:
+                        raise ValueError('status code is not equal to the one in the response')
+                except (TypeError, ValueError) as exc:
+                    logger.warning(
+                        'Inconsistent status codes returned by the server %r != %r; parsing exception: %r',
+                        error.get('status'), response.status_code, exc
+                    )
+                    status = response.status_code
+
+                raise interpret_b2_error(
+                    status,
+                    str(error['code']) if 'code' in error else None,
+                    str(error['message']) if 'message' in error else None,
+                    response.headers,
+                    post_params,
+                )
+            return response
 
-    This test takes a while to run and is not used in the automated tests
-    during building.  Run the test by hand to exercise the code.
-    """
+        except B2Error:
+            raise  # pass through exceptions from just above
 
-    from .exception import BadJson
+        except requests.ConnectionError as e0:
+            e1 = e0.args[0]
+            if isinstance(e1, requests.packages.urllib3.exceptions.MaxRetryError):
+                msg = e1.args[0]
+                if 'nodename nor servname provided, or not known' in msg:
+                    # Unknown host, or DNS failing.  In the context of calling
+                    # B2, this means that something is down between here and
+                    # Backblaze, so we treat it like 503 Service Unavailable.
+                    raise UnknownHost()
+            elif isinstance(e1, requests.packages.urllib3.exceptions.ProtocolError):
+                e2 = e1.args[1]
+                if isinstance(e2, socket.error):
+                    if len(e2.args) >= 2 and e2.args[1] == 'Broken pipe':
+                        # Broken pipes are usually caused by the service rejecting
+                        # an upload request for cause, so we use a 400 Bad Request
+                        # code.
+                        raise BrokenPipe()
+            raise B2ConnectionError(str(e0))
+
+        except requests.Timeout as e:
+            raise B2RequestTimeout(str(e))
+
+        except Exception as e:
+            text = repr(e)
+
+            # This is a special case to handle when urllib3 doesn't translate
+            # ECONNRESET into something that requests can turn into something
+            # we understand.  The SysCallError is from the optional library
+            # pyOpenSsl, which we don't require, so we can't import it and
+            # catch it explicitly.
+            #
+            # The text from one such error looks like this: SysCallError(104, 'ECONNRESET')
+            if text.startswith('SysCallError'):
+                if 'ECONNRESET' in text:
+                    raise ConnectionReset()
 
-    b2_http = B2Http()
+            logger.exception('_translate_errors has intercepted an unexpected exception')
+            raise UnknownError(text)
 
-    # Error from B2
-    print('TEST: error object from B2')
-    try:
-        b2_http.post_json_return_json(
-            'https://api.backblazeb2.com/b2api/v1/b2_get_file_info', {}, {}
-        )
-        assert False, 'should have failed with bad json'
-    except BadJson as e:
-        assert str(e) == 'Bad request: required field fileId is missing'
-
-    # Successful get
-    print('TEST: get')
-    with b2_http.get_content(
-        'https://api.backblazeb2.com/test/echo_zeros?length=10', {}
-    ) as response:
-        assert response.status_code == 200
-        response_data = b''.join(response.iter_content())
-        assert response_data == b'\x00' * 10
-
-    # Successful post
-    print('TEST: post')
-    response_dict = b2_http.post_json_return_json(
-        'https://api.backblazeb2.com/api/build_version', {}, {}
-    )
-    assert 'timestamp' in response_dict
-
-    # Unknown host
-    print('TEST: unknown host')
-    try:
-        b2_http.post_json_return_json('https://unknown.backblazeb2.com', {}, {})
-        assert False, 'should have failed with unknown host'
-    except UnknownHost:
-        pass
-
-    # Broken pipe
-    print('TEST: broken pipe')
-    try:
-        data = io.BytesIO(b'\x00' * 10000000)
-        b2_http.post_content_return_json('https://api.backblazeb2.com/bad_url', {}, data)
-        assert False, 'should have failed with broken pipe'
-    except BrokenPipe:
-        pass
-
-    # Generic connection error
-    print('TEST: generic connection error')
-    try:
-        with b2_http.get_content('https://www.backblazeb2.com:80/bad_url', {}) as response:
-            assert False, 'should have failed with connection error'
-            response.iter_content()  # make pyflakes happy
-    except B2ConnectionError:
-        pass
+    @classmethod
+    def _translate_and_retry(
+        cls, fcn: Callable, try_count: int, post_params: dict[str, Any] | None = None
+    ):
+        """
+        Try calling fcn try_count times, retrying only if
+        the exception is a retryable B2Error.
+
+        :param fcn: request function to call
+        :param try_count: a number of retries
+        :param post_params: request parameters
+        """
+        # For all but the last try, catch the exception.
+        wait_time = 1.0
+        max_wait_time = 64
+        for _ in range(try_count - 1):
+            try:
+                return cls._translate_errors(fcn, post_params)
+            except B2Error as e:
+                if not e.should_retry_http():
+                    raise
+                logger.debug(str(e), exc_info=True)
+                if e.retry_after_seconds is not None:
+                    sleep_duration = e.retry_after_seconds
+                    sleep_reason = 'server asked us to'
+                else:
+                    sleep_duration = wait_time
+                    sleep_reason = 'that is what the default exponential backoff is'
+
+                logger.info(
+                    'Pausing thread for %i seconds because %s',
+                    sleep_duration,
+                    sleep_reason,
+                )
+                time.sleep(sleep_duration)
+
+                # Set up wait time for the next iteration
+                wait_time *= 1.5
+                if wait_time > max_wait_time:
+                    # avoid clients synchronizing and causing a wave
+                    # of requests when connectivity is restored
+                    wait_time = max_wait_time + random()
+
+        # If the last try gets an exception, it will be raised.
+        return cls._translate_errors(fcn, post_params)
+
+
+class NotDecompressingHTTPAdapter(HTTPAdapter):
+    """
+    HTTP adapter that uses :class:`b2sdk._internal.requests.NotDecompressingResponse` instead of the default
+    :code:`requests.Response` class.
+    """
+
+    def build_response(self, req, resp):
+        return NotDecompressingResponse.from_builtin_response(super().build_response(req, resp))
```

### Comparing `b2sdk-1.9.0/b2sdk/bounded_queue_executor.py` & `b2sdk-2.0.0/b2sdk/_internal/bounded_queue_executor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 ######################################################################
 #
-# File: b2sdk/bounded_queue_executor.py
+# File: b2sdk/_internal/bounded_queue_executor.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import threading
 
 
-class BoundedQueueExecutor(object):
+class BoundedQueueExecutor:
     """
     Wrap a concurrent.futures.Executor and limits the number of requests that
     can be queued at once.  Requests to submit() tasks block until
     there is room in the queue.
 
     The number of available slots in the queue is tracked with a
     semaphore that is acquired before queueing an action, and
```

### Comparing `b2sdk-1.9.0/b2sdk/cache.py` & `b2sdk-2.0.0/b2sdk/_internal/cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 ######################################################################
 #
-# File: b2sdk/cache.py
+# File: b2sdk/_internal/cache.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
-from typing import Optional
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from b2sdk._internal.account_info.abstract import AbstractAccountInfo
 
 
 class AbstractCache(metaclass=ABCMeta):
     def clear(self):
         self.set_bucket_name_cache(tuple())
 
     @abstractmethod
@@ -21,18 +25,26 @@
         pass
 
     @abstractmethod
     def get_bucket_name_or_none_from_allowed(self):
         pass
 
     @abstractmethod
-    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> Optional[str]:
+    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> str | None:
         pass
 
     @abstractmethod
+    def list_bucket_names_ids(self) -> list[tuple[str, str]]:
+        """
+        List buckets in the cache.
+
+        :return: list of tuples (bucket_name, bucket_id)
+        """
+
+    @abstractmethod
     def save_bucket(self, bucket):
         pass
 
     @abstractmethod
     def set_bucket_name_cache(self, buckets):
         pass
 
@@ -44,70 +56,79 @@
     """
     A cache that does nothing.
     """
 
     def get_bucket_id_or_none_from_bucket_name(self, name):
         return None
 
-    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> Optional[str]:
+    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> str | None:
         return None
 
     def get_bucket_name_or_none_from_allowed(self):
         return None
 
+    def list_bucket_names_ids(self) -> list[tuple[str, str]]:
+        return []
+
     def save_bucket(self, bucket):
         pass
 
     def set_bucket_name_cache(self, buckets):
         pass
 
 
 class InMemoryCache(AbstractCache):
     """
     A cache that stores the information in memory.
     """
 
     def __init__(self):
         self.name_id_map = {}
-        self.bucket_name = ''
+        self.bucket_name = None
 
     def get_bucket_id_or_none_from_bucket_name(self, name):
         return self.name_id_map.get(name)
 
-    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> Optional[str]:
+    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> str | None:
         for name, cached_id_ in self.name_id_map.items():
             if cached_id_ == bucket_id:
                 return name
         return None
 
     def get_bucket_name_or_none_from_allowed(self):
         return self.bucket_name
 
+    def list_bucket_names_ids(self) -> list[tuple[str, str]]:
+        return sorted(tuple(item) for item in self.name_id_map.items())
+
     def save_bucket(self, bucket):
         self.name_id_map[bucket.name] = bucket.id_
 
     def set_bucket_name_cache(self, buckets):
         self.name_id_map = dict(self._name_id_iterator(buckets))
 
 
 class AuthInfoCache(AbstractCache):
     """
     A cache that stores data persistently in StoredAccountInfo.
     """
 
-    def __init__(self, info):
+    def __init__(self, info: AbstractAccountInfo):
         self.info = info
 
     def get_bucket_id_or_none_from_bucket_name(self, name):
         return self.info.get_bucket_id_or_none_from_bucket_name(name)
 
-    def get_bucket_name_or_none_from_bucket_id(self, bucket_id) -> Optional[str]:
+    def get_bucket_name_or_none_from_bucket_id(self, bucket_id) -> str | None:
         return self.info.get_bucket_name_or_none_from_bucket_id(bucket_id)
 
     def get_bucket_name_or_none_from_allowed(self):
         return self.info.get_bucket_name_or_none_from_allowed()
 
+    def list_bucket_names_ids(self) -> list[tuple[str, str]]:
+        return self.info.list_bucket_names_ids()
+
     def save_bucket(self, bucket):
         self.info.save_bucket(bucket)
 
     def set_bucket_name_cache(self, buckets):
         self.info.refresh_entire_bucket_name_cache(self._name_id_iterator(buckets))
```

### Comparing `b2sdk-1.9.0/b2sdk/download_dest.py` & `b2sdk-2.0.0/b2sdk/v1/download_dest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 ######################################################################
 #
-# File: b2sdk/download_dest.py
+# File: b2sdk/v1/download_dest.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import io
 import os
 from abc import abstractmethod
 from contextlib import contextmanager
 
-from b2sdk.stream.progress import WritingStreamWithProgress
+from b2sdk._internal.stream.progress import WritingStreamWithProgress
 
-from .utils import B2TraceMetaAbstract, limit_trace_arguments, set_file_mtime
+from b2sdk._internal.utils import B2TraceMetaAbstract, limit_trace_arguments, set_file_mtime
 
 
 class AbstractDownloadDestination(metaclass=B2TraceMetaAbstract):
     """
     Interface to a destination for a downloaded file.
     """
 
@@ -85,22 +86,18 @@
         return self.write_to_local_file_context(mod_time_millis)
 
     @contextmanager
     def write_to_local_file_context(self, mod_time_millis):
         completed = False
         try:
             # Open the file and let the caller write it.
-            with io.open(self.local_file_path, self.MODE) as f:
+            with open(self.local_file_path, self.MODE) as f:
                 yield f
 
-            # After it's closed, set the mod time.
-            # This is an ugly hack to make the tests work.  I can't think
-            # of any other cases where set_file_mtime might fail.
-            if self.local_file_path != os.devnull:
-                set_file_mtime(self.local_file_path, mod_time_millis)
+            set_file_mtime(self.local_file_path, mod_time_millis)
 
             # Set the flag that means to leave the downloaded file on disk.
             completed = True
 
         finally:
             # This is a best-effort attempt to clean up files that
             # failed to download, so we don't leave partial files
@@ -115,19 +112,19 @@
     Does not truncate the target file, seeks to a given offset just after opening
     a descriptor.
     """
     MODE = 'rb+'
 
     def __init__(self, local_file_path, seek_target):
         self._seek_target = seek_target
-        super(PreSeekedDownloadDest, self).__init__(local_file_path)
+        super().__init__(local_file_path)
 
     @contextmanager
     def write_to_local_file_context(self, *args, **kwargs):
-        with super(PreSeekedDownloadDest, self).write_to_local_file_context(*args, **kwargs) as f:
+        with super().write_to_local_file_context(*args, **kwargs) as f:
             f.seek(self._seek_target)
             yield f
 
 
 class DownloadDestBytes(AbstractDownloadDestination):
     """
     Store a downloaded file into bytes in memory.
```

### Comparing `b2sdk-1.9.0/b2sdk/encryption/setting.py` & `b2sdk-2.0.0/b2sdk/_internal/encryption/setting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,72 @@
 ######################################################################
 #
-# File: b2sdk/encryption/setting.py
+# File: b2sdk/_internal/encryption/setting.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
+import enum
 import logging
-from typing import Optional
 import urllib
 import urllib.parse
 
+from ..http_constants import SSE_C_KEY_ID_FILE_INFO_KEY_NAME, SSE_C_KEY_ID_HEADER
 from ..utils import b64_of_bytes, md5_of_bytes
-from .types import ENCRYPTION_MODES_WITH_MANDATORY_ALGORITHM, ENCRYPTION_MODES_WITH_MANDATORY_KEY
-from .types import EncryptionAlgorithm, EncryptionMode
-
-SSE_C_KEY_ID_FILE_INFO_KEY_NAME = 'sse_c_key_id'
+from .types import (
+    ENCRYPTION_MODES_WITH_MANDATORY_ALGORITHM,
+    ENCRYPTION_MODES_WITH_MANDATORY_KEY,
+    EncryptionAlgorithm,
+    EncryptionMode,
+)
 
 logger = logging.getLogger(__name__)
 
 
+class _UnknownKeyId(enum.Enum):
+    """The purpose of this enum is to provide a sentinel that can be used with type annotations."""
+    unknown_key_id = 0
+
+
+UNKNOWN_KEY_ID = _UnknownKeyId.unknown_key_id
+"""
+Value for EncryptionKey.key_id that signifies that the key id may or may not be defined. Useful when establishing
+encryption settings based on user input (and not based on B2 cloud data).
+"""
+
+
 class EncryptionKey:
     """
     Hold information about encryption key: the key itself, and its id. The id may be None, if it's not set
-    in encrypted file's fileInfo. The secret may be None, if encryption metadata is read from the server.
+    in encrypted file's fileInfo, or UNKNOWN_KEY_ID when that information is missing.
+    The secret may be None, if encryption metadata is read from the server.
     """
     SECRET_REPR = '******'
 
-    def __init__(self, secret: Optional[bytes], key_id: Optional[str]):
+    def __init__(self, secret: bytes | None, key_id: str | None | _UnknownKeyId):
         self.secret = secret
         self.key_id = key_id
 
     def __eq__(self, other):
         return self.secret == other.secret and self.key_id == other.key_id
 
     def __repr__(self):
         key_repr = self.SECRET_REPR
         if self.secret is None:
             key_repr = None
-        return '<%s(%s, %s)>' % (self.__class__.__name__, key_repr, self.key_id)
+
+        if self.key_id is UNKNOWN_KEY_ID:
+            key_id_repr = 'unknown'
+        else:
+            key_id_repr = repr(self.key_id)
+        return f'<{self.__class__.__name__}({key_repr}, {key_id_repr})>'
 
     def as_dict(self):
         """
         Dump EncryptionKey as dict for serializing a to json for requests.
         """
         if self.secret is not None:
             return {
@@ -72,29 +94,28 @@
     def __init__(
         self,
         mode: EncryptionMode,
         algorithm: EncryptionAlgorithm = None,
         key: EncryptionKey = None,
     ):
         """
-        :param b2sdk.v1.EncryptionMode mode: encryption mode
-        :param b2sdk.v1.EncryptionAlgorithm algorithm: encryption algorithm
-        :param b2sdk.v1.EncryptionKey key: encryption key object for SSE-C
+        :param b2sdk.v2.EncryptionMode mode: encryption mode
+        :param b2sdk.v2.EncryptionAlgorithm algorithm: encryption algorithm
+        :param b2sdk.v2.EncryptionKey key: encryption key object for SSE-C
         """
         self.mode = mode
         self.algorithm = algorithm
         self.key = key
         if self.mode == EncryptionMode.NONE and (self.algorithm or self.key):
             raise ValueError("cannot specify algorithm or key for 'plaintext' encryption mode")
         if self.mode in ENCRYPTION_MODES_WITH_MANDATORY_ALGORITHM and not self.algorithm:
-            raise ValueError('must specify algorithm for encryption mode %s' % (self.mode,))
+            raise ValueError(f'must specify algorithm for encryption mode {self.mode}')
         if self.mode in ENCRYPTION_MODES_WITH_MANDATORY_KEY and not self.key:
             raise ValueError(
-                'must specify key for encryption mode %s and algorithm %s' %
-                (self.mode, self.algorithm)
+                f'must specify key for encryption mode {self.mode} and algorithm {self.algorithm}'
             )
 
     def __eq__(self, other):
         if other is None:
             raise ValueError('cannot compare a known encryption setting to an unknown one')
         return self.mode == other.mode and self.algorithm == other.algorithm and self.key == other.key
 
@@ -141,64 +162,70 @@
     def add_to_upload_headers(self, headers):
         if self.mode == EncryptionMode.NONE:
             # as of 2021-03-16, server always fails it
             headers['X-Bz-Server-Side-Encryption'] = self.mode.name
         elif self.mode == EncryptionMode.SSE_B2:
             self._add_sse_b2_headers(headers)
         elif self.mode == EncryptionMode.SSE_C:
+            if self.key.key_id is UNKNOWN_KEY_ID:
+                raise ValueError('Cannot upload a file with an unknown key id')
             self._add_sse_c_headers(headers)
             if self.key.key_id is not None:
-                header = 'X-Bz-Info-%s' % (SSE_C_KEY_ID_FILE_INFO_KEY_NAME,)
+                header = SSE_C_KEY_ID_HEADER
                 if headers.get(header) is not None and headers[header] != self.key.key_id:
                     raise ValueError(
-                        'Ambiguous key id set: "%s" in headers and "%s" in %s' %
-                        (headers[header], self.key.key_id, self.__class__.__name__)
+                        f'Ambiguous key id set: "{headers[header]}" in headers and "{self.key.key_id}" in {self.__class__.__name__}'
                     )
                 headers[header] = urllib.parse.quote(str(self.key.key_id))
         else:
-            raise NotImplementedError('unsupported encryption setting: %s' % (self,))
+            raise NotImplementedError(f'unsupported encryption setting: {self}')
 
     def add_to_download_headers(self, headers):
         if self.mode == EncryptionMode.NONE:
             return
         elif self.mode == EncryptionMode.SSE_B2:
             self._add_sse_b2_headers(headers)
         elif self.mode == EncryptionMode.SSE_C:
             self._add_sse_c_headers(headers)
         else:
-            raise NotImplementedError('unsupported encryption setting: %s' % (self,))
+            raise NotImplementedError(f'unsupported encryption setting: {self}')
 
     def _add_sse_b2_headers(self, headers):
         headers['X-Bz-Server-Side-Encryption'] = self.algorithm.name
 
     def _add_sse_c_headers(self, headers):
         if self.key.secret is None:
             raise ValueError('Cannot use an unknown key in http headers')
         headers['X-Bz-Server-Side-Encryption-Customer-Algorithm'] = self.algorithm.name
         headers['X-Bz-Server-Side-Encryption-Customer-Key'] = self.key.key_b64()
         headers['X-Bz-Server-Side-Encryption-Customer-Key-Md5'] = self.key.key_md5()
 
-    def add_key_id_to_file_info(self, file_info: Optional[dict]):
+    def add_key_id_to_file_info(self, file_info: dict | None):
         if self.key is None or self.key.key_id is None:
             return file_info
+        if self.key.key_id is UNKNOWN_KEY_ID:
+            raise ValueError('Cannot add an unknown key id to file info')
         if file_info is None:
             file_info = {}
         if file_info.get(SSE_C_KEY_ID_FILE_INFO_KEY_NAME) is not None and file_info[
             SSE_C_KEY_ID_FILE_INFO_KEY_NAME] != self.key.key_id:
             raise ValueError(
-                'Ambiguous key id set: "%s" in file_info and "%s" in %s' % (
+                'Ambiguous key id set: "{}" in file_info and "{}" in {}'.format(
                     file_info[SSE_C_KEY_ID_FILE_INFO_KEY_NAME], self.key.key_id,
                     self.__class__.__name__
                 )
             )
         file_info[SSE_C_KEY_ID_FILE_INFO_KEY_NAME] = self.key.key_id
         return file_info
 
     def __repr__(self):
-        return '<%s(%s, %s, %s)>' % (self.__class__.__name__, self.mode, self.algorithm, self.key)
+        return f'<{self.__class__.__name__}({self.mode}, {self.algorithm}, {self.key})>'
+
+    def is_unknown(self):
+        return self.mode == EncryptionMode.NONE
 
 
 class EncryptionSettingFactory:
     # 2021-03-17: for the bucket the response of the server is:
     # if authorized to read:
     #    "mode": "none"
     #    or
@@ -232,15 +259,15 @@
         file_info = file_version_dict.get('fileInfo')
         if file_info is not None and SSE_C_KEY_ID_FILE_INFO_KEY_NAME in file_info:
             key_id = urllib.parse.unquote(file_info[SSE_C_KEY_ID_FILE_INFO_KEY_NAME])
 
         return cls._from_value_dict(sse, key_id=key_id)
 
     @classmethod
-    def from_bucket_dict(cls, bucket_dict: dict) -> Optional[EncryptionSetting]:
+    def from_bucket_dict(cls, bucket_dict: dict) -> EncryptionSetting | None:
         """
         Returns EncryptionSetting for the given bucket dict retrieved from the api, or None if unauthorized
 
         Example inputs:
 
         .. code-block:: python
 
@@ -305,26 +332,27 @@
             if mode == EncryptionMode.SSE_C:
                 kwargs['key'] = EncryptionKey(key_id=key_id, secret=None)
 
         return EncryptionSetting(**kwargs)
 
     @classmethod
     def from_response_headers(cls, headers):
-
-        mode = EncryptionMode(headers.get('X-Bz-Server-Side-Encryption', 'none'))
-        kwargs = {
-            'mode': mode,
-        }
-        if mode == EncryptionMode.SSE_C:
-            kwargs['key'] = EncryptionKey(secret=None, key_id=None)
-        algorithm = headers.get('X-Bz-Server-Side-Encryption-Customer-Algorithm')
-        if algorithm is not None:
-            kwargs['algorithm'] = EncryptionAlgorithm(algorithm)
-
-        return EncryptionSetting(**kwargs)
+        if 'X-Bz-Server-Side-Encryption' in headers:
+            mode = EncryptionMode.SSE_B2
+            algorithm = EncryptionAlgorithm(headers['X-Bz-Server-Side-Encryption'])
+            return EncryptionSetting(mode, algorithm)
+        if 'X-Bz-Server-Side-Encryption-Customer-Algorithm' in headers:
+            mode = EncryptionMode.SSE_C
+            algorithm = EncryptionAlgorithm(
+                headers['X-Bz-Server-Side-Encryption-Customer-Algorithm']
+            )
+            key_id = headers.get(SSE_C_KEY_ID_HEADER)
+            key = EncryptionKey(secret=None, key_id=key_id)
+            return EncryptionSetting(mode, algorithm, key)
+        return EncryptionSetting(EncryptionMode.NONE)
 
 
 SSE_NONE = EncryptionSetting(mode=EncryptionMode.NONE,)
 """
 Commonly used "no encryption" setting
 """
```

### Comparing `b2sdk-1.9.0/b2sdk/encryption/types.py` & `b2sdk-2.0.0/b2sdk/_internal/encryption/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 ######################################################################
 #
-# File: b2sdk/encryption/types.py
+# File: b2sdk/_internal/encryption/types.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 from enum import Enum, unique
 
 
 @unique
 class EncryptionAlgorithm(Enum):
     """Encryption algorithm."""
 
     AES256 = 'AES256'
 
+    def get_length(self) -> int:
+        if self is EncryptionAlgorithm.AES256:
+            return int(256 / 8)
+
+        raise NotImplementedError()
+
 
 @unique
 class EncryptionMode(Enum):
     """Encryption mode."""
 
     UNKNOWN = None  #: unknown encryption mode (sdk doesn't know or used key has no rights to know)
     NONE = "none"  #: no encryption (plaintext)
```

### Comparing `b2sdk-1.9.0/b2sdk/exception.py` & `b2sdk-2.0.0/b2sdk/_internal/exception.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 ######################################################################
 #
-# File: b2sdk/exception.py
+# File: b2sdk/_internal/exception.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from abc import ABCMeta
-
+import logging
 import re
-from typing import Any, Dict, Optional
+import warnings
+from abc import ABCMeta
+from typing import Any
 
-from .utils import camelcase_to_underscore
+from .utils import camelcase_to_underscore, trace_call
 
 UPLOAD_TOKEN_USED_CONCURRENTLY_ERROR_MESSAGE_RE = re.compile(
     r'^more than one upload using auth token (?P<token>[^)]+)$'
 )
 
+COPY_SOURCE_TOO_BIG_ERROR_MESSAGE_RE = re.compile(r'^Copy source too big: (?P<size>[\d]+)$')
+
+logger = logging.getLogger(__name__)
+
 
 class B2Error(Exception, metaclass=ABCMeta):
     def __init__(self, *args, **kwargs):
         """
         Python 2 does not like it when you pass unicode as the message
         in an exception.  We like to use file names in exception messages.
         To avoid problems, if the message has any non-ascii characters in
         it, they are replaced with backslash-uNNNN.
 
         https://pythonhosted.org/kitchen/unicode-frustrations.html#frustration-5-exceptions
         """
         # If the exception is caused by a b2 server response,
         # the server MAY have included instructions to pause the thread before issuing any more requests
         self.retry_after_seconds = None
-        super(B2Error, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     @property
     def prefix(self):
         """
         Nice, auto-generated error message prefix.
 
         >>> B2SimpleError().prefix
@@ -62,21 +68,25 @@
         """
         Return true if this is an error that should tell the upload
         code to get a new upload URL and try the upload again.
         """
         return False
 
 
+class InvalidUserInput(B2Error):
+    pass
+
+
 class B2SimpleError(B2Error, metaclass=ABCMeta):
     """
     A B2Error with a message prefix.
     """
 
     def __str__(self):
-        return '%s: %s' % (self.prefix, super(B2SimpleError, self).__str__())
+        return f'{self.prefix}: {super().__str__()}'
 
 
 class NotAllowedByAppKeyError(B2SimpleError, metaclass=ABCMeta):
     """
     Base class for errors caused by restrictions on an application key.
     """
 
@@ -120,21 +130,21 @@
 
 class CapabilityNotAllowed(NotAllowedByAppKeyError):
     pass
 
 
 class ChecksumMismatch(TransientErrorMixin, B2Error):
     def __init__(self, checksum_type, expected, actual):
-        super(ChecksumMismatch, self).__init__()
+        super().__init__()
         self.checksum_type = checksum_type
         self.expected = expected
         self.actual = actual
 
     def __str__(self):
-        return '%s checksum mismatch -- bad data' % (self.checksum_type,)
+        return f'{self.checksum_type} checksum mismatch -- bad data'
 
 
 class B2HttpCallbackException(B2SimpleError):
     pass
 
 
 class B2HttpCallbackPostRequestException(B2HttpCallbackException):
@@ -154,15 +164,15 @@
     The clock on the server differs from the local clock by too much.
     """
 
     def __init__(self, clock_skew_seconds):
         """
         :param int clock_skew_seconds: The difference: local_clock - server_clock
         """
-        super(ClockSkew, self).__init__()
+        super().__init__()
         self.clock_skew_seconds = clock_skew_seconds
 
     def __str__(self):
         if self.clock_skew_seconds < 0:
             return 'ClockSkew: local clock is %d seconds behind server' % (
                 -self.clock_skew_seconds,
             )
@@ -196,22 +206,22 @@
     # if a timeout is hit during upload, it is not guaranteed that the the server has released the upload token lock already, so we'll use a new token
     def should_retry_http(self):
         return False
 
 
 class DestFileNewer(B2Error):
     def __init__(self, dest_path, source_path, dest_prefix, source_prefix):
-        super(DestFileNewer, self).__init__()
+        super().__init__()
         self.dest_path = dest_path
         self.source_path = source_path
         self.dest_prefix = dest_prefix
         self.source_prefix = source_prefix
 
     def __str__(self):
-        return 'source file is older than destination: %s%s with a time of %s cannot be synced to %s%s with a time of %s, unless a valid newer_file_mode is provided' % (
+        return 'source file is older than destination: {}{} with a time of {} cannot be synced to {}{} with a time of {}, unless a valid newer_file_mode is provided'.format(
             self.source_prefix,
             self.source_path.relative_path,
             self.source_path.mod_time,
             self.dest_prefix,
             self.dest_path.relative_path,
             self.dest_path.mod_time,
         )
@@ -226,34 +236,42 @@
 
 class ResourceNotFound(B2SimpleError):
     prefix = 'No such file, bucket, or endpoint'
 
 
 class FileOrBucketNotFound(ResourceNotFound):
     def __init__(self, bucket_name=None, file_id_or_name=None):
-        super(FileOrBucketNotFound, self).__init__()
+        super().__init__()
         self.bucket_name = bucket_name
         self.file_id_or_name = file_id_or_name
 
     def __str__(self):
         file_str = ('file [%s]' % self.file_id_or_name) if self.file_id_or_name else 'a file'
         bucket_str = ('bucket [%s]' % self.bucket_name) if self.bucket_name else 'a bucket'
-        return 'Could not find %s within %s' % (file_str, bucket_str)
+        return f'Could not find {file_str} within {bucket_str}'
+
+
+class BucketIdNotFound(ResourceNotFound):
+    def __init__(self, bucket_id):
+        self.bucket_id = bucket_id
+
+    def __str__(self):
+        return f'Bucket with id={self.bucket_id} not found'
 
 
 class FileAlreadyHidden(B2SimpleError):
     pass
 
 
 class FileNameNotAllowed(NotAllowedByAppKeyError):
     pass
 
 
 class FileNotPresent(FileOrBucketNotFound):
-    def __str__(self):  # overriden to retain message across prev versions
+    def __str__(self):  # overridden to retain message across prev versions
         return "File not present%s" % (': ' + self.file_id_or_name if self.file_id_or_name else "")
 
 
 class UnusableFileName(B2SimpleError):
     """
     Raise when a filename doesn't meet the rules.
 
@@ -269,15 +287,15 @@
 
 class SSECKeyIdMismatchInCopy(InvalidMetadataDirective):
     pass
 
 
 class InvalidRange(B2Error):
     def __init__(self, content_length, range_):
-        super(InvalidRange, self).__init__()
+        super().__init__()
         self.content_length = content_length
         self.range_ = range_
 
     def __str__(self):
         return 'A range of %d-%d was requested (size of %d), but cloud could only serve %d of that' % (
             self.range_[0],
             self.range_[1],
@@ -288,103 +306,115 @@
 
 class InvalidUploadSource(B2SimpleError):
     pass
 
 
 class BadRequest(B2Error):
     def __init__(self, message, code):
-        super(BadRequest, self).__init__()
+        super().__init__()
         self.message = message
         self.code = code
 
     def __str__(self):
-        return '%s (%s)' % (self.message, self.code)
+        return f'{self.message} ({self.code})'
+
+
+class CopySourceTooBig(BadRequest):
+    def __init__(self, message, code, size: int):
+        super().__init__(message, code)
+        self.size = size
 
 
 class Unauthorized(B2Error):
     def __init__(self, message, code):
-        super(Unauthorized, self).__init__()
+        super().__init__()
         self.message = message
         self.code = code
 
     def __str__(self):
-        return '%s (%s)' % (self.message, self.code)
+        return f'{self.message} ({self.code})'
 
     def should_retry_upload(self):
         return True
 
 
+class EmailNotVerified(Unauthorized):
+    def should_retry_upload(self):
+        return False
+
+
 class InvalidAuthToken(Unauthorized):
     """
     Specific type of Unauthorized that means the auth token is invalid.
     This is not the case where the auth token is valid, but does not
     allow access.
     """
 
     def __init__(self, message, code):
-        super(InvalidAuthToken,
-              self).__init__('Invalid authorization token. Server said: ' + message, code)
+        super().__init__('Invalid authorization token. Server said: ' + message, code)
 
 
 class RestrictedBucket(B2Error):
     def __init__(self, bucket_name):
-        super(RestrictedBucket, self).__init__()
+        super().__init__()
         self.bucket_name = bucket_name
 
     def __str__(self):
         return 'Application key is restricted to bucket: %s' % self.bucket_name
 
 
+class RestrictedBucketMissing(RestrictedBucket):
+    def __init__(self):
+        super().__init__('')
+
+    def __str__(self):
+        return 'Application key is restricted to a bucket that doesn\'t exist'
+
+
 class MaxFileSizeExceeded(B2Error):
     def __init__(self, size, max_allowed_size):
-        super(MaxFileSizeExceeded, self).__init__()
+        super().__init__()
         self.size = size
         self.max_allowed_size = max_allowed_size
 
     def __str__(self):
-        return 'Allowed file size of exceeded: %s > %s' % (
-            self.size,
-            self.max_allowed_size,
-        )
+        return f'Allowed file size of exceeded: {self.size} > {self.max_allowed_size}'
 
 
 class MaxRetriesExceeded(B2Error):
     def __init__(self, limit, exception_info_list):
-        super(MaxRetriesExceeded, self).__init__()
+        super().__init__()
         self.limit = limit
         self.exception_info_list = exception_info_list
 
     def __str__(self):
         exceptions = '\n'.join(str(wrapped_error) for wrapped_error in self.exception_info_list)
-        return 'FAILED to upload after %s tries. Encountered exceptions: %s' % (
-            self.limit,
-            exceptions,
-        )
+        return f'FAILED to upload after {self.limit} tries. Encountered exceptions: {exceptions}'
 
 
 class MissingPart(B2SimpleError):
     prefix = 'Part number has not been uploaded'
 
 
 class NonExistentBucket(FileOrBucketNotFound):
-    def __str__(self):  # overriden to retain message across prev versions
+    def __str__(self):  # overridden to retain message across prev versions
         return "No such bucket%s" % (': ' + self.bucket_name if self.bucket_name else "")
 
 
 class FileSha1Mismatch(B2SimpleError):
     prefix = 'Upload file SHA1 mismatch'
 
 
 class PartSha1Mismatch(B2Error):
     def __init__(self, key):
-        super(PartSha1Mismatch, self).__init__()
+        super().__init__()
         self.key = key
 
     def __str__(self):
-        return 'Part number %s has wrong SHA1' % (self.key,)
+        return f'Part number {self.key} has wrong SHA1'
 
 
 class ServiceError(TransientErrorMixin, B2Error):
     """
     Used for HTTP status codes 500 through 599.
     """
 
@@ -402,27 +432,27 @@
 class TransactionCapExceeded(CapExceeded):
     def __str__(self):
         return 'Cannot perform the operation, transaction cap exceeded.'
 
 
 class TooManyRequests(B2Error):
     def __init__(self, retry_after_seconds=None):
-        super(TooManyRequests, self).__init__()
+        super().__init__()
         self.retry_after_seconds = retry_after_seconds
 
     def __str__(self):
         return 'Too many requests'
 
     def should_retry_http(self):
         return True
 
 
 class TruncatedOutput(TransientErrorMixin, B2Error):
     def __init__(self, bytes_read, file_size):
-        super(TruncatedOutput, self).__init__()
+        super().__init__()
         self.bytes_read = bytes_read
         self.file_size = file_size
 
     def __str__(self):
         return 'only %d of %d bytes read' % (
             self.bytes_read,
             self.file_size,
@@ -449,19 +479,19 @@
 class UnsatisfiableRange(B2Error):
     def __str__(self):
         return "The range in the request is outside the size of the file"
 
 
 class UploadTokenUsedConcurrently(B2Error):
     def __init__(self, token):
-        super(UploadTokenUsedConcurrently, self).__init__()
+        super().__init__()
         self.token = token
 
     def __str__(self):
-        return "More than one concurrent upload using auth token %s" % (self.token,)
+        return f"More than one concurrent upload using auth token {self.token}"
 
 
 class AccessDenied(B2Error):
     def __str__(self):
         return "This call with these parameters is not allowed for this auth token"
 
 
@@ -472,29 +502,89 @@
 
 class RetentionWriteError(AccessDenied):
     def __str__(self):
         return "Auth token not authorized to write retention or file already in 'compliance' mode or " \
                "bypassGovernance=true parameter missing"
 
 
-class WrongEncryptionModeForBucketDefault(B2Error):
+class WrongEncryptionModeForBucketDefault(InvalidUserInput):
     def __init__(self, encryption_mode):
         super().__init__()
         self.encryption_mode = encryption_mode
 
     def __str__(self):
-        return "%s cannot be used as default for a bucket." % (self.encryption_mode,)
+        return f"{self.encryption_mode} cannot be used as default for a bucket."
 
 
+class CopyArgumentsMismatch(InvalidUserInput):
+    pass
+
+
+class DisablingFileLockNotSupported(B2Error):
+    def __str__(self):
+        return "Disabling file lock is not supported"
+
+
+class SourceReplicationConflict(B2Error):
+    def __str__(self):
+        return "Operation not supported for buckets with source replication"
+
+
+class EnablingFileLockOnRestrictedBucket(B2Error):
+    def __str__(self):
+        return "Turning on file lock for a restricted bucket is not allowed"
+
+
+class InvalidJsonResponse(B2SimpleError):
+    UP_TO_BYTES_COUNT = 200
+
+    def __init__(self, content: bytes):
+        self.content = content
+        message = self.content[:self.UP_TO_BYTES_COUNT].decode('utf-8', errors='replace')
+        if len(self.content) > self.UP_TO_BYTES_COUNT:
+            message += '...'
+
+        super().__init__(message)
+
+
+class PotentialS3EndpointPassedAsRealm(InvalidJsonResponse):
+    pass
+
+
+class DestinationError(B2Error):
+    pass
+
+
+class DestinationDirectoryError(DestinationError):
+    pass
+
+
+class DestinationDirectoryDoesntExist(DestinationDirectoryError):
+    pass
+
+
+class DestinationParentIsNotADirectory(DestinationDirectoryError):
+    pass
+
+
+class DestinationIsADirectory(DestinationDirectoryError):
+    pass
+
+
+class DestinationDirectoryDoesntAllowOperation(DestinationDirectoryError):
+    pass
+
+
+@trace_call(logger)
 def interpret_b2_error(
     status: int,
-    code: Optional[str],
-    message: Optional[str],
-    response_headers: Dict[str, Any],
-    post_params: Optional[Dict[str, Any]] = None
+    code: str | None,
+    message: str | None,
+    response_headers: dict[str, Any],
+    post_params: dict[str, Any] | None = None
 ) -> B2Error:
     post_params = post_params or {}
     if status == 400 and code == "already_hidden":
         return FileAlreadyHidden(post_params.get('fileName'))
     elif status == 400 and code == 'bad_json':
         return BadJson(message)
     elif (
@@ -516,24 +606,56 @@
         return ResourceNotFound()
     elif status == 400 and code == "duplicate_bucket_name":
         return DuplicateBucketName(post_params.get('bucketName'))
     elif status == 400 and code == "missing_part":
         return MissingPart(post_params.get('fileId'))
     elif status == 400 and code == "part_sha1_mismatch":
         return PartSha1Mismatch(post_params.get('fileId'))
-    elif status == 400 and code == "bad_request":
+    elif status == 400 and code == "bad_bucket_id":
+        return BucketIdNotFound(post_params.get('bucketId'))
+    elif status == 400 and code == "auth_token_limit":
         matcher = UPLOAD_TOKEN_USED_CONCURRENTLY_ERROR_MESSAGE_RE.match(message)
-        if matcher is not None:
-            token = matcher.group('token')
-            return UploadTokenUsedConcurrently(token)
+        assert matcher is not None, f"unexpected error message: {message}"
+        token = matcher.group('token')
+        return UploadTokenUsedConcurrently(token)
+    elif status == 400 and code == "source_too_large":
+        matcher = COPY_SOURCE_TOO_BIG_ERROR_MESSAGE_RE.match(message)
+        assert matcher is not None, f"unexpected error message: {message}"
+        size = int(matcher.group('size'))
+        return CopySourceTooBig(message, code, size)
+    elif status == 400 and code == 'file_lock_conflict':
+        return DisablingFileLockNotSupported()
+    elif status == 400 and code == 'source_replication_conflict':
+        return SourceReplicationConflict()
+    elif status == 400 and code == 'restricted_bucket_conflict':
+        return EnablingFileLockOnRestrictedBucket()
+    elif status == 400 and code == 'bad_request':
+
+        # it's "bad_request" on 2022-09-14, but will become 'disabling_file_lock_not_allowed'  # TODO: cleanup after 2022-09-22
+        if message == 'fileLockEnabled value of false is not allowed when bucket is already file lock enabled.':
+            return DisablingFileLockNotSupported()
+
+        # it's "bad_request" on 2022-09-14, but will become 'source_replication_conflict'  # TODO: cleanup after 2022-09-22
+        if message == 'Turning on file lock for an existing bucket having source replication configuration is not allowed.':
+            return SourceReplicationConflict()
+
+        # it's "bad_request" on 2022-09-14, but will become 'restricted_bucket_conflict'  # TODO: cleanup after 2022-09-22
+        if message == 'Turning on file lock for a restricted bucket is not allowed.':
+            return EnablingFileLockOnRestrictedBucket()
+
         return BadRequest(message, code)
     elif status == 400:
+        warnings.warn(
+            f"bad request exception with an unknown `code`. message={message}, code={code}"
+        )
         return BadRequest(message, code)
     elif status == 401 and code in ("bad_auth_token", "expired_auth_token"):
         return InvalidAuthToken(message, code)
+    elif status == 401 and code == 'email_not_verified':
+        return EmailNotVerified(message, code)
     elif status == 401:
         return Unauthorized(message, code)
     elif status == 403 and code == "storage_cap_exceeded":
         return StorageCapExceeded()
     elif status == 403 and code == "transaction_cap_exceeded":
         return TransactionCapExceeded()
     elif status == 403 and code == "access_denied":
```

### Comparing `b2sdk-1.9.0/b2sdk/file_lock.py` & `b2sdk-2.0.0/b2sdk/_internal/file_lock.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ######################################################################
 #
-# File: b2sdk/file_lock.py
+# File: b2sdk/_internal/file_lock.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from typing import Optional
 import enum
 
 from .exception import UnexpectedCloudBehaviour
 
 ACTIONS_WITHOUT_LOCK_SETTINGS = frozenset(['hide', 'folder'])
 
 
@@ -28,15 +28,15 @@
 RETENTION_MODES_REQUIRING_PERIODS = frozenset({RetentionMode.COMPLIANCE, RetentionMode.GOVERNANCE})
 
 
 class RetentionPeriod:
     """Represent a time period (either in days or in years) that is used as a default for bucket retention"""
     KNOWN_UNITS = ['days', 'years']
 
-    def __init__(self, years: Optional[int] = None, days: Optional[int] = None):
+    def __init__(self, years: int | None = None, days: int | None = None):
         """Create a retention period, provide exactly one of: days, years"""
         assert (years is None) != (days is None)
         if years is not None:
             self.duration = years
             self.unit = 'years'
         else:
             self.duration = days
@@ -60,31 +60,31 @@
     def as_dict(self):
         return {
             "duration": self.duration,
             "unit": self.unit,
         }
 
     def __repr__(self):
-        return '%s(%s %s)' % (self.__class__.__name__, self.duration, self.unit)
+        return f'{self.__class__.__name__}({self.duration} {self.unit})'
 
     def __eq__(self, other):
         return self.unit == other.unit and self.duration == other.duration
 
 
 class FileRetentionSetting:
     """Represent file retention settings, i.e. whether the file is retained, in which mode and until when"""
 
-    def __init__(self, mode: RetentionMode, retain_until: Optional[int] = None):
+    def __init__(self, mode: RetentionMode, retain_until: int | None = None):
         if mode in RETENTION_MODES_REQUIRING_PERIODS and retain_until is None:
-            raise ValueError('must specify retain_until for retention mode %s' % (mode,))
+            raise ValueError(f'must specify retain_until for retention mode {mode}')
         self.mode = mode
         self.retain_until = retain_until
 
     @classmethod
-    def from_file_version_dict(cls, file_version_dict: dict) -> 'FileRetentionSetting':
+    def from_file_version_dict(cls, file_version_dict: dict) -> FileRetentionSetting:
         """
         Returns FileRetentionSetting for the given file_version_dict retrieved from the api. E.g.
 
         .. code-block ::
 
             {
                 "action": "upload",
@@ -120,27 +120,31 @@
             return cls(RetentionMode.UNKNOWN, None)
 
         return cls.from_file_retention_value_dict(file_retention_dict['value'])
 
     @classmethod
     def from_file_retention_value_dict(
         cls, file_retention_value_dict: dict
-    ) -> 'FileRetentionSetting':
+    ) -> FileRetentionSetting:
 
         mode = file_retention_value_dict['mode']
         if mode is None:
             return NO_RETENTION_FILE_SETTING
 
         return cls(
             RetentionMode(mode),
             file_retention_value_dict['retainUntilTimestamp'],
         )
 
     @classmethod
-    def from_response_headers(cls, headers) -> 'FileRetentionSetting':
+    def from_server_response(cls, server_response: dict) -> FileRetentionSetting:
+        return cls.from_file_retention_value_dict(server_response['fileRetention'])
+
+    @classmethod
+    def from_response_headers(cls, headers) -> FileRetentionSetting:
         retention_mode_header = 'X-Bz-File-Retention-Mode'
         retain_until_header = 'X-Bz-File-Retention-Retain-Until-Timestamp'
         if retention_mode_header in headers:
             if retain_until_header in headers:
                 retain_until = int(headers[retain_until_header])
             else:
                 retain_until = None
@@ -171,17 +175,15 @@
         # moment, but it should be
         headers['X-Bz-File-Retention-Retain-Until-Timestamp'] = str(self.retain_until)
 
     def __eq__(self, other):
         return self.mode == other.mode and self.retain_until == other.retain_until
 
     def __repr__(self):
-        return '%s(%s, %s)' % (
-            self.__class__.__name__, repr(self.mode.value), repr(self.retain_until)
-        )
+        return f'{self.__class__.__name__}({repr(self.mode.value)}, {repr(self.retain_until)})'
 
 
 @enum.unique
 class LegalHold(enum.Enum):
     """Enum holding information about legalHold switch in a file."""
 
     ON = 'on'  #: legal hold set to "on"
@@ -198,32 +200,36 @@
         return self is LegalHold.OFF or self is LegalHold.UNSET
 
     def is_unknown(self):
         """Is the legalHold switch unknown?"""
         return self is LegalHold.UNKNOWN
 
     @classmethod
-    def from_file_version_dict(cls, file_version_dict: dict) -> 'LegalHold':
+    def from_file_version_dict(cls, file_version_dict: dict) -> LegalHold:
         if 'legalHold' not in file_version_dict:
             if file_version_dict['action'] not in ACTIONS_WITHOUT_LOCK_SETTINGS:
                 raise UnexpectedCloudBehaviour(
                     'legalHold not provided for file version with action=%s' %
                     (file_version_dict['action'])
                 )
             return cls.UNSET
         if not file_version_dict['legalHold']['isClientAuthorizedToRead']:
             return cls.UNKNOWN
         return cls.from_string_or_none(file_version_dict['legalHold']['value'])
 
     @classmethod
-    def from_string_or_none(cls, string: Optional[str]) -> 'LegalHold':
+    def from_server_response(cls, server_response: dict) -> LegalHold:
+        return cls.from_string_or_none(server_response['legalHold'])
+
+    @classmethod
+    def from_string_or_none(cls, string: str | None) -> LegalHold:
         return cls(string)
 
     @classmethod
-    def from_response_headers(cls, headers) -> 'LegalHold':
+    def from_response_headers(cls, headers) -> LegalHold:
         legal_hold_header = 'X-Bz-File-Legal-Hold'
         if legal_hold_header in headers:
             return cls(headers['X-Bz-File-Legal-Hold'])
         if 'X-Bz-Client-Unauthorized-To-Read' in headers and legal_hold_header in headers[
             'X-Bz-Client-Unauthorized-To-Read'].split(','):
             return cls.UNKNOWN
         return cls.UNSET  # the bucket is not file-lock-enabled or the header is missing for any other reason
@@ -234,31 +240,22 @@
         if self.is_on():
             return self.__class__.ON.value
         return self.__class__.OFF.value
 
     def add_to_upload_headers(self, headers):
         headers['X-Bz-File-Legal-Hold'] = self.to_server()
 
-    def to_dict_repr(self):
-        if self.is_on():
-            return self.__class__.ON.value
-        elif self.is_off():
-            return self.__class__.OFF.value
-        elif self.is_unknown():
-            return self.__class__.UNKNOWN.value
-        raise ValueError('Unrepresentable value')
-
 
 class BucketRetentionSetting:
     """Represent bucket's default file retention settings, i.e. whether the files should be retained, in which mode
        and for how long"""
 
-    def __init__(self, mode: RetentionMode, period: Optional[RetentionPeriod] = None):
+    def __init__(self, mode: RetentionMode, period: RetentionPeriod | None = None):
         if mode in RETENTION_MODES_REQUIRING_PERIODS and period is None:
-            raise ValueError('must specify period for retention mode %s' % (mode,))
+            raise ValueError(f'must specify period for retention mode {mode}')
         self.mode = mode
         self.period = period
 
     @classmethod
     def from_bucket_retention_dict(cls, retention_dict: dict):
         """
         Build a BucketRetentionSetting from an object returned by the server, such as:
@@ -292,25 +289,25 @@
             raise ValueError('cannot use an unknown file lock configuration in requests')
         return self.as_dict()
 
     def __eq__(self, other):
         return self.mode == other.mode and self.period == other.period
 
     def __repr__(self):
-        return '%s(%s, %s)' % (self.__class__.__name__, repr(self.mode.value), repr(self.period))
+        return f'{self.__class__.__name__}({repr(self.mode.value)}, {repr(self.period)})'
 
 
 class FileLockConfiguration:
     """Represent bucket's file lock configuration, i.e. whether the file lock mechanism is enabled and default
     file retention"""
 
     def __init__(
         self,
         default_retention: BucketRetentionSetting,
-        is_file_lock_enabled: Optional[bool],
+        is_file_lock_enabled: bool | None,
     ):
         self.default_retention = default_retention
         self.is_file_lock_enabled = is_file_lock_enabled
 
     @classmethod
     def from_bucket_dict(cls, bucket_dict):
         """
@@ -354,15 +351,15 @@
             "isFileLockEnabled": self.is_file_lock_enabled,
         }
 
     def __eq__(self, other):
         return self.default_retention == other.default_retention and self.is_file_lock_enabled == other.is_file_lock_enabled
 
     def __repr__(self):
-        return '%s(%s, %s)' % (
+        return '{}({}, {})'.format(
             self.__class__.__name__, repr(self.default_retention), repr(self.is_file_lock_enabled)
         )
 
 
 UNKNOWN_BUCKET_RETENTION = BucketRetentionSetting(RetentionMode.UNKNOWN)
 """Commonly used "unknown" default bucket retention setting"""
 UNKNOWN_FILE_LOCK_CONFIGURATION = FileLockConfiguration(UNKNOWN_BUCKET_RETENTION, None)
```

### Comparing `b2sdk-1.9.0/b2sdk/large_file/part.py` & `b2sdk-2.0.0/b2sdk/_internal/large_file/part.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 ######################################################################
 #
-# File: b2sdk/large_file/part.py
+# File: b2sdk/_internal/large_file/part.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 
-class PartFactory(object):
+class PartFactory:
     @classmethod
     def from_list_parts_dict(cls, part_dict):
         return Part(
             part_dict['fileId'],
             part_dict['partNumber'],
             part_dict['contentLength'],
             part_dict['contentSha1'],
         )
 
 
-class Part(object):
+class Part:
     """
     A structure which represents a *part* of a large file upload.
 
     :ivar str ~.file_id: ``fileId``
     :ivar int ~.part_number: part number, starting with 1
     :ivar str ~.content_length: content length, in bytes
     :ivar str ~.content_sha1: checksum
@@ -33,15 +34,15 @@
     def __init__(self, file_id, part_number, content_length, content_sha1):
         self.file_id = file_id
         self.part_number = part_number
         self.content_length = content_length
         self.content_sha1 = content_sha1
 
     def __repr__(self):
-        return '<%s %s %s %s %s>' % (
+        return '<{} {} {} {} {}>'.format(
             self.__class__.__name__, self.file_id, self.part_number, self.content_length,
             self.content_sha1
         )
 
     def __eq__(self, other):
         return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
```

### Comparing `b2sdk-1.9.0/b2sdk/large_file/services.py` & `b2sdk-2.0.0/b2sdk/_internal/large_file/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 ######################################################################
 #
-# File: b2sdk/large_file/services.py
+# File: b2sdk/_internal/large_file/services.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from typing import Optional
+from b2sdk._internal.encryption.setting import EncryptionSetting
+from b2sdk._internal.file_lock import FileRetentionSetting, LegalHold
+from b2sdk._internal.file_version import FileIdAndName
+from b2sdk._internal.large_file.part import PartFactory
+from b2sdk._internal.large_file.unfinished_large_file import UnfinishedLargeFile
 
-from b2sdk.encryption.setting import EncryptionSetting
-from b2sdk.file_lock import FileRetentionSetting, LegalHold
-from b2sdk.file_version import FileIdAndName
-from b2sdk.large_file.part import PartFactory
-from b2sdk.large_file.unfinished_large_file import UnfinishedLargeFile
 
+class LargeFileServices:
+
+    UNFINISHED_LARGE_FILE_CLASS = staticmethod(UnfinishedLargeFile)
 
-class LargeFileServices(object):
     def __init__(self, services):
         self.services = services
 
     def list_parts(self, file_id, start_part_number=None, batch_size=None):
         """
-        Generator that yields a :py:class:`b2sdk.v1.Part` for each of the parts that have been uploaded.
+        Generator that yields a :py:class:`b2sdk.v2.Part` for each of the parts that have been uploaded.
 
         :param str file_id: the ID of the large file that is not finished
         :param int start_part_number: the first part number to return; defaults to the first part
         :param int batch_size: the number of parts to fetch at a time from the server
         :rtype: generator
         """
         batch_size = batch_size or 100
@@ -39,30 +41,30 @@
             if start_part_number is None:
                 break
 
     def list_unfinished_large_files(
         self, bucket_id, start_file_id=None, batch_size=None, prefix=None
     ):
         """
-        A generator that yields an :py:class:`b2sdk.v1.UnfinishedLargeFile` for each
+        A generator that yields an :py:class:`b2sdk.v2.UnfinishedLargeFile` for each
         unfinished large file in the bucket, starting at the given file, filtering by prefix.
 
         :param str bucket_id: bucket id
         :param str,None start_file_id: a file ID to start from or None to start from the beginning
         :param int,None batch_size: max file count
         :param str,None prefix: file name prefix filter
-        :rtype: generator[b2sdk.v1.UnfinishedLargeFile]
+        :rtype: generator[b2sdk.v2.UnfinishedLargeFile]
         """
         batch_size = batch_size or 100
         while True:
             batch = self.services.session.list_unfinished_large_files(
                 bucket_id, start_file_id, batch_size, prefix
             )
             for file_dict in batch['files']:
-                yield UnfinishedLargeFile(file_dict)
+                yield self.UNFINISHED_LARGE_FILE_CLASS(file_dict)
             start_file_id = batch.get('nextFileId')
             if start_file_id is None:
                 break
 
     def get_unfinished_large_file(self, bucket_id, large_file_id, prefix=None):
         result = list(
             self.list_unfinished_large_files(
@@ -80,29 +82,29 @@
 
     def start_large_file(
         self,
         bucket_id,
         file_name,
         content_type=None,
         file_info=None,
-        encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
     ):
         """
         Start a large file transfer.
 
         :param str file_name: a file name
         :param str,None content_type: the MIME type, or ``None`` to accept the default based on file extension of the B2 file name
         :param dict,None file_info: a file info to store with the file or ``None`` to not store anything
-        :param b2sdk.v1.EncryptionSetting encryption: encryption settings (``None`` if unknown)
-        :param b2sdk.v1.LegalHold legal_hold: legal hold setting
-        :param b2sdk.v1.FileRetentionSetting file_retention: file retention setting
+        :param b2sdk.v2.EncryptionSetting encryption: encryption settings (``None`` if unknown)
+        :param b2sdk.v2.FileRetentionSetting file_retention: file retention setting
+        :param b2sdk.v2.LegalHold legal_hold: legal hold setting
         """
-        return UnfinishedLargeFile(
+        return self.UNFINISHED_LARGE_FILE_CLASS(
             self.services.session.start_large_file(
                 bucket_id,
                 file_name,
                 content_type,
                 file_info,
                 server_side_encryption=encryption,
                 file_retention=file_retention,
```

### Comparing `b2sdk-1.9.0/b2sdk/large_file/unfinished_large_file.py` & `b2sdk-2.0.0/b2sdk/v2/large_file.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,40 @@
 ######################################################################
 #
-# File: b2sdk/large_file/unfinished_large_file.py
+# File: b2sdk/v2/large_file.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from b2sdk.encryption.setting import EncryptionSettingFactory
-from b2sdk.file_lock import FileRetentionSetting, LegalHold
+from b2sdk import _v3 as v3
 
 
-class UnfinishedLargeFile(object):
+class UnfinishedLargeFile(v3.UnfinishedLargeFile):
     """
     A structure which represents a version of a file (in B2 cloud).
 
     :ivar str ~.file_id: ``fileId``
     :ivar str ~.file_name: full file name (with path)
     :ivar str ~.account_id: account ID
     :ivar str ~.bucket_id: bucket ID
     :ivar str ~.content_type: :rfc:`822` content type, for example ``"application/octet-stream"``
     :ivar dict ~.file_info: file info dict
     """
 
+    # In v3, cache_control is a property.
+    # We set this to None so that it can be assigned to in __init__.
+    cache_control = None
+
     def __init__(self, file_dict):
         """
         Initialize from one file returned by ``b2_start_large_file`` or ``b2_list_unfinished_large_files``.
         """
-        self.file_id = file_dict['fileId']
-        self.file_name = file_dict['fileName']
-        self.account_id = file_dict['accountId']
-        self.bucket_id = file_dict['bucketId']
-        self.content_type = file_dict['contentType']
-        self.file_info = file_dict['fileInfo']
-        self.encryption = EncryptionSettingFactory.from_file_version_dict(file_dict)
-        self.file_retention = FileRetentionSetting.from_file_version_dict(file_dict)
-        self.legal_hold = LegalHold.from_file_version_dict(file_dict)
-
-    def __repr__(self):
-        return '<%s %s %s>' % (self.__class__.__name__, self.bucket_id, self.file_name)
+        super().__init__(file_dict)
+        self.cache_control = (file_dict['fileInfo'] or {}).get('b2-cache-control')
 
-    def __eq__(self, other):
-        return isinstance(other, self.__class__) and self.__dict__ == other.__dict__
 
-    def __ne__(self, other):
-        return not (self == other)
+class LargeFileServices(v3.LargeFileServices):
+    UNFINISHED_LARGE_FILE_CLASS = staticmethod(UnfinishedLargeFile)
```

### Comparing `b2sdk-1.9.0/b2sdk/progress.py` & `b2sdk-2.0.0/b2sdk/_internal/progress.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 ######################################################################
 #
-# File: b2sdk/progress.py
+# File: b2sdk/_internal/progress.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from abc import ABCMeta, abstractmethod
 import time
+from abc import ABCMeta, abstractmethod
+
+from .utils.escape import escape_control_chars
 
 try:
     from tqdm import tqdm  # displays a nice progress bar
 except ImportError:
     tqdm = None  # noqa
 
 
@@ -23,41 +26,64 @@
     on progress.
 
     This interface just accepts the number of bytes transferred so far.
     Subclasses will need to know the total size if they want to report
     a percent done.
     """
 
-    def __init__(self):
+    def __init__(self, description: str = ''):
+        self.description = description
         self._closed = False
 
     @abstractmethod
-    def set_total_bytes(self, total_byte_count):
+    def set_total_bytes(self, total_byte_count: int) -> None:
         """
         Always called before __enter__ to set the expected total number of bytes.
 
         May be called more than once if an upload is retried.
 
-        :param int total_byte_count: expected total number of bytes
+        :param total_byte_count: expected total number of bytes
         """
 
     @abstractmethod
-    def bytes_completed(self, byte_count):
+    def bytes_completed(self, byte_count: int) -> None:
         """
         Report the given number of bytes that have been transferred
         so far.  This is not a delta, it is the total number of bytes
         transferred so far.
 
-        Transfer can fail and restart from beginning so byte count can
+        Transfer can fail and restart from the beginning, so byte count can
         decrease between calls.
 
-        :param int byte_count: number of bytes have been transferred
+        :param byte_count: number of bytes have been transferred
+        """
+
+    def _can_change_description(self) -> bool:
+        """
+        Determines, on a per-implementation basis, whether the description can be changed at this time.
         """
+        return True
+
+    def change_description(self, new_description: str) -> bool:
+        """
+        Ability to change the description after the listener is started.
+
+        Note: whether the change of description is allowed depends on the implementation.
+        The safest option is to change the description before setting the total bytes.
 
-    def close(self):
+        :param new_description: the new description to be used
+        :return: information whether the description was changed
+        """
+        if not self._can_change_description():
+            return False
+
+        self.description = new_description
+        return True
+
+    def close(self) -> None:
         """
         Must be called when you're done with the listener.
         In well-structured code, should be called only once.
         """
         #import traceback, sys; traceback.print_stack(file=sys.stdout)
         assert self._closed is False, 'progress listener was closed twice! uncomment the line above to debug this'
         self._closed = True
@@ -74,121 +100,130 @@
         """
         self.close()
 
 
 class TqdmProgressListener(AbstractProgressListener):
     """
     Progress listener based on tqdm library.
+
+    This listener displays a nice progress bar, but requires `tqdm` package to be installed.
     """
 
-    def __init__(self, description, *args, **kwargs):
-        self.description = description
+    def __init__(self, *args, **kwargs):
+        if tqdm is None:
+            raise ModuleNotFoundError("No module named 'tqdm' found")
         self.tqdm = None  # set in set_total_bytes()
         self.prev_value = 0
-        super(TqdmProgressListener, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
-    def set_total_bytes(self, total_byte_count):
+    def set_total_bytes(self, total_byte_count: int) -> None:
         if self.tqdm is None:
             self.tqdm = tqdm(
-                desc=self.description,
+                desc=escape_control_chars(self.description),
                 total=total_byte_count,
                 unit='B',
                 unit_scale=True,
                 leave=True,
                 miniters=1,
                 smoothing=0.1,
                 mininterval=0.2,
             )
 
-    def bytes_completed(self, byte_count):
+    def bytes_completed(self, byte_count: int) -> None:
         # tqdm doesn't support running the progress bar backwards,
         # so on an upload retry, it just won't move until it gets
         # past the point where it failed.
         if self.prev_value < byte_count:
             self.tqdm.update(byte_count - self.prev_value)
             self.prev_value = byte_count
 
-    def close(self):
+    def _can_change_description(self) -> bool:
+        return self.tqdm is None
+
+    def close(self) -> None:
         if self.tqdm is not None:
             self.tqdm.close()
-        super(TqdmProgressListener, self).close()
+        super().close()
 
 
 class SimpleProgressListener(AbstractProgressListener):
     """
     Just a simple progress listener which prints info on a console.
     """
 
-    def __init__(self, description, *args, **kwargs):
-        self.desc = description
+    def __init__(self, *args, **kwargs):
         self.complete = 0
         self.last_time = time.time()
         self.any_printed = False
-        super(SimpleProgressListener, self).__init__(*args, **kwargs)
+        self.total = 0  # set in set_total_bytes()
+        super().__init__(*args, **kwargs)
 
-    def set_total_bytes(self, total_byte_count):
+    def set_total_bytes(self, total_byte_count: int) -> None:
         self.total = total_byte_count
 
-    def bytes_completed(self, byte_count):
+    def bytes_completed(self, byte_count: int) -> None:
         now = time.time()
         elapsed = now - self.last_time
         if 3 <= elapsed and self.total != 0:
             if not self.any_printed:
-                print(self.desc)
+                print(escape_control_chars(self.description))
             print('     %d%%' % int(100.0 * byte_count / self.total))
             self.last_time = now
             self.any_printed = True
 
-    def close(self):
+    def _can_change_description(self) -> bool:
+        return not self.any_printed
+
+    def close(self) -> None:
         if self.any_printed:
             print('    DONE.')
-        super(SimpleProgressListener, self).close()
+        super().close()
 
 
 class DoNothingProgressListener(AbstractProgressListener):
     """
     This listener gives no output whatsoever.
     """
 
-    def set_total_bytes(self, total_byte_count):
+    def set_total_bytes(self, total_byte_count: int) -> None:
         pass
 
-    def bytes_completed(self, byte_count):
+    def bytes_completed(self, byte_count: int) -> None:
         pass
 
 
 class ProgressListenerForTest(AbstractProgressListener):
     """
-    Capture all of the calls so they can be checked.
+    Capture all the calls so they can be checked.
     """
 
     def __init__(self, *args, **kwargs):
         self.calls = []
-        super(ProgressListenerForTest, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
-    def set_total_bytes(self, total_byte_count):
+    def set_total_bytes(self, total_byte_count: int) -> None:
         self.calls.append('set_total_bytes(%d)' % (total_byte_count,))
 
-    def bytes_completed(self, byte_count):
+    def bytes_completed(self, byte_count: int) -> None:
         self.calls.append('bytes_completed(%d)' % (byte_count,))
 
-    def close(self):
+    def close(self) -> None:
         self.calls.append('close()')
-        super(ProgressListenerForTest, self).close()
+        super().close()
 
-    def get_calls(self):
+    def get_calls(self) -> list[str]:
         return self.calls
 
 
-def make_progress_listener(description, quiet):
+def make_progress_listener(description: str, quiet: bool) -> AbstractProgressListener:
     """
-    Return a progress listener object depending on some conditions.
+    Produce the best progress listener available for the given parameters.
 
-    :param str description: listener description
-    :param bool quiet: if ``True``, do not output anything
+    :param description: listener description
+    :param quiet: if ``True``, do not output anything
     :return: a listener object
     """
     if quiet:
         return DoNothingProgressListener()
     elif tqdm is not None:
         return TqdmProgressListener(description)
     else:
```

### Comparing `b2sdk-1.9.0/b2sdk/raw_api.py` & `b2sdk-2.0.0/b2sdk/_internal/raw_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,111 @@
 ######################################################################
 #
-# File: b2sdk/raw_api.py
+# File: b2sdk/_internal/raw_api.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import base64
-import io
-import os
-import random
-import re
-import sys
-import time
-import traceback
 from abc import ABCMeta, abstractmethod
 from enum import Enum, unique
 from logging import getLogger
-from typing import Any, Dict, Optional
+from typing import Any
 
-from .b2http import B2Http
-from .exception import FileOrBucketNotFound, ResourceNotFound, UnusableFileName, InvalidMetadataDirective, WrongEncryptionModeForBucketDefault, AccessDenied, SSECKeyError, RetentionWriteError
-from .encryption.setting import EncryptionAlgorithm, EncryptionMode, EncryptionSetting
-from .file_lock import BucketRetentionSetting, FileRetentionSetting, NO_RETENTION_FILE_SETTING, RetentionMode, RetentionPeriod, LegalHold
-from .utils import b2_url_encode, hex_sha1_of_stream
+from .utils.escape import unprintable_to_hex
+from .utils.typing import JSON
+
+try:
+    from typing_extensions import NotRequired, TypedDict
+except ImportError:
+    from typing import NotRequired, TypedDict
+
+from .encryption.setting import EncryptionMode, EncryptionSetting
+from .exception import (
+    AccessDenied,
+    FileOrBucketNotFound,
+    InvalidMetadataDirective,
+    ResourceNotFound,
+    RetentionWriteError,
+    SSECKeyError,
+    UnusableFileName,
+    WrongEncryptionModeForBucketDefault,
+)
+from .file_lock import BucketRetentionSetting, FileRetentionSetting, LegalHold
+from .http_constants import FILE_INFO_HEADER_PREFIX
+from .replication.setting import ReplicationConfiguration
+from .utils import b2_url_encode
+from .utils.docs import ensure_b2sdk_doc_urls
 
 # All supported realms
 REALM_URLS = {
     'production': 'https://api.backblazeb2.com',
     'dev': 'http://api.backblazeb2.xyz:8180',
     'staging': 'https://api.backblaze.net',
 }
 
 # All possible capabilities
 ALL_CAPABILITIES = [
     'listKeys',
     'writeKeys',
     'deleteKeys',
     'listBuckets',
+    'listAllBucketNames',
+    'readBuckets',
     'writeBuckets',
     'deleteBuckets',
     'readBucketEncryption',
     'writeBucketEncryption',
     'readBucketRetentions',
     'writeBucketRetentions',
-    'writeFileRetentions',
-    'writeFileLegalHolds',
     'readFileRetentions',
+    'writeFileRetentions',
     'readFileLegalHolds',
+    'writeFileLegalHolds',
+    'readBucketReplications',
+    'writeBucketReplications',
+    'bypassGovernance',
     'listFiles',
     'readFiles',
     'shareFiles',
     'writeFiles',
     'deleteFiles',
 ]
 
-# Standard names for file info entries
-SRC_LAST_MODIFIED_MILLIS = 'src_last_modified_millis'
-
-# Special X-Bz-Content-Sha1 value to verify checksum at the end
-HEX_DIGITS_AT_END = 'hex_digits_at_end'
-
 # API version number to use when calling the service
 API_VERSION = 'v2'
 
 logger = getLogger(__name__)
 
 
 @unique
 class MetadataDirectiveMode(Enum):
     """ Mode of handling metadata when copying a file """
     COPY = 401  #: copy metadata from the source file
     REPLACE = 402  #: ignore the source file metadata and set it to provided values
 
 
+@ensure_b2sdk_doc_urls
+class LifecycleRule(TypedDict):
+    """
+    Lifecycle Rule.
+
+    External documentation: `B2 Cloud Storage Lifecycle Rules`_.
+
+    .. _B2 Cloud Storage Lifecycle Rules: https://www.backblaze.com/docs/cloud-storage-lifecycle-rules
+    """
+    fileNamePrefix: str
+    daysFromHidingToDeleting: NotRequired[int | None]
+    daysFromUploadingToHiding: NotRequired[int | None]
+
+
 class AbstractRawApi(metaclass=ABCMeta):
     """
     Direct access to the B2 web apis.
     """
 
     @abstractmethod
     def authorize_account(self, realm_url, application_key_id, application_key):
@@ -97,48 +123,49 @@
         source_file_id,
         new_file_name,
         bytes_range=None,
         metadata_directive=None,
         content_type=None,
         file_info=None,
         destination_bucket_id=None,
-        destination_server_side_encryption: Optional[EncryptionSetting] = None,
-        source_server_side_encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        destination_server_side_encryption: EncryptionSetting | None = None,
+        source_server_side_encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
     ):
         pass
 
     @abstractmethod
     def copy_part(
         self,
         api_url,
         account_auth_token,
         source_file_id,
         large_file_id,
         part_number,
         bytes_range=None,
-        destination_server_side_encryption: Optional[EncryptionSetting] = None,
-        source_server_side_encryption: Optional[EncryptionSetting] = None,
+        destination_server_side_encryption: EncryptionSetting | None = None,
+        source_server_side_encryption: EncryptionSetting | None = None,
     ):
         pass
 
     @abstractmethod
     def create_bucket(
         self,
         api_url,
         account_auth_token,
         account_id,
         bucket_name,
         bucket_type,
         bucket_info=None,
         cors_rules=None,
-        lifecycle_rules=None,
-        default_server_side_encryption: Optional[EncryptionSetting] = None,
-        is_file_lock_enabled: Optional[bool] = None,
+        lifecycle_rules: list[LifecycleRule] | None = None,
+        default_server_side_encryption: EncryptionSetting | None = None,
+        is_file_lock_enabled: bool | None = None,
+        replication: ReplicationConfiguration | None = None,
     ):
         pass
 
     @abstractmethod
     def create_key(
         self, api_url, account_auth_token, account_id, capabilities, key_name,
         valid_duration_seconds, bucket_id, name_prefix
@@ -147,49 +174,51 @@
 
     @abstractmethod
     def download_file_from_url(
         self,
         account_auth_token_or_none,
         url,
         range_=None,
-        encryption: Optional[EncryptionSetting] = None,
+        encryption: EncryptionSetting | None = None,
     ):
         pass
 
     @abstractmethod
     def delete_key(self, api_url, account_auth_token, application_key_id):
         pass
 
     @abstractmethod
     def delete_bucket(self, api_url, account_auth_token, account_id, bucket_id):
         pass
 
     @abstractmethod
-    def delete_file_version(self, api_url, account_auth_token, file_id, file_name):
+    def delete_file_version(
+        self, api_url, account_auth_token, file_id, file_name, bypass_governance: bool = False
+    ):
         pass
 
     @abstractmethod
     def finish_large_file(self, api_url, account_auth_token, file_id, part_sha1_array):
         pass
 
     @abstractmethod
     def get_download_authorization(
         self, api_url, account_auth_token, bucket_id, file_name_prefix, valid_duration_in_seconds
     ):
         pass
 
     @abstractmethod
     def get_file_info_by_id(self, api_url: str, account_auth_token: str,
-                            file_id: str) -> Dict[str, Any]:
+                            file_id: str) -> dict[str, Any]:
         pass
 
     @abstractmethod
     def get_file_info_by_name(
         self, download_url: str, account_auth_token: str, bucket_name: str, file_name: str
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         pass
 
     @abstractmethod
     def get_upload_url(self, api_url, account_auth_token, bucket_id):
         pass
 
     @abstractmethod
@@ -268,34 +297,36 @@
         self,
         api_url,
         account_auth_token,
         bucket_id,
         file_name,
         content_type,
         file_info,
-        server_side_encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        server_side_encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
     ):
         pass
 
     @abstractmethod
     def update_bucket(
         self,
         api_url,
         account_auth_token,
         account_id,
         bucket_id,
         bucket_type=None,
         bucket_info=None,
         cors_rules=None,
-        lifecycle_rules=None,
+        lifecycle_rules: list[LifecycleRule] | None = None,
         if_revision_is=None,
-        default_server_side_encryption: Optional[EncryptionSetting] = None,
-        default_retention: Optional[BucketRetentionSetting] = None,
+        default_server_side_encryption: EncryptionSetting | None = None,
+        default_retention: BucketRetentionSetting | None = None,
+        replication: ReplicationConfiguration | None = None,
+        is_file_lock_enabled: bool | None = None,
     ):
         pass
 
     @abstractmethod
     def update_file_retention(
         self,
         api_url,
@@ -303,52 +334,93 @@
         file_id,
         file_name,
         file_retention: FileRetentionSetting,
         bypass_governance: bool = False,
     ):
         pass
 
+    @classmethod
+    def get_upload_file_headers(
+        cls,
+        upload_auth_token: str,
+        file_name: str,
+        content_length: int,
+        content_type: str,
+        content_sha1: str,
+        file_info: dict,
+        server_side_encryption: EncryptionSetting | None,
+        file_retention: FileRetentionSetting | None,
+        legal_hold: LegalHold | None,
+        custom_upload_timestamp: int | None = None,
+    ) -> dict:
+        headers = {
+            'Authorization': upload_auth_token,
+            'Content-Length': str(content_length),
+            'X-Bz-File-Name': b2_url_encode(file_name),
+            'Content-Type': content_type,
+            'X-Bz-Content-Sha1': content_sha1,
+        }
+        for k, v in file_info.items():
+            headers[FILE_INFO_HEADER_PREFIX + k] = b2_url_encode(v)
+        if server_side_encryption is not None:
+            assert server_side_encryption.mode in (
+                EncryptionMode.NONE, EncryptionMode.SSE_B2, EncryptionMode.SSE_C
+            )
+            server_side_encryption.add_to_upload_headers(headers)
+
+        if legal_hold is not None:
+            legal_hold.add_to_upload_headers(headers)
+
+        if file_retention is not None:
+            file_retention.add_to_to_upload_headers(headers)
+
+        if custom_upload_timestamp is not None:
+            headers['X-Bz-Custom-Upload-Timestamp'] = str(custom_upload_timestamp)
+
+        return headers
+
     @abstractmethod
     def upload_file(
         self,
         upload_url,
         upload_auth_token,
         file_name,
         content_length,
         content_type,
         content_sha1,
-        file_infos,
+        file_info,
         data_stream,
-        server_side_encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        server_side_encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
     ):
         pass
 
     @abstractmethod
     def upload_part(
         self,
         upload_url,
         upload_auth_token,
         part_number,
         content_length,
         sha1_sum,
         input_stream,
-        server_side_encryption: Optional[EncryptionSetting] = None,
+        server_side_encryption: EncryptionSetting | None = None,
     ):
         pass
 
     def get_download_url_by_id(self, download_url, file_id):
-        return '%s/b2api/%s/b2_download_file_by_id?fileId=%s' % (download_url, API_VERSION, file_id)
+        return f'{download_url}/b2api/{API_VERSION}/b2_download_file_by_id?fileId={file_id}'
 
     def get_download_url_by_name(self, download_url, bucket_name, file_name):
         return download_url + '/file/' + bucket_name + '/' + b2_url_encode(file_name)
 
 
-class B2RawApi(AbstractRawApi):
+class B2RawHTTPApi(AbstractRawApi):
     """
     Provide access to the B2 web APIs, exactly as they are provided by b2.
 
     Requires that you provide all necessary URLs and auth tokens for each call.
 
     Each API call decodes the returned JSON and returns a dict.
 
@@ -360,50 +432,53 @@
     And this class can be tested by exercising each call just once,
     which is relatively quick.
     """
 
     def __init__(self, b2_http):
         self.b2_http = b2_http
 
-    def _post_json(self, base_url, api_name, auth, **params) -> Dict[str, Any]:
+    def _post_json(self, base_url: str, endpoint: str, auth: str, **params) -> JSON:
         """
         A helper method for calling an API with the given auth and params.
 
         :param base_url: something like "https://api001.backblazeb2.com/"
         :param auth: passed in Authorization header
-        :param api_name: example: "b2_create_bucket"
+        :param endpoint: example: "b2_create_bucket"
         :param args: the rest of the parameters are passed to b2
         :return: the decoded JSON response
-        :rtype: dict
         """
-        url = '%s/b2api/%s/%s' % (base_url, API_VERSION, api_name)
+        url = f'{base_url}/b2api/{API_VERSION}/{endpoint}'
         headers = {'Authorization': auth}
         return self.b2_http.post_json_return_json(url, headers, params)
 
+    def _get_json(self, base_url: str, endpoint: str, auth: str, **params) -> JSON:
+        url = f'{base_url}/b2api/{API_VERSION}/{endpoint}'
+        headers = {'Authorization': auth}
+        return self.b2_http.request_content_return_json('GET', url, headers, params=params)
+
     def authorize_account(self, realm_url, application_key_id, application_key):
-        auth = b'Basic ' + base64.b64encode(
-            ('%s:%s' % (application_key_id, application_key)).encode()
-        )
+        auth = f"Basic {base64.b64encode(f'{application_key_id}:{application_key}'.encode()).decode()}"
         return self._post_json(realm_url, 'b2_authorize_account', auth)
 
     def cancel_large_file(self, api_url, account_auth_token, file_id):
         return self._post_json(api_url, 'b2_cancel_large_file', account_auth_token, fileId=file_id)
 
     def create_bucket(
         self,
         api_url,
         account_auth_token,
         account_id,
         bucket_name,
         bucket_type,
         bucket_info=None,
         cors_rules=None,
-        lifecycle_rules=None,
-        default_server_side_encryption: Optional[EncryptionSetting] = None,
-        is_file_lock_enabled: Optional[bool] = None,
+        lifecycle_rules: list[LifecycleRule] | None = None,
+        default_server_side_encryption: EncryptionSetting | None = None,
+        is_file_lock_enabled: bool | None = None,
+        replication: ReplicationConfiguration | None = None,
     ):
         kwargs = dict(
             accountId=account_id,
             bucketName=bucket_name,
             bucketType=bucket_type,
         )
         if bucket_info is not None:
@@ -415,14 +490,16 @@
         if default_server_side_encryption is not None:
             if not default_server_side_encryption.mode.can_be_set_as_bucket_default():
                 raise WrongEncryptionModeForBucketDefault(default_server_side_encryption.mode)
             kwargs['defaultServerSideEncryption'
                   ] = default_server_side_encryption.serialize_to_json_for_request()
         if is_file_lock_enabled is not None:
             kwargs['fileLockEnabled'] = is_file_lock_enabled
+        if replication is not None:
+            kwargs['replicationConfiguration'] = replication.serialize_to_json_for_request()
         return self._post_json(
             api_url,
             'b2_create_bucket',
             account_auth_token,
             **kwargs,
         )
 
@@ -447,21 +524,24 @@
             api_url,
             'b2_delete_bucket',
             account_auth_token,
             accountId=account_id,
             bucketId=bucket_id
         )
 
-    def delete_file_version(self, api_url, account_auth_token, file_id, file_name):
+    def delete_file_version(
+        self, api_url, account_auth_token, file_id, file_name, bypass_governance: bool = False
+    ):
         return self._post_json(
             api_url,
             'b2_delete_file_version',
             account_auth_token,
             fileId=file_id,
-            fileName=file_name
+            fileName=file_name,
+            bypassGovernance=bypass_governance,
         )
 
     def delete_key(self, api_url, account_auth_token, application_key_id):
         return self._post_json(
             api_url,
             'b2_delete_key',
             account_auth_token,
@@ -469,23 +549,23 @@
         )
 
     def download_file_from_url(
         self,
         account_auth_token_or_none,
         url,
         range_=None,
-        encryption: Optional[EncryptionSetting] = None,
+        encryption: EncryptionSetting | None = None,
     ):
         """
         Issue a streaming request for download of a file, potentially authorized.
 
         :param str account_auth_token_or_none: an optional account auth token to pass in
         :param str url: the full URL to download from
         :param tuple range: two-element tuple for http Range header
-        :param b2sdk.v1.EncryptionSetting encryption: encryption settings for downloading
+        :param b2sdk.v2.EncryptionSetting encryption: encryption settings for downloading
         :return: b2_http response
         """
         request_headers = {}
         _add_range_header(request_headers, range_)
 
         if encryption is not None:
             assert encryption.mode in (
@@ -518,20 +598,20 @@
             account_auth_token,
             bucketId=bucket_id,
             fileNamePrefix=file_name_prefix,
             validDurationInSeconds=valid_duration_in_seconds
         )
 
     def get_file_info_by_id(self, api_url: str, account_auth_token: str,
-                            file_id: str) -> Dict[str, Any]:
+                            file_id: str) -> dict[str, Any]:
         return self._post_json(api_url, 'b2_get_file_info', account_auth_token, fileId=file_id)
 
     def get_file_info_by_name(
         self, download_url: str, account_auth_token: str, bucket_name: str, file_name: str
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         download_url = self.get_download_url_by_name(download_url, bucket_name, file_name)
         try:
             response = self.b2_http.head_content(
                 download_url, headers={"Authorization": account_auth_token}
             )
             return response.headers
         except ResourceNotFound:
@@ -659,31 +739,38 @@
         self,
         api_url,
         account_auth_token,
         bucket_id,
         file_name,
         content_type,
         file_info,
-        server_side_encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        server_side_encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
     ):
         kwargs = {}
         if server_side_encryption is not None:
             assert server_side_encryption.mode in (
                 EncryptionMode.NONE, EncryptionMode.SSE_B2, EncryptionMode.SSE_C
             )
             kwargs['serverSideEncryption'] = server_side_encryption.serialize_to_json_for_request()
 
+            if server_side_encryption.mode == EncryptionMode.SSE_C:
+                file_info = server_side_encryption.add_key_id_to_file_info(file_info)
+
         if legal_hold is not None:
             kwargs['legalHold'] = legal_hold.to_server()
 
         if file_retention is not None:
             kwargs['fileRetention'] = file_retention.serialize_to_json_for_request()
 
+        if custom_upload_timestamp is not None:
+            kwargs['custom_upload_timestamp'] = custom_upload_timestamp
+
         return self._post_json(
             api_url,
             'b2_start_large_file',
             account_auth_token,
             bucketId=bucket_id,
             fileName=file_name,
             fileInfo=file_info,
@@ -696,21 +783,21 @@
         api_url,
         account_auth_token,
         account_id,
         bucket_id,
         bucket_type=None,
         bucket_info=None,
         cors_rules=None,
-        lifecycle_rules=None,
+        lifecycle_rules: list[LifecycleRule] | None = None,
         if_revision_is=None,
-        default_server_side_encryption: Optional[EncryptionSetting] = None,
-        default_retention: Optional[BucketRetentionSetting] = None,
+        default_server_side_encryption: EncryptionSetting | None = None,
+        default_retention: BucketRetentionSetting | None = None,
+        replication: ReplicationConfiguration | None = None,
+        is_file_lock_enabled: bool | None = None,
     ):
-        assert bucket_info is not None or bucket_type is not None
-
         kwargs = {}
         if if_revision_is is not None:
             kwargs['ifRevisionIs'] = if_revision_is
         if bucket_info is not None:
             kwargs['bucketInfo'] = bucket_info
         if bucket_type is not None:
             kwargs['bucketType'] = bucket_type
@@ -721,14 +808,20 @@
         if default_server_side_encryption is not None:
             if not default_server_side_encryption.mode.can_be_set_as_bucket_default():
                 raise WrongEncryptionModeForBucketDefault(default_server_side_encryption.mode)
             kwargs['defaultServerSideEncryption'
                   ] = default_server_side_encryption.serialize_to_json_for_request()
         if default_retention is not None:
             kwargs['defaultRetention'] = default_retention.serialize_to_json_for_request()
+        if replication is not None:
+            kwargs['replicationConfiguration'] = replication.serialize_to_json_for_request()
+        if is_file_lock_enabled is not None:
+            kwargs['fileLockEnabled'] = is_file_lock_enabled
+
+        assert kwargs
 
         return self._post_json(
             api_url,
             'b2_update_bucket',
             account_auth_token,
             accountId=account_id,
             bucketId=bucket_id,
@@ -775,29 +868,14 @@
                 fileId=file_id,
                 fileName=file_name,
                 legalHold=legal_hold.to_server(),
             )
         except AccessDenied:
             raise RetentionWriteError()
 
-    def unprintable_to_hex(self, string):
-        """
-        Replace unprintable chars in string with a hex representation.
-
-        :param string: an arbitrary string, possibly with unprintable characters.
-        :return: the string, with unprintable characters changed to hex (e.g., "\x07")
-
-        """
-        unprintables_pattern = re.compile(r'[\x00-\x1f]')
-
-        def hexify(match):
-            return r'\x{0:02x}'.format(ord(match.group()))
-
-        return unprintables_pattern.sub(hexify, string)
-
     def check_b2_filename(self, filename):
         """
         Raise an appropriate exception with details if the filename is unusable.
 
         See https://www.backblaze.com/b2/docs/files.html for the rules.
 
         :param filename: a proposed filename in unicode
@@ -807,16 +885,16 @@
         length_in_bytes = len(encoded_name)
         if length_in_bytes < 1:
             raise UnusableFileName("Filename must be at least 1 character.")
         if length_in_bytes > 1024:
             raise UnusableFileName("Filename is too long (can be at most 1024 bytes).")
         lowest_unicode_value = ord(min(filename))
         if lowest_unicode_value < 32:
-            message = u"Filename \"{0}\" contains code {1} (hex {2:02x}), less than 32.".format(
-                self.unprintable_to_hex(filename), lowest_unicode_value, lowest_unicode_value
+            message = "Filename \"{}\" contains code {} (hex {:02x}), less than 32.".format(
+                unprintable_to_hex(filename), lowest_unicode_value, lowest_unicode_value
             )
             raise UnusableFileName(message)
         # No DEL for you.
         if '\x7f' in filename:
             raise UnusableFileName("DEL character (0x7f) not allowed.")
         if filename[0] == '/' or filename[-1] == '/':
             raise UnusableFileName("Filename may not start or end with '/'.")
@@ -830,67 +908,63 @@
         self,
         upload_url,
         upload_auth_token,
         file_name,
         content_length,
         content_type,
         content_sha1,
-        file_infos,
+        file_info: dict,
         data_stream,
-        server_side_encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        server_side_encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
     ):
         """
         Upload one, small file to b2.
 
         :param upload_url: the upload_url from b2_authorize_account
         :param upload_auth_token: the auth token from b2_authorize_account
         :param file_name: the name of the B2 file
         :param content_length: number of bytes in the file
         :param content_type: MIME type
         :param content_sha1: hex SHA1 of the contents of the file
-        :param file_infos: extra file info to upload
+        :param file_info: extra file info to upload
         :param data_stream: a file like object from which the contents of the file can be read
+        :param server_side_encryption: encryption setting for the file
+        :param file_retention: retention setting for the file
+        :param legal_hold: legal hold setting for the file
+        :param custom_upload_timestamp: custom upload timestamp for the file
         :return:
         """
         # Raise UnusableFileName if the file_name doesn't meet the rules.
         self.check_b2_filename(file_name)
-        headers = {
-            'Authorization': upload_auth_token,
-            'Content-Length': str(content_length),
-            'X-Bz-File-Name': b2_url_encode(file_name),
-            'Content-Type': content_type,
-            'X-Bz-Content-Sha1': content_sha1,
-        }
-        for k, v in file_infos.items():
-            headers['X-Bz-Info-' + k] = b2_url_encode(v)
-        if server_side_encryption is not None:
-            assert server_side_encryption.mode in (
-                EncryptionMode.NONE, EncryptionMode.SSE_B2, EncryptionMode.SSE_C
-            )
-            server_side_encryption.add_to_upload_headers(headers)
-
-        if legal_hold is not None:
-            legal_hold.add_to_upload_headers(headers)
-
-        if file_retention is not None:
-            file_retention.add_to_to_upload_headers(headers)
-
+        headers = self.get_upload_file_headers(
+            upload_auth_token=upload_auth_token,
+            file_name=file_name,
+            content_length=content_length,
+            content_type=content_type,
+            content_sha1=content_sha1,
+            file_info=file_info,
+            server_side_encryption=server_side_encryption,
+            file_retention=file_retention,
+            legal_hold=legal_hold,
+            custom_upload_timestamp=custom_upload_timestamp,
+        )
         return self.b2_http.post_content_return_json(upload_url, headers, data_stream)
 
     def upload_part(
         self,
         upload_url,
         upload_auth_token,
         part_number,
         content_length,
         content_sha1,
         data_stream,
-        server_side_encryption: Optional[EncryptionSetting] = None,
+        server_side_encryption: EncryptionSetting | None = None,
     ):
         headers = {
             'Authorization': upload_auth_token,
             'Content-Length': str(content_length),
             'X-Bz-Part-Number': str(part_number),
             'X-Bz-Content-Sha1': content_sha1
         }
@@ -909,18 +983,18 @@
         source_file_id,
         new_file_name,
         bytes_range=None,
         metadata_directive=None,
         content_type=None,
         file_info=None,
         destination_bucket_id=None,
-        destination_server_side_encryption: Optional[EncryptionSetting] = None,
-        source_server_side_encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        destination_server_side_encryption: EncryptionSetting | None = None,
+        source_server_side_encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
     ):
         kwargs = {}
         if bytes_range is not None:
             range_dict = {}
             _add_range_header(range_dict, bytes_range)
             kwargs['range'] = range_dict['Range']
 
@@ -977,16 +1051,16 @@
         self,
         api_url,
         account_auth_token,
         source_file_id,
         large_file_id,
         part_number,
         bytes_range=None,
-        destination_server_side_encryption: Optional[EncryptionSetting] = None,
-        source_server_side_encryption: Optional[EncryptionSetting] = None,
+        destination_server_side_encryption: EncryptionSetting | None = None,
+        source_server_side_encryption: EncryptionSetting | None = None,
     ):
         kwargs = {}
         if bytes_range is not None:
             range_dict = {}
             _add_range_header(range_dict, bytes_range)
             kwargs['range'] = range_dict['Range']
         if destination_server_side_encryption is not None:
@@ -1011,385 +1085,13 @@
                 partNumber=part_number,
                 **kwargs
             )
         except AccessDenied:
             raise SSECKeyError()
 
 
-def test_raw_api():
-    """
-    Exercise the code in B2RawApi by making each call once, just
-    to make sure the parameters are passed in, and the result is
-    passed back.
-
-    The goal is to be a complete test of B2RawApi, so the tests for
-    the rest of the code can use the simulator.
-
-    Prints to stdout if things go wrong.
-
-    :return: 0 on success, non-zero on failure
-    """
-    try:
-        raw_api = B2RawApi(B2Http())
-        test_raw_api_helper(raw_api)
-        return 0
-    except Exception:
-        traceback.print_exc(file=sys.stdout)
-        return 1
-
-
-def test_raw_api_helper(raw_api):
-    """
-    Try each of the calls to the raw api.  Raise an
-    exception if anything goes wrong.
-
-    This uses a Backblaze account that is just for this test.
-    The account uses the free level of service, which should
-    be enough to run this test a reasonable number of times
-    each day.  If somebody abuses the account for other things,
-    this test will break and we'll have to do something about
-    it.
-    """
-    application_key_id = os.environ.get('B2_TEST_APPLICATION_KEY_ID')
-    if application_key_id is None:
-        print('B2_TEST_APPLICATION_KEY_ID is not set.', file=sys.stderr)
-        sys.exit(1)
-
-    application_key = os.environ.get('B2_TEST_APPLICATION_KEY')
-    if application_key is None:
-        print('B2_TEST_APPLICATION_KEY is not set.', file=sys.stderr)
-        sys.exit(1)
-
-    realm = os.environ.get('B2_TEST_ENVIRONMENT', 'production')
-    realm_url = REALM_URLS.get(realm, realm)
-
-    # b2_authorize_account
-    print('b2_authorize_account')
-    auth_dict = raw_api.authorize_account(realm_url, application_key_id, application_key)
-    account_id = auth_dict['accountId']
-    account_auth_token = auth_dict['authorizationToken']
-    api_url = auth_dict['apiUrl']
-    download_url = auth_dict['downloadUrl']
-
-    # b2_create_key
-    print('b2_create_key')
-    key_dict = raw_api.create_key(
-        api_url,
-        account_auth_token,
-        account_id,
-        ['readFiles'],
-        'testKey',
-        None,
-        None,
-        None,
-    )
-
-    # b2_list_keys
-    print('b2_list_keys')
-    raw_api.list_keys(api_url, account_auth_token, account_id, 10)
-
-    # b2_delete_key
-    print('b2_delete_key')
-    raw_api.delete_key(api_url, account_auth_token, key_dict['applicationKeyId'])
-
-    # b2_create_bucket, with a unique bucket name
-    # Include the account ID in the bucket name to be
-    # sure it doesn't collide with bucket names from
-    # other accounts.
-    print('b2_create_bucket')
-    bucket_name = 'test-raw-api-%s-%d-%d' % (
-        account_id, int(time.time()), random.randint(1000, 9999)
-    )
-
-    # very verbose http debug
-    #import http.client; http.client.HTTPConnection.debuglevel = 1
-
-    bucket_dict = raw_api.create_bucket(
-        api_url,
-        account_auth_token,
-        account_id,
-        bucket_name,
-        'allPublic',
-        is_file_lock_enabled=True,
-    )
-    bucket_id = bucket_dict['bucketId']
-    first_bucket_revision = bucket_dict['revision']
-
-    ##################
-    print('b2_update_bucket')
-    sse_b2_aes = EncryptionSetting(
-        mode=EncryptionMode.SSE_B2,
-        algorithm=EncryptionAlgorithm.AES256,
-    )
-    sse_none = EncryptionSetting(mode=EncryptionMode.NONE)
-    for encryption_setting, default_retention in [
-        (
-            sse_none,
-            BucketRetentionSetting(mode=RetentionMode.GOVERNANCE, period=RetentionPeriod(days=1))
-        ),
-        (sse_b2_aes, None),
-        (sse_b2_aes, BucketRetentionSetting(RetentionMode.NONE)),
-    ]:
-        bucket_dict = raw_api.update_bucket(
-            api_url,
-            account_auth_token,
-            account_id,
-            bucket_id,
-            'allPublic',
-            default_server_side_encryption=encryption_setting,
-            default_retention=default_retention,
-        )
-
-    # b2_list_buckets
-    print('b2_list_buckets')
-    bucket_list_dict = raw_api.list_buckets(api_url, account_auth_token, account_id)
-    #print(bucket_list_dict)
-
-    # b2_get_upload_url
-    print('b2_get_upload_url')
-    upload_url_dict = raw_api.get_upload_url(api_url, account_auth_token, bucket_id)
-    upload_url = upload_url_dict['uploadUrl']
-    upload_auth_token = upload_url_dict['authorizationToken']
-
-    # b2_upload_file
-    print('b2_upload_file')
-    file_name = 'test.txt'
-    file_contents = b'hello world'
-    file_sha1 = hex_sha1_of_stream(io.BytesIO(file_contents), len(file_contents))
-    file_dict = raw_api.upload_file(
-        upload_url,
-        upload_auth_token,
-        file_name,
-        len(file_contents),
-        'text/plain',
-        file_sha1,
-        {'color': 'blue'},
-        io.BytesIO(file_contents),
-        server_side_encryption=sse_b2_aes,
-    )
-
-    file_id = file_dict['fileId']
-
-    # b2_list_file_versions
-    print('b2_list_file_versions')
-    list_versions_dict = raw_api.list_file_versions(api_url, account_auth_token, bucket_id)
-    assert [file_name] == [f_dict['fileName'] for f_dict in list_versions_dict['files']]
-
-    # b2_download_file_by_id with auth
-    print('b2_download_file_by_id (auth)')
-    url = raw_api.get_download_url_by_id(download_url, file_id)
-    with raw_api.download_file_from_url(account_auth_token, url) as response:
-        data = next(response.iter_content(chunk_size=len(file_contents)))
-        assert data == file_contents, data
-
-    # b2_download_file_by_id no auth
-    print('b2_download_file_by_id (no auth)')
-    url = raw_api.get_download_url_by_id(download_url, file_id)
-    with raw_api.download_file_from_url(None, url) as response:
-        data = next(response.iter_content(chunk_size=len(file_contents)))
-        assert data == file_contents, data
-
-    # b2_download_file_by_name with auth
-    print('b2_download_file_by_name (auth)')
-    url = raw_api.get_download_url_by_name(download_url, bucket_name, file_name)
-    with raw_api.download_file_from_url(account_auth_token, url) as response:
-        data = next(response.iter_content(chunk_size=len(file_contents)))
-        assert data == file_contents, data
-
-    # b2_download_file_by_name no auth
-    print('b2_download_file_by_name (no auth)')
-    url = raw_api.get_download_url_by_name(download_url, bucket_name, file_name)
-    with raw_api.download_file_from_url(None, url) as response:
-        data = next(response.iter_content(chunk_size=len(file_contents)))
-        assert data == file_contents, data
-
-    # b2_get_download_authorization
-    print('b2_get_download_authorization')
-    download_auth = raw_api.get_download_authorization(
-        api_url, account_auth_token, bucket_id, file_name[:-2], 12345
-    )
-    download_auth_token = download_auth['authorizationToken']
-
-    # b2_download_file_by_name with download auth
-    print('b2_download_file_by_name (download auth)')
-    url = raw_api.get_download_url_by_name(download_url, bucket_name, file_name)
-    with raw_api.download_file_from_url(download_auth_token, url) as response:
-        data = next(response.iter_content(chunk_size=len(file_contents)))
-        assert data == file_contents, data
-
-    # b2_list_file_names
-    print('b2_list_file_names')
-    list_names_dict = raw_api.list_file_names(api_url, account_auth_token, bucket_id)
-    assert [file_name] == [f_dict['fileName'] for f_dict in list_names_dict['files']]
-
-    # b2_list_file_names (start, count)
-    print('b2_list_file_names (start, count)')
-    list_names_dict = raw_api.list_file_names(
-        api_url, account_auth_token, bucket_id, start_file_name=file_name, max_file_count=5
-    )
-    assert [file_name] == [f_dict['fileName'] for f_dict in list_names_dict['files']]
-
-    # b2_copy_file
-    print('b2_copy_file')
-    copy_file_name = 'test_copy.txt'
-    raw_api.copy_file(api_url, account_auth_token, file_id, copy_file_name)
-
-    # b2_get_file_info_by_id
-    print('b2_get_file_info_by_id')
-    file_info_dict = raw_api.get_file_info_by_id(api_url, account_auth_token, file_id)
-    assert file_info_dict['fileName'] == file_name
-
-    # b2_get_file_info_by_name
-    print('b2_get_file_info_by_name (no auth)')
-    info_headers = raw_api.get_file_info_by_name(download_url, None, bucket_name, file_name)
-    assert info_headers['x-bz-file-id'] == file_id
-
-    # b2_get_file_info_by_name
-    print('b2_get_file_info_by_name (auth)')
-    info_headers = raw_api.get_file_info_by_name(
-        download_url, account_auth_token, bucket_name, file_name
-    )
-    assert info_headers['x-bz-file-id'] == file_id
-
-    # b2_get_file_info_by_name
-    print('b2_get_file_info_by_name (download auth)')
-    info_headers = raw_api.get_file_info_by_name(
-        download_url, download_auth_token, bucket_name, file_name
-    )
-    assert info_headers['x-bz-file-id'] == file_id
-
-    # b2_hide_file
-    print('b2_hide_file')
-    raw_api.hide_file(api_url, account_auth_token, bucket_id, file_name)
-
-    # b2_start_large_file
-    print('b2_start_large_file')
-    file_info = {'color': 'red'}
-    large_info = raw_api.start_large_file(
-        api_url,
-        account_auth_token,
-        bucket_id,
-        file_name,
-        'text/plain',
-        file_info,
-        server_side_encryption=sse_b2_aes,
-    )
-    large_file_id = large_info['fileId']
-
-    # b2_get_upload_part_url
-    print('b2_get_upload_part_url')
-    upload_part_dict = raw_api.get_upload_part_url(api_url, account_auth_token, large_file_id)
-    upload_part_url = upload_part_dict['uploadUrl']
-    upload_path_auth = upload_part_dict['authorizationToken']
-
-    # b2_upload_part
-    print('b2_upload_part')
-    part_contents = b'hello part'
-    part_sha1 = hex_sha1_of_stream(io.BytesIO(part_contents), len(part_contents))
-    raw_api.upload_part(
-        upload_part_url, upload_path_auth, 1, len(part_contents), part_sha1,
-        io.BytesIO(part_contents)
-    )
-
-    # b2_copy_part
-    print('b2_copy_part')
-    raw_api.copy_part(api_url, account_auth_token, file_id, large_file_id, 2, (0, 5))
-
-    # b2_list_parts
-    print('b2_list_parts')
-    parts_response = raw_api.list_parts(api_url, account_auth_token, large_file_id, 1, 100)
-    assert [1, 2] == [part['partNumber'] for part in parts_response['parts']]
-
-    # b2_list_unfinished_large_files
-    unfinished_list = raw_api.list_unfinished_large_files(api_url, account_auth_token, bucket_id)
-    assert [file_name] == [f_dict['fileName'] for f_dict in unfinished_list['files']]
-    assert file_info == unfinished_list['files'][0]['fileInfo']
-
-    # b2_finish_large_file
-    print('b2_finish_large_file')
-    try:
-        raw_api.finish_large_file(api_url, account_auth_token, large_file_id, [part_sha1])
-        raise Exception('finish should have failed')
-    except Exception as e:
-        assert 'large files must have at least 2 parts' in str(e)
-    # TODO: make another attempt to finish but this time successfully
-
-    # b2_update_bucket
-    print('b2_update_bucket')
-    updated_bucket = raw_api.update_bucket(
-        api_url,
-        account_auth_token,
-        account_id,
-        bucket_id,
-        'allPrivate',
-        bucket_info={'color': 'blue'},
-        default_retention=BucketRetentionSetting(
-            mode=RetentionMode.GOVERNANCE, period=RetentionPeriod(days=1)
-        ),
-    )
-    assert first_bucket_revision < updated_bucket['revision']
-
-    # Clean up this test.
-    _clean_and_delete_bucket(raw_api, api_url, account_auth_token, account_id, bucket_id)
-
-    # Clean up from old tests. Empty and delete any buckets more than an hour old.
-    for bucket_dict in bucket_list_dict['buckets']:
-        bucket_id = bucket_dict['bucketId']
-        bucket_name = bucket_dict['bucketName']
-        if _should_delete_bucket(bucket_name):
-            print('cleaning up old bucket: ' + bucket_name)
-            _clean_and_delete_bucket(raw_api, api_url, account_auth_token, account_id, bucket_id)
-
-
-def _clean_and_delete_bucket(raw_api, api_url, account_auth_token, account_id, bucket_id):
-    # Delete the files. This test never creates more than a few files,
-    # so one call to list_file_versions should get them all.
-    versions_dict = raw_api.list_file_versions(api_url, account_auth_token, bucket_id)
-    for version_dict in versions_dict['files']:
-        file_id = version_dict['fileId']
-        file_name = version_dict['fileName']
-        action = version_dict['action']
-        if action in ['hide', 'upload']:
-            print('b2_delete_file', file_name, action)
-            if action == 'upload' and version_dict[
-                'fileRetention'] and version_dict['fileRetention']['value']['mode'] is not None:
-                raw_api.update_file_retention(
-                    api_url,
-                    account_auth_token,
-                    file_id,
-                    file_name,
-                    NO_RETENTION_FILE_SETTING,
-                    bypass_governance=True
-                )
-            raw_api.delete_file_version(api_url, account_auth_token, file_id, file_name)
-        else:
-            print('b2_cancel_large_file', file_name)
-            raw_api.cancel_large_file(api_url, account_auth_token, file_id)
-
-    # Delete the bucket
-    print('b2_delete_bucket', bucket_id)
-    raw_api.delete_bucket(api_url, account_auth_token, account_id, bucket_id)
-
-
-def _should_delete_bucket(bucket_name):
-    # Bucket names for this test look like: c7b22d0b0ad7-1460060364-5670
-    # Other buckets should not be deleted.
-    match = re.match(r'^test-raw-api-[a-f0-9]+-([0-9]+)-([0-9]+)', bucket_name)
-    if match is None:
-        return False
-
-    # Is it more than an hour old?
-    bucket_time = int(match.group(1))
-    now = time.time()
-    return bucket_time + 3600 <= now
-
-
 def _add_range_header(headers, range_):
     if range_ is not None:
         assert len(range_) == 2, range_
         assert (range_[0] + 0) <= (range_[1] + 0), range_  # not strings
         assert range_[0] >= 0, range_
         headers['Range'] = "bytes=%d-%d" % range_
-
-
-if __name__ == '__main__':
-    test_raw_api()
```

### Comparing `b2sdk-1.9.0/b2sdk/raw_simulator.py` & `b2sdk-2.0.0/b2sdk/_internal/raw_simulator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,85 @@
 ######################################################################
 #
-# File: b2sdk/raw_simulator.py
+# File: b2sdk/_internal/raw_simulator.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from typing import Optional
 import collections
 import io
 import logging
 import random
 import re
-import time
 import threading
-from contextlib import contextmanager
+import time
+from contextlib import contextmanager, suppress
+
+from requests.structures import CaseInsensitiveDict
 
 from .b2http import ResponseContextManager
 from .encryption.setting import EncryptionMode, EncryptionSetting
 from .exception import (
+    AccessDenied,
     BadJson,
+    BadRequest,
     BadUploadUrl,
     ChecksumMismatch,
     Conflict,
+    CopySourceTooBig,
+    DisablingFileLockNotSupported,
     DuplicateBucketName,
     FileNotPresent,
     FileSha1Mismatch,
     InvalidAuthToken,
     InvalidMetadataDirective,
     MissingPart,
     NonExistentBucket,
     PartSha1Mismatch,
+    SourceReplicationConflict,
+    SSECKeyError,
     Unauthorized,
     UnsatisfiableRange,
-    SSECKeyError,
 )
-from .file_lock import BucketRetentionSetting, FileRetentionSetting, NO_RETENTION_BUCKET_SETTING, UNKNOWN_FILE_LOCK_CONFIGURATION, LegalHold
-from .raw_api import AbstractRawApi, HEX_DIGITS_AT_END, MetadataDirectiveMode, ALL_CAPABILITIES
-from .utils import (
-    b2_url_decode,
-    b2_url_encode,
-    ConcurrentUsedAuthTokenGuard,
-    hex_sha1_of_bytes,
+from .file_lock import (
+    NO_RETENTION_BUCKET_SETTING,
+    BucketRetentionSetting,
+    FileRetentionSetting,
+    LegalHold,
+    RetentionMode,
 )
+from .file_version import UNVERIFIED_CHECKSUM_PREFIX
+from .http_constants import FILE_INFO_HEADER_PREFIX, HEX_DIGITS_AT_END
+from .raw_api import ALL_CAPABILITIES, AbstractRawApi, LifecycleRule, MetadataDirectiveMode
+from .replication.setting import ReplicationConfiguration
+from .replication.types import ReplicationStatus
 from .stream.hashing import StreamWithHash
+from .utils import ConcurrentUsedAuthTokenGuard, b2_url_decode, b2_url_encode, hex_sha1_of_bytes
 
 logger = logging.getLogger(__name__)
 
 
 def get_bytes_range(data_bytes, bytes_range):
     """ Slice bytes array using bytes range """
     if bytes_range is None:
         return data_bytes
     if bytes_range[0] > bytes_range[1]:
         raise UnsatisfiableRange()
     if bytes_range[0] < 0:
         raise UnsatisfiableRange()
     if bytes_range[1] > len(data_bytes):
         raise UnsatisfiableRange()
-    return data_bytes[bytes_range[0]:bytes_range[1]]
+    return data_bytes[bytes_range[0]:bytes_range[1] + 1]
 
 
-class KeySimulator(object):
+class KeySimulator:
     """
     Hold information about one application key, which can be either
     a master application key, or one created with create_key().
     """
 
     def __init__(
         self, account_id, name, application_key_id, key, capabilities, expiration_timestamp_or_none,
@@ -76,24 +88,25 @@
         self.name = name
         self.account_id = account_id
         self.application_key_id = application_key_id
         self.key = key
         self.capabilities = capabilities
         self.expiration_timestamp_or_none = expiration_timestamp_or_none
         self.bucket_id_or_none = bucket_id_or_none
+        self.bucket_name_or_none = bucket_name_or_none
         self.name_prefix_or_none = name_prefix_or_none
 
     def as_key(self):
         return dict(
             accountId=self.account_id,
             bucketId=self.bucket_id_or_none,
-            applicationKey=self.key,
             applicationKeyId=self.application_key_id,
             capabilities=self.capabilities,
-            expirationTimestamp=self.expiration_timestamp_or_none,
+            expirationTimestamp=self.expiration_timestamp_or_none and
+            self.expiration_timestamp_or_none * 1000,
             keyName=self.name,
             namePrefix=self.name_prefix_or_none,
         )
 
     def as_created_key(self):
         """
         Return the dict returned by b2_create_key.
@@ -106,20 +119,21 @@
 
     def get_allowed(self):
         """
         Return the 'allowed' structure to include in the response from b2_authorize_account.
         """
         return dict(
             bucketId=self.bucket_id_or_none,
+            bucketName=self.bucket_name_or_none,
             capabilities=self.capabilities,
             namePrefix=self.name_prefix_or_none,
         )
 
 
-class PartSimulator(object):
+class PartSimulator:
     def __init__(self, file_id, part_number, content_length, content_sha1, part_data):
         self.file_id = file_id
         self.part_number = part_number
         self.content_length = content_length
         self.content_sha1 = content_sha1
         self.part_data = part_data
 
@@ -128,37 +142,45 @@
             fileId=self.file_id,
             partNumber=self.part_number,
             contentLength=self.content_length,
             contentSha1=self.content_sha1
         )  # yapf: disable
 
 
-class FileSimulator(object):
+class FileSimulator:
     """
     One of three: an unfinished large file, a finished file, or a deletion marker.
     """
 
     CHECK_ENCRYPTION = True
+    SPECIAL_FILE_INFOS = {  # when downloading, these file info keys are translated to specialized headers
+        'b2-content-disposition': 'Content-Disposition',
+        'b2-content-language': 'Content-Language',
+        'b2-expires': 'Expires',
+        'b2-cache-control': 'Cache-Control',
+        'b2-content-encoding': 'Content-Encoding',
+    }
 
     def __init__(
         self,
         account_id,
         bucket,
         file_id,
         action,
         name,
         content_type,
         content_sha1,
         file_info,
         data_bytes,
         upload_timestamp,
         range_=None,
-        server_side_encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
+        server_side_encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
         legal_hold: LegalHold = LegalHold.UNSET,
+        replication_status: ReplicationStatus | None = None,
     ):
         if action == 'hide':
             assert server_side_encryption is None
         else:
             assert server_side_encryption is not None
         self.account_id = account_id
         self.bucket = bucket
@@ -174,14 +196,15 @@
         self.file_info = file_info
         self.data_bytes = data_bytes
         self.upload_timestamp = upload_timestamp
         self.range_ = range_
         self.server_side_encryption = server_side_encryption
         self.file_retention = file_retention
         self.legal_hold = legal_hold if legal_hold is not None else LegalHold.UNSET
+        self.replication_status = replication_status
 
         if action == 'start':
             self.parts = []
 
     @classmethod
     @contextmanager
     def dont_check_encryption(cls):
@@ -202,22 +225,30 @@
         elif range_ is not None:
             if range_[1] >= len(self.data_bytes):  # requested too much
                 content_length = len(self.data_bytes)
             else:
                 content_length = range_[1] - range_[0] + 1
         else:
             content_length = len(self.data_bytes)
-        headers = {
-            'content-length': content_length,
-            'content-type': self.content_type,
-            'x-bz-content-sha1': self.content_sha1,
-            'x-bz-upload-timestamp': self.upload_timestamp,
-            'x-bz-file-id': self.file_id,
-            'x-bz-file-name': self.name,
-        }
+        headers = CaseInsensitiveDict(
+            {
+                'content-length': content_length,
+                'content-type': self.content_type,
+                'x-bz-content-sha1': self.content_sha1,
+                'x-bz-upload-timestamp': self.upload_timestamp,
+                'x-bz-file-id': self.file_id,
+                'x-bz-file-name': b2_url_encode(self.name),
+            }
+        )
+        for key, value in self.file_info.items():
+            key_lower = key.lower()
+            if key_lower in self.SPECIAL_FILE_INFOS:
+                headers[self.SPECIAL_FILE_INFOS[key_lower]] = value
+            else:
+                headers[FILE_INFO_HEADER_PREFIX + key] = b2_url_encode(value)
 
         if account_auth_token_or_none is not None and self.bucket.is_file_lock_enabled:
             not_permitted = []
 
             if not self.is_allowed_to_read_file_retention(account_auth_token_or_none):
                 not_permitted.append('X-Bz-File-Retention-Mode')
                 not_permitted.append('X-Bz-File-Retain-Until-Timestamp')
@@ -229,52 +260,67 @@
                 not_permitted.append('X-Bz-File-Legal-Hold')
             else:
                 headers['X-Bz-File-Legal-Hold'] = self.legal_hold and 'on' or 'off'
 
             if not_permitted:
                 headers['X-Bz-Client-Unauthorized-To-Read'] = ','.join(not_permitted)
 
+        if self.server_side_encryption is not None:
+            if self.server_side_encryption.mode == EncryptionMode.SSE_B2:
+                headers['X-Bz-Server-Side-Encryption'] = self.server_side_encryption.algorithm.value
+            elif self.server_side_encryption.mode == EncryptionMode.SSE_C:
+                headers['X-Bz-Server-Side-Encryption-Customer-Algorithm'
+                       ] = self.server_side_encryption.algorithm.value
+                headers['X-Bz-Server-Side-Encryption-Customer-Key-Md5'
+                       ] = self.server_side_encryption.key.key_md5()
+            elif self.server_side_encryption.mode in (EncryptionMode.NONE, EncryptionMode.UNKNOWN):
+                pass
+            else:
+                raise ValueError(f'Unsupported encryption mode: {self.server_side_encryption.mode}')
+
         if range_ is not None:
             headers['Content-Range'] = 'bytes %d-%d/%d' % (
-                range_[0], range_[0] + content_length, len(self.data_bytes)
+                range_[0], range_[0] + content_length - 1, len(self.data_bytes)
             )  # yapf: disable
-        for key, value in self.file_info.items():
-            headers['x-bz-info-' + key] = value
         return headers
 
     def as_upload_result(self, account_auth_token):
         result = dict(
             fileId=self.file_id,
             fileName=self.name,
             accountId=self.account_id,
             bucketId=self.bucket.bucket_id,
             contentLength=len(self.data_bytes) if self.data_bytes is not None else 0,
             contentType=self.content_type,
             contentSha1=self.content_sha1,
             fileInfo=self.file_info,
             action=self.action,
             uploadTimestamp=self.upload_timestamp,
+            replicationStatus=self.replication_status and self.replication_status.value,
         )  # yapf: disable
         if self.server_side_encryption is not None:
             result['serverSideEncryption'
                   ] = self.server_side_encryption.serialize_to_json_for_request()
         result['fileRetention'] = self._file_retention_dict(account_auth_token)
         result['legalHold'] = self._legal_hold_dict(account_auth_token)
         return result
 
     def as_list_files_dict(self, account_auth_token):
         result = dict(
+            accountId=self.account_id,
+            bucketId=self.bucket.bucket_id,
             fileId=self.file_id,
             fileName=self.name,
             contentLength=len(self.data_bytes) if self.data_bytes is not None else 0,
             contentType=self.content_type,
             contentSha1=self.content_sha1,
             fileInfo=self.file_info,
             action=self.action,
             uploadTimestamp=self.upload_timestamp,
+            replicationStatus=self.replication_status and self.replication_status.value,
         )  # yapf: disable
         if self.server_side_encryption is not None:
             result['serverSideEncryption'
                   ] = self.server_side_encryption.serialize_to_json_for_request()
         result['fileRetention'] = self._file_retention_dict(account_auth_token)
         result['legalHold'] = self._legal_hold_dict(account_auth_token)
         return result
@@ -290,25 +336,29 @@
             fileId=self.file_id,
             fileName=self.name,
             accountId=self.account_id,
             bucketId=self.bucket.bucket_id,
             contentType=self.content_type,
             fileInfo=self.file_info,
             uploadTimestamp=self.upload_timestamp,
+            replicationStatus=self.replication_status and self.replication_status.value,
         )  # yapf: disable
         if self.server_side_encryption is not None:
             result['serverSideEncryption'
                   ] = self.server_side_encryption.serialize_to_json_for_request()
         result['fileRetention'] = self._file_retention_dict(account_auth_token)
         result['legalHold'] = self._legal_hold_dict(account_auth_token)
         return result
 
     def _file_retention_dict(self, account_auth_token):
         if not self.is_allowed_to_read_file_retention(account_auth_token):
-            return UNKNOWN_FILE_LOCK_CONFIGURATION
+            return {
+                'isClientAuthorizedToRead': False,
+                'value': None,
+            }
 
         file_lock_configuration = {'isClientAuthorizedToRead': True}
         if self.file_retention is None:
             file_lock_configuration['value'] = {'mode': None}
         else:
             file_lock_configuration['value'] = {'mode': self.file_retention.mode.value}
             if self.file_retention.retain_until is not None:
@@ -366,15 +416,15 @@
         if len(parts) <= max_part_count:
             next_part_number = None
         else:
             next_part_number = parts[max_part_count]['partNumber']
             parts = parts[:max_part_count]
         return dict(parts=parts, nextPartNumber=next_part_number)
 
-    def check_encryption(self, request_encryption: Optional[EncryptionSetting]):
+    def check_encryption(self, request_encryption: EncryptionSetting | None):
         if not self.CHECK_ENCRYPTION:
             return
         file_mode, file_secret = self._get_encryption_mode_and_secret(self.server_side_encryption)
         request_mode, request_secret = self._get_encryption_mode_and_secret(request_encryption)
 
         if file_mode in (None, EncryptionMode.NONE):
             assert request_mode in (None, EncryptionMode.NONE)
@@ -382,29 +432,29 @@
             assert request_mode in (None, EncryptionMode.NONE, EncryptionMode.SSE_B2)
         elif file_mode == EncryptionMode.SSE_C:
             if request_mode != EncryptionMode.SSE_C or file_secret != request_secret:
                 raise SSECKeyError()
         else:
             raise ValueError('Unsupported EncryptionMode: %s' % (file_mode))
 
-    def _get_encryption_mode_and_secret(self, encryption: Optional[EncryptionSetting]):
+    def _get_encryption_mode_and_secret(self, encryption: EncryptionSetting | None):
         if encryption is None:
             return None, None
         mode = encryption.mode
         if encryption.key is None:
             secret = None
         else:
             secret = encryption.key.secret
         return mode, secret
 
 
 FakeRequest = collections.namedtuple('FakeRequest', 'url headers')
 
 
-class FakeResponse(object):
+class FakeResponse:
     def __init__(self, account_auth_token_or_none, file_sim, url, range_=None):
         self.data_bytes = file_sim.data_bytes
         self.headers = file_sim.as_download_headers(account_auth_token_or_none, range_)
         self.url = url
         self.range_ = range_
         if range_ is not None:
             self.data_bytes = self.data_bytes[range_[0]:range_[1] + 1]
@@ -415,47 +465,49 @@
         while start <= len(self.data_bytes):
             time.sleep(rnd.random() * 0.01)
             yield self.data_bytes[start:start + chunk_size]
             start += chunk_size
 
     @property
     def request(self):
-        headers = {}
+        headers = CaseInsensitiveDict()
         if self.range_ is not None:
-            headers['Range'] = '%s-%s' % self.range_
+            headers['Range'] = '{}-{}'.format(*self.range_)
         return FakeRequest(self.url, headers)
 
     def close(self):
         pass
 
 
-class BucketSimulator(object):
+class BucketSimulator:
 
     # File IDs start at 9999 and count down, so they sort in the order
     # returned by list_file_versions. The IDs are strings.
     FIRST_FILE_NUMBER = 9999
 
     FIRST_FILE_ID = str(FIRST_FILE_NUMBER)
 
     FILE_SIMULATOR_CLASS = FileSimulator
     RESPONSE_CLASS = FakeResponse
+    MAX_SIMPLE_COPY_SIZE = 200  # should be same as RawSimulator.MIN_PART_SIZE
 
     def __init__(
         self,
         api,
         account_id,
         bucket_id,
         bucket_name,
         bucket_type,
         bucket_info=None,
         cors_rules=None,
-        lifecycle_rules=None,
+        lifecycle_rules: list[LifecycleRule] | None = None,
         options_set=None,
         default_server_side_encryption=None,
-        is_file_lock_enabled: Optional[bool] = None,
+        is_file_lock_enabled: bool | None = None,
+        replication: ReplicationConfiguration | None = None,
     ):
         assert bucket_type in ['allPrivate', 'allPublic']
         self.api = api
         self.account_id = account_id
         self.bucket_name = bucket_name
         self.bucket_id = bucket_id
         self.bucket_type = bucket_type
@@ -464,22 +516,31 @@
         self.lifecycle_rules = lifecycle_rules or []
         self.options_set = options_set or set()
         self.revision = 1
         self.upload_url_counter = iter(range(200))
         # File IDs count down, so that the most recent will come first when they are sorted.
         self.file_id_counter = iter(range(self.FIRST_FILE_NUMBER, 0, -1))
         self.upload_timestamp_counter = iter(range(5000, 9999))
-        self.file_id_to_file = dict()
-        # It would be nice to use an OrderedDict for this, but 2.6 doesn't have it.
-        self.file_name_and_id_to_file = dict()
+        self.file_id_to_file: dict[str, FileSimulator] = dict()
+        self.file_name_and_id_to_file: dict[tuple[str, str], FileSimulator] = dict()
         if default_server_side_encryption is None:
             default_server_side_encryption = EncryptionSetting(mode=EncryptionMode.NONE)
         self.default_server_side_encryption = default_server_side_encryption
         self.is_file_lock_enabled = is_file_lock_enabled
         self.default_retention = NO_RETENTION_BUCKET_SETTING
+        self.replication = replication
+        if self.replication is not None:
+            assert self.replication.asReplicationSource is None or self.replication.asReplicationSource.rules
+            assert self.replication.asReplicationDestination is None or self.replication.asReplicationDestination.sourceToDestinationKeyMapping
+
+    def get_file(self, file_id, file_name) -> FileSimulator:
+        try:
+            return self.file_name_and_id_to_file[(file_name, file_id)]
+        except KeyError:
+            raise FileNotPresent(file_id_or_name=file_id)
 
     def is_allowed_to_read_bucket_encryption_setting(self, account_auth_token):
         return self._check_capability(account_auth_token, 'readBucketEncryption')
 
     def is_allowed_to_read_bucket_retention(self, account_auth_token):
         return self._check_capability(account_auth_token, 'readBucketRetentions')
 
@@ -500,90 +561,116 @@
         if self.is_allowed_to_read_bucket_encryption_setting(account_auth_token):
             default_sse['isClientAuthorizedToRead'] = True
             default_sse['value'] = {'mode': self.default_server_side_encryption.mode.value}
             if self.default_server_side_encryption.algorithm is not None:
                 default_sse['value']['algorithm'
                                     ] = self.default_server_side_encryption.algorithm.value
         else:
-            default_sse['value'] = {'mode': EncryptionMode.UNKNOWN}
+            default_sse['value'] = {'mode': EncryptionMode.UNKNOWN.value}
 
         if self.is_allowed_to_read_bucket_retention(account_auth_token):
             file_lock_configuration = {
                 'isClientAuthorizedToRead': True,
                 'value': {
                     'defaultRetention': {
                         'mode': self.default_retention.mode.value,
-                        'period': self.default_retention.period,
+                        'period': self.default_retention.period.as_dict() if self.default_retention.period else None,
                     },
                     'isFileLockEnabled': self.is_file_lock_enabled,
                 },
             }  # yapf: disable
         else:
             file_lock_configuration = {'isClientAuthorizedToRead': False, 'value': None}
+
+        replication = self.replication and {
+            'isClientAuthorizedToRead': True,
+            'value': self.replication.as_dict(),
+        }
+
         return dict(
             accountId=self.account_id,
             bucketName=self.bucket_name,
             bucketId=self.bucket_id,
             bucketType=self.bucket_type,
             bucketInfo=self.bucket_info,
             corsRules=self.cors_rules,
             lifecycleRules=self.lifecycle_rules,
             options=self.options_set,
             revision=self.revision,
             defaultServerSideEncryption=default_sse,
             fileLockConfiguration=file_lock_configuration,
+            replicationConfiguration=replication,
         )
 
     def cancel_large_file(self, file_id):
         file_sim = self.file_id_to_file[file_id]
         key = (file_sim.name, file_id)
         del self.file_name_and_id_to_file[key]
         del self.file_id_to_file[file_id]
         return dict(
             accountId=self.account_id,
             bucketId=self.bucket_id,
             fileId=file_id,
             fileName=file_sim.name
         )  # yapf: disable
 
-    def delete_file_version(self, file_id, file_name):
+    def delete_file_version(
+        self, account_auth_token, file_id, file_name, bypass_governance: bool = False
+    ):
         key = (file_name, file_id)
-        file_sim = self.file_name_and_id_to_file[key]
+        file_sim = self.get_file(file_id, file_name)
+        if file_sim.file_retention:
+            if file_sim.file_retention.retain_until and file_sim.file_retention.retain_until > int(
+                time.time()
+            ):
+                if file_sim.file_retention.mode == RetentionMode.COMPLIANCE:
+                    raise AccessDenied()
+                elif file_sim.file_retention.mode == RetentionMode.GOVERNANCE:
+                    if not bypass_governance:
+                        raise AccessDenied()
+                    if not self._check_capability(account_auth_token, 'bypassGovernance'):
+                        raise AccessDenied()
+
         del self.file_name_and_id_to_file[key]
         del self.file_id_to_file[file_id]
         return dict(fileId=file_id, fileName=file_name, uploadTimestamp=file_sim.upload_timestamp)
 
     def download_file_by_id(
         self,
         account_auth_token_or_none,
         file_id,
         url,
         range_=None,
-        encryption: Optional[EncryptionSetting] = None,
+        encryption: EncryptionSetting | None = None,
     ):
         file_sim = self.file_id_to_file[file_id]
         file_sim.check_encryption(encryption)
         return self._download_file_sim(account_auth_token_or_none, file_sim, url, range_=range_)
 
     def download_file_by_name(
         self,
         account_auth_token_or_none,
         file_name,
         url,
         range_=None,
-        encryption: Optional[EncryptionSetting] = None,
+        encryption: EncryptionSetting | None = None,
     ):
         files = self.list_file_names(self.api.current_token, file_name,
                                      1)['files']  # token is not important here
         if len(files) == 0:
             raise FileNotPresent(file_id_or_name=file_name)
+
         file_dict = files[0]
-        if file_dict['fileName'] != file_name or file_dict['action'] != 'upload':
+        if file_dict['fileName'] != file_name:
             raise FileNotPresent(file_id_or_name=file_name)
+
         file_sim = self.file_name_and_id_to_file[(file_name, file_dict['fileId'])]
+        if not file_sim.is_visible():
+            raise FileNotPresent(file_id_or_name=file_name)
+
         file_sim.check_encryption(encryption)
         return self._download_file_sim(account_auth_token_or_none, file_sim, url, range_=range_)
 
     def _download_file_sim(self, account_auth_token_or_none, file_sim, url, range_=None):
         return ResponseContextManager(
             self.RESPONSE_CLASS(
                 account_auth_token_or_none,
@@ -598,15 +685,16 @@
         file_sim.finish(part_sha1_array)
         return file_sim.as_upload_result(account_auth_token)
 
     def get_file_info_by_id(self, account_auth_token, file_id):
         return self.file_id_to_file[file_id].as_upload_result(account_auth_token)
 
     def get_file_info_by_name(self, account_auth_token, file_name):
-        for ((name, id), file) in self.file_name_and_id_to_file.items():
+        # Sorting files by name and ID, so lower ID (newer upload) is returned first.
+        for ((name, id), file) in sorted(self.file_name_and_id_to_file.items()):
             if file_name == name:
                 return file.as_download_headers(account_auth_token_or_none=account_auth_token)
         raise FileNotPresent(file_id_or_name=file_name, bucket_name=self.bucket_name)
 
     def get_upload_url(self, account_auth_token):
         upload_id = next(self.upload_url_counter)
         upload_url = 'https://upload.example.com/%s/%d/%s' % (
@@ -664,28 +752,29 @@
             'fileId': file_id,
             'fileName': file_name,
             'legalHold': legal_hold.to_server(),
         }
 
     def copy_file(
         self,
+        account_auth_token,
         file_id,
         new_file_name,
         bytes_range=None,
         metadata_directive=None,
         content_type=None,
         file_info=None,
         destination_bucket_id=None,
-        destination_server_side_encryption: Optional[EncryptionSetting] = None,
-        source_server_side_encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        destination_server_side_encryption: EncryptionSetting | None = None,
+        source_server_side_encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
     ):
         if metadata_directive is not None:
-            assert metadata_directive in tuple(MetadataDirectiveMode)
+            assert metadata_directive in tuple(MetadataDirectiveMode), metadata_directive
             if metadata_directive is MetadataDirectiveMode.COPY and (
                 content_type is not None or file_info is not None
             ):
                 raise InvalidMetadataDirective(
                     'content_type and file_info should be None when metadata_directive is COPY'
                 )
             elif metadata_directive is MetadataDirectiveMode.REPLACE and content_type is None:
@@ -694,38 +783,72 @@
                 )
 
         file_sim = self.file_id_to_file[file_id]
         file_sim.check_encryption(source_server_side_encryption)
         new_file_id = self._next_file_id()
 
         data_bytes = get_bytes_range(file_sim.data_bytes, bytes_range)
+        if len(data_bytes) > self.MAX_SIMPLE_COPY_SIZE:
+            raise CopySourceTooBig(
+                'Copy source too big: %i' % (len(data_bytes),),
+                'bad_request',
+                len(data_bytes),
+            )
 
         destination_bucket = self.api.bucket_id_to_bucket.get(destination_bucket_id, self)
         sse = destination_server_side_encryption or self.default_server_side_encryption
         copy_file_sim = self.FILE_SIMULATOR_CLASS(
             self.account_id,
             destination_bucket,
             new_file_id,
-            'copy',
+            'upload',
             new_file_name,
             file_sim.content_type,
-            file_sim.content_sha1,
+            hex_sha1_of_bytes(data_bytes),  # we hash here again because bytes_range may not cover the full source
             file_sim.file_info,
             data_bytes,
             next(self.upload_timestamp_counter),
             server_side_encryption=sse,
             file_retention=file_retention,
             legal_hold=legal_hold,
-        )
+        )  # yapf: disable
+        destination_bucket.file_id_to_file[copy_file_sim.file_id] = copy_file_sim
+        destination_bucket.file_name_and_id_to_file[copy_file_sim.sort_key()] = copy_file_sim
 
         if metadata_directive is MetadataDirectiveMode.REPLACE:
             copy_file_sim.content_type = content_type
             copy_file_sim.file_info = file_info or file_sim.file_info
 
-        return copy_file_sim
+        ## long term storage of that file has action="upload", but here we need to return action="copy", just this once
+        #class TestFileVersionFactory(FileVersionFactory):
+        #    FILE_VERSION_CLASS = self.FILE_SIMULATOR_CLASS
+
+        #file_version_dict = copy_file_sim.as_upload_result(account_auth_token)
+        #del file_version_dict['action']
+        #print(file_version_dict)
+        #copy_file_sim_with_action_copy = TestFileVersionFactory(self.api).from_api_response(file_version_dict, force_action='copy')
+        #return copy_file_sim_with_action_copy
+
+        # TODO: the code above cannot be used right now because FileSimulator.__init__ is incompatible with FileVersionFactory / FileVersion.__init__ - refactor is needed
+        # for now we'll just return the newly constructed object with a copy action...
+        return self.FILE_SIMULATOR_CLASS(
+            self.account_id,
+            destination_bucket,
+            new_file_id,
+            'copy',
+            new_file_name,
+            copy_file_sim.content_type,
+            copy_file_sim.content_sha1,
+            copy_file_sim.file_info,
+            data_bytes,
+            copy_file_sim.upload_timestamp,
+            server_side_encryption=sse,
+            file_retention=file_retention,
+            legal_hold=legal_hold,
+        )
 
     def list_file_names(
         self,
         account_auth_token,
         start_file_name=None,
         max_file_count=None,
         prefix=None,
@@ -746,14 +869,16 @@
                 prev_file_name = file_name
                 file_sim = self.file_name_and_id_to_file[key]
                 if file_sim.is_visible():
                     result_files.append(file_sim.as_list_files_dict(account_auth_token))
                     if len(result_files) == max_file_count:
                         next_file_name = file_sim.name + ' '
                         break
+                else:
+                    logger.debug('skipping invisible file during listing: %s', key)
         return dict(files=result_files, nextFileName=next_file_name)
 
     def list_file_versions(
         self,
         account_auth_token,
         start_file_name=None,
         start_file_id=None,
@@ -813,101 +938,131 @@
 
     def start_large_file(
         self,
         account_auth_token,
         file_name,
         content_type,
         file_info,
-        server_side_encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        server_side_encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
     ):
         file_id = self._next_file_id()
         sse = server_side_encryption or self.default_server_side_encryption
         if sse:  # FIXME: remove this part when RawApi<->Encryption adapters are implemented properly
             file_info = sse.add_key_id_to_file_info(file_info)
+
+        upload_timestamp = next(self.upload_timestamp_counter)
+        if custom_upload_timestamp is not None:
+            upload_timestamp = custom_upload_timestamp
+
         file_sim = self.FILE_SIMULATOR_CLASS(
             self.account_id, self, file_id, 'start', file_name, content_type, 'none',
-            file_info, None, next(self.upload_timestamp_counter), server_side_encryption=sse,
+            file_info, None, upload_timestamp, server_side_encryption=sse,
             file_retention=file_retention, legal_hold=legal_hold,
         )  # yapf: disable
         self.file_id_to_file[file_id] = file_sim
         self.file_name_and_id_to_file[file_sim.sort_key()] = file_sim
         return file_sim.as_start_large_file_result(account_auth_token)
 
     def _update_bucket(
         self,
         bucket_type=None,
         bucket_info=None,
         cors_rules=None,
-        lifecycle_rules=None,
-        if_revision_is: Optional[int] = None,
-        default_server_side_encryption: Optional[EncryptionSetting] = None,
-        default_retention: Optional[BucketRetentionSetting] = None,
+        lifecycle_rules: list[LifecycleRule] | None = None,
+        if_revision_is: int | None = None,
+        default_server_side_encryption: EncryptionSetting | None = None,
+        default_retention: BucketRetentionSetting | None = None,
+        replication: ReplicationConfiguration | None = None,
+        is_file_lock_enabled: bool | None = None,
     ):
         if if_revision_is is not None and self.revision != if_revision_is:
             raise Conflict()
 
+        if is_file_lock_enabled is not None:
+            if self.is_file_lock_enabled and not is_file_lock_enabled:
+                raise DisablingFileLockNotSupported()
+
+            if (
+                not self.is_file_lock_enabled and is_file_lock_enabled and self.replication and
+                self.replication.is_source
+            ):
+                raise SourceReplicationConflict()
+
+            self.is_file_lock_enabled = is_file_lock_enabled
+
         if bucket_type is not None:
             self.bucket_type = bucket_type
         if bucket_info is not None:
             self.bucket_info = bucket_info
         if cors_rules is not None:
             self.cors_rules = cors_rules
         if lifecycle_rules is not None:
             self.lifecycle_rules = lifecycle_rules
         if default_server_side_encryption is not None:
             self.default_server_side_encryption = default_server_side_encryption
         if default_retention:
             self.default_retention = default_retention
+        if replication is not None:
+            self.replication = replication
+
         self.revision += 1
         return self.bucket_dict(self.api.current_token)
 
     def upload_file(
         self,
-        upload_id,
-        upload_auth_token,
-        file_name,
-        content_length,
-        content_type,
-        content_sha1,
-        file_infos,
+        upload_id: str,
+        upload_auth_token: str,
+        file_name: str,
+        content_length: int,
+        content_type: str,
+        content_sha1: str,
+        file_info: dict,
         data_stream,
-        server_side_encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        server_side_encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
     ):
         data_bytes = self._simulate_chunked_post(data_stream, content_length)
         assert len(data_bytes) == content_length
         if content_sha1 == HEX_DIGITS_AT_END:
             content_sha1 = data_bytes[-40:].decode()
             data_bytes = data_bytes[0:-40]
             content_length -= 40
         elif len(content_sha1) != 40:
             raise ValueError(content_sha1)
         computed_sha1 = hex_sha1_of_bytes(data_bytes)
         if content_sha1 != computed_sha1:
             raise FileSha1Mismatch(file_name)
+        if content_sha1 == 'do_not_verify':
+            content_sha1 = UNVERIFIED_CHECKSUM_PREFIX + computed_sha1
         file_id = self._next_file_id()
 
         encryption = server_side_encryption or self.default_server_side_encryption
         if encryption:  # FIXME: remove this part when RawApi<->Encryption adapters are implemented properly
-            file_infos = encryption.add_key_id_to_file_info(file_infos)
+            file_info = encryption.add_key_id_to_file_info(file_info)
+
+        upload_timestamp = next(self.upload_timestamp_counter)
+        if custom_upload_timestamp is not None:
+            upload_timestamp = custom_upload_timestamp
 
         file_sim = self.FILE_SIMULATOR_CLASS(
             self.account_id,
             self,
             file_id,
             'upload',
             file_name,
             content_type,
             content_sha1,
-            file_infos,
+            file_info,
             data_bytes,
-            next(self.upload_timestamp_counter),
+            upload_timestamp,
             server_side_encryption=encryption,
             file_retention=file_retention,
             legal_hold=legal_hold,
         )
         self.file_id_to_file[file_id] = file_sim
         self.file_name_and_id_to_file[file_sim.sort_key()] = file_sim
         return file_sim.as_upload_result(upload_auth_token)
@@ -915,28 +1070,30 @@
     def upload_part(
         self,
         file_id,
         part_number,
         content_length,
         sha1_sum,
         input_stream,
-        server_side_encryption: Optional[EncryptionSetting] = None,
+        server_side_encryption: EncryptionSetting | None = None,
     ):
-        file_sim = self.file_id_to_file[file_id]
         part_data = self._simulate_chunked_post(input_stream, content_length)
         assert len(part_data) == content_length
         if sha1_sum == HEX_DIGITS_AT_END:
             sha1_sum = part_data[-40:].decode()
             part_data = part_data[0:-40]
             content_length -= 40
         computed_sha1 = hex_sha1_of_bytes(part_data)
         if sha1_sum != computed_sha1:
             raise PartSha1Mismatch(file_id)
+
+        file_sim = self.file_id_to_file[file_id]
         part = PartSimulator(file_sim.file_id, part_number, content_length, sha1_sum, part_data)
         file_sim.add_part(part_number, part)
+
         result = dict(
             fileId=file_id,
             partNumber=part_number,
             contentLength=content_length,
             contentSha1=sha1_sum,
         )  # yapf: disable
         if server_side_encryption is not None:
@@ -974,43 +1131,44 @@
 
     def _next_file_id(self):
         return str(next(self.file_id_counter))
 
 
 class RawSimulator(AbstractRawApi):
     """
-    Implement the same interface as B2RawApi by simulating all of the
+    Implement the same interface as B2RawHTTPApi by simulating all of the
     calls and keeping state in memory.
 
     The intended use for this class is for unit tests that test things
-    built on top of B2RawApi.
+    built on top of B2RawHTTPApi.
     """
 
     BUCKET_SIMULATOR_CLASS = BucketSimulator
     API_URL = 'http://api.example.com'
     S3_API_URL = 'http://s3.api.example.com'
     DOWNLOAD_URL = 'http://download.example.com'
 
     MIN_PART_SIZE = 200
+    MAX_PART_ID = 10000
 
     # This is the maximum duration in seconds that an application key can be valid (1000 days).
     MAX_DURATION_IN_SECONDS = 86400000
 
     UPLOAD_PART_MATCHER = re.compile('https://upload.example.com/part/([^/]*)')
     UPLOAD_URL_MATCHER = re.compile(r'https://upload.example.com/([^/]*)/([^/]*)')
     DOWNLOAD_URL_MATCHER = re.compile(
         DOWNLOAD_URL + '(?:' + '|'.join(
             (
-                '/b2api/v[0-9]+/b2_download_file_by_id\?fileId=(?P<file_id>[^/]+)',
+                r'/b2api/v[0-9]+/b2_download_file_by_id\?fileId=(?P<file_id>[^/]+)',
                 '/file/(?P<bucket_name>[^/]+)/(?P<file_name>.+)',
             )
         ) + ')$'
     )  # yapf: disable
 
-    def __init__(self):
+    def __init__(self, b2_http=None):
         # Map from application_key_id to KeySimulator.
         # The entry for the master application key ID is for the master application
         # key for the account, and the entries with non-master application keys
         # are for keys created b2 createKey().
         self.key_id_to_key = dict()
 
         # Map from auth token to the KeySimulator for it.
@@ -1025,18 +1183,18 @@
 
         # Counter for generating auth tokens.
         self.auth_token_counter = 0
 
         # Counter for generating account IDs an their matching master application keys.
         self.account_counter = 0
 
-        self.bucket_name_to_bucket = dict()
-        self.bucket_id_to_bucket = dict()
+        self.bucket_name_to_bucket: dict[str, BucketSimulator] = dict()
+        self.bucket_id_to_bucket: dict[str, BucketSimulator] = dict()
         self.bucket_id_counter = iter(range(100))
-        self.file_id_to_bucket_id = {}
+        self.file_id_to_bucket_id: dict[str, str] = {}
         self.all_application_keys = []
         self.app_key_counter = 0
         self.upload_errors = []
 
     def expire_auth_token(self, auth_token):
         """
         Simulate the auth token expiring.
@@ -1119,17 +1277,18 @@
         api_url,
         account_auth_token,
         account_id,
         bucket_name,
         bucket_type,
         bucket_info=None,
         cors_rules=None,
-        lifecycle_rules=None,
-        default_server_side_encryption: Optional[EncryptionSetting] = None,
-        is_file_lock_enabled: Optional[bool] = None,
+        lifecycle_rules: list[LifecycleRule] | None = None,
+        default_server_side_encryption: EncryptionSetting | None = None,
+        is_file_lock_enabled: bool | None = None,
+        replication: ReplicationConfiguration | None = None,
     ):
         if not re.match(r'^[-a-zA-Z0-9]*$', bucket_name):
             raise BadJson('illegal bucket name: ' + bucket_name)
         self._assert_account_auth(api_url, account_auth_token, account_id, 'writeBuckets')
         if bucket_name in self.bucket_name_to_bucket:
             raise DuplicateBucketName(bucket_name)
         bucket_id = 'bucket_' + str(next(self.bucket_id_counter))
@@ -1141,14 +1300,15 @@
             bucket_type,
             bucket_info,
             cors_rules,
             lifecycle_rules,
             # watch out for options!
             default_server_side_encryption=default_server_side_encryption,
             is_file_lock_enabled=is_file_lock_enabled,
+            replication=replication,
         )
         self.bucket_name_to_bucket[bucket_name] = bucket
         self.bucket_id_to_bucket[bucket_id] = bucket
         return bucket.bucket_dict(account_auth_token)  # TODO it should be an object, right?
 
     def create_key(
         self,
@@ -1175,18 +1335,21 @@
         else:
             expiration_timestamp_or_none = int(time.time() + valid_duration_seconds)
 
         index = self.app_key_counter
         self.app_key_counter += 1
         application_key_id = 'appKeyId%d' % (index,)
         app_key = 'appKey%d' % (index,)
-        if bucket_id is None:
-            bucket_name_or_none = None
-        else:
-            bucket_name_or_none = self._get_bucket_by_id(bucket_id).bucket_name
+        bucket_name_or_none = None
+        if bucket_id is not None:
+            # It is possible for bucketId to be filled and bucketName to be empty.
+            # It can happen when the bucket was deleted.
+            with suppress(NonExistentBucket):
+                bucket_name_or_none = self._get_bucket_by_id(bucket_id).bucket_name
+
         key_sim = KeySimulator(
             account_id=account_id,
             name=key_name,
             application_key_id=application_key_id,
             key=app_key,
             capabilities=capabilities,
             expiration_timestamp_or_none=expiration_timestamp_or_none,
@@ -1194,19 +1357,23 @@
             bucket_name_or_none=bucket_name_or_none,
             name_prefix_or_none=name_prefix,
         )
         self.key_id_to_key[application_key_id] = key_sim
         self.all_application_keys.append(key_sim)
         return key_sim.as_created_key()
 
-    def delete_file_version(self, api_url, account_auth_token, file_id, file_name):
-        bucket_id = self.file_id_to_bucket_id[file_id]
+    def delete_file_version(
+        self, api_url, account_auth_token, file_id, file_name, bypass_governance: bool = False
+    ):
+        bucket_id = self.file_id_to_bucket_id.get(file_id)
+        if not bucket_id:
+            raise FileNotPresent(file_id_or_name=file_id)
         bucket = self._get_bucket_by_id(bucket_id)
         self._assert_account_auth(api_url, account_auth_token, bucket.account_id, 'deleteFiles')
-        return bucket.delete_file_version(file_id, file_name)
+        return bucket.delete_file_version(account_auth_token, file_id, file_name, bypass_governance)
 
     def update_file_retention(
         self,
         api_url,
         account_auth_token,
         file_id,
         file_name,
@@ -1248,15 +1415,15 @@
         return bucket.bucket_dict(account_auth_token)
 
     def download_file_from_url(
         self,
         account_auth_token_or_none,
         url,
         range_=None,
-        encryption: Optional[EncryptionSetting] = None
+        encryption: EncryptionSetting | None = None
     ):
         # TODO: check auth token if bucket is not public
         matcher = self.DOWNLOAD_URL_MATCHER.match(url)
         assert matcher is not None, url
         groupdict = matcher.groupdict()
         file_id = groupdict['file_id']
         bucket_name = groupdict['bucket_name']
@@ -1281,20 +1448,24 @@
                 encryption=encryption,
             )
         else:
             assert False
 
     def delete_key(self, api_url, account_auth_token, application_key_id):
         assert api_url == self.API_URL
-        return dict(
-            accountId='accountId',
-            applicationKeyId=application_key_id,
-            keyName='keyName',
-            capabilities=['listBuckets', 'readBuckets', 'writeBuckets']
-        )
+        key_sim = self.key_id_to_key.pop(application_key_id, None)
+        if key_sim is None:
+            raise BadRequest(
+                f'application key does not exist: {application_key_id}',
+                'bad_request',
+            )
+        self.all_application_keys = [
+            key for key in self.all_application_keys if key.application_key_id != application_key_id
+        ]
+        return key_sim.as_key()
 
     def finish_large_file(self, api_url, account_auth_token, file_id, part_sha1_array):
         bucket_id = self.file_id_to_bucket_id[file_id]
         bucket = self._get_bucket_by_id(bucket_id)
         self._assert_account_auth(api_url, account_auth_token, bucket.account_id, 'writeFiles')
         return bucket.finish_large_file(account_auth_token, file_id, part_sha1_array)
 
@@ -1353,56 +1524,55 @@
         bytes_range=None,
         metadata_directive=None,
         content_type=None,
         file_info=None,
         destination_bucket_id=None,
         destination_server_side_encryption=None,
         source_server_side_encryption=None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
     ):
         bucket_id = self.file_id_to_bucket_id[source_file_id]
         bucket = self._get_bucket_by_id(bucket_id)
         self._assert_account_auth(api_url, account_auth_token, bucket.account_id, 'writeFiles')
+
+        if destination_bucket_id:
+            # TODO: Handle and raise proper exception after server docs get updated
+            dest_bucket = self.bucket_id_to_bucket[destination_bucket_id]
+            assert dest_bucket.account_id == bucket.account_id
+        else:
+            dest_bucket = bucket
+
         copy_file_sim = bucket.copy_file(
+            account_auth_token,
             source_file_id,
             new_file_name,
             bytes_range,
             metadata_directive,
             content_type,
             file_info,
             destination_bucket_id,
             destination_server_side_encryption=destination_server_side_encryption,
             source_server_side_encryption=source_server_side_encryption,
             file_retention=file_retention,
             legal_hold=legal_hold,
         )
 
-        if destination_bucket_id:
-            # TODO: Handle and raise proper exception after server docs get updated
-            dest_bucket = self.bucket_id_to_bucket[destination_bucket_id]
-            assert dest_bucket.account_id == bucket.account_id
-        else:
-            dest_bucket = bucket
-
-        dest_bucket.file_id_to_file[copy_file_sim.file_id] = copy_file_sim
-        dest_bucket.file_name_and_id_to_file[copy_file_sim.sort_key()] = copy_file_sim
-
         return copy_file_sim.as_upload_result(account_auth_token)
 
     def copy_part(
         self,
         api_url,
         account_auth_token,
         source_file_id,
         large_file_id,
         part_number,
         bytes_range=None,
-        destination_server_side_encryption: Optional[EncryptionSetting] = None,
-        source_server_side_encryption: Optional[EncryptionSetting] = None,
+        destination_server_side_encryption: EncryptionSetting | None = None,
+        source_server_side_encryption: EncryptionSetting | None = None,
     ):
         if destination_server_side_encryption is not None and destination_server_side_encryption.mode == EncryptionMode.SSE_B2:
             raise ValueError(
                 'unsupported sse mode for copy_part!'
             )  # SSE-B2 is only to be marked in b2_start_large_file
         src_bucket_id = self.file_id_to_bucket_id[source_file_id]
         src_bucket = self._get_bucket_by_id(src_bucket_id)
@@ -1513,16 +1683,34 @@
         api_url,
         account_auth_token,
         account_id,
         max_key_count=1000,
         start_application_key_id=None
     ):
         self._assert_account_auth(api_url, account_auth_token, account_id, 'listKeys')
-        keys = map(lambda key: key.as_key(), self.all_application_keys)
-        return dict(keys=keys, nextKeyId=None)
+        next_application_key_id = None
+        all_keys_sorted = sorted(self.all_application_keys, key=lambda key: key.application_key_id)
+        if start_application_key_id is None:
+            keys = all_keys_sorted[:max_key_count]
+            if max_key_count < len(all_keys_sorted):
+                next_application_key_id = all_keys_sorted[max_key_count].application_key_id
+        else:
+            keys = []
+            got_already = 0
+            for ind, key in enumerate(all_keys_sorted):
+                if key.application_key_id >= start_application_key_id:
+                    keys.append(key)
+                    got_already += 1
+                    if got_already == max_key_count:
+                        if ind < len(all_keys_sorted) - 1:
+                            next_application_key_id = all_keys_sorted[ind + 1].application_key_id
+                        break
+
+        key_dicts = map(lambda key: key.as_key(), keys)
+        return dict(keys=list(key_dicts), nextApplicationKeyId=next_application_key_id)
 
     def list_parts(self, api_url, account_auth_token, file_id, start_part_number, max_part_count):
         bucket_id = self.file_id_to_bucket_id[file_id]
         bucket = self._get_bucket_by_id(bucket_id)
         self._assert_account_auth(api_url, account_auth_token, bucket.account_id, 'writeFiles')
         return bucket.list_parts(file_id, start_part_number, max_part_count)
 
@@ -1549,73 +1737,114 @@
         self,
         api_url,
         account_auth_token,
         bucket_id,
         file_name,
         content_type,
         file_info,
-        server_side_encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        server_side_encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
     ):
         bucket = self._get_bucket_by_id(bucket_id)
         self._assert_account_auth(api_url, account_auth_token, bucket.account_id, 'writeFiles')
         result = bucket.start_large_file(
             account_auth_token,
             file_name,
             content_type,
             file_info,
             server_side_encryption,
             file_retention,
             legal_hold,
+            custom_upload_timestamp=custom_upload_timestamp,
         )
         self.file_id_to_bucket_id[result['fileId']] = bucket_id
 
         return result
 
     def update_bucket(
         self,
         api_url,
         account_auth_token,
         account_id,
         bucket_id,
         bucket_type=None,
         bucket_info=None,
         cors_rules=None,
-        lifecycle_rules=None,
+        lifecycle_rules: list[LifecycleRule] | None = None,
         if_revision_is=None,
-        default_server_side_encryption: Optional[EncryptionSetting] = None,
-        default_retention: Optional[BucketRetentionSetting] = None,
+        default_server_side_encryption: EncryptionSetting | None = None,
+        default_retention: BucketRetentionSetting | None = None,
+        replication: ReplicationConfiguration | None = None,
+        is_file_lock_enabled: bool | None = None,
     ):
-        assert bucket_type or bucket_info or cors_rules or lifecycle_rules or default_server_side_encryption
+        assert bucket_type or bucket_info or cors_rules or lifecycle_rules or default_server_side_encryption or replication or is_file_lock_enabled is not None
         bucket = self._get_bucket_by_id(bucket_id)
         self._assert_account_auth(api_url, account_auth_token, bucket.account_id, 'writeBuckets')
         return bucket._update_bucket(
             bucket_type=bucket_type,
             bucket_info=bucket_info,
             cors_rules=cors_rules,
             lifecycle_rules=lifecycle_rules,
             if_revision_is=if_revision_is,
             default_server_side_encryption=default_server_side_encryption,
             default_retention=default_retention,
+            replication=replication,
+            is_file_lock_enabled=is_file_lock_enabled,
+        )
+
+    @classmethod
+    def get_upload_file_headers(
+        cls,
+        upload_auth_token: str,
+        file_name: str,
+        content_length: int,
+        content_type: str,
+        content_sha1: str,
+        file_info: dict,
+        server_side_encryption: EncryptionSetting | None,
+        file_retention: FileRetentionSetting | None,
+        legal_hold: LegalHold | None,
+        custom_upload_timestamp: int | None = None,
+    ) -> dict:
+
+        # fix to allow calculating headers on unknown key - only for simulation
+        if server_side_encryption is not None \
+           and server_side_encryption.mode == EncryptionMode.SSE_C \
+           and server_side_encryption.key.secret is None:
+            server_side_encryption.key.secret = b'secret'
+
+        return super().get_upload_file_headers(
+            upload_auth_token=upload_auth_token,
+            file_name=file_name,
+            content_length=content_length,
+            content_type=content_type,
+            content_sha1=content_sha1,
+            file_info=file_info,
+            server_side_encryption=server_side_encryption,
+            file_retention=file_retention,
+            legal_hold=legal_hold,
+            custom_upload_timestamp=custom_upload_timestamp,
         )
 
     def upload_file(
         self,
-        upload_url,
-        upload_auth_token,
-        file_name,
-        content_length,
-        content_type,
-        content_sha1,
-        file_infos,
+        upload_url: str,
+        upload_auth_token: str,
+        file_name: str,
+        content_length: int,
+        content_type: str,
+        content_sha1: str,
+        file_info: dict,
         data_stream,
-        server_side_encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        server_side_encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
     ):
         with ConcurrentUsedAuthTokenGuard(
             self.currently_used_auth_tokens[upload_auth_token], upload_auth_token
         ):
             assert upload_url == upload_auth_token
             url_match = self.UPLOAD_URL_MATCHER.match(upload_url)
             if url_match is None:
@@ -1624,49 +1853,68 @@
                 raise self.upload_errors.pop(0)
             bucket_id, upload_id = url_match.groups()
             bucket = self._get_bucket_by_id(bucket_id)
             if server_side_encryption is not None:
                 assert server_side_encryption.mode in (
                     EncryptionMode.NONE, EncryptionMode.SSE_B2, EncryptionMode.SSE_C
                 )
-                file_infos = server_side_encryption.add_key_id_to_file_info(file_infos)
+                file_info = server_side_encryption.add_key_id_to_file_info(file_info)
+
+            # we don't really need headers further on
+            # but we still simulate their calculation
+            _ = self.get_upload_file_headers(
+                upload_auth_token=upload_auth_token,
+                file_name=file_name,
+                content_length=content_length,
+                content_type=content_type,
+                content_sha1=content_sha1,
+                file_info=file_info,
+                server_side_encryption=server_side_encryption,
+                file_retention=file_retention,
+                legal_hold=legal_hold,
+                custom_upload_timestamp=custom_upload_timestamp,
+            )
+
             response = bucket.upload_file(
                 upload_id,
                 upload_auth_token,
                 file_name,
                 content_length,
                 content_type,
                 content_sha1,
-                file_infos,
+                file_info,
                 data_stream,
                 server_side_encryption,
                 file_retention,
                 legal_hold,
+                custom_upload_timestamp,
             )
             file_id = response['fileId']
             self.file_id_to_bucket_id[file_id] = bucket_id
 
         return response
 
     def upload_part(
         self,
         upload_url,
         upload_auth_token,
         part_number,
         content_length,
         sha1_sum,
         input_stream,
-        server_side_encryption: Optional[EncryptionSetting] = None,
+        server_side_encryption: EncryptionSetting | None = None,
     ):
         with ConcurrentUsedAuthTokenGuard(
             self.currently_used_auth_tokens[upload_auth_token], upload_auth_token
         ):
             url_match = self.UPLOAD_PART_MATCHER.match(upload_url)
             if url_match is None:
                 raise BadUploadUrl(upload_url)
+            elif part_number > self.MAX_PART_ID:
+                raise BadRequest('Part number must be in range 1 - 10000', 'bad_request')
             file_id = url_match.group(1)
             bucket_id = self.file_id_to_bucket_id[file_id]
             bucket = self._get_bucket_by_id(bucket_id)
             part = bucket.upload_part(
                 file_id, part_number, content_length, sha1_sum, input_stream, server_side_encryption
             )
         return part
@@ -1684,15 +1932,15 @@
             raise Unauthorized('', 'unauthorized')
         if key_sim.bucket_id_or_none is not None and key_sim.bucket_id_or_none != bucket_id:
             raise Unauthorized('', 'unauthorized')
         if key_sim.name_prefix_or_none is not None:
             if file_name is not None and not file_name.startswith(key_sim.name_prefix_or_none):
                 raise Unauthorized('', 'unauthorized')
 
-    def _get_bucket_by_id(self, bucket_id):
+    def _get_bucket_by_id(self, bucket_id) -> BucketSimulator:
         if bucket_id not in self.bucket_id_to_bucket:
             raise NonExistentBucket(bucket_id)
         return self.bucket_id_to_bucket[bucket_id]
 
     def _get_bucket_by_name(self, bucket_name):
         if bucket_name not in self.bucket_name_to_bucket:
             raise NonExistentBucket(bucket_name)
```

### Comparing `b2sdk-1.9.0/b2sdk/session.py` & `b2sdk-2.0.0/b2sdk/_internal/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,80 @@
 ######################################################################
 #
-# File: b2sdk/session.py
+# File: b2sdk/_internal/session.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from functools import partial
-from enum import Enum, unique
-from typing import Any, Dict, Optional
 import logging
+from enum import Enum, unique
+from functools import partial
+from typing import Any
 
-from b2sdk.account_info.sqlite_account_info import SqliteAccountInfo
-from b2sdk.account_info.exception import MissingAccountData
-from b2sdk.b2http import B2Http
-from b2sdk.cache import AuthInfoCache, DummyCache
-from b2sdk.encryption.setting import EncryptionSetting
-from b2sdk.exception import (InvalidAuthToken, Unauthorized)
-from b2sdk.file_lock import BucketRetentionSetting, FileRetentionSetting, LegalHold
-from b2sdk.raw_api import ALL_CAPABILITIES, B2RawApi, REALM_URLS
+from b2sdk._internal.account_info.abstract import AbstractAccountInfo
+from b2sdk._internal.account_info.exception import MissingAccountData
+from b2sdk._internal.account_info.sqlite_account_info import SqliteAccountInfo
+from b2sdk._internal.api_config import DEFAULT_HTTP_API_CONFIG, B2HttpApiConfig
+from b2sdk._internal.b2http import B2Http
+from b2sdk._internal.cache import AbstractCache, AuthInfoCache, DummyCache
+from b2sdk._internal.encryption.setting import EncryptionSetting
+from b2sdk._internal.exception import InvalidAuthToken, Unauthorized
+from b2sdk._internal.file_lock import BucketRetentionSetting, FileRetentionSetting, LegalHold
+from b2sdk._internal.raw_api import ALL_CAPABILITIES, REALM_URLS, LifecycleRule
+from b2sdk._internal.replication.setting import ReplicationConfiguration
 
 logger = logging.getLogger(__name__)
 
 
 @unique
 class TokenType(Enum):
     API = 'api'
     API_TOKEN_ONLY = 'api_token_only'
     UPLOAD_PART = 'upload_part'
     UPLOAD_SMALL = 'upload_small'
 
 
-class B2Session(object):
+class B2Session:
     """
         A facade that supplies the correct api_url and account_auth_token
         to methods of underlying raw_api and reauthorizes if necessary.
     """
     SQLITE_ACCOUNT_INFO_CLASS = staticmethod(SqliteAccountInfo)
+    B2HTTP_CLASS = staticmethod(B2Http)
 
-    def __init__(self, account_info=None, cache=None, raw_api=None):
+    def __init__(
+        self,
+        account_info: AbstractAccountInfo | None = None,
+        cache: AbstractCache | None = None,
+        api_config: B2HttpApiConfig = DEFAULT_HTTP_API_CONFIG
+    ):
         """
         Initialize Session using given account info.
 
-        :param account_info: an instance of :class:`~b2sdk.v1.UrlPoolAccountInfo`,
+        :param account_info: an instance of :class:`~b2sdk.v2.UrlPoolAccountInfo`,
                       or any custom class derived from
-                      :class:`~b2sdk.v1.AbstractAccountInfo`
+                      :class:`~b2sdk.v2.AbstractAccountInfo`
                       To learn more about Account Info objects, see here
-                      :class:`~b2sdk.v1.SqliteAccountInfo`
+                      :class:`~b2sdk.v2.SqliteAccountInfo`
 
         :param cache: an instance of the one of the following classes:
-                      :class:`~b2sdk.cache.DummyCache`, :class:`~b2sdk.cache.InMemoryCache`,
-                      :class:`~b2sdk.cache.AuthInfoCache`,
-                      or any custom class derived from :class:`~b2sdk.cache.AbstractCache`
+                      :class:`~b2sdk._internal.cache.DummyCache`, :class:`~b2sdk._internal.cache.InMemoryCache`,
+                      :class:`~b2sdk._internal.cache.AuthInfoCache`,
+                      or any custom class derived from :class:`~b2sdk._internal.cache.AbstractCache`
                       It is used by B2Api to cache the mapping between bucket name and bucket ids.
-                      default is :class:`~b2sdk.cache.DummyCache`
+                      default is :class:`~b2sdk._internal.cache.DummyCache`
 
-        :param raw_api: an instance of one of the following classes:
-                        :class:`~b2sdk.raw_api.B2RawApi`, :class:`~b2sdk.raw_simulator.RawSimulator`,
-                        or any custom class derived from :class:`~b2sdk.raw_api.AbstractRawApi`
-                        It makes network-less unit testing simple by using :class:`~b2sdk.raw_simulator.RawSimulator`,
-                        in tests and :class:`~b2sdk.raw_api.B2RawApi` in production.
-                        default is :class:`~b2sdk.raw_api.B2RawApi`
+        :param api_config
         """
 
-        self.raw_api = raw_api or B2RawApi(B2Http())
+        self.raw_api = api_config.raw_api_class(self.B2HTTP_CLASS(api_config))
         if account_info is None:
             account_info = self.SQLITE_ACCOUNT_INFO_CLASS()
             if cache is None:
                 cache = AuthInfoCache(account_info)
         if cache is None:
             cache = DummyCache()
 
@@ -123,41 +128,43 @@
             download_url=response['downloadUrl'],
             absolute_minimum_part_size=response['absoluteMinimumPartSize'],
             recommended_part_size=response['recommendedPartSize'],
             application_key=application_key,
             realm=realm,
             s3_api_url=response['s3ApiUrl'],
             allowed=allowed,
-            application_key_id=application_key_id
+            application_key_id=application_key_id,
         )
 
     def cancel_large_file(self, file_id):
         return self._wrap_default_token(self.raw_api.cancel_large_file, file_id)
 
     def create_bucket(
         self,
         account_id,
         bucket_name,
         bucket_type,
         bucket_info=None,
         cors_rules=None,
-        lifecycle_rules=None,
+        lifecycle_rules: list[LifecycleRule] | None = None,
         default_server_side_encryption=None,
-        is_file_lock_enabled: Optional[bool] = None,
+        is_file_lock_enabled: bool | None = None,
+        replication: ReplicationConfiguration | None = None,
     ):
         return self._wrap_default_token(
             self.raw_api.create_bucket,
             account_id,
             bucket_name,
             bucket_type,
             bucket_info=bucket_info,
             cors_rules=cors_rules,
             lifecycle_rules=lifecycle_rules,
             default_server_side_encryption=default_server_side_encryption,
             is_file_lock_enabled=is_file_lock_enabled,
+            replication=replication,
         )
 
     def create_key(
         self, account_id, capabilities, key_name, valid_duration_seconds, bucket_id, name_prefix
     ):
         return self._wrap_default_token(
             self.raw_api.create_key,
@@ -171,20 +178,20 @@
 
     def delete_key(self, application_key_id):
         return self._wrap_default_token(self.raw_api.delete_key, application_key_id)
 
     def delete_bucket(self, account_id, bucket_id):
         return self._wrap_default_token(self.raw_api.delete_bucket, account_id, bucket_id)
 
-    def delete_file_version(self, file_id, file_name):
-        return self._wrap_default_token(self.raw_api.delete_file_version, file_id, file_name)
+    def delete_file_version(self, file_id, file_name, bypass_governance: bool = False):
+        return self._wrap_default_token(
+            self.raw_api.delete_file_version, file_id, file_name, bypass_governance
+        )
 
-    def download_file_from_url(
-        self, url, range_=None, encryption: Optional[EncryptionSetting] = None
-    ):
+    def download_file_from_url(self, url, range_=None, encryption: EncryptionSetting | None = None):
         return self._wrap_token(
             self.raw_api.download_file_from_url,
             TokenType.API_TOKEN_ONLY,
             url,
             range_=range_,
             encryption=encryption,
         )
@@ -194,18 +201,18 @@
 
     def get_download_authorization(self, bucket_id, file_name_prefix, valid_duration_in_seconds):
         return self._wrap_default_token(
             self.raw_api.get_download_authorization, bucket_id, file_name_prefix,
             valid_duration_in_seconds
         )
 
-    def get_file_info_by_id(self, file_id: str) -> Dict[str, Any]:
+    def get_file_info_by_id(self, file_id: str) -> dict[str, Any]:
         return self._wrap_default_token(self.raw_api.get_file_info_by_id, file_id)
 
-    def get_file_info_by_name(self, bucket_name: str, file_name: str) -> Dict[str, Any]:
+    def get_file_info_by_name(self, bucket_name: str, file_name: str) -> dict[str, Any]:
         return self._wrap_default_token(self.raw_api.get_file_info_by_name, bucket_name, file_name)
 
     def get_upload_url(self, bucket_id):
         return self._wrap_default_token(self.raw_api.get_upload_url, bucket_id)
 
     def get_upload_part_url(self, file_id):
         return self._wrap_default_token(self.raw_api.get_upload_part_url, file_id)
@@ -283,90 +290,98 @@
 
     def start_large_file(
         self,
         bucket_id,
         file_name,
         content_type,
         file_info,
-        server_side_encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        server_side_encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
     ):
         return self._wrap_default_token(
             self.raw_api.start_large_file,
             bucket_id,
             file_name,
             content_type,
             file_info,
             server_side_encryption,
             file_retention=file_retention,
             legal_hold=legal_hold,
+            custom_upload_timestamp=custom_upload_timestamp,
         )
 
     def update_bucket(
         self,
         account_id,
         bucket_id,
         bucket_type=None,
         bucket_info=None,
         cors_rules=None,
-        lifecycle_rules=None,
+        lifecycle_rules: list[LifecycleRule] | None = None,
         if_revision_is=None,
-        default_server_side_encryption: Optional[EncryptionSetting] = None,
-        default_retention: Optional[BucketRetentionSetting] = None,
+        default_server_side_encryption: EncryptionSetting | None = None,
+        default_retention: BucketRetentionSetting | None = None,
+        replication: ReplicationConfiguration | None = None,
+        is_file_lock_enabled: bool | None = None,
     ):
         return self._wrap_default_token(
             self.raw_api.update_bucket,
             account_id,
             bucket_id,
             bucket_type=bucket_type,
             bucket_info=bucket_info,
             cors_rules=cors_rules,
             lifecycle_rules=lifecycle_rules,
             if_revision_is=if_revision_is,
             default_server_side_encryption=default_server_side_encryption,
             default_retention=default_retention,
+            replication=replication,
+            is_file_lock_enabled=is_file_lock_enabled,
         )
 
     def upload_file(
         self,
         bucket_id,
         file_name,
         content_length,
         content_type,
         content_sha1,
-        file_infos,
+        file_info,
         data_stream,
-        server_side_encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        server_side_encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
     ):
         return self._wrap_token(
             self.raw_api.upload_file,
             TokenType.UPLOAD_SMALL,
             bucket_id,
             file_name,
             content_length,
             content_type,
             content_sha1,
-            file_infos,
+            file_info,
             data_stream,
             server_side_encryption,
             file_retention=file_retention,
             legal_hold=legal_hold,
+            custom_upload_timestamp=custom_upload_timestamp,
         )
 
     def upload_part(
         self,
         file_id,
         part_number,
         content_length,
         sha1_sum,
         input_stream,
-        server_side_encryption: Optional[EncryptionSetting] = None,
+        server_side_encryption: EncryptionSetting | None = None,
     ):
         return self._wrap_token(
             self.raw_api.upload_part,
             TokenType.UPLOAD_PART,
             file_id,
             part_number,
             content_length,
@@ -388,18 +403,18 @@
         source_file_id,
         new_file_name,
         bytes_range=None,
         metadata_directive=None,
         content_type=None,
         file_info=None,
         destination_bucket_id=None,
-        destination_server_side_encryption: Optional[EncryptionSetting] = None,
-        source_server_side_encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        destination_server_side_encryption: EncryptionSetting | None = None,
+        source_server_side_encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
     ):
         return self._wrap_default_token(
             self.raw_api.copy_file,
             source_file_id,
             new_file_name,
             bytes_range=bytes_range,
             metadata_directive=metadata_directive,
@@ -414,16 +429,16 @@
 
     def copy_part(
         self,
         source_file_id,
         large_file_id,
         part_number,
         bytes_range=None,
-        destination_server_side_encryption: Optional[EncryptionSetting] = None,
-        source_server_side_encryption: Optional[EncryptionSetting] = None,
+        destination_server_side_encryption: EncryptionSetting | None = None,
+        source_server_side_encryption: EncryptionSetting | None = None,
     ):
         return self._wrap_default_token(
             self.raw_api.copy_part,
             source_file_id,
             large_file_id,
             part_number,
             bytes_range=bytes_range,
@@ -483,17 +498,15 @@
             key_messages.append("restricted to bucket '" + bucket_name + "'")
         if name_prefix is not None:
             key_messages.append("restricted to files that start with '" + name_prefix + "'")
         if not key_messages:
             key_messages.append('with no restrictions')
 
         # Make a new message
-        new_message = unauthorized.message
-        if new_message == '':
-            new_message = 'unauthorized'
+        new_message = unauthorized.message or 'unauthorized'
         new_message += ' for application key ' + ', '.join(key_messages)
 
         return Unauthorized(new_message, unauthorized.code)
 
     def _get_upload_data(self, bucket_id):
         """
         Take ownership of an upload URL / auth token for the bucket and
```

### Comparing `b2sdk-1.9.0/b2sdk/stream/__init__.py` & `b2sdk-2.0.0/b2sdk/_internal/stream/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 ######################################################################
 #
-# File: b2sdk/stream/__init__.py
+# File: b2sdk/_internal/stream/__init__.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 from .hashing import StreamWithHash
 from .progress import ReadingStreamWithProgress, WritingStreamWithProgress
 from .range import RangeOfInputStream
 
 __all__ = [
     'RangeOfInputStream',
```

### Comparing `b2sdk-1.9.0/b2sdk/stream/chained.py` & `b2sdk-2.0.0/b2sdk/_internal/stream/chained.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 ######################################################################
 #
-# File: b2sdk/stream/chained.py
+# File: b2sdk/_internal/stream/chained.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import io
-
 from abc import ABCMeta, abstractmethod
 
-from b2sdk.stream.base import ReadOnlyStreamMixin
+from b2sdk._internal.stream.base import ReadOnlyStreamMixin
 
 
 class ChainedStream(ReadOnlyStreamMixin, io.IOBase):
     """ Chains multiple streams in single stream, sort of what :py:class:`itertools.chain` does for iterators.
 
     Cleans up buffers of underlying streams when closed.
 
     Can be seeked to beginning (when retrying upload, for example).
     Closes underlying streams as soon as they reaches EOF, but clears their buffers
     when the chained stream is closed for underlying streams that follow
-    :py:class:`b2sdk.v1.StreamOpener` cleanup interface, for example
-    :py:class:`b2sdk.v1.CachedBytesStreamOpener`
+    :py:class:`b2sdk.v2.StreamOpener` cleanup interface, for example
+    :py:class:`b2sdk.v2.CachedBytesStreamOpener`
     """
 
     def __init__(self, stream_openers):
         """
         :param list stream_openeres: list of callables that return opened streams
         """
         stream_openers = list(stream_openers)
         if not stream_openers:
             raise ValueError('chain_links cannot be empty')
         self.stream_openers = stream_openers
         self._stream_openers_iterator = iter(self.stream_openers)
         self._current_stream = None
         self._pos = 0
-        super(ChainedStream, self).__init__()
+        super().__init__()
 
     @property
     def stream(self):
         """ Return currently processed stream. """
         if self._current_stream is None:
             self._next_stream()
         return self._current_stream
@@ -120,25 +120,25 @@
                     self._next_stream()
                     if self.stream is current_stream:
                         break
 
         if not byte_arrays:
             data = byte_arrays[0]
         else:
-            data = bytes().join(byte_arrays)
+            data = b''.join(byte_arrays)
         self._pos += len(data)
         return data
 
     def close(self):
         if self._current_stream is not None:
             self._current_stream.close()
         for stream_opener in self.stream_openers:
             if hasattr(stream_opener, 'cleanup'):
                 stream_opener.cleanup()
-        super(ChainedStream, self).close()
+        super().close()
 
 
 class StreamOpener(metaclass=ABCMeta):
     """ Abstract class to define stream opener with cleanup. """
 
     @abstractmethod
     def __call__(self):
```

### Comparing `b2sdk-1.9.0/b2sdk/stream/hashing.py` & `b2sdk-2.0.0/b2sdk/_internal/stream/hashing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 ######################################################################
 #
-# File: b2sdk/stream/hashing.py
+# File: b2sdk/_internal/stream/hashing.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import hashlib
 import io
 
-from b2sdk.stream.wrapper import StreamWithLengthWrapper
-from b2sdk.stream.base import ReadOnlyStreamMixin
+from b2sdk._internal.stream.base import ReadOnlyStreamMixin
+from b2sdk._internal.stream.wrapper import StreamWithLengthWrapper
 
 
 class StreamWithHash(ReadOnlyStreamMixin, StreamWithLengthWrapper):
     """
     Wrap a file-like object, calculates SHA1 while reading
     and appends hash at the end.
     """
@@ -25,42 +26,42 @@
         """
         :param stream: the stream to read from
         """
         self.digest = self.get_digest()
         total_length = None
         if stream_length is not None:
             total_length = stream_length + self.digest.digest_size * 2
-        super(StreamWithHash, self).__init__(stream, length=total_length)
+        super().__init__(stream, length=total_length)
         self.hash = None
         self.hash_read = 0
 
     def seek(self, pos, whence=0):
         """
         Seek to a given position in the stream.
 
         :param int pos: position in the stream
         """
         if pos != 0 or whence != 0:
             raise io.UnsupportedOperation('Stream with hash can only be seeked to beginning')
         self.digest = self.get_digest()
         self.hash = None
         self.hash_read = 0
-        return super(StreamWithHash, self).seek(0)
+        return super().seek(0)
 
     def read(self, size=None):
         """
         Read data from the stream.
 
         :param int size: number of bytes to read
         :return: read data
         :rtype: bytes|None
         """
         data = b''
         if self.hash is None:
-            data = super(StreamWithHash, self).read(size)
+            data = super().read(size)
             # Update hash
             self.digest.update(data)
 
             # Check for end of stream
             if size is None or len(data) < size:
                 self.hash = self.digest.hexdigest()
                 if size is not None:
```

### Comparing `b2sdk-1.9.0/b2sdk/stream/progress.py` & `b2sdk-2.0.0/b2sdk/_internal/stream/progress.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 ######################################################################
 #
-# File: b2sdk/stream/progress.py
+# File: b2sdk/_internal/stream/progress.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from b2sdk.stream.wrapper import StreamWrapper
+from b2sdk._internal.stream.wrapper import StreamWrapper
 
 
 class AbstractStreamWithProgress(StreamWrapper):
     """
     Wrap a file-like object and updates a ProgressListener
     as data is read / written.
     In the abstract class, read and write methods do not update
     the progress - child classes shall do it.
     """
 
     def __init__(self, stream, progress_listener, offset=0):
         """
 
         :param stream: the stream to read from or write to
-        :param b2sdk.v1.AbstractProgressListener progress_listener: the listener that we tell about progress
+        :param b2sdk.v2.AbstractProgressListener progress_listener: the listener that we tell about progress
         :param int offset: the starting byte offset in the file
         """
-        super(AbstractStreamWithProgress, self).__init__(stream)
+        super().__init__(stream)
         assert progress_listener is not None
         self.progress_listener = progress_listener
         self.bytes_completed = 0
         self.offset = offset
 
     def _progress_update(self, delta):
         self.bytes_completed += delta
         self.progress_listener.bytes_completed(self.bytes_completed + self.offset)
 
+    def __str__(self):
+        return str(self.stream)
+
 
 class ReadingStreamWithProgress(AbstractStreamWithProgress):
     """
     Wrap a file-like object, updates progress while reading.
     """
 
     def __init__(self, *args, **kwargs):
         length = kwargs.pop('length', None)
-        super(ReadingStreamWithProgress, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.length = length
 
     def read(self, size=None):
         """
         Read data from the stream.
 
         :param int size: number of bytes to read
         :return: data read from the stream
         """
-        data = super(ReadingStreamWithProgress, self).read(size)
+        data = super().read(size)
         self._progress_update(len(data))
         return data
 
     def seek(self, pos, whence=0):
-        pos = super(ReadingStreamWithProgress, self).seek(pos, whence=whence)
+        pos = super().seek(pos, whence=whence)
         # reset progress to current stream position - assumption is that ReadingStreamWithProgress would not be used
         # for random access streams, and seek is only used to reset stream to beginning to retry file upload
         # and multipart file upload would open and use different file descriptor for each part;
         # this logic cannot be used for WritingStreamWithProgress because multipart download has to use
         # single file descriptor and synchronize writes so seeking cannot be understood there as progress reset
         # and writing  progress is always monotonic
         self.bytes_completed = pos
@@ -81,8 +85,8 @@
     def write(self, data):
         """
         Write data to the stream.
 
         :param bytes data: data to write to the stream
         """
         self._progress_update(len(data))
-        return super(WritingStreamWithProgress, self).write(data)
+        return super().write(data)
```

### Comparing `b2sdk-1.9.0/b2sdk/stream/range.py` & `b2sdk-2.0.0/b2sdk/_internal/stream/range.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 ######################################################################
 #
-# File: b2sdk/stream/range.py
+# File: b2sdk/_internal/stream/range.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import io
 
-from b2sdk.stream.wrapper import StreamWithLengthWrapper
-from b2sdk.stream.base import ReadOnlyStreamMixin
+from b2sdk._internal.stream.base import ReadOnlyStreamMixin
+from b2sdk._internal.stream.wrapper import StreamWithLengthWrapper
 
 
 class RangeOfInputStream(ReadOnlyStreamMixin, StreamWithLengthWrapper):
     """
     Wrap a file-like object (read only) and read the selected
     range of the file.
     """
 
     def __init__(self, stream, offset, length):
         """
         :param stream: a seekable stream
         :param int offset: offset in the stream
         :param int length: max number of bytes to read
         """
-        super(RangeOfInputStream, self).__init__(stream, length)
+        super().__init__(stream, length)
         self.offset = offset
         self.relative_pos = 0
         self.stream.seek(self.offset)
 
     def seek(self, pos, whence=0):
         """
         Seek to a given position in the stream.
 
         :param int pos: position in the stream relative to steam offset
         :return: new position relative to stream offset
         :rtype: int
         """
         if whence != 0:
             raise io.UnsupportedOperation('only SEEK_SET is supported')
-        abs_pos = super(RangeOfInputStream, self).seek(self.offset + pos)
+        abs_pos = super().seek(self.offset + pos)
         self.relative_pos = abs_pos - self.offset
         return self.tell()
 
     def tell(self):
         """
         Return current stream position relative to offset.
 
@@ -66,12 +67,18 @@
             to_read = remaining
         else:
             to_read = min(size, remaining)
         data = self.stream.read(to_read)
         self.relative_pos += len(data)
         return data
 
+    def close(self):
+        super().close()
+        # TODO: change the use cases of this class to close the file objects passed to it, instead of having
+        # RangeOfInputStream close it's members upon garbage collection
+        self.stream.close()
+
 
 def wrap_with_range(stream, stream_length, range_offset, range_length):
     if range_offset == 0 and range_length == stream_length:
         return stream
     return RangeOfInputStream(stream, range_offset, range_length)
```

### Comparing `b2sdk-1.9.0/b2sdk/stream/wrapper.py` & `b2sdk-2.0.0/b2sdk/_internal/stream/wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 ######################################################################
 #
-# File: b2sdk/stream/wrapper.py
+# File: b2sdk/_internal/stream/wrapper.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import io
 
 
 class StreamWrapper(io.IOBase):
     """
     Wrapper for a file-like object.
     """
 
     def __init__(self, stream):
         """
         :param stream: the stream to read from or write to
         """
         self.stream = stream
-        super(StreamWrapper, self).__init__()
+        super().__init__()
 
     def seekable(self):
         return self.stream.seekable()
 
     def seek(self, pos, whence=0):
         """
         Seek to a given position in the stream.
@@ -75,27 +76,23 @@
         """
         Write data to the stream.
 
         :param data: a data to write to the stream
         """
         return self.stream.write(data)
 
-    def close(self):
-        super(StreamWrapper, self).close()
-        self.stream.close()
-
 
 class StreamWithLengthWrapper(StreamWrapper):
     """
     Wrapper for a file-like object that supports `__len__` interface
     """
 
     def __init__(self, stream, length=None):
         """
         :param stream: the stream to read from or write to
         :param int length: length of the stream
         """
-        super(StreamWithLengthWrapper, self).__init__(stream)
+        super().__init__(stream)
         self.length = length
 
     def __len__(self):
         return self.length
```

### Comparing `b2sdk-1.9.0/b2sdk/sync/action.py` & `b2sdk-2.0.0/b2sdk/_internal/sync/action.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 ######################################################################
 #
-# File: b2sdk/sync/action.py
+# File: b2sdk/_internal/sync/action.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from abc import ABCMeta, abstractmethod
-
+import contextlib
 import logging
 import os
-from ..download_dest import DownloadDestLocalFile
-from .encryption_provider import AbstractSyncEncryptionSettingsProvider
-from ..bucket import Bucket
+from abc import ABCMeta, abstractmethod
+from contextlib import suppress
 
-from ..raw_api import SRC_LAST_MODIFIED_MILLIS
+from ..bucket import Bucket
+from ..file_version import FileVersion
+from ..http_constants import SRC_LAST_MODIFIED_MILLIS
+from ..scan.path import B2Path
+from ..sync.report import ProgressReport, SyncReport
+from ..transfer.outbound.outbound_source import OutboundTransferSource
 from ..transfer.outbound.upload_source import UploadSourceLocalFile
-from .path import B2SyncPath
+from ..utils.escape import escape_control_chars
+from .encryption_provider import AbstractSyncEncryptionSettingsProvider
 from .report import SyncFileReporter
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractAction(metaclass=ABCMeta):
     """
@@ -31,271 +36,317 @@
     are then run by a pool of threads.
 
     An action can depend on other actions completing.  An example of
     this is making sure a CreateBucketAction happens before an
     UploadFileAction.
     """
 
-    def run(self, bucket, reporter, dry_run=False):
+    def run(self, bucket: Bucket, reporter: ProgressReport, dry_run: bool = False):
         """
         Main action routine.
 
         :param bucket: a Bucket object
-        :type bucket: b2sdk.bucket.Bucket
+        :type bucket: b2sdk._internal.bucket.Bucket
         :param reporter: a place to report errors
         :param dry_run: if True, perform a dry run
         :type dry_run: bool
         """
         try:
             if not dry_run:
                 self.do_action(bucket, reporter)
             self.do_report(bucket, reporter)
         except Exception as e:
             logger.exception('an exception occurred in a sync action')
             reporter.error(str(self) + ": " + repr(e) + ' ' + str(e))
             raise  # Re-throw so we can identify failed actions
 
     @abstractmethod
-    def get_bytes(self):
+    def get_bytes(self) -> int:
         """
         Return the number of bytes to transfer for this action.
-
-        :rtype: int
         """
 
     @abstractmethod
-    def do_action(self, bucket, reporter):
+    def do_action(self, bucket: Bucket, reporter: ProgressReport) -> None:
         """
         Perform the action, returning only after the action is completed.
 
         :param bucket: a Bucket object
-        :type bucket: b2sdk.bucket.Bucket
         :param reporter: a place to report errors
         """
 
     @abstractmethod
-    def do_report(self, bucket, reporter):
+    def do_report(self, bucket: Bucket, reporter: ProgressReport) -> None:
         """
         Report the action performed.
 
         :param bucket: a Bucket object
-        :type bucket: b2sdk.bucket.Bucket
         :param reporter: a place to report errors
         """
 
 
 class B2UploadAction(AbstractAction):
     """
     File uploading action.
     """
 
     def __init__(
         self,
-        local_full_path,
-        relative_name,
-        b2_file_name,
-        mod_time_millis,
-        size,
+        local_full_path: str,
+        relative_name: str,
+        b2_file_name: str,
+        mod_time_millis: int,
+        size: int,
         encryption_settings_provider: AbstractSyncEncryptionSettingsProvider,
     ):
         """
-        :param str local_full_path: a local file path
-        :param str relative_name: a relative file name
-        :param str b2_file_name: a name of a new remote file
-        :param int mod_time_millis: file modification time in milliseconds
-        :param int size: a file size
-        :param b2sdk.v1.AbstractSyncEncryptionSettingsProvider encryption_settings_provider: encryption setting provider
+        :param local_full_path: a local file path
+        :param relative_name: a relative file name
+        :param b2_file_name: a name of a new remote file
+        :param mod_time_millis: file modification time in milliseconds
+        :param size: a file size
+        :param encryption_settings_provider: encryption setting provider
         """
         self.local_full_path = local_full_path
         self.relative_name = relative_name
         self.b2_file_name = b2_file_name
         self.mod_time_millis = mod_time_millis
         self.size = size
         self.encryption_settings_provider = encryption_settings_provider
+        self.large_file_sha1 = None
+        # TODO: Remove once we drop Python 3.7 support
+        self.cached_upload_source = None
 
-    def get_bytes(self):
+    def get_bytes(self) -> int:
         """
         Return file size.
-
-        :rtype: int
         """
         return self.size
 
-    def do_action(self, bucket, reporter):
+    @property
+    # TODO: Use @functools.cached_property once we drop Python 3.7 support
+    def _upload_source(self) -> UploadSourceLocalFile:
+        """ Upload source if the file was to be uploaded in full """
+        # NOTE: We're caching this to ensure that sha1 is not recalculated.
+        if self.cached_upload_source is None:
+            self.cached_upload_source = UploadSourceLocalFile(self.local_full_path)
+        return self.cached_upload_source
+
+    def get_all_sources(self) -> list[OutboundTransferSource]:
+        """ Get list of sources required to complete this upload """
+        return [self._upload_source]
+
+    def do_action(self, bucket: Bucket, reporter: ProgressReport) -> None:
         """
         Perform the uploading action, returning only after the action is completed.
 
-        :param b2sdk.v1.Bucket bucket: a Bucket object
+        :param bucket: a Bucket object
         :param reporter: a place to report errors
         """
         if reporter:
             progress_listener = SyncFileReporter(reporter)
         else:
             progress_listener = None
         file_info = {SRC_LAST_MODIFIED_MILLIS: str(self.mod_time_millis)}
         encryption = self.encryption_settings_provider.get_setting_for_upload(
             bucket=bucket,
             b2_file_name=self.b2_file_name,
             file_info=file_info,
             length=self.size,
         )
-        bucket.upload(
-            UploadSourceLocalFile(self.local_full_path),
-            self.b2_file_name,
-            file_info=file_info,
-            progress_listener=progress_listener,
-            encryption=encryption,
-        )
 
-    def do_report(self, bucket, reporter):
+        sources = self.get_all_sources()
+        large_file_sha1 = None
+
+        if len(sources) > 1:
+            # The upload will be incremental, calculate the large_file_sha1
+            large_file_sha1 = self._upload_source.get_content_sha1()
+
+        with contextlib.ExitStack() as exit_stack:
+            if progress_listener:
+                exit_stack.enter_context(progress_listener)
+            bucket.concatenate(
+                sources,
+                self.b2_file_name,
+                progress_listener=progress_listener,
+                file_info=file_info,
+                encryption=encryption,
+                large_file_sha1=large_file_sha1,
+            )
+
+    def do_report(self, bucket: Bucket, reporter: ProgressReport) -> None:
         """
         Report the uploading action performed.
 
         :param bucket: a Bucket object
-        :type bucket: b2sdk.bucket.Bucket
         :param reporter: a place to report errors
         """
-        reporter.print_completion('upload ' + self.relative_name)
+        reporter.print_completion(f'upload {escape_control_chars(self.relative_name)}')
+
+    def __str__(self) -> str:
+        return f'b2_upload({self.local_full_path}, {self.b2_file_name}, {self.mod_time_millis})'
+
+
+class B2IncrementalUploadAction(B2UploadAction):
+    def __init__(
+        self,
+        local_full_path: str,
+        relative_name: str,
+        b2_file_name: str,
+        mod_time_millis: int,
+        size: int,
+        encryption_settings_provider: AbstractSyncEncryptionSettingsProvider,
+        file_version: FileVersion | None = None,
+        absolute_minimum_part_size: int | None = None,
+    ):
+        """
+        :param local_full_path: a local file path
+        :param relative_name: a relative file name
+        :param b2_file_name: a name of a new remote file
+        :param mod_time_millis: file modification time in milliseconds
+        :param size: a file size
+        :param encryption_settings_provider: encryption setting provider
+        :param file_version: version of file currently on the server
+        :param absolute_minimum_part_size: minimum file part size for large files
+        """
+        super().__init__(
+            local_full_path, relative_name, b2_file_name, mod_time_millis, size,
+            encryption_settings_provider
+        )
+        self.file_version = file_version
+        self.absolute_minimum_part_size = absolute_minimum_part_size
 
-    def __str__(self):
-        return 'b2_upload(%s, %s, %s)' % (
-            self.local_full_path, self.b2_file_name, self.mod_time_millis
+    def get_all_sources(self) -> list[OutboundTransferSource]:
+        return self._upload_source.get_incremental_sources(
+            self.file_version, self.absolute_minimum_part_size
         )
 
 
 class B2HideAction(AbstractAction):
-    def __init__(self, relative_name, b2_file_name):
+    def __init__(self, relative_name: str, b2_file_name: str):
         """
         :param relative_name: a relative file name
-        :type relative_name: str
         :param b2_file_name: a name of a remote file
-        :type b2_file_name: str
         """
         self.relative_name = relative_name
         self.b2_file_name = b2_file_name
 
-    def get_bytes(self):
+    def get_bytes(self) -> int:
         """
         Return file size.
 
         :return: always zero
         :rtype: int
         """
         return 0
 
-    def do_action(self, bucket, reporter):
+    def do_action(self, bucket: Bucket, reporter: ProgressReport) -> None:
         """
         Perform the hiding action, returning only after the action is completed.
 
         :param bucket: a Bucket object
-        :type bucket: b2sdk.bucket.Bucket
         :param reporter: a place to report errors
         """
         bucket.hide_file(self.b2_file_name)
 
-    def do_report(self, bucket, reporter):
+    def do_report(self, bucket: Bucket, reporter: SyncReport):
         """
         Report the hiding action performed.
 
         :param bucket: a Bucket object
-        :type bucket: b2sdk.bucket.Bucket
         :param reporter: a place to report errors
         """
         reporter.update_transfer(1, 0)
-        reporter.print_completion('hide   ' + self.relative_name)
+        reporter.print_completion(f'hide   {escape_control_chars(self.relative_name)}')
 
-    def __str__(self):
-        return 'b2_hide(%s)' % (self.b2_file_name,)
+    def __str__(self) -> str:
+        return f'b2_hide({self.b2_file_name})'
 
 
 class B2DownloadAction(AbstractAction):
     def __init__(
         self,
-        source_path: B2SyncPath,
+        source_path: B2Path,
         b2_file_name: str,
         local_full_path: str,
         encryption_settings_provider: AbstractSyncEncryptionSettingsProvider,
     ):
         """
-        :param b2sdk.v1.B2SyncPath source_path: the file to be downloaded
-        :param str b2_file_name: b2_file_name
-        :param str local_full_path: a local file path
-        :param b2sdk.v1.AbstractSyncEncryptionSettingsProvider encryption_settings_provider: encryption setting provider
+        :param source_path: the file to be downloaded
+        :param b2_file_name: b2_file_name
+        :param local_full_path: a local file path
+        :param encryption_settings_provider: encryption setting provider
         """
         self.source_path = source_path
         self.b2_file_name = b2_file_name
         self.local_full_path = local_full_path
         self.encryption_settings_provider = encryption_settings_provider
 
-    def get_bytes(self):
+    def get_bytes(self) -> int:
         """
         Return file size.
-
-        :rtype: int
         """
         return self.source_path.size
 
-    def _ensure_directory_existence(self):
+    def _ensure_directory_existence(self) -> None:
+        # TODO: this can fail to multiple reasons (e.g. path is a file, permissions etc).
+        #   We could provide nice exceptions for it.
         parent_dir = os.path.dirname(self.local_full_path)
         if not os.path.isdir(parent_dir):
-            try:
+            with suppress(OSError):
                 os.makedirs(parent_dir)
-            except OSError:
-                pass
         if not os.path.isdir(parent_dir):
-            raise Exception('could not create directory %s' % (parent_dir,))
+            raise Exception(f'could not create directory {parent_dir}')
 
-    def do_action(self, bucket, reporter):
+    def do_action(self, bucket: Bucket, reporter: ProgressReport) -> None:
         """
         Perform the downloading action, returning only after the action is completed.
 
-        :param b2sdk.v1.Bucket bucket: a Bucket object
+        :param bucket: a Bucket object
         :param reporter: a place to report errors
         """
         self._ensure_directory_existence()
 
         if reporter:
             progress_listener = SyncFileReporter(reporter)
         else:
             progress_listener = None
 
         # Download the file to a .tmp file
         download_path = self.local_full_path + '.b2.sync.tmp'
-        download_dest = DownloadDestLocalFile(download_path)
 
         encryption = self.encryption_settings_provider.get_setting_for_download(
             bucket=bucket,
             file_version=self.source_path.selected_version,
         )
-
-        bucket.download_file_by_id(
-            self.source_path.selected_version.id_,
-            download_dest,
-            progress_listener,
-            encryption=encryption,
-        )
+        with contextlib.ExitStack() as exit_stack:
+            if progress_listener:
+                exit_stack.enter_context(progress_listener)
+            downloaded_file = bucket.download_file_by_id(
+                self.source_path.selected_version.id_,
+                progress_listener=progress_listener,
+                encryption=encryption,
+            )
+            downloaded_file.save_to(download_path)
 
         # Move the file into place
-        try:
+        with suppress(OSError):
             os.unlink(self.local_full_path)
-        except OSError:
-            pass
         os.rename(download_path, self.local_full_path)
 
-    def do_report(self, bucket, reporter):
+    def do_report(self, bucket: Bucket, reporter: ProgressReport) -> None:
         """
         Report the downloading action performed.
 
         :param bucket: a Bucket object
-        :type bucket: b2sdk.bucket.Bucket
         :param reporter: a place to report errors
         """
         reporter.print_completion('dnload ' + self.source_path.relative_path)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return (
             'b2_download(%s, %s, %s, %d)' % (
                 self.b2_file_name, self.source_path.selected_version.id_, self.local_full_path,
                 self.source_path.mod_time
             )
         )
 
@@ -304,49 +355,46 @@
     """
     File copying action.
     """
 
     def __init__(
         self,
         b2_file_name: str,
-        source_path: B2SyncPath,
+        source_path: B2Path,
         dest_b2_file_name,
         source_bucket: Bucket,
         destination_bucket: Bucket,
         encryption_settings_provider: AbstractSyncEncryptionSettingsProvider,
     ):
         """
-        :param str b2_file_name: a b2_file_name
-        :param b2sdk.v1.B2SyncPath source_path: the file to be copied
-        :param str dest_b2_file_name: a name of a destination remote file
-        :param Bucket source_bucket: bucket to copy from
-        :param Bucket destination_bucket: bucket to copy to
-        :param b2sdk.v1.AbstractSyncEncryptionSettingsProvider encryption_settings_provider: encryption setting provider
+        :param b2_file_name: a b2_file_name
+        :param source_path: the file to be copied
+        :param dest_b2_file_name: a name of a destination remote file
+        :param source_bucket: bucket to copy from
+        :param destination_bucket: bucket to copy to
+        :param encryption_settings_provider: encryption setting provider
         """
         self.b2_file_name = b2_file_name
         self.source_path = source_path
         self.dest_b2_file_name = dest_b2_file_name
         self.encryption_settings_provider = encryption_settings_provider
         self.source_bucket = source_bucket
         self.destination_bucket = destination_bucket
 
-    def get_bytes(self):
+    def get_bytes(self) -> int:
         """
         Return file size.
-
-        :rtype: int
         """
         return self.source_path.size
 
-    def do_action(self, bucket, reporter):
+    def do_action(self, bucket: Bucket, reporter: ProgressReport) -> None:
         """
         Perform the copying action, returning only after the action is completed.
 
         :param bucket: a Bucket object
-        :type bucket: b2sdk.bucket.Bucket
         :param reporter: a place to report errors
         """
         if reporter:
             progress_listener = SyncFileReporter(reporter)
         else:
             progress_listener = None
 
@@ -357,128 +405,122 @@
 
         destination_encryption = self.encryption_settings_provider.get_destination_setting_for_copy(
             bucket=self.destination_bucket,
             source_file_version=self.source_path.selected_version,
             dest_b2_file_name=self.dest_b2_file_name,
         )
 
-        bucket.copy(
-            self.source_path.selected_version.id_,
-            self.dest_b2_file_name,
-            length=self.source_path.size,
-            progress_listener=progress_listener,
-            destination_encryption=destination_encryption,
-            source_encryption=source_encryption,
-            source_file_info=self.source_path.selected_version.file_info,
-            source_content_type=self.source_path.selected_version.content_type,
-        )
+        with contextlib.ExitStack() as exit_stack:
+            if progress_listener:
+                exit_stack.enter_context(progress_listener)
+            bucket.copy(
+                self.source_path.selected_version.id_,
+                self.dest_b2_file_name,
+                length=self.source_path.size,
+                progress_listener=progress_listener,
+                destination_encryption=destination_encryption,
+                source_encryption=source_encryption,
+                source_file_info=self.source_path.selected_version.file_info,
+                source_content_type=self.source_path.selected_version.content_type,
+            )
 
-    def do_report(self, bucket, reporter):
+    def do_report(self, bucket: Bucket, reporter: ProgressReport) -> None:
         """
         Report the copying action performed.
 
         :param bucket: a Bucket object
-        :type bucket: b2sdk.bucket.Bucket
         :param reporter: a place to report errors
         """
         reporter.print_completion('copy ' + self.source_path.relative_path)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return (
             'b2_copy(%s, %s, %s, %d)' % (
                 self.b2_file_name, self.source_path.selected_version.id_, self.dest_b2_file_name,
                 self.source_path.mod_time
             )
         )
 
 
 class B2DeleteAction(AbstractAction):
-    def __init__(self, relative_name, b2_file_name, file_id, note):
+    def __init__(self, relative_name: str, b2_file_name: str, file_id: str, note: str):
         """
-        :param str relative_name: a relative file name
-        :param str b2_file_name: a name of a remote file
-        :param str file_id: a file ID
-        :param str note: a deletion note
+        :param relative_name: a relative file name
+        :param b2_file_name: a name of a remote file
+        :param file_id: a file ID
+        :param note: a deletion note
         """
         self.relative_name = relative_name
         self.b2_file_name = b2_file_name
         self.file_id = file_id
         self.note = note
 
-    def get_bytes(self):
+    def get_bytes(self) -> int:
         """
         Return file size.
 
         :return: always zero
-        :rtype: int
         """
         return 0
 
-    def do_action(self, bucket, reporter):
+    def do_action(self, bucket: Bucket, reporter: ProgressReport):
         """
         Perform the deleting action, returning only after the action is completed.
 
         :param bucket: a Bucket object
-        :type bucket: b2sdk.bucket.Bucket
         :param reporter: a place to report errors
         """
         bucket.api.delete_file_version(self.file_id, self.b2_file_name)
 
-    def do_report(self, bucket, reporter):
+    def do_report(self, bucket: Bucket, reporter: SyncReport):
         """
         Report the deleting action performed.
 
         :param bucket: a Bucket object
-        :type bucket: b2sdk.bucket.Bucket
         :param reporter: a place to report errors
         """
         reporter.update_transfer(1, 0)
-        reporter.print_completion('delete ' + self.relative_name + ' ' + self.note)
+        reporter.print_completion(f"delete {escape_control_chars(self.relative_name)} {self.note}")
 
-    def __str__(self):
-        return 'b2_delete(%s, %s, %s)' % (self.b2_file_name, self.file_id, self.note)
+    def __str__(self) -> str:
+        return f'b2_delete({self.b2_file_name}, {self.file_id}, {self.note})'
 
 
 class LocalDeleteAction(AbstractAction):
-    def __init__(self, relative_name, full_path):
+    def __init__(self, relative_name: str, full_path: str):
         """
         :param relative_name: a relative file name
-        :type relative_name: str
         :param full_path: a full local path
-        :type: str
         """
         self.relative_name = relative_name
         self.full_path = full_path
 
-    def get_bytes(self):
+    def get_bytes(self) -> int:
         """
         Return file size.
 
         :return: always zero
-        :rtype: int
         """
         return 0
 
-    def do_action(self, bucket, reporter):
+    def do_action(self, bucket: Bucket, reporter: ProgressReport):
         """
         Perform the deleting of a local file action,
         returning only after the action is completed.
 
         :param bucket: a Bucket object
-        :type bucket: b2sdk.bucket.Bucket
         :param reporter: a place to report errors
         """
         os.unlink(self.full_path)
 
-    def do_report(self, bucket, reporter):
+    def do_report(self, bucket: Bucket, reporter: SyncReport):
         """
         Report the deleting of a local file action performed.
 
         :param bucket: a Bucket object
-        :type bucket: b2sdk.bucket.Bucket
         :param reporter: a place to report errors
         """
         reporter.update_transfer(1, 0)
-        reporter.print_completion('delete ' + self.relative_name)
+        reporter.print_completion(f'delete {escape_control_chars(self.relative_name)}')
 
-    def __str__(self):
-        return 'local_delete(%s)' % (self.full_path)
+    def __str__(self) -> str:
+        return f'local_delete({self.full_path})'
```

### Comparing `b2sdk-1.9.0/b2sdk/sync/encryption_provider.py` & `b2sdk-2.0.0/b2sdk/_internal/sync/encryption_provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 ######################################################################
 #
-# File: b2sdk/sync/encryption_provider.py
+# File: b2sdk/_internal/sync/encryption_provider.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
-from typing import Dict, Optional
 
-from ..encryption.setting import EncryptionSetting
 from ..bucket import Bucket
+from ..encryption.setting import EncryptionSetting
 from ..file_version import FileVersion
 
 
 class AbstractSyncEncryptionSettingsProvider(metaclass=ABCMeta):
     """
     Object which provides an appropriate EncryptionSetting object
     for sync, i.e. complex operations with multiple sources and destinations
     """
 
     @abstractmethod
     def get_setting_for_upload(
         self,
         bucket: Bucket,
         b2_file_name: str,
-        file_info: Optional[dict],
+        file_info: dict | None,
         length: int,
-    ) -> Optional[EncryptionSetting]:
+    ) -> EncryptionSetting | None:
         """
         Return an EncryptionSetting for uploading an object or None if server should decide.
         """
 
     @abstractmethod
     def get_source_setting_for_copy(
         self,
         bucket: Bucket,
         source_file_version: FileVersion,
-    ) -> Optional[EncryptionSetting]:
+    ) -> EncryptionSetting | None:
         """
         Return an EncryptionSetting for a source of copying an object or None if not required
         """
 
     @abstractmethod
     def get_destination_setting_for_copy(
         self,
         bucket: Bucket,
         dest_b2_file_name: str,
         source_file_version: FileVersion,
-        target_file_info: Optional[dict] = None,
-    ) -> Optional[EncryptionSetting]:
+        target_file_info: dict | None = None,
+    ) -> EncryptionSetting | None:
         """
         Return an EncryptionSetting for a destination for copying an object or None if server should decide
         """
 
     @abstractmethod
     def get_setting_for_download(
         self,
         bucket: Bucket,
         file_version: FileVersion,
-    ) -> Optional[EncryptionSetting]:
+    ) -> EncryptionSetting | None:
         """
         Return an EncryptionSetting for downloading an object from, or None if not required
         """
 
 
 class ServerDefaultSyncEncryptionSettingsProvider(AbstractSyncEncryptionSettingsProvider):
     """
@@ -93,28 +93,27 @@
     """
     Basic encryption setting provider that supports exactly one encryption setting per bucket for reading
     and one encryption setting per bucket for writing
     """
 
     def __init__(
         self,
-        read_bucket_settings: Dict[str, Optional[EncryptionSetting]],
-        write_bucket_settings: Dict[str, Optional[EncryptionSetting]],
+        read_bucket_settings: dict[str, EncryptionSetting | None],
+        write_bucket_settings: dict[str, EncryptionSetting | None],
     ):
         self.read_bucket_settings = read_bucket_settings
         self.write_bucket_settings = write_bucket_settings
 
-    def get_setting_for_upload(self, bucket, *args, **kwargs) -> Optional[EncryptionSetting]:
+    def get_setting_for_upload(self, bucket, *args, **kwargs) -> EncryptionSetting | None:
         return self.write_bucket_settings.get(bucket.name)
 
     def get_source_setting_for_copy(self, bucket, *args, **kwargs) -> None:
         return self.read_bucket_settings.get(bucket.name)
 
-    def get_destination_setting_for_copy(self, bucket, *args,
-                                         **kwargs) -> Optional[EncryptionSetting]:
+    def get_destination_setting_for_copy(self, bucket, *args, **kwargs) -> EncryptionSetting | None:
         return self.write_bucket_settings.get(bucket.name)
 
     def get_setting_for_download(self, bucket, *args, **kwargs) -> None:
         return self.read_bucket_settings.get(bucket.name)
 
     def __repr__(self):
-        return '<%s:%s>' % (self.__class__.__name__, self.bucket_settings)
+        return f'<{self.__class__.__name__}:{self.bucket_settings}>'
```

### Comparing `b2sdk-1.9.0/b2sdk/sync/exception.py` & `b2sdk-2.0.0/b2sdk/_internal/scan/exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 ######################################################################
 #
-# File: b2sdk/sync/exception.py
+# File: b2sdk/_internal/scan/exception.py
 #
-# Copyright 2019 Backblaze Inc. All Rights Reserved.
+# Copyright 2022 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 from contextlib import contextmanager
-from typing import Iterator, Type
+from typing import Iterator
 
 from ..exception import B2Error, B2SimpleError
 
 
 class EnvironmentEncodingError(B2Error):
     """
     Raised when a file name can not be decoded with system encoding.
@@ -21,23 +22,23 @@
 
     def __init__(self, filename, encoding):
         """
         :param filename: an encoded file name
         :type filename: str, bytes
         :param str encoding: file name encoding
         """
-        super(EnvironmentEncodingError, self).__init__()
+        super().__init__()
         self.filename = filename
         self.encoding = encoding
 
     def __str__(self):
-        return """file name %s cannot be decoded with system encoding (%s).
+        return """file name {} cannot be decoded with system encoding ({}).
 We think this is an environment error which you should workaround by
 setting your system encoding properly, for example like this:
-export LANG=en_US.UTF-8""" % (
+export LANG=en_US.UTF-8""".format(
             self.filename,
             self.encoding,
         )
 
 
 class InvalidArgument(B2Error):
     """
@@ -45,47 +46,43 @@
     """
 
     def __init__(self, parameter_name, message):
         """
         :param parameter_name: name of the function argument
         :param message: brief explanation of misconfiguration
         """
-        super(InvalidArgument, self).__init__()
+        super().__init__()
         self.parameter_name = parameter_name
         self.message = message
 
     def __str__(self):
-        return "%s %s" % (self.parameter_name, self.message)
+        return f"{self.parameter_name} {self.message}"
 
 
-class IncompleteSync(B2SimpleError):
-    pass
-
-
-class UnSyncableFilename(B2Error):
+class UnsupportedFilename(B2Error):
     """
-    Raised when a filename is not supported by the sync operation
+    Raised when a filename is not supported by the scan operation
     """
 
     def __init__(self, message, filename):
         """
         :param message: brief explanation of why the filename was not supported
         :param filename: name of the file which is not supported
         """
-        super(UnSyncableFilename, self).__init__()
+        super().__init__()
         self.filename = filename
         self.message = message
 
     def __str__(self):
-        return "%s: %s" % (self.message, self.filename)
+        return f"{self.message}: {self.filename}"
 
 
 @contextmanager
 def check_invalid_argument(parameter_name: str, message: str,
-                           *exceptions: Type[Exception]) -> Iterator[None]:
+                           *exceptions: type[Exception]) -> Iterator[None]:
     """Raise `InvalidArgument` in case of one of given exception was thrown."""
     try:
         yield
     except exceptions as exc:
         if not message:
             message = str(exc)
         raise InvalidArgument(parameter_name, message) from exc
```

### Comparing `b2sdk-1.9.0/b2sdk/sync/folder.py` & `b2sdk-2.0.0/b2sdk/_internal/scan/folder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 ######################################################################
 #
-# File: b2sdk/sync/folder.py
+# File: b2sdk/_internal/scan/folder.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import logging
 import os
 import platform
 import re
 import sys
-
 from abc import ABCMeta, abstractmethod
-from .exception import EmptyDirectory, EnvironmentEncodingError, UnSyncableFilename, NotADirectory, UnableToCreateDirectory
-from .path import B2SyncPath, LocalSyncPath
-from .report import SyncReport
-from .scan_policies import DEFAULT_SCAN_MANAGER, ScanPoliciesManager
+from pathlib import Path
+from typing import Iterator
+
 from ..utils import fix_windows_path_limit, get_file_mtime, is_file_readable
+from .exception import (
+    EmptyDirectory,
+    EnvironmentEncodingError,
+    NotADirectory,
+    UnableToCreateDirectory,
+    UnsupportedFilename,
+)
+from .path import AbstractPath, B2Path, LocalPath
+from .policies import DEFAULT_SCAN_MANAGER, ScanPoliciesManager
+from .report import ProgressReport
 
 DRIVE_MATCHER = re.compile(r"^([A-Za-z]):([/\\])")
 ABSOLUTE_PATH_MATCHER = re.compile(r"^(/)|^(\\)")
 RELATIVE_PATH_MATCHER = re.compile(
                            # "abc" and "xyz" represent anything, including "nothing"
     r"^(\.\.[/\\])|" +     # ../abc or ..\abc
     r"^(\.[/\\])|" +       # ./abc or .\abc
@@ -46,15 +55,16 @@
     system.
 
     Files in B2 may have multiple versions, while files in local
     folders have just one.
     """
 
     @abstractmethod
-    def all_files(self, reporter, policies_manager=DEFAULT_SCAN_MANAGER):
+    def all_files(self, reporter: ProgressReport | None,
+                  policies_manager=DEFAULT_SCAN_MANAGER) -> Iterator[AbstractPath]:
         """
         Return an iterator over all of the files in the folder, in
         the order that B2 uses.
 
         It also performs filtering using policies manager.
 
         No matter what the folder separator on the local file system
@@ -83,56 +93,60 @@
 
         :param file_name: a file name
         :type file_name: str
         :rtype: str
         """
 
 
-def join_b2_path(relative_dir_path: str, file_name: str):
+def join_b2_path(relative_dir_path: str | Path, file_name: str):
     """
     Like os.path.join, but for B2 file names where the root directory is called ''.
     """
-    if relative_dir_path == '':
+    relative_dir_path = str(relative_dir_path)
+    if relative_dir_path in ('', '.'):
         return file_name
     else:
         return relative_dir_path + '/' + file_name
 
 
 class LocalFolder(AbstractFolder):
     """
     Folder interface to a directory on the local machine.
     """
 
-    def __init__(self, root):
+    def __init__(self, root: str | Path):
         """
         Initialize a new folder.
 
         :param root: path to the root of the local folder.  Must be unicode.
-        :type root: str
         """
+        if isinstance(root, Path):
+            root = str(root)
         if not isinstance(root, str):
-            raise ValueError('folder path should be unicode: %s' % repr(root))
+            raise ValueError('folder path should be str or pathlib.Path: %s' % repr(root))
         self.root = fix_windows_path_limit(os.path.abspath(root))
 
     def folder_type(self):
         """
         Return folder type.
 
         :rtype: str
         """
         return 'local'
 
-    def all_files(self, reporter, policies_manager=DEFAULT_SCAN_MANAGER):
+    def all_files(self, reporter: ProgressReport | None,
+                  policies_manager=DEFAULT_SCAN_MANAGER) -> Iterator[LocalPath]:
         """
         Yield all files.
 
         :param reporter: a place to report errors
         :param policies_manager: a policy manager object, default is DEFAULT_SCAN_MANAGER
         """
-        yield from self._walk_relative_paths(self.root, '', reporter, policies_manager)
+        root_path = Path(self.root)
+        yield from self._walk_relative_paths(root_path, Path(''), reporter, policies_manager)
 
     def make_full_path(self, file_name):
         """
         Convert a file name into an absolute path, ensure it is not outside self.root
 
         :param file_name: a file name
         :type file_name: str
@@ -144,15 +158,15 @@
         full_path = os.path.normpath(os.path.join(self.root, file_name))
 
         # Get the common prefix between the new full_path and self.root
         common_prefix = os.path.commonprefix([full_path, self.root])
 
         # Ensure the new full_path is inside the self.root directory
         if common_prefix != self.root:
-            raise UnSyncableFilename("illegal file name", full_path)
+            raise UnsupportedFilename("illegal file name", full_path)
 
         return full_path
 
     def ensure_present(self):
         """
         Make sure that the directory exists.
         """
@@ -170,25 +184,31 @@
         """
         self.ensure_present()
 
         if not os.listdir(self.root):
             raise EmptyDirectory(self.root)
 
     def _walk_relative_paths(
-        self, local_dir: str, relative_dir_path: str, reporter: SyncReport,
-        policies_manager: ScanPoliciesManager
+        self,
+        local_dir: Path,
+        relative_dir_path: Path,
+        reporter: ProgressReport,
+        policies_manager: ScanPoliciesManager,
+        visited_symlinks: set[int] | None = None,
     ):
         """
         Yield a File object for each of the files anywhere under this folder, in the
         order they would appear in B2, unless the path is excluded by policies manager.
 
-        :param relative_dir_path: the path of this dir relative to the sync point, or '' if at sync point
+        :param local_dir: the path to the local directory that we are currently inspecting
+        :param relative_dir_path: the path of this dir relative to the scan point, or Path('') if at scan point
+        :param reporter: a reporter object to report errors and warnings
+        :param policies_manager: a policies manager object
+        :param visited_symlinks: a set of paths to symlinks that have already been visited. Using inode numbers to reduce memory usage
         """
-        if not isinstance(local_dir, str):
-            raise ValueError('folder path should be unicode: %s' % repr(local_dir))
 
         # Collect the names.  We do this before returning any results, because
         # directories need to sort as if their names end in '/'.
         #
         # With a directory containing 'a', 'a.txt', and 'a0.txt', with 'a' being
         # a directory containing 'b.txt', and 'c.txt', the results returned
         # should be:
@@ -196,76 +216,97 @@
         #    a.txt
         #    a/b.txt
         #    a/c.txt
         #    a0.txt
         #
         # This is because in Unicode '.' comes before '/', which comes before '0'.
         names = []  # list of (name, local_path, relative_file_path)
-        for name in os.listdir(local_dir):
-            # We expect listdir() to return unicode if dir_path is unicode.
-            # If the file name is not valid, based on the file system
-            # encoding, then listdir() will return un-decoded str/bytes.
-            if not isinstance(name, str):
-                name = self._handle_non_unicode_file_name(name)
+
+        visited_symlinks = visited_symlinks or set()
+
+        if local_dir.is_symlink():
+            real_path = local_dir.resolve()
+            inode_number = real_path.stat().st_ino
+
+            visited_symlinks_count = len(visited_symlinks)
+
+            # Add symlink to visited_symlinks to prevent infinite symlink loops
+            visited_symlinks.add(inode_number)
+
+            # Check if set size has changed, if not, symlink has already been visited
+            if len(visited_symlinks) == visited_symlinks_count:
+                # Infinite symlink loop detected, report warning and skip symlink
+                if reporter is not None:
+                    reporter.circular_symlink_skipped(str(local_dir))
+                return
+
+            visited_symlinks.add(inode_number)
+
+        for name in (x.name for x in local_dir.iterdir()):
 
             if '/' in name:
-                raise UnSyncableFilename(
-                    "sync does not support file names that include '/'",
-                    "%s in dir %s" % (name, local_dir)
+                raise UnsupportedFilename(
+                    "scan does not support file names that include '/'",
+                    f"{name} in dir {local_dir}"
                 )
 
-            local_path = os.path.join(local_dir, name)
-            relative_file_path = join_b2_path(
-                relative_dir_path, name
-            )  # file path relative to the sync point
+            local_path = local_dir / name
+            relative_file_path = join_b2_path(relative_dir_path, name)
 
             # Skip broken symlinks or other inaccessible files
-            if not is_file_readable(local_path, reporter):
+            if not is_file_readable(str(local_path), reporter):
                 continue
 
-            if policies_manager.exclude_all_symlinks and os.path.islink(local_path):
+            if policies_manager.exclude_all_symlinks and local_path.is_symlink():
                 if reporter is not None:
-                    reporter.symlink_skipped(local_path)
+                    reporter.symlink_skipped(str(local_path))
                 continue
 
-            if os.path.isdir(local_path):
+            if local_path.is_dir():
                 name += '/'
-                if policies_manager.should_exclude_local_directory(relative_file_path):
+                if policies_manager.should_exclude_local_directory(str(relative_file_path)):
                     continue
 
-            names.append((name, local_path, relative_file_path))
+            # remove the leading './' from the relative path to ensure backward compatibility
+            relative_file_path_str = str(relative_file_path)
+            if relative_file_path_str.startswith("./"):
+                relative_file_path_str = relative_file_path_str[2:]
+            names.append((name, local_path, relative_file_path_str))
 
         # Yield all of the answers.
         #
         # Sorting the list of triples puts them in the right order because 'name',
         # the sort key, is the first thing in the triple.
         for (name, local_path, relative_file_path) in sorted(names):
             if name.endswith('/'):
-                for subdir_file in self._walk_relative_paths(
-                    local_path, relative_file_path, reporter, policies_manager
-                ):
-                    yield subdir_file
+                yield from self._walk_relative_paths(
+                    local_path,
+                    relative_file_path,
+                    reporter,
+                    policies_manager,
+                    visited_symlinks,
+                )
             else:
                 # Check that the file still exists and is accessible, since it can take a long time
                 # to iterate through large folders
-                if is_file_readable(local_path, reporter):
-                    file_mod_time = get_file_mtime(local_path)
-                    file_size = os.path.getsize(local_path)
-
-                    local_sync_path = LocalSyncPath(
-                        absolute_path=self.make_full_path(relative_file_path),
-                        relative_path=relative_file_path,
+                if is_file_readable(str(local_path), reporter):
+                    file_mod_time = get_file_mtime(str(local_path))
+                    file_size = local_path.stat().st_size
+
+                    local_scan_path = LocalPath(
+                        absolute_path=self.make_full_path(str(relative_file_path)),
+                        relative_path=str(relative_file_path),
                         mod_time=file_mod_time,
                         size=file_size,
                     )
 
-                    if policies_manager.should_exclude_local_path(local_sync_path):
+                    if policies_manager.should_exclude_local_path(local_scan_path):
                         continue
 
-                    yield local_sync_path
+                    yield local_scan_path
 
     @classmethod
     def _handle_non_unicode_file_name(cls, name):
         """
         Decide what to do with a name returned from os.listdir()
         that isn't unicode.  We think that this only happens when
         the file name can't be decoded using the file system
@@ -274,15 +315,15 @@
         """
         # if it's all ascii, allow it
         if all(b <= 127 for b in name):
             return name
         raise EnvironmentEncodingError(repr(name), sys.getfilesystemencoding())
 
     def __repr__(self):
-        return 'LocalFolder(%s)' % (self.root,)
+        return f'LocalFolder({self.root})'
 
 
 def b2_parent_dir(file_name):
     # Various Parent dir getting method have been tested, and this one seems to be the faste
     # After dropping python 3.9 support: refactor this use the "match" syntax
     try:
         dir_name, _ = file_name.rsplit('/', 1)
@@ -299,25 +340,29 @@
     def __init__(self, bucket_name, folder_name, api):
         """
         :param bucket_name: a name of the bucket
         :type bucket_name: str
         :param folder_name: a folder name
         :type folder_name: str
         :param api: an API object
-        :type api: b2sdk.api.B2Api
+        :type api: b2sdk._internal.api.B2Api
         """
         self.bucket_name = bucket_name
         self.folder_name = folder_name
         self.bucket = api.get_bucket_by_name(bucket_name)
         self.api = api
-        self.prefix = '' if self.folder_name == '' else self.folder_name + '/'
+        self.prefix = self.folder_name
+        if self.prefix and self.prefix[-1] != '/':
+            self.prefix += '/'
 
     def all_files(
-        self, reporter: SyncReport, policies_manager: ScanPoliciesManager = DEFAULT_SCAN_MANAGER
-    ):
+        self,
+        reporter: ProgressReport | None,
+        policies_manager: ScanPoliciesManager = DEFAULT_SCAN_MANAGER
+    ) -> Iterator[B2Path]:
         """
         Yield all files.
         """
         current_name = None
         last_ignored_dir = None
         current_versions = []
         current_file_version = None
@@ -342,54 +387,54 @@
 
             if policies_manager.should_exclude_b2_file_version(file_version, file_name):
                 continue
 
             self._validate_file_name(file_name)
 
             if current_name != file_name and current_name is not None and current_versions:
-                yield B2SyncPath(
+                yield B2Path(
                     relative_path=current_name,
                     selected_version=current_versions[0],
                     all_versions=current_versions
                 )
                 current_versions = []
 
             current_name = file_name
             current_versions.append(file_version)
 
         if current_name is not None and current_versions:
-            yield B2SyncPath(
+            yield B2Path(
                 relative_path=current_name,
                 selected_version=current_versions[0],
                 all_versions=current_versions
             )
 
     def get_file_versions(self):
         for file_version, _ in self.bucket.ls(
             self.folder_name,
-            show_versions=True,
+            latest_only=False,
             recursive=True,
         ):
             yield file_version
 
     def _validate_file_name(self, file_name):
         # Do not allow relative paths in file names
         if RELATIVE_PATH_MATCHER.search(file_name):
-            raise UnSyncableFilename(
-                "sync does not support file names that include relative paths", file_name
+            raise UnsupportedFilename(
+                "scan does not support file names that include relative paths", file_name
             )
         # Do not allow absolute paths in file names
         if ABSOLUTE_PATH_MATCHER.search(file_name):
-            raise UnSyncableFilename(
-                "sync does not support file names with absolute paths", file_name
+            raise UnsupportedFilename(
+                "scan does not support file names with absolute paths", file_name
             )
         # On Windows, do not allow drive letters in file names
         if platform.system() == "Windows" and DRIVE_MATCHER.search(file_name):
-            raise UnSyncableFilename(
-                "sync does not support file names with drive letters", file_name
+            raise UnsupportedFilename(
+                "scan does not support file names with drive letters", file_name
             )
 
     def folder_type(self):
         """
         Return folder type.
 
         :rtype: str
@@ -405,8 +450,8 @@
         """
         if self.folder_name == '':
             return file_name
         else:
             return self.folder_name + '/' + file_name
 
     def __str__(self):
-        return 'B2Folder(%s, %s)' % (self.bucket_name, self.folder_name)
+        return f'B2Folder({self.bucket_name}, {self.folder_name})'
```

### Comparing `b2sdk-1.9.0/b2sdk/sync/folder_parser.py` & `b2sdk-2.0.0/b2sdk/_internal/scan/folder_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 ######################################################################
 #
-# File: b2sdk/sync/folder_parser.py
+# File: b2sdk/_internal/scan/folder_parser.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 from .exception import InvalidArgument
 from .folder import B2Folder, LocalFolder
 
 
-def parse_sync_folder(folder_name, api, local_folder_class=LocalFolder, b2_folder_class=B2Folder):
+def parse_folder(folder_name, api, local_folder_class=LocalFolder, b2_folder_class=B2Folder):
     """
     Take either a local path, or a B2 path, and returns a Folder
     object for it.
 
-    B2 paths look like: b2://bucketName/path/name.  The '//' is optional,
-    because the previous sync command didn't use it.
+    B2 paths look like: b2://bucketName/path/name.  The '//' is optional.
 
     Anything else is treated like a local folder.
 
     :param folder_name: a name of the folder, either local or remote
     :type folder_name: str
     :param api: an API object
-    :type api: :class:`~b2sdk.v1.B2Api`
+    :type api: :class:`~b2sdk.v2.B2Api`
     :param local_folder_class: class to handle local folders
-    :type local_folder_class: `~b2sdk.v1.AbstractFolder`
+    :type local_folder_class: `~b2sdk.v2.AbstractFolder`
     :param b2_folder_class: class to handle B2 folders
-    :type b2_folder_class: `~b2sdk.v1.AbstractFolder`
+    :type b2_folder_class: `~b2sdk.v2.AbstractFolder`
     """
     if folder_name.startswith('b2://'):
         return _parse_bucket_and_folder(folder_name[5:], api, b2_folder_class)
     elif folder_name.startswith('b2:') and folder_name[3].isalnum():
         return _parse_bucket_and_folder(folder_name[3:], api, b2_folder_class)
     else:
         return local_folder_class(folder_name)
```

### Comparing `b2sdk-1.9.0/b2sdk/sync/path.py` & `b2sdk-2.0.0/b2sdk/_internal/scan/path.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 ######################################################################
 #
-# File: b2sdk/sync/path.py
+# File: b2sdk/_internal/scan/path.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import List
 
 from ..file_version import FileVersion
 
 
-class AbstractSyncPath(ABC):
+class AbstractPath(ABC):
     """
     Represent a path in a source or destination folder - be it B2 or local
     """
 
     def __init__(self, relative_path: str, mod_time: int, size: int):
         self.relative_path = relative_path
         self.mod_time = mod_time
         self.size = size
 
     @abstractmethod
     def is_visible(self) -> bool:
         """Is the path visible/not deleted on it's storage"""
 
     def __repr__(self):
-        return '%s(%s, %s, %s)' % (
+        return '{}({}, {}, {})'.format(
             self.__class__.__name__, repr(self.relative_path), repr(self.mod_time), repr(self.size)
         )
 
 
-class LocalSyncPath(AbstractSyncPath):
+class LocalPath(AbstractPath):
     __slots__ = ['absolute_path', 'relative_path', 'mod_time', 'size']
 
     def __init__(self, absolute_path: str, relative_path: str, mod_time: int, size: int):
         self.absolute_path = absolute_path
         super().__init__(relative_path, mod_time, size)
 
     def is_visible(self) -> bool:
@@ -48,19 +48,19 @@
         return (
             self.absolute_path == other.absolute_path and
             self.relative_path == other.relative_path and self.mod_time == other.mod_time and
             self.size == other.size
         )
 
 
-class B2SyncPath(AbstractSyncPath):
+class B2Path(AbstractPath):
     __slots__ = ['relative_path', 'selected_version', 'all_versions']
 
     def __init__(
-        self, relative_path: str, selected_version: FileVersion, all_versions: List[FileVersion]
+        self, relative_path: str, selected_version: FileVersion, all_versions: list[FileVersion]
     ):
         self.selected_version = selected_version
         self.all_versions = all_versions
         self.relative_path = relative_path
 
     def is_visible(self) -> bool:
         return self.selected_version.action != 'hide'
@@ -70,21 +70,18 @@
         return self.selected_version.mod_time_millis
 
     @property
     def size(self) -> int:
         return self.selected_version.size
 
     def __repr__(self):
-        return '%s(%s, [%s])' % (
+        return '{}({}, [{}])'.format(
             self.__class__.__name__, self.relative_path, ', '.join(
-                '(%s, %s, %s)' % (
-                    repr(fv.id_),
-                    repr(fv.mod_time_millis),
-                    repr(fv.action),
-                ) for fv in self.all_versions
+                f'({repr(fv.id_)}, {repr(fv.mod_time_millis)}, {repr(fv.action)})'
+                for fv in self.all_versions
             )
         )
 
     def __eq__(self, other):
         return (
             self.relative_path == other.relative_path and
             self.selected_version == other.selected_version and
```

### Comparing `b2sdk-1.9.0/b2sdk/sync/policy.py` & `b2sdk-2.0.0/b2sdk/_internal/sync/policy.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 ######################################################################
 #
-# File: b2sdk/sync/policy.py
+# File: b2sdk/_internal/sync/policy.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
+import logging
 from abc import ABCMeta, abstractmethod
 from enum import Enum, unique
-from typing import Optional
-
-import logging
+from typing import cast
 
 from ..exception import DestFileNewer
-from .encryption_provider import AbstractSyncEncryptionSettingsProvider, SERVER_DEFAULT_SYNC_ENCRYPTION_SETTINGS_PROVIDER
-from .action import LocalDeleteAction, B2CopyAction, B2DeleteAction, B2DownloadAction, B2HideAction, B2UploadAction
-from .exception import InvalidArgument
-from .folder import AbstractFolder
-from .path import AbstractSyncPath
+from ..scan.exception import InvalidArgument
+from ..scan.folder import AbstractFolder, B2Folder
+from ..scan.path import AbstractPath, B2Path
+from ..transfer.outbound.upload_source import UploadMode
+from .action import (
+    B2CopyAction,
+    B2DeleteAction,
+    B2DownloadAction,
+    B2HideAction,
+    B2IncrementalUploadAction,
+    B2UploadAction,
+    LocalDeleteAction,
+)
+from .encryption_provider import (
+    SERVER_DEFAULT_SYNC_ENCRYPTION_SETTINGS_PROVIDER,
+    AbstractSyncEncryptionSettingsProvider,
+)
 
 ONE_DAY_IN_MS = 24 * 60 * 60 * 1000
 
 logger = logging.getLogger(__name__)
 
 
 @unique
@@ -47,51 +59,57 @@
     Abstract policy class.
     """
     DESTINATION_PREFIX = NotImplemented
     SOURCE_PREFIX = NotImplemented
 
     def __init__(
         self,
-        source_path: AbstractSyncPath,
+        source_path: AbstractPath | None,
         source_folder: AbstractFolder,
-        dest_path: AbstractSyncPath,
+        dest_path: AbstractPath | None,
         dest_folder: AbstractFolder,
         now_millis: int,
         keep_days: int,
         newer_file_mode: NewerFileSyncMode,
         compare_threshold: int,
         compare_version_mode: CompareVersionMode = CompareVersionMode.MODTIME,
         encryption_settings_provider:
         AbstractSyncEncryptionSettingsProvider = SERVER_DEFAULT_SYNC_ENCRYPTION_SETTINGS_PROVIDER,
+        upload_mode: UploadMode = UploadMode.FULL,
+        absolute_minimum_part_size: int | None = None,
     ):
         """
-        :param b2sdk.v1.AbstractSyncPath source_path: source file object
-        :param b2sdk.v1.AbstractFolder source_folder: source folder object
-        :param b2sdk.v1.AbstractSyncPath dest_path: destination file object
-        :param b2sdk.v1.AbstractFolder dest_folder: destination folder object
-        :param int now_millis: current time in milliseconds
-        :param int keep_days: days to keep before delete
-        :param b2sdk.v1.NewerFileSyncMode newer_file_mode: setting which determines handling for destination files newer than on the source
-        :param int compare_threshold: when comparing with size or time for sync
-        :param b2sdk.v1.COMPARE_VERSION_MODES compare_version_mode: how to compare source and destination files
-        :param b2sdk.v1.AbstractSyncEncryptionSettingsProvider encryption_settings_provider: encryption setting provider
+        :param source_path: source file object
+        :param source_folder: source folder object
+        :param dest_path: destination file object
+        :param dest_folder: destination folder object
+        :param now_millis: current time in milliseconds
+        :param keep_days: days to keep before delete
+        :param newer_file_mode: setting which determines handling for destination files newer than on the source
+        :param compare_threshold: when comparing with size or time for sync
+        :param compare_version_mode: how to compare source and destination files
+        :param encryption_settings_provider: encryption setting provider
+        :param upload_mode: file upload mode
+        :param absolute_minimum_part_size: minimum file part size that can be uploaded to the server
         """
         self._source_path = source_path
         self._source_folder = source_folder
         self._dest_path = dest_path
         self._keep_days = keep_days
         self._newer_file_mode = newer_file_mode
         self._compare_version_mode = compare_version_mode
         self._compare_threshold = compare_threshold
         self._dest_folder = dest_folder
         self._now_millis = now_millis
         self._transferred = False
         self._encryption_settings_provider = encryption_settings_provider
+        self._upload_mode = upload_mode
+        self._absolute_minimum_part_size = absolute_minimum_part_size
 
-    def _should_transfer(self):
+    def _should_transfer(self) -> bool:
         """
         Decide whether to transfer the file from the source to the destination.
         """
         if self._source_path is None or not self._source_path.is_visible():
             # No source file.  Nothing to transfer.
             return False
         elif self._dest_path is None:
@@ -106,29 +124,29 @@
                 self._compare_version_mode,
                 self._newer_file_mode,
             )
 
     @classmethod
     def files_are_different(
         cls,
-        source_path: AbstractSyncPath,
-        dest_path: AbstractSyncPath,
-        compare_threshold: Optional[int] = None,
+        source_path: AbstractPath,
+        dest_path: AbstractPath,
+        compare_threshold: int | None = None,
         compare_version_mode: CompareVersionMode = CompareVersionMode.MODTIME,
         newer_file_mode: NewerFileSyncMode = NewerFileSyncMode.RAISE_ERROR,
     ):
         """
         Compare two files and determine if the the destination file
         should be replaced by the source file.
 
-        :param b2sdk.v1.AbstractSyncPath source_path: source file object
-        :param b2sdk.v1.AbstractSyncPath dest_path: destination file object
+        :param b2sdk.v2.AbstractPath source_path: source file object
+        :param b2sdk.v2.AbstractPath dest_path: destination file object
         :param int compare_threshold: compare threshold when comparing by time or size
-        :param b2sdk.v1.CompareVersionMode compare_version_mode: source file version comparator method
-        :param b2sdk.v1.NewerFileSyncMode newer_file_mode: newer destination handling method
+        :param b2sdk.v2.CompareVersionMode compare_version_mode: source file version comparator method
+        :param b2sdk.v2.NewerFileSyncMode newer_file_mode: newer destination handling method
         """
         # Optionally set a compare threshold for fuzzy comparison
         compare_threshold = compare_threshold or 0
 
         # Compare using file name only
         if compare_version_mode == CompareVersionMode.NONE:
             return False
@@ -196,24 +214,25 @@
         """
         if self._should_transfer():
             yield self._make_transfer_action()
             self._transferred = True
 
         assert self._dest_path is not None or self._source_path is not None
 
-        for action in self._get_hide_delete_actions():
-            yield action
+        yield from self._get_hide_delete_actions()
 
     def _get_hide_delete_actions(self):
         """
         Subclass policy can override this to hide or delete files.
         """
         return []
 
-    def _get_source_mod_time(self):
+    def _get_source_mod_time(self) -> int:
+        if self._source_path is None:
+            return 0
         return self._source_path.mod_time
 
     @abstractmethod
     def _make_transfer_action(self):
         """
         Return an action representing transfer of file according to the selected policy.
         """
@@ -224,63 +243,74 @@
     File is synced down (from the cloud to disk).
     """
     DESTINATION_PREFIX = 'local://'
     SOURCE_PREFIX = 'b2://'
 
     def _make_transfer_action(self):
         return B2DownloadAction(
-            self._source_path,
+            cast(B2Path, self._source_path),
             self._source_folder.make_full_path(self._source_path.relative_path),
             self._dest_folder.make_full_path(self._source_path.relative_path),
             self._encryption_settings_provider,
         )
 
 
 class UpPolicy(AbstractFileSyncPolicy):
     """
     File is synced up (from disk the cloud).
     """
     DESTINATION_PREFIX = 'b2://'
     SOURCE_PREFIX = 'local://'
 
     def _make_transfer_action(self):
-        return B2UploadAction(
-            self._source_folder.make_full_path(self._source_path.relative_path),
-            self._source_path.relative_path,
-            self._dest_folder.make_full_path(self._source_path.relative_path),
-            self._get_source_mod_time(),
-            self._source_path.size,
-            self._encryption_settings_provider,
-        )
+        # Find out if we want to append with new bytes or replace completely
+        if self._upload_mode == UploadMode.INCREMENTAL and self._dest_path:
+            return B2IncrementalUploadAction(
+                self._source_folder.make_full_path(self._source_path.relative_path),
+                self._source_path.relative_path,
+                self._dest_folder.make_full_path(self._source_path.relative_path),
+                self._get_source_mod_time(),
+                self._source_path.size,
+                self._encryption_settings_provider,
+                cast(B2Path, self._dest_path).selected_version,
+                self._absolute_minimum_part_size,
+            )
+        else:
+            return B2UploadAction(
+                self._source_folder.make_full_path(self._source_path.relative_path),
+                self._source_path.relative_path,
+                self._dest_folder.make_full_path(self._source_path.relative_path),
+                self._get_source_mod_time(),
+                self._source_path.size,
+                self._encryption_settings_provider,
+            )
 
 
 class UpAndDeletePolicy(UpPolicy):
     """
     File is synced up (from disk to the cloud) and the delete flag is SET.
     """
 
     def _get_hide_delete_actions(self):
-        for action in super(UpAndDeletePolicy, self)._get_hide_delete_actions():
-            yield action
-        for action in make_b2_delete_actions(
+        yield from super()._get_hide_delete_actions()
+        yield from make_b2_delete_actions(
             self._source_path,
             self._dest_path,
             self._dest_folder,
             self._transferred,
-        ):
-            yield action
+        )
 
 
 class UpAndKeepDaysPolicy(UpPolicy):
     """
     File is synced up (from disk to the cloud) and the keepDays flag is SET.
     """
 
     def _get_hide_delete_actions(self):
-        for action in super(UpAndKeepDaysPolicy, self)._get_hide_delete_actions():
+        for action in super()._get_hide_delete_actions():
             yield action
         for action in make_b2_keep_days_actions(
             self._source_path,
             self._dest_path,
             self._dest_folder,
             self._transferred,
             self._keep_days,
@@ -291,16 +321,15 @@
 
 class DownAndDeletePolicy(DownPolicy):
     """
     File is synced down (from the cloud to disk) and the delete flag is SET.
     """
 
     def _get_hide_delete_actions(self):
-        for action in super(DownAndDeletePolicy, self)._get_hide_delete_actions():
-            yield action
+        yield from super()._get_hide_delete_actions()
         if self._dest_path is not None and (
             self._source_path is None or not self._source_path.is_visible()
         ):
             yield LocalDeleteAction(
                 self._dest_path.relative_path,
                 self._dest_folder.make_full_path(self._dest_path.relative_path)
             )
@@ -320,18 +349,18 @@
     DESTINATION_PREFIX = 'b2://'
     SOURCE_PREFIX = 'b2://'
 
     def _make_transfer_action(self):
 
         return B2CopyAction(
             self._source_folder.make_full_path(self._source_path.relative_path),
-            self._source_path,
+            cast(B2Path, self._source_path),
             self._dest_folder.make_full_path(self._source_path.relative_path),
-            self._source_folder.bucket,
-            self._dest_folder.bucket,
+            cast(B2Folder, self._source_folder).bucket,
+            cast(B2Folder, self._dest_folder).bucket,
             self._encryption_settings_provider,
         )
 
 
 class CopyAndDeletePolicy(CopyPolicy):
     """
     File is copied (server-side) and the delete flag is SET.
@@ -368,39 +397,39 @@
             yield action
 
 
 def make_b2_delete_note(version, index, transferred):
     """
     Create a note message for delete action.
 
-    :param b2sdk.v1.FileVersionInfo version: an object which contains file version info
+    :param b2sdk.v2.FileVersion version: an object which contains file version info
     :param int index: file version index
     :param bool transferred: if True, file has been transferred, False otherwise
     """
     note = ''
     if version.action == 'hide':
         note = '(hide marker)'
     elif transferred or 0 < index:
         note = '(old version)'
     return note
 
 
 def make_b2_delete_actions(
-    source_path: AbstractSyncPath,
-    dest_path: AbstractSyncPath,
+    source_path: AbstractPath | None,
+    dest_path: B2Path | None,
     dest_folder: AbstractFolder,
     transferred: bool,
 ):
     """
     Create the actions to delete files stored on B2, which are not present locally.
 
-    :param b2sdk.v1.AbstractSyncPath source_path: source file object
-    :param b2sdk.v1.AbstractSyncPath dest_path: destination file object
-    :param b2sdk.v1.AbstractFolder dest_folder: destination folder
-    :param bool transferred: if True, file has been transferred, False otherwise
+    :param source_path: source file object
+    :param dest_path: destination file object
+    :param dest_folder: destination folder
+    :param transferred: if True, file has been transferred, False otherwise
     """
     if dest_path is None:
         # B2 does not really store folders, so there is no need to hide
         # them or delete them
         return
     for version_index, version in enumerate(dest_path.all_versions):
         keep = (version_index == 0) and (source_path is not None) and not transferred
@@ -410,37 +439,37 @@
                 dest_folder.make_full_path(dest_path.relative_path),
                 version.id_,
                 make_b2_delete_note(version, version_index, transferred),
             )
 
 
 def make_b2_keep_days_actions(
-    source_path: AbstractSyncPath,
-    dest_path: AbstractSyncPath,
+    source_path: AbstractPath | None,
+    dest_path: B2Path | None,
     dest_folder: AbstractFolder,
     transferred: bool,
     keep_days: int,
     now_millis: int,
 ):
     """
     Create the actions to hide or delete existing versions of a file
     stored in b2.
 
     When keepDays is set, all files that were visible any time from
     keepDays ago until now must be kept.  If versions were uploaded 5
     days ago, 15 days ago, and 25 days ago, and the keepDays is 10,
-    only the 25-day old version can be deleted.  The 15 day-old version
+    only the 25 day-old version can be deleted.  The 15 day-old version
     was visible 10 days ago.
 
-    :param b2sdk.v1.AbstractSyncPath source_path: source file object
-    :param b2sdk.v1.AbstractSyncPath dest_path: destination file object
-    :param b2sdk.v1.AbstractFolder dest_folder: destination folder object
-    :param bool transferred: if True, file has been transferred, False otherwise
-    :param int keep_days: how many days to keep a file
-    :param int now_millis: current time in milliseconds
+    :param source_path: source file object
+    :param dest_path: destination file object
+    :param dest_folder: destination folder object
+    :param transferred: if True, file has been transferred, False otherwise
+    :param keep_days: how many days to keep a file
+    :param now_millis: current time in milliseconds
     """
     deleting = False
     if dest_path is None:
         # B2 does not really store folders, so there is no need to hide
         # them or delete them
         return
     for version_index, version in enumerate(dest_path.all_versions):
@@ -451,15 +480,15 @@
         # BUT NOT ALWAYS. The mod time we have is the src_last_modified_millis
         # from the file info (if present), or the upload start time
         # (if not present). The user-specified src_last_modified_millis
         # may not be in order. Because of that, we no longer
         # assert that age_days is non-decreasing.
         #
         # Note that if there is an out-of-order date that is old enough
-        # to trigger deletions, all of the versions uploaded before that
+        # to trigger deletions, all the versions uploaded before that
         # (the ones after it in the list) will be deleted, even if they
         # aren't over the age threshold.
 
         # Do we need to hide this version?
         if version_index == 0 and source_path is None and version.action == 'upload':
             yield B2HideAction(
                 dest_path.relative_path, dest_folder.make_full_path(dest_path.relative_path)
```

### Comparing `b2sdk-1.9.0/b2sdk/sync/policy_manager.py` & `b2sdk-2.0.0/b2sdk/_internal/sync/policy_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,97 @@
 ######################################################################
 #
-# File: b2sdk/sync/policy_manager.py
+# File: b2sdk/_internal/sync/policy_manager.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from .policy import CopyAndDeletePolicy, CopyAndKeepDaysPolicy, CopyPolicy, \
-    DownAndDeletePolicy, DownAndKeepDaysPolicy, DownPolicy, UpAndDeletePolicy, \
-    UpAndKeepDaysPolicy, UpPolicy
-from .path import AbstractSyncPath
+from ..scan.folder import AbstractFolder
+from ..scan.path import AbstractPath
+from ..transfer.outbound.upload_source import UploadMode
+from .encryption_provider import AbstractSyncEncryptionSettingsProvider
+from .policy import (
+    AbstractFileSyncPolicy,
+    CompareVersionMode,
+    CopyAndDeletePolicy,
+    CopyAndKeepDaysPolicy,
+    CopyPolicy,
+    DownAndDeletePolicy,
+    DownAndKeepDaysPolicy,
+    DownPolicy,
+    NewerFileSyncMode,
+    UpAndDeletePolicy,
+    UpAndKeepDaysPolicy,
+    UpPolicy,
+)
 
 
-class SyncPolicyManager(object):
+class SyncPolicyManager:
     """
     Policy manager; implement a logic to get a correct policy class
     and create a policy object based on various parameters.
     """
 
     def __init__(self):
         self.policies = {}  # dict<,>
 
     def get_policy(
         self,
-        sync_type,
-        source_path: AbstractSyncPath,
-        source_folder,
-        dest_path: AbstractSyncPath,
-        dest_folder,
-        now_millis,
-        delete,
-        keep_days,
-        newer_file_mode,
-        compare_threshold,
-        compare_version_mode,
-        encryption_settings_provider,
-    ):
+        sync_type: str,
+        source_path: AbstractPath | None,
+        source_folder: AbstractFolder,
+        dest_path: AbstractPath | None,
+        dest_folder: AbstractFolder,
+        now_millis: int,
+        delete: bool,
+        keep_days: int,
+        newer_file_mode: NewerFileSyncMode,
+        compare_threshold: int,
+        compare_version_mode: CompareVersionMode,
+        encryption_settings_provider: AbstractSyncEncryptionSettingsProvider,
+        upload_mode: UploadMode,
+        absolute_minimum_part_size: int,
+    ) -> AbstractFileSyncPolicy:
         """
         Return a policy object.
 
-        :param str sync_type: synchronization type
-        :param b2sdk.v1.AbstractSyncPath source_path: source file
-        :param str source_folder: a source folder path
-        :param b2sdk.v1.AbstractSyncPath dest_path: destination file
-        :param str dest_folder: a destination folder path
-        :param int now_millis: current time in milliseconds
-        :param bool delete: delete policy
-        :param int keep_days: keep for days policy
-        :param b2sdk.v1.NewerFileSyncMode newer_file_mode: setting which determines handling for destination files newer than on the source
-        :param int compare_threshold: difference between file modification time or file size
-        :param b2sdk.v1.CompareVersionMode compare_version_mode: setting which determines how to compare source and destination files
-        :param b2sdk.v1.AbstractSyncEncryptionSettingsProvider encryption_settings_provider: an object which decides which encryption to use (if any)
+        :param sync_type: synchronization type
+        :param source_path: source file
+        :param source_folder: a source folder path
+        :param dest_path: destination file
+        :param dest_folder: a destination folder path
+        :param now_millis: current time in milliseconds
+        :param delete: delete policy
+        :param keep_days: keep for days policy
+        :param newer_file_mode: setting which determines handling for destination files newer than on the source
+        :param compare_threshold: difference between file modification time or file size
+        :param compare_version_mode: setting which determines how to compare source and destination files
+        :param encryption_settings_provider: an object which decides which encryption to use (if any)
+        :param upload_mode: determines how file uploads are handled
+        :param absolute_minimum_part_size: minimum file part size for large files
         :return: a policy object
         """
         policy_class = self.get_policy_class(sync_type, delete, keep_days)
         return policy_class(
             source_path,
             source_folder,
             dest_path,
             dest_folder,
             now_millis,
             keep_days,
             newer_file_mode,
             compare_threshold,
             compare_version_mode,
             encryption_settings_provider,
+            upload_mode,
+            absolute_minimum_part_size,
         )
 
     def get_policy_class(self, sync_type, delete, keep_days):
         """
         Get policy class by a given sync type.
 
         :param str sync_type: synchronization type
@@ -96,16 +117,12 @@
             if delete:
                 return CopyAndDeletePolicy
             elif keep_days:
                 return CopyAndKeepDaysPolicy
             else:
                 return CopyPolicy
         raise NotImplementedError(
-            'invalid sync type: %s, keep_days: %s, delete: %s' % (
-                sync_type,
-                keep_days,
-                delete,
-            )
+            f'invalid sync type: {sync_type}, keep_days: {keep_days}, delete: {delete}'
         )
 
 
 POLICY_MANAGER = SyncPolicyManager()
```

### Comparing `b2sdk-1.9.0/b2sdk/sync/scan_policies.py` & `b2sdk-2.0.0/b2sdk/_internal/scan/policies.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 ######################################################################
 #
-# File: b2sdk/sync/scan_policies.py
+# File: b2sdk/_internal/scan/policies.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import logging
 import re
-from typing import Optional, Union, Iterable
+from typing import Iterable
 
-from .exception import InvalidArgument, check_invalid_argument
-from .path import LocalSyncPath
 from ..file_version import FileVersion
+from .exception import InvalidArgument, check_invalid_argument
+from .path import LocalPath
 
 logger = logging.getLogger(__name__)
 
-try:  # python 3.5 and 3.6 compatibility
-    regex_class = re.Pattern
-except AttributeError:
-    regex_class = re._pattern_type
-
 
-class RegexSet(object):
+class RegexSet:
     """
     Hold a (possibly empty) set of regular expressions and know how to check
     whether a string matches any of them.
     """
 
     def __init__(self, regex_iterable):
         """
@@ -43,15 +39,15 @@
         :param s: a string to check
         :type s: str
         :rtype: bool
         """
         return any(c.match(s) is not None for c in self._compiled_list)
 
 
-def convert_dir_regex_to_dir_prefix_regex(dir_regex):
+def convert_dir_regex_to_dir_prefix_regex(dir_regex: str | re.Pattern) -> str:
     """
     The patterns used to match directory names (and file names) are allowed
     to match a prefix of the name.  This 'feature' was unintentional, but is
     being retained for compatibility.
 
     This means that a regex that matches a directory name can't be used directly
     to match against a file name and test whether the file should be excluded
@@ -65,23 +61,25 @@
     On the other hand, the pattern 'photos$' should match 'photos/kitten.jpg',
     but not 'photos2/puppy.jpg', nor 'photos.txt'
 
     If the original regex is valid, there are only two cases to consider:
     either the regex ends in '$' or does not.
 
     :param dir_regex: a regular expression string or literal
-    :type dir_regex: str
+    :return: a regular expression string which matches the directory prefix
     """
+    if isinstance(dir_regex, re.Pattern):
+        dir_regex = dir_regex.pattern
     if dir_regex.endswith('$'):
         return dir_regex[:-1] + r'/'
     else:
         return dir_regex + r'.*?/'
 
 
-class IntegerRange(object):
+class IntegerRange:
     """
     Hold a range of two integers. If the range value is None, it indicates that
     the value should be treated as -Inf (for begin) or +Inf (for end).
     """
 
     def __init__(self, begin, end):
         """
@@ -106,38 +104,38 @@
             ge_begin = item >= self._begin
         if self._end is not None:
             le_end = item <= self._end
 
         return ge_begin and le_end
 
 
-class ScanPoliciesManager(object):
+class ScanPoliciesManager:
     """
-    Policy object used when scanning folders for syncing, used to decide
-    which files to include in the list of files to be synced.
+    Policy object used when scanning folders, used to decide
+    which files to include in the list of files.
 
     Code that scans through files should at least use should_exclude_file()
     to decide whether each file should be included; it will check include/exclude
     patterns for file names, as well as patterns for excluding directories.
 
     Code that scans may optionally use should_exclude_directory() to test whether
     it can skip a directory completely and not bother listing the files and
     sub-directories in it.
     """
 
     def __init__(
         self,
-        exclude_dir_regexes: Iterable[Union[str, regex_class]] = tuple(),
-        exclude_file_regexes: Iterable[Union[str, regex_class]] = tuple(),
-        include_file_regexes: Iterable[Union[str, regex_class]] = tuple(),
+        exclude_dir_regexes: Iterable[str | re.Pattern] = tuple(),
+        exclude_file_regexes: Iterable[str | re.Pattern] = tuple(),
+        include_file_regexes: Iterable[str | re.Pattern] = tuple(),
         exclude_all_symlinks: bool = False,
-        exclude_modified_before: Optional[int] = None,
-        exclude_modified_after: Optional[int] = None,
-        exclude_uploaded_before: Optional[int] = None,
-        exclude_uploaded_after: Optional[int] = None,
+        exclude_modified_before: int | None = None,
+        exclude_modified_after: int | None = None,
+        exclude_uploaded_before: int | None = None,
+        exclude_uploaded_after: int | None = None,
     ):
         """
         :param exclude_dir_regexes: regexes to exclude directories
         :param exclude_file_regexes: regexes to exclude files
         :param include_file_regexes: regexes to include files
         :param exclude_all_symlinks: if True, exclude all symlinks
         :param exclude_modified_before: optionally exclude file versions (both local and b2) modified before (in millis)
@@ -187,45 +185,45 @@
             )
 
     def _should_exclude_relative_path(self, relative_path: str):
         if self._include_file_set.matches(relative_path):
             return False
         return self._exclude_file_set.matches(relative_path)
 
-    def should_exclude_local_path(self, local_path: LocalSyncPath):
+    def should_exclude_local_path(self, local_path: LocalPath):
         """
-        Whether a local path should be excluded from the Sync or not.
+        Whether a local path should be excluded from the scan or not.
 
         This method assumes that the directory holding the `path_` has already been checked for exclusion.
         """
         if local_path.mod_time not in self._include_mod_time_range:
             return True
         return self._should_exclude_relative_path(local_path.relative_path)
 
     def should_exclude_b2_file_version(self, file_version: FileVersion, relative_path: str):
         """
-        Whether a b2 file version should be excluded from the Sync or not.
+        Whether a b2 file version should be excluded from the scan or not.
 
         This method assumes that the directory holding the `path_` has already been checked for exclusion.
         """
         if file_version.upload_timestamp not in self._include_upload_time_range:
             return True
         if file_version.mod_time_millis not in self._include_mod_time_range:
             return True
         return self._should_exclude_relative_path(relative_path)
 
     def should_exclude_b2_directory(self, dir_path: str):
         """
-        Given the path of a directory, relative to the sync point,
+        Given the path of a directory, relative to the scan point,
         decide if all of the files in it should be excluded from the scan.
         """
         return self._exclude_dir_set.matches(dir_path)
 
     def should_exclude_local_directory(self, dir_path: str):
         """
-        Given the path of a directory, relative to the sync point,
+        Given the path of a directory, relative to the scan point,
         decide if all of the files in it should be excluded from the scan.
         """
         return self._exclude_dir_set.matches(dir_path)
 
 
 DEFAULT_SCAN_MANAGER = ScanPoliciesManager()
```

### Comparing `b2sdk-1.9.0/b2sdk/sync/sync.py` & `b2sdk-2.0.0/b2sdk/_internal/sync/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,91 +1,47 @@
 ######################################################################
 #
-# File: b2sdk/sync/sync.py
+# File: b2sdk/_internal/sync/sync.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-import logging
 import concurrent.futures as futures
+import logging
 from enum import Enum, unique
+from typing import cast
 
 from ..bounded_queue_executor import BoundedQueueExecutor
-from .encryption_provider import AbstractSyncEncryptionSettingsProvider, SERVER_DEFAULT_SYNC_ENCRYPTION_SETTINGS_PROVIDER
-from .exception import InvalidArgument, IncompleteSync
-from .folder import AbstractFolder
-from .path import AbstractSyncPath
+from ..scan.exception import InvalidArgument
+from ..scan.folder import AbstractFolder, B2Folder, LocalFolder
+from ..scan.path import AbstractPath
+from ..scan.policies import DEFAULT_SCAN_MANAGER, ScanPoliciesManager
+from ..scan.scan import zip_folders
+from ..transfer.outbound.upload_source import UploadMode
+from .encryption_provider import (
+    SERVER_DEFAULT_SYNC_ENCRYPTION_SETTINGS_PROVIDER,
+    AbstractSyncEncryptionSettingsProvider,
+)
+from .exception import IncompleteSync
 from .policy import CompareVersionMode, NewerFileSyncMode
 from .policy_manager import POLICY_MANAGER, SyncPolicyManager
 from .report import SyncReport
-from .scan_policies import DEFAULT_SCAN_MANAGER
 
 logger = logging.getLogger(__name__)
 
 
-def next_or_none(iterator):
-    """
-    Return the next item from the iterator, or None if there are no more.
-    """
-    try:
-        return next(iterator)
-    except StopIteration:
-        return None
-
-
-def zip_folders(folder_a, folder_b, reporter, policies_manager=DEFAULT_SCAN_MANAGER):
-    """
-    Iterate over all of the files in the union of two folders,
-    matching file names.
-
-    Each item is a pair (file_a, file_b) with the corresponding file
-    in both folders.  Either file (but not both) will be None if the
-    file is in only one folder.
-
-    :param b2sdk.sync.folder.AbstractFolder folder_a: first folder object.
-    :param b2sdk.sync.folder.AbstractFolder folder_b: second folder object.
-    :param reporter: reporter object
-    :param policies_manager: policies manager object
-    :return: yields two element tuples
-    """
-
-    iter_a = folder_a.all_files(reporter, policies_manager)
-    iter_b = folder_b.all_files(reporter)
-
-    current_a = next_or_none(iter_a)
-    current_b = next_or_none(iter_b)
-
-    while current_a is not None or current_b is not None:
-        if current_a is None:
-            yield (None, current_b)
-            current_b = next_or_none(iter_b)
-        elif current_b is None:
-            yield (current_a, None)
-            current_a = next_or_none(iter_a)
-        elif current_a.relative_path < current_b.relative_path:
-            yield (current_a, None)
-            current_a = next_or_none(iter_a)
-        elif current_b.relative_path < current_a.relative_path:
-            yield (None, current_b)
-            current_b = next_or_none(iter_b)
-        else:
-            assert current_a.relative_path == current_b.relative_path
-            yield (current_a, current_b)
-            current_a = next_or_none(iter_a)
-            current_b = next_or_none(iter_b)
-
-
 def count_files(local_folder, reporter, policies_manager):
     """
     Count all of the files in a local folder.
 
-    :param b2sdk.sync.folder.AbstractFolder local_folder: a folder object.
+    :param b2sdk._internal.scan.folder.AbstractFolder local_folder: a folder object.
     :param reporter: reporter object
     """
     # Don't pass in a reporter to all_files.  Broken symlinks will be reported
     # during the next pass when the source and dest files are compared.
     for _ in local_folder.all_files(None, policies_manager=policies_manager):
         reporter.update_total(1)
     reporter.end_total()
@@ -131,37 +87,46 @@
         dry_run=False,
         allow_empty_source=False,
         newer_file_mode=NewerFileSyncMode.RAISE_ERROR,
         keep_days_or_delete=KeepOrDeleteMode.NO_DELETE,
         compare_version_mode=CompareVersionMode.MODTIME,
         compare_threshold=None,
         keep_days=None,
+        sync_policy_manager: SyncPolicyManager = POLICY_MANAGER,
+        upload_mode: UploadMode = UploadMode.FULL,
+        absolute_minimum_part_size: int | None = None,
     ):
         """
         Initialize synchronizer class and validate arguments
 
         :param int max_workers: max number of workers
-        :param policies_manager: policies manager object
+        :param policies_manager: object which decides which files to process
         :param bool dry_run: test mode, does not actually transfer/delete when enabled
         :param bool allow_empty_source: if True, do not check whether source folder is empty
-        :param b2sdk.v1.NewerFileSyncMode newer_file_mode: setting which determines handling for destination files newer than on the source
-        :param b2sdk.v1.KeepOrDeleteMode keep_days_or_delete: setting which determines if we should delete or not delete or keep for `keep_days`
-        :param b2sdk.v1.CompareVersionMode compare_version_mode: how to compare the source and destination files to find new ones
+        :param b2sdk.v2.NewerFileSyncMode newer_file_mode: setting which determines handling for destination files newer than on the source
+        :param b2sdk.v2.KeepOrDeleteMode keep_days_or_delete: setting which determines if we should delete or not delete or keep for `keep_days`
+        :param b2sdk.v2.CompareVersionMode compare_version_mode: how to compare the source and destination files to find new ones
         :param int compare_threshold: should be greater than 0, default is 0
-        :param int keep_days: if keep_days_or_delete is `b2sdk.v1.KeepOrDeleteMode.KEEP_BEFORE_DELETE`, then this should be greater than 0
+        :param int keep_days: if keep_days_or_delete is `b2sdk.v2.KeepOrDeleteMode.KEEP_BEFORE_DELETE`, then this should be greater than 0
+        :param SyncPolicyManager sync_policy_manager: object which decides what to do with each file (upload, download, delete, copy, hide etc)
+        :param b2sdk.v2.UploadMode upload_mode: determines how file uploads are handled
+        :param int absolute_minimum_part_size: minimum file part size for large files
         """
         self.newer_file_mode = newer_file_mode
         self.keep_days_or_delete = keep_days_or_delete
         self.keep_days = keep_days
         self.compare_version_mode = compare_version_mode
         self.compare_threshold = compare_threshold or 0
         self.dry_run = dry_run
         self.allow_empty_source = allow_empty_source
-        self.policies_manager = policies_manager
+        self.policies_manager = policies_manager  # actually it should be called scan_policies_manager
+        self.sync_policy_manager = sync_policy_manager
         self.max_workers = max_workers
+        self.upload_mode = upload_mode
+        self.absolute_minimum_part_size = absolute_minimum_part_size
         self._validate()
 
     def _validate(self):
         if self.compare_threshold < 0:
             raise InvalidArgument('compare_threshold', 'must be a positive integer')
 
         if self.newer_file_mode not in tuple(NewerFileSyncMode):
@@ -186,44 +151,44 @@
             raise InvalidArgument(
                 'compare_version_mode',
                 'must be one of :%s' % CompareVersionMode.__members__,
             )
 
     def sync_folders(
         self,
-        source_folder,
-        dest_folder,
-        now_millis,
-        reporter,
+        source_folder: AbstractFolder,
+        dest_folder: AbstractFolder,
+        now_millis: int,
+        reporter: SyncReport | None,
         encryption_settings_provider:
         AbstractSyncEncryptionSettingsProvider = SERVER_DEFAULT_SYNC_ENCRYPTION_SETTINGS_PROVIDER,
     ):
         """
         Syncs two folders.  Always ensures that every file in the
         source is also in the destination.  Deletes any file versions
         in the destination older than history_days.
 
-        :param b2sdk.sync.folder.AbstractFolder source_folder: source folder object
-        :param b2sdk.sync.folder.AbstractFolder dest_folder: destination folder object
-        :param int now_millis: current time in milliseconds
-        :param b2sdk.sync.report.SyncReport,None reporter: progress reporter
-        :param b2sdk.v1.AbstractSyncEncryptionSettingsProvider encryption_settings_provider: encryption setting provider
+        :param source_folder: source folder object
+        :param dest_folder: destination folder object
+        :param now_millis: current time in milliseconds
+        :param reporter: progress reporter
+        :param encryption_settings_provider: encryption setting provider
         """
         source_type = source_folder.folder_type()
         dest_type = dest_folder.folder_type()
 
         if source_type != 'b2' and dest_type != 'b2':
             raise ValueError('Sync between two local folders is not supported!')
 
         # For downloads, make sure that the target directory is there.
         if dest_type == 'local' and not self.dry_run:
-            dest_folder.ensure_present()
+            cast(LocalFolder, dest_folder).ensure_present()
 
         if source_type == 'local' and not self.allow_empty_source:
-            source_folder.ensure_non_empty()
+            cast(LocalFolder, source_folder).ensure_non_empty()
 
         # Make an executor to count files and run all of the actions. This is
         # not the same as the executor in the API object which is used for
         # uploads. The tasks in this executor wait for uploads. Putting them
         # in the same thread pool could lead to deadlock.
         #
         # We use an executor with a bounded queue to avoid using up lots of memory
@@ -237,17 +202,17 @@
             # that should be fastest, and it provides scale for the progress reporting.
             sync_executor.submit(count_files, source_folder, reporter, self.policies_manager)
 
         # Bucket for scheduling actions.
         # For bucket-to-bucket sync, the bucket for the API calls should be the destination.
         action_bucket = None
         if dest_type == 'b2':
-            action_bucket = dest_folder.bucket
+            action_bucket = cast(B2Folder, dest_folder).bucket
         elif source_type == 'b2':
-            action_bucket = source_folder.bucket
+            action_bucket = cast(B2Folder, source_folder).bucket
 
         # Schedule each of the actions.
         for action in self._make_folder_sync_actions(
             source_folder,
             dest_folder,
             now_millis,
             reporter,
@@ -264,36 +229,36 @@
 
     def _make_folder_sync_actions(
         self,
         source_folder: AbstractFolder,
         dest_folder: AbstractFolder,
         now_millis: int,
         reporter: SyncReport,
-        policies_manager: SyncPolicyManager = DEFAULT_SCAN_MANAGER,
+        policies_manager: ScanPoliciesManager = DEFAULT_SCAN_MANAGER,
         encryption_settings_provider:
         AbstractSyncEncryptionSettingsProvider = SERVER_DEFAULT_SYNC_ENCRYPTION_SETTINGS_PROVIDER,
     ):
         """
         Yield a sequence of actions that will sync the destination
         folder to the source folder.
 
-        :param b2sdk.v1.AbstractFolder source_folder: source folder object
-        :param b2sdk.v1.AbstractFolder dest_folder: destination folder object
-        :param int now_millis: current time in milliseconds
-        :param b2sdk.v1.SyncReport reporter: reporter object
-        :param b2sdk.v1.SyncPolicyManager policies_manager: policies manager object
-        :param b2sdk.v1.AbstractSyncEncryptionSettingsProvider encryption_settings_provider: encryption setting provider
+        :param source_folder: source folder object
+        :param dest_folder: destination folder object
+        :param now_millis: current time in milliseconds
+        :param reporter: reporter object
+        :param policies_manager: object which decides which files to process
+        :param encryption_settings_provider: encryption setting provider
         """
         if self.keep_days_or_delete == KeepOrDeleteMode.KEEP_BEFORE_DELETE and dest_folder.folder_type(
         ) == 'local':
             raise InvalidArgument('keep_days_or_delete', 'cannot be used for local files')
 
         source_type = source_folder.folder_type()
         dest_type = dest_folder.folder_type()
-        sync_type = '%s-to-%s' % (source_type, dest_type)
+        sync_type = f'{source_type}-to-{dest_type}'
         if source_type != 'b2' and dest_type != 'b2':
             raise ValueError('Sync between two local folders is not supported!')
 
         total_files = 0
         total_bytes = 0
         for source_path, dest_path in zip_folders(
             source_folder,
@@ -332,44 +297,45 @@
                 # more API calls. Instead, we count them when comparing.
                 reporter.end_total()
             reporter.end_compare(total_files, total_bytes)
 
     def _make_file_sync_actions(
         self,
         sync_type: str,
-        source_path: AbstractSyncPath,
-        dest_path: AbstractSyncPath,
+        source_path: AbstractPath | None,
+        dest_path: AbstractPath | None,
         source_folder: AbstractFolder,
         dest_folder: AbstractFolder,
         now_millis: int,
         encryption_settings_provider:
         AbstractSyncEncryptionSettingsProvider = SERVER_DEFAULT_SYNC_ENCRYPTION_SETTINGS_PROVIDER,
     ):
         """
         Yields the sequence of actions needed to sync the two files
 
-        :param str sync_type: synchronization type
-        :param b2sdk.v1.AbstractSyncPath source_path: source file object
-        :param b2sdk.v1.AbstractSyncPath dest_path: destination file object
-        :param b2sdk.v1.AbstractFolder source_folder: a source folder object
-        :param b2sdk.v1.AbstractFolder dest_folder: a destination folder object
-        :param int now_millis: current time in milliseconds
-        :param b2sdk.v1.AbstractSyncEncryptionSettingsProvider encryption_settings_provider: encryption setting provider
+        :param sync_type: synchronization type
+        :param source_path: source file object
+        :param dest_path: destination file object
+        :param source_folder: a source folder object
+        :param dest_folder: a destination folder object
+        :param now_millis: current time in milliseconds
+        :param encryption_settings_provider: encryption setting provider
         """
         delete = self.keep_days_or_delete == KeepOrDeleteMode.DELETE
-        keep_days = self.keep_days
 
-        policy = POLICY_MANAGER.get_policy(
+        policy = self.sync_policy_manager.get_policy(
             sync_type,
             source_path,
             source_folder,
             dest_path,
             dest_folder,
             now_millis,
             delete,
-            keep_days,
+            self.keep_days,
             self.newer_file_mode,
             self.compare_threshold,
             self.compare_version_mode,
             encryption_settings_provider=encryption_settings_provider,
+            upload_mode=self.upload_mode,
+            absolute_minimum_part_size=self.absolute_minimum_part_size,
         )
         return policy.get_all_actions()
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/__init__.py` & `b2sdk-2.0.0/b2sdk/_internal/transfer/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 ######################################################################
 #
-# File: b2sdk/transfer/__init__.py
+# File: b2sdk/_internal/transfer/__init__.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 from .inbound.download_manager import DownloadManager
 from .outbound.copy_manager import CopyManager
 from .outbound.upload_manager import UploadManager
 from .emerge.emerger import Emerger
 
 __all__ = [
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/emerge/executor.py` & `b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,87 @@
 ######################################################################
 #
-# File: b2sdk/transfer/emerge/executor.py
+# File: b2sdk/_internal/transfer/emerge/executor.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
+import logging
 import threading
-
 from abc import ABCMeta, abstractmethod
-from typing import Optional
+from typing import TYPE_CHECKING
 
-from b2sdk.encryption.setting import EncryptionSetting
-from b2sdk.exception import MaxFileSizeExceeded
-from b2sdk.file_lock import FileRetentionSetting, LegalHold, NO_RETENTION_FILE_SETTING
-from b2sdk.transfer.outbound.large_file_upload_state import LargeFileUploadState
-from b2sdk.transfer.outbound.upload_source import UploadSourceStream
-from b2sdk.utils import interruptible_get_result
+from b2sdk._internal.encryption.setting import EncryptionSetting
+from b2sdk._internal.exception import MaxFileSizeExceeded
+from b2sdk._internal.file_lock import NO_RETENTION_FILE_SETTING, FileRetentionSetting, LegalHold
+from b2sdk._internal.http_constants import LARGE_FILE_SHA1
+from b2sdk._internal.transfer.outbound.large_file_upload_state import LargeFileUploadState
+from b2sdk._internal.transfer.outbound.upload_source import UploadSourceStream
 
 AUTO_CONTENT_TYPE = 'b2/x-auto'
 
+logger = logging.getLogger(__name__)
+
+if TYPE_CHECKING:
+    from b2sdk._internal.transfer.emerge.planner.part_definition import UploadEmergePartDefinition
+    from b2sdk._internal.transfer.emerge.planner.planner import StreamingEmergePlan
+
 
-class EmergeExecutor(object):
+class EmergeExecutor:
     def __init__(self, services):
         self.services = services
 
     def execute_emerge_plan(
         self,
         emerge_plan,
         bucket_id,
         file_name,
         content_type,
         file_info,
         progress_listener,
         continue_large_file_id=None,
         max_queue_size=None,
-        encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
     ):
         if emerge_plan.is_large_file():
             execution = LargeFileEmergeExecution(
                 self.services,
                 bucket_id,
                 file_name,
                 content_type,
                 file_info,
                 progress_listener,
                 encryption=encryption,
                 file_retention=file_retention,
                 legal_hold=legal_hold,
                 continue_large_file_id=continue_large_file_id,
                 max_queue_size=max_queue_size,
+                custom_upload_timestamp=custom_upload_timestamp,
             )
         else:
             if continue_large_file_id is not None:
                 raise ValueError('Cannot resume emerging single part plan.')
             execution = SmallFileEmergeExecution(
                 self.services,
                 bucket_id,
                 file_name,
                 content_type,
                 file_info,
                 progress_listener,
                 encryption=encryption,
                 file_retention=file_retention,
                 legal_hold=legal_hold,
+                custom_upload_timestamp=custom_upload_timestamp,
             )
         return execution.execute_plan(emerge_plan)
 
 
 class BaseEmergeExecution(metaclass=ABCMeta):
     DEFAULT_CONTENT_TYPE = AUTO_CONTENT_TYPE
 
@@ -79,27 +89,29 @@
         self,
         services,
         bucket_id,
         file_name,
         content_type,
         file_info,
         progress_listener,
-        encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
     ):
         self.services = services
         self.bucket_id = bucket_id
         self.file_name = file_name
         self.content_type = content_type
         self.file_info = file_info
         self.progress_listener = progress_listener
         self.encryption = encryption
         self.file_retention = file_retention
         self.legal_hold = legal_hold
+        self.custom_upload_timestamp = custom_upload_timestamp
 
     @abstractmethod
     def execute_plan(self, emerge_plan):
         pass
 
 
 class SmallFileEmergeExecution(BaseEmergeExecution):
@@ -120,38 +132,40 @@
         self,
         services,
         bucket_id,
         file_name,
         content_type,
         file_info,
         progress_listener,
-        encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
         continue_large_file_id=None,
         max_queue_size=None,
+        custom_upload_timestamp: int | None = None,
     ):
-        super(LargeFileEmergeExecution, self).__init__(
+        super().__init__(
             services,
             bucket_id,
             file_name,
             content_type,
             file_info,
             progress_listener,
             encryption=encryption,
             file_retention=file_retention,
             legal_hold=legal_hold,
+            custom_upload_timestamp=custom_upload_timestamp,
         )
         self.continue_large_file_id = continue_large_file_id
         self.max_queue_size = max_queue_size
         self._semaphore = None
         if self.max_queue_size is not None:
             self._semaphore = threading.Semaphore(self.max_queue_size)
 
-    def execute_plan(self, emerge_plan):
+    def execute_plan(self, emerge_plan: StreamingEmergePlan):
         total_length = emerge_plan.get_total_length()
         encryption = self.encryption
 
         if total_length is not None and total_length > self.MAX_LARGE_FILE_SIZE:
             raise MaxFileSizeExceeded(total_length, self.MAX_LARGE_FILE_SIZE)
 
         plan_id = emerge_plan.get_plan_id()
@@ -171,14 +185,15 @@
             self.file_name,
             file_info,
             self.continue_large_file_id,
             encryption=encryption,
             file_retention=self.file_retention,
             legal_hold=self.legal_hold,
             emerge_parts_dict=emerge_parts_dict,
+            custom_upload_timestamp=self.custom_upload_timestamp,
         )
 
         if unfinished_file is None:
             if self.content_type is None:
                 content_type = self.DEFAULT_CONTENT_TYPE
             else:
                 content_type = self.content_type
@@ -189,42 +204,41 @@
                 file_info,
                 encryption=encryption,
                 file_retention=self.file_retention,
                 legal_hold=self.legal_hold,
             )
         file_id = unfinished_file.file_id
 
-        with self.progress_listener:
-            large_file_upload_state = LargeFileUploadState(self.progress_listener)
+        large_file_upload_state = LargeFileUploadState(self.progress_listener)
 
-            part_futures = []
-            for part_number, emerge_part in emerge_plan.enumerate_emerge_parts():
-                execution_step_factory = LargeFileEmergeExecutionStepFactory(
-                    self,
-                    emerge_part,
-                    part_number,
-                    file_id,
-                    large_file_upload_state,
-                    finished_parts=finished_parts,
-                    # it already knows encryption from BaseMergeExecution being passed as self
-                )
-                execution_step = execution_step_factory.get_execution_step()
-                future = self._execute_step(execution_step)
-                part_futures.append(future)
-
-            # Collect the sha1 checksums of the parts as the uploads finish.
-            # If any of them raised an exception, that same exception will
-            # be raised here by result()
-            part_sha1_array = [interruptible_get_result(f)['contentSha1'] for f in part_futures]
+        part_futures = []
+        for part_number, emerge_part in emerge_plan.enumerate_emerge_parts():
+            execution_step_factory = LargeFileEmergeExecutionStepFactory(
+                self,
+                emerge_part,
+                part_number,
+                file_id,
+                large_file_upload_state,
+                finished_parts=finished_parts,
+                # it already knows encryption from BaseMergeExecution being passed as self
+            )
+            execution_step = execution_step_factory.get_execution_step()
+            future = self._execute_step(execution_step)
+            part_futures.append(future)
+
+        # Collect the sha1 checksums of the parts as the uploads finish.
+        # If any of them raised an exception, that same exception will
+        # be raised here by result()
+        part_sha1_array = [f.result()['contentSha1'] for f in part_futures]
 
         # Finish the large file
         response = self.services.session.finish_large_file(file_id, part_sha1_array)
         return self.services.api.file_version_factory.from_api_response(response)
 
-    def _execute_step(self, execution_step):
+    def _execute_step(self, execution_step: UploadPartExecutionStep):
         semaphore = self._semaphore
         if semaphore is None:
             return execution_step.execute()
         else:
             semaphore.acquire()
             try:
                 future = execution_step.execute()
@@ -238,17 +252,18 @@
     def _get_unfinished_file_and_parts(
         self,
         bucket_id,
         file_name,
         file_info,
         continue_large_file_id,
         encryption: EncryptionSetting,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
         emerge_parts_dict=None,
+        custom_upload_timestamp: int | None = None,
     ):
         if 'listFiles' not in self.services.session.account_info.get_allowed()['capabilities']:
             return None, {}
 
         unfinished_file = None
         finished_parts = {}
 
@@ -272,156 +287,277 @@
                 bucket_id,
                 file_name,
                 file_info,
                 emerge_parts_dict,
                 encryption,
                 file_retention,
                 legal_hold,
+                custom_upload_timestamp=custom_upload_timestamp,
             )
         elif emerge_parts_dict is not None:
             unfinished_file, finished_parts = self._match_unfinished_file_if_possible(
                 bucket_id,
                 file_name,
                 file_info,
                 emerge_parts_dict,
                 encryption,
                 file_retention,
                 legal_hold,
+                custom_upload_timestamp=custom_upload_timestamp,
             )
         return unfinished_file, finished_parts
 
-    def _find_unfinished_file_by_plan_id(
+    def _find_matching_unfinished_file(
         self,
         bucket_id,
         file_name,
         file_info,
         emerge_parts_dict,
         encryption: EncryptionSetting,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
+        check_file_info_without_large_file_sha1: bool | None = False,
+        eager_mode: bool | None = False,
     ):
+        """
+        Search for a matching unfinished large file in the specified bucket.
+
+        In case a matching file is found but has inconsistencies (for example, mismatching file info or encryption settings),
+        mismatches are logged.
+
+        :param bucket_id: The identifier of the bucket where the unfinished file resides.
+        :param file_name: The name of the file to be matched.
+        :param file_info: Information about the file to be uploaded.
+        :param emerge_parts_dict: A dictionary containing the parts of the file to be emerged.
+        :param encryption: The encryption settings for the file.
+        :param file_retention: The retention settings for the file, if any.
+        :param legal_hold: The legal hold status of the file, if any.
+        :param custom_upload_timestamp: The custom timestamp for the upload, if any.
+        :param check_file_info_without_large_file_sha1: A flag indicating whether the file information should be checked without the `large_file_sha1`.
+        :param eager_mode: A flag indicating whether the first matching file should be returned.
+        
+        :return: A tuple of the best matching unfinished file and its finished parts. If no match is found, returns `None`.
+        """
+
         file_retention = file_retention or NO_RETENTION_FILE_SETTING
-        assert 'plan_id' in file_info
         best_match_file = None
         best_match_parts = {}
         best_match_parts_len = 0
+
         for file_ in self.services.large_file.list_unfinished_large_files(
             bucket_id, prefix=file_name
         ):
-            if file_.file_info != file_info:
+            if file_.file_name != file_name:
+                logger.debug('Rejecting %s: file name mismatch', file_.file_id)
                 continue
-            # FIXME: encryption is None ???
-            if encryption is None or file_.encryption != encryption:
+
+            if file_.file_info != file_info:
+                if check_file_info_without_large_file_sha1:
+                    file_info_without_large_file_sha1 = self._get_file_info_without_large_file_sha1(
+                        file_info
+                    )
+                    if file_info_without_large_file_sha1 != self._get_file_info_without_large_file_sha1(
+                        file_.file_info
+                    ):
+                        logger.debug(
+                            'Rejecting %s: file info mismatch after dropping `large_file_sha1`',
+                            file_.file_id
+                        )
+                        continue
+                else:
+                    logger.debug('Rejecting %s: file info mismatch', file_.file_id)
+                    continue
+
+            if encryption is not None and encryption != file_.encryption:
+                logger.debug('Rejecting %s: encryption mismatch', file_.file_id)
                 continue
 
             if legal_hold is None:
                 if LegalHold.UNSET != file_.legal_hold:
-                    # Uploading and not providing legal_hold means that server's response about that file version
-                    # will have legal_hold=LegalHold.UNSET
+                    logger.debug('Rejecting %s: legal hold mismatch (not unset)', file_.file_id)
                     continue
             elif legal_hold != file_.legal_hold:
+                logger.debug('Rejecting %s: legal hold mismatch', file_.file_id)
                 continue
 
             if file_retention != file_.file_retention:
-                # if `file_.file_retention` is UNKNOWN then we skip - lib user can still
-                # pass UKNOWN file_retention here - but raw_api/server won't allow it
-                # and we don't check it here
+                logger.debug('Rejecting %s: retention mismatch', file_.file_id)
+                continue
+
+            if custom_upload_timestamp is not None and file_.upload_timestamp != custom_upload_timestamp:
+                logger.debug('Rejecting %s: custom_upload_timestamp mismatch', file_.file_id)
                 continue
+
             finished_parts = {}
+
             for part in self.services.large_file.list_parts(file_.file_id):
+
                 emerge_part = emerge_parts_dict.get(part.part_number)
+
                 if emerge_part is None:
-                    # large file with same `plan_id` has more parts than current plan
-                    # so we want to skip this large file because it is broken
+                    # something is wrong - we have a part that we don't know about
+                    # so we can't resume this upload
+                    logger.debug(
+                        'Rejecting %s: part %s not found in emerge parts, giving up.',
+                        file_.file_id, part.part_number
+                    )
                     finished_parts = None
                     break
+
+                # Compare part sizes
+                if emerge_part.get_length() != part.content_length:
+                    logger.debug(
+                        'Rejecting %s: part %s size mismatch', file_.file_id, part.part_number
+                    )
+                    continue  # part size doesn't match - so we reupload
+
+                # Compare part hashes
                 if emerge_part.is_hashable() and emerge_part.get_sha1() != part.content_sha1:
-                    continue  # auto-healing - `plan_id` matches but part.sha1 doesn't - so we reupload
+                    logger.debug(
+                        'Rejecting %s: part %s sha1 mismatch', file_.file_id, part.part_number
+                    )
+                    continue  # part.sha1 doesn't match - so we reupload
+
                 finished_parts[part.part_number] = part
+
             if finished_parts is None:
                 continue
+
             finished_parts_len = len(finished_parts)
-            if best_match_file is None or finished_parts_len > best_match_parts_len:
+
+            if finished_parts and (
+                best_match_file is None or finished_parts_len > best_match_parts_len
+            ):
                 best_match_file = file_
                 best_match_parts = finished_parts
                 best_match_parts_len = finished_parts_len
+
+            if eager_mode and best_match_file is not None:
+                break
+
         return best_match_file, best_match_parts
 
-    def _match_unfinished_file_if_possible(
+    def _find_unfinished_file_by_plan_id(
         self,
         bucket_id,
         file_name,
         file_info,
         emerge_parts_dict,
         encryption: EncryptionSetting,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
     ):
         """
-        Find an unfinished file that may be used to resume a large file upload.  The
-        file is found using the filename and comparing the uploaded parts against
-        the local file.
+        Search for a matching unfinished large file by plan_id in the specified bucket.
 
-        This is only possible if the application key being used allows ``listFiles`` access.
+        This function aims to locate a matching unfinished large file using the plan_id and the supplied parameters. 
+        It's used to resume an interrupted upload, centralizing the shared logic between `_find_unfinished_file_by_plan_id` 
+        and `_match_unfinished_file_if_possible`.
+
+        In case a matching file is found but has inconsistencies (for example, mismatching file info or encryption settings), 
+        the function checks if 'plan_id' is in file_info, as this is a prerequisite.
+
+        :param bucket_id: The identifier of the bucket where the unfinished file resides.
+        :param file_name: The name of the file to be matched.
+        :param file_info: Information about the file to be uploaded.
+        :param emerge_parts_dict: A dictionary containing the parts of the file to be emerged.
+        :param encryption: The encryption settings for the file.
+        :param file_retention: The retention settings for the file, if any.
+        :param legal_hold: The legal hold status of the file, if any.
+        :param custom_upload_timestamp: The custom timestamp for the upload, if any.
+        
+        :return: A tuple of the best matching unfinished file and its finished parts. If no match is found, it returns `None`.
         """
-        file_retention = file_retention or NO_RETENTION_FILE_SETTING
-        for file_ in self.services.large_file.list_unfinished_large_files(
-            bucket_id, prefix=file_name
-        ):
-            if file_.file_name != file_name:
-                continue
-            if file_.file_info != file_info:
-                continue
-            # FIXME: what if `encryption is None` - match ANY encryption? :)
-            if encryption is not None and encryption != file_.encryption:
-                continue
+        if 'plan_id' not in file_info:
+            raise ValueError("The 'plan_id' key must be in file_info dictionary.")
 
-            if legal_hold is None:
-                if LegalHold.UNSET != file_.legal_hold:
-                    # Uploading and not providing legal_hold means that server's response about that file version
-                    # will have legal_hold=LegalHold.UNSET
-                    continue
-            elif legal_hold != file_.legal_hold:
-                continue
+        return self._find_matching_unfinished_file(
+            bucket_id=bucket_id,
+            file_name=file_name,
+            file_info=file_info,
+            emerge_parts_dict=emerge_parts_dict,
+            encryption=encryption,
+            file_retention=file_retention or NO_RETENTION_FILE_SETTING,
+            legal_hold=legal_hold,
+            custom_upload_timestamp=custom_upload_timestamp,
+            check_file_info_without_large_file_sha1=False,
+        )
 
-            if file_retention != file_.file_retention:
-                # if `file_.file_retention` is UNKNOWN then we skip - lib user can still
-                # pass UKNOWN file_retention here - but raw_api/server won't allow it
-                # and we don't check it here
-                continue
-            files_match = True
-            finished_parts = {}
-            for part in self.services.large_file.list_parts(file_.file_id):
-                emerge_part = emerge_parts_dict.get(part.part_number)
-                if emerge_part is None:
-                    files_match = False
-                    break
+    @classmethod
+    def _get_file_info_without_large_file_sha1(
+        cls,
+        file_info: dict[str, str] | None,
+    ) -> dict[str, str] | None:
+        if not file_info or LARGE_FILE_SHA1 not in file_info:
+            return file_info
+        out_file_info = dict(file_info)
+        del out_file_info[LARGE_FILE_SHA1]
+        return out_file_info
 
-                # Compare part sizes
-                if emerge_part.get_length() != part.content_length:
-                    files_match = False
-                    break
+    def _match_unfinished_file_if_possible(
+        self,
+        bucket_id,
+        file_name,
+        file_info,
+        emerge_parts_dict,
+        encryption: EncryptionSetting,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
+    ):
+        """
+        Scan for a suitable unfinished large file in the specified bucket to resume upload.
 
-                # Compare hash
-                assert emerge_part.is_hashable()
-                sha1_sum = emerge_part.get_sha1()
-                if sha1_sum != part.content_sha1:
-                    files_match = False
-                    break
+        This function examines each unfinished large file for a possible match with the provided
+        parameters. This enables resumption of an interrupted upload by reusing the unfinished file,
+        provided that file's info and additional parameters match.
+
+        Along with the filename and file info, additional parameters like encryption, file retention,
+        legal hold, custom upload timestamp, and cache control are compared for a match. The
+        'emerge_parts_dict' is also cross-checked for matching file parts.
+
+        Function is eager to find a match, and will return the first match it finds. If no match is
+        found, it returns `None`.
+
+        :param bucket_id: The identifier of the bucket containing the unfinished file.
+        :param file_name: The name of the file to find.
+        :param file_info: Information about the file to be uploaded.
+        :param emerge_parts_dict: A dictionary of the parts of the file to be emerged.
+        :param encryption: The encryption settings for the file.
+        :param file_retention: The retention settings for the file, if applicable.
+        :param legal_hold: The legal hold status of the file, if applicable.
+        :param custom_upload_timestamp: The custom timestamp for the upload, if set.
+        
+        :return: A tuple of the best matching unfinished file and its finished parts. If no match is found, returns `None`.
+        """
+        logger.debug('Checking for matching unfinished large files for %s...', file_name)
 
-                # Save part
-                finished_parts[part.part_number] = part
+        file_, finished_parts = self._find_matching_unfinished_file(
+            bucket_id,
+            file_name,
+            file_info,
+            emerge_parts_dict,
+            encryption,
+            file_retention,
+            legal_hold,
+            custom_upload_timestamp,
+            check_file_info_without_large_file_sha1=True,
+            eager_mode=True,
+        )
 
-            # Skip not matching files or unfinished files with no uploaded parts
-            if not files_match or not finished_parts:
-                continue
+        if file_ is None:
+            logger.debug('No matching unfinished files found.')
+            return None, {}
 
-            # Return first matched file
-            return file_, finished_parts
-        return None, {}
+        logger.debug(
+            'Unfinished file %s matches with %i finished parts', file_.file_id, len(finished_parts)
+        )
+        return file_, finished_parts
 
 
 class BaseExecutionStepFactory(metaclass=ABCMeta):
     def __init__(self, emerge_execution, emerge_part):
         self.emerge_execution = emerge_execution
         self.emerge_part = emerge_part
 
@@ -450,21 +586,21 @@
         )
 
 
 class LargeFileEmergeExecutionStepFactory(BaseExecutionStepFactory):
     def __init__(
         self,
         emerge_execution,
-        emerge_part,
+        emerge_part: UploadEmergePartDefinition,
         part_number,
         large_file_id,
         large_file_upload_state,
         finished_parts=None,
     ):
-        super(LargeFileEmergeExecutionStepFactory, self).__init__(emerge_execution, emerge_part)
+        super().__init__(emerge_execution, emerge_part)
         self.part_number = part_number
         self.large_file_id = large_file_id
         self.large_file_upload_state = large_file_upload_state
         self.finished_parts = finished_parts or {}
 
     def create_copy_execution_step(self, copy_range):
         return CopyPartExecutionStep(
@@ -574,14 +710,15 @@
             execution.file_name,
             execution.content_type or execution.DEFAULT_CONTENT_TYPE,
             execution.file_info or {},
             execution.progress_listener,
             encryption=execution.encryption,
             file_retention=execution.file_retention,
             legal_hold=execution.legal_hold,
+            custom_upload_timestamp=execution.custom_upload_timestamp,
         )
 
 
 class UploadPartExecutionStep(BaseExecutionStep):
     def __init__(
         self,
         emerge_execution,
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/emerge/planner/part_definition.py` & `b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/planner/part_definition.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 ######################################################################
 #
-# File: b2sdk/transfer/emerge/planner/part_definition.py
+# File: b2sdk/_internal/transfer/emerge/planner/part_definition.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 from functools import partial
+from typing import TYPE_CHECKING
 
-from b2sdk.stream.chained import ChainedStream
-from b2sdk.stream.range import wrap_with_range
+from b2sdk._internal.stream.chained import ChainedStream
+from b2sdk._internal.stream.range import wrap_with_range
+from b2sdk._internal.utils import hex_sha1_of_unlimited_stream
 
-from b2sdk.utils import hex_sha1_of_unlimited_stream
+if TYPE_CHECKING:
+    from b2sdk._internal.transfer.emerge.unbound_write_intent import UnboundSourceBytes
 
 
 class BaseEmergePartDefinition(metaclass=ABCMeta):
     @abstractmethod
     def get_length(self):
         pass
 
@@ -34,15 +38,15 @@
         return False
 
     def get_sha1(self):
         return None
 
 
 class UploadEmergePartDefinition(BaseEmergePartDefinition):
-    def __init__(self, upload_source, relative_offset, length):
+    def __init__(self, upload_source: UnboundSourceBytes, relative_offset, length):
         self.upload_source = upload_source
         self.relative_offset = relative_offset
         self.length = length
         self._sha1 = None
 
     def __repr__(self):
         return (
@@ -92,18 +96,15 @@
 class UploadSubpartsEmergePartDefinition(BaseEmergePartDefinition):
     def __init__(self, upload_subparts):
         self.upload_subparts = upload_subparts
         self._is_hashable = all(subpart.is_hashable() for subpart in upload_subparts)
         self._sha1 = None
 
     def __repr__(self):
-        return '<{classname} upload_subparts={upload_subparts}>'.format(
-            classname=self.__class__.__name__,
-            upload_subparts=repr(self.upload_subparts),
-        )
+        return f'<{self.__class__.__name__} upload_subparts={repr(self.upload_subparts)}>'
 
     def get_length(self):
         return sum(subpart.length for subpart in self.upload_subparts)
 
     def get_part_id(self):
         if self.is_hashable():
             return self.get_sha1()
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/emerge/planner/planner.py` & `b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/planner/planner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 ######################################################################
 #
-# File: b2sdk/transfer/emerge/planner/planner.py
+# File: b2sdk/_internal/transfer/emerge/planner/planner.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import hashlib
 import json
-
+import typing
 from abc import ABCMeta, abstractmethod
 from collections import deque
-from itertools import chain
+from math import ceil
 
-from b2sdk.transfer.emerge.planner.part_definition import (
+from b2sdk._internal.exception import InvalidUserInput
+from b2sdk._internal.http_constants import (
+    DEFAULT_MAX_PART_SIZE,
+    DEFAULT_MIN_PART_SIZE,
+    DEFAULT_RECOMMENDED_UPLOAD_PART_SIZE,
+)
+from b2sdk._internal.transfer.emerge.planner.part_definition import (
     CopyEmergePartDefinition,
     UploadEmergePartDefinition,
     UploadSubpartsEmergePartDefinition,
 )
-from b2sdk.transfer.emerge.planner.upload_subpart import (
+from b2sdk._internal.transfer.emerge.planner.upload_subpart import (
     LocalSourceUploadSubpart,
     RemoteSourceUploadSubpart,
 )
+from b2sdk._internal.utils import iterator_peek
 
-MEGABYTE = 1000 * 1000
-GIGABYTE = 1000 * MEGABYTE
+if typing.TYPE_CHECKING:
+    from b2sdk._internal.account_info.abstract import AbstractAccountInfo
 
 
-class UploadBuffer(object):
+class UploadBuffer:
     """ data container used by EmergePlanner for temporary storage of write intents """
 
     def __init__(self, start_offset, buff=None):
         self._start_offset = start_offset
         self._buff = buff or []
         if self._buff:
             self._end_offset = self._buff[-1][1]
@@ -75,60 +83,118 @@
             if start_idx == 0:
                 start_offset = self.start_offset
             else:
                 start_offset = self._buff[start_idx - 1:start_idx][0][1]
         return self.__class__(start_offset, buff_slice)
 
 
-class EmergePlanner(object):
+def _filter_out_none(*args):
+    return (arg for arg in args if arg is not None)
+
+
+class EmergePlanner:
     """ Creates a list of actions required for advanced creation of an object in the cloud from an iterator of write intent objects """
-    DEFAULT_MIN_PART_SIZE = 5 * MEGABYTE
-    DEFAULT_RECOMMENDED_UPLOAD_PART_SIZE = 100 * MEGABYTE
-    DEFAULT_MAX_PART_SIZE = 5 * GIGABYTE
 
     def __init__(
         self,
-        min_part_size=None,
-        recommended_upload_part_size=None,
-        max_part_size=None,
+        min_part_size: int | None = None,
+        recommended_upload_part_size: int | None = None,
+        max_part_size: int | None = None,
     ):
-        self.min_part_size = min_part_size or self.DEFAULT_MIN_PART_SIZE
-        self.recommended_upload_part_size = recommended_upload_part_size or self.DEFAULT_RECOMMENDED_UPLOAD_PART_SIZE
-        self.max_part_size = max_part_size or self.DEFAULT_MAX_PART_SIZE
-        assert self.min_part_size <= self.recommended_upload_part_size <= self.max_part_size
+        # ensure default values do not break min<=recommended<=max condition,
+        # while respecting user input and not auto fixing if something was provided explicitly
+        self.min_part_size = min(
+            DEFAULT_MIN_PART_SIZE, *_filter_out_none(recommended_upload_part_size, max_part_size)
+        ) if min_part_size is None else min_part_size
+        self.recommended_upload_part_size = recommended_upload_part_size or max(
+            DEFAULT_RECOMMENDED_UPLOAD_PART_SIZE, self.min_part_size
+        )
+        self.max_part_size = max_part_size or max(
+            DEFAULT_MAX_PART_SIZE, self.recommended_upload_part_size
+        )
+        if self.min_part_size > self.recommended_upload_part_size:
+            raise InvalidUserInput(
+                f"min_part_size value ({self.min_part_size}) exceeding recommended_upload_part_size value ({self.recommended_upload_part_size})"
+            )
+        if self.recommended_upload_part_size > self.max_part_size:
+            raise InvalidUserInput(
+                f"recommended_upload_part_size value ({self.recommended_upload_part_size}) exceeding max_part_size value ({self.max_part_size})"
+            )
 
     @classmethod
     def from_account_info(
         cls,
-        account_info,
+        account_info: AbstractAccountInfo,
         min_part_size=None,
         recommended_upload_part_size=None,
         max_part_size=None
     ):
-        # TODO: add support for getting `min_part_size` and `max_part_size` from account info
         if recommended_upload_part_size is None:
             recommended_upload_part_size = account_info.get_recommended_part_size()
-        if min_part_size is None and recommended_upload_part_size < cls.DEFAULT_MIN_PART_SIZE:
-            min_part_size = recommended_upload_part_size
-        if max_part_size is None and recommended_upload_part_size > cls.DEFAULT_MAX_PART_SIZE:
-            max_part_size = recommended_upload_part_size
+            # AccountInfo defaults should not break the min<=recommended<=max condition when
+            # other params were provided explicitly
+            if min_part_size is not None:
+                recommended_upload_part_size = max(recommended_upload_part_size, min_part_size)
+            if max_part_size is not None:
+                recommended_upload_part_size = min(recommended_upload_part_size, max_part_size)
         kwargs = {
             'min_part_size': min_part_size,
             'recommended_upload_part_size': recommended_upload_part_size,
             'max_part_size': max_part_size,
         }
         return cls(**{key: value for key, value in kwargs.items() if value is not None})
 
     def get_emerge_plan(self, write_intents):
         write_intents = sorted(write_intents, key=lambda intent: intent.destination_offset)
+
+        # the upload part size recommended by the server causes errors with files larger than 1TB
+        # (with the current 100MB part size and 10000 part count limit).
+        # Therefore here we increase the recommended upload part size if needed.
+        # the constant is for handling mixed upload/copy in concatenate etc
+        max_destination_offset = max(intent.destination_end_offset for intent in write_intents)
+        self.recommended_upload_part_size = max(
+            self.recommended_upload_part_size,
+            min(
+                ceil(1.5 * max_destination_offset / 10000),
+                self.max_part_size,
+            )
+        )
+        assert self.min_part_size <= self.recommended_upload_part_size <= self.max_part_size, (
+            self.min_part_size, self.recommended_upload_part_size, self.max_part_size
+        )
         return self._get_emerge_plan(write_intents, EmergePlan)
 
     def get_streaming_emerge_plan(self, write_intent_iterator):
         return self._get_emerge_plan(write_intent_iterator, StreamingEmergePlan)
 
+    def get_unbound_emerge_plan(self, write_intent_iterator):
+        """
+        For unbound streams we skip the whole process of bunching different parts together,
+        validating them and splitting by operation type. We can do this, because:
+        1. there will be no copy operations at all;
+        2. we don't want to pull more data than actually needed;
+        3. all the data is ordered;
+        4. we don't want anything else to touch our buffers.
+        Furthermore, we're using StreamingEmergePlan, as it checks whether we have one or more
+        chunks to work with, and picks a proper upload method.
+        """
+        return StreamingEmergePlan(self._get_simple_emerge_parts(write_intent_iterator))
+
+    def _get_simple_emerge_parts(self, write_intent_iterator):
+        # Assumption here is that we need to do no magic. We are receiving
+        # a read-only stream that cannot be seeked and is only for uploading
+        # purposes. Moreover, we assume that each write intent we received is
+        # a nice, enclosed buffer with enough data to make the cloud happy.
+        for write_intent in write_intent_iterator:
+            yield UploadEmergePartDefinition(
+                write_intent.outbound_source,
+                relative_offset=0,
+                length=write_intent.length,
+            )
+
     def _get_emerge_plan(self, write_intent_iterator, plan_class):
         return plan_class(
             self._get_emerge_parts(
                 self._select_intent_fragments(self._validatation_iterator(write_intent_iterator))
             )
         )
 
@@ -163,15 +229,15 @@
             if intent is None:
                 last = True
 
             # incoming intent is different - this means that now we have to decide what to do:
             # if this is a copy intent and we want to copy it server-side, then we have to
             # flush the whole upload buffer we accumulated so far, but OTOH we may decide that we just want to
             # append it to upload buffer (see complete, untrivial logic below) and then maybe
-            # flush some upload parts from upload bufffer (if there is enough in the buffer)
+            # flush some upload parts from upload buffer (if there is enough in the buffer)
 
             current_len = current_end - upload_buffer.end_offset
             # should we flush the upload buffer or do we have to add a chunk of the copy first?
             if current_intent.is_copy() and current_len >= min_part_size:
                 # check if we can flush upload buffer or there is some missing bytes to fill it to `min_part_size`
                 if upload_buffer.intent_count() > 0 and upload_buffer.length < min_part_size:
                     missing_length = min_part_size - upload_buffer.length
@@ -279,36 +345,36 @@
         for part_size in part_sizes:
             yield EmergePart(CopyEmergePartDefinition(copy_source, relative_offset, part_size))
             relative_offset += part_size
 
     def _buff_split(self, upload_buffer):
         """ Split upload buffer to parts candidates - smaller upload buffers.
 
-        :rtype iterator[b2sdk.transfer.emerge.planner.planner.UploadBuffer]:
+        :rtype iterator[b2sdk._internal.transfer.emerge.planner.planner.UploadBuffer]:
         """
         if upload_buffer.intent_count() == 0:
             return
         tail_buffer = upload_buffer
         while True:
             if tail_buffer.length < self.recommended_upload_part_size + self.min_part_size:
                 # `EmergePlanner_buff_partition` can split in such way that tail part
                 # can be smaller than `min_part_size` - to avoid unnecessary download of possible
-                # incoming copy intent, we don't split futher
+                # incoming copy intent, we don't split further
                 yield tail_buffer
                 return
             head_buff, tail_buffer = self._buff_partition(tail_buffer)
             yield head_buff
 
     def _buff_partition(self, upload_buffer):
         """ Split upload buffer to two parts (smaller upload buffers).
 
-        In result left part cannot be splitted more, and nothing can be assumed about right part.
+        In result left part cannot be split more, and nothing can be assumed about right part.
 
-        :rtype tuple(b2sdk.transfer.emerge.planner.planner.UploadBuffer,
-                     b2sdk.transfer.emerge.planner.planner.UploadBuffer):
+        :rtype tuple(b2sdk._internal.transfer.emerge.planner.planner.UploadBuffer,
+                     b2sdk._internal.transfer.emerge.planner.planner.UploadBuffer):
         """
         left_buff = UploadBuffer(upload_buffer.start_offset)
         buff_start = upload_buffer.start_offset
         for idx, (intent, fragment_end) in enumerate(upload_buffer.iter_items()):
             candidate_size = fragment_end - buff_start
             if candidate_size > self.recommended_upload_part_size:
                 right_fragment_size = candidate_size - self.recommended_upload_part_size
@@ -320,23 +386,23 @@
                 left_buff.append(intent, fragment_end)
                 if candidate_size == self.recommended_upload_part_size:
                     return left_buff, upload_buffer.get_slice(start_idx=idx + 1)
 
         return left_buff, UploadBuffer(left_buff.end_offset)
 
     def _select_intent_fragments(self, write_intent_iterator):
-        """ Select overapping write intent fragments to use.
+        """ Select overlapping write intent fragments to use.
 
         To solve overlapping intents selection, intents can be split to smaller fragments.
-        Those fragments are yieled as soon as decision can be made to use them,
+        Those fragments are yielded as soon as decision can be made to use them,
         so there is possibility that one intent is yielded in multiple fragments. Those
         would be merged again by higher level iterator that produces emerge parts, but
         in principle this merging can happen here. Not merging it is a code design decision
         to make this function easier to implement and also it would allow yielding emerge parts
-        a bit quickier.
+        a bit quicker.
         """
 
         # `protected_intent_length` for upload state is 0, so it would generate at most single intent fragment
         # every loop iteration, but algorithm is not assuming that - one may one day choose to
         # protect upload fragments length too - eg. to avoid situation when file is opened to
         # read just small number of bytes and then switch to another overlapping upload source
         upload_intents_state = IntentsState()
@@ -365,15 +431,15 @@
             for intent, intent_fragment_end in intent_fragments:
                 yield intent, intent_fragment_end
                 last_sent_offset = intent_fragment_end
 
             if incoming_offset is not None and last_sent_offset < incoming_offset:
                 raise ValueError(
                     'Cannot emerge file with holes. '
-                    'Found hole range: ({}, {})'.format(last_sent_offset, incoming_offset)
+                    f'Found hole range: ({last_sent_offset}, {incoming_offset})'
                 )
 
             if incoming_intent is None:
                 yield None, None  # lets yield sentinel for cleaner `_get_emerge_parts` implementation
                 return
             if incoming_intent.is_upload():
                 upload_intents_state.add(incoming_intent)
@@ -381,15 +447,15 @@
                 copy_intents_state.add(incoming_intent)
             else:
                 raise RuntimeError('This should not happen at all!')
 
     def _merge_intent_fragments(self, start_offset, upload_intents, copy_intents):
         """ Select "competing" upload and copy fragments.
 
-        Upload and copy fragments may overlap so we nedd to choose right one
+        Upload and copy fragments may overlap so we need to choose right one
         to use - copy fragments are prioritized unless this fragment is unprotected
         (we use "protection" as an abstract for "short copy" fragments - meaning upload
         fragments have higher priority than "short copy")
         """
         upload_intents = deque(upload_intents)
         copy_intents = deque(copy_intents)
         while True:
@@ -427,15 +493,15 @@
                 raise ValueError('Planner cannot support write intents of unknown length')
             if write_intent.destination_offset < last_offset:
                 raise ValueError('Write intent stream have to be sorted by destination offset')
             last_offset = write_intent.destination_offset
             yield write_intent
 
 
-class IntentsState(object):
+class IntentsState:
     """ Store and process state of incoming write intents to solve
     overlapping intents selection in streaming manner.
 
     It does not check if intents are of the same kind (upload/copy), but the intention
     was to use it to split incoming intents by kind (two intents state are required then).
     If there would be no need for differentiating incoming intents, this would
     still work - so intent kind is ignored at this level. To address "short copy"
@@ -472,15 +538,15 @@
     def state_update(self, last_sent_offset, incoming_offset):
         """ Update the state using incoming intent offset.
 
         It has to be called *before* ``IntentsState.add`` and even if incoming intent
         would not be added to this intents state. It would yield a state of this stream
         of intents (like copy or upload) from ``last_sent_offset`` to ``incoming_offset``.
         So here happens the first stage of solving overlapping intents selection - but
-        write intent iterator can be splitted to multiple substreams (like copy and upload)
+        write intent iterator can be split to multiple substreams (like copy and upload)
         so additional stage is required to cover this.
         """
         if self._current_intent is not None:
             if last_sent_offset >= self._current_intent_end:
                 self._set_current_intent(None, None)
 
         # `effective_incoming_offset` is a safeguard after intent iterator is drained
@@ -555,15 +621,15 @@
     def _is_current_intent_protected(self):
         """ States if current intent is protected.
 
         Intent can be split to smaller fragments, but to choose upload over "small copy"
         we need to know for fragment if it is a "small copy" or not. In result of solving
         overlapping intents selection there might be a situation when original intent was not
         a small copy, but in effect it will be used only partially and in effect it may be a "small copy".
-        Algorithm attempts to aviod using smaller fragments than ``protected_intent_length`` but
+        Algorithm attempts to avoid using smaller fragments than ``protected_intent_length`` but
         sometimes it may be impossible. So if this function returns ``False`` it means
         that used length of this intent is smaller than ``protected_intent_length`` and the algorithm
         was unable to avoid this.
         """
         return self._can_be_protected(self._current_intent_start, self._current_intent_end)
 
     def _can_be_protected(self, start, end):
@@ -588,15 +654,15 @@
 
     def enumerate_emerge_parts(self):
         return enumerate(self.emerge_parts, 1)
 
 
 class EmergePlan(BaseEmergePlan):
     def __init__(self, emerge_parts):
-        super(EmergePlan, self).__init__(list(emerge_parts))
+        super().__init__(list(emerge_parts))
         self._is_large_file = len(self.emerge_parts) > 1
 
     def is_large_file(self):
         return self._is_large_file
 
     def get_total_length(self):
         return sum(emerge_part.get_length() for emerge_part in self.emerge_parts)
@@ -607,48 +673,44 @@
 
         json_id = json.dumps([emerge_part.get_part_id() for emerge_part in self.emerge_parts])
         return hashlib.sha1(json_id.encode()).hexdigest()
 
 
 class StreamingEmergePlan(BaseEmergePlan):
     def __init__(self, emerge_parts_iterator):
-        emerge_parts, self._is_large_file = self._peek_for_large_file(emerge_parts_iterator)
-        super(StreamingEmergePlan, self).__init__(emerge_parts)
+        emerge_parts_iterator, self._is_large_file = self._peek_for_large_file(
+            emerge_parts_iterator
+        )
+        super().__init__(emerge_parts_iterator)
 
     def is_large_file(self):
         return self._is_large_file
 
     def get_total_length(self):
         return None
 
     def get_plan_id(self):
         return None
 
     def _peek_for_large_file(self, emerge_parts_iterator):
-        first_part = next(emerge_parts_iterator, None)
-        if first_part is None:
+        peeked, emerge_parts_iterator = iterator_peek(emerge_parts_iterator, 2)
+
+        if not peeked:
             raise ValueError('Empty emerge parts iterator')
 
-        second_part = next(emerge_parts_iterator, None)
-        if second_part is None:
-            return iter([first_part]), False
-        else:
-            return chain([first_part, second_part], emerge_parts_iterator), True
+        return emerge_parts_iterator, len(peeked) > 1
 
 
-class EmergePart(object):
+class EmergePart:
     def __init__(self, part_definition, verification_ranges=None):
         self.part_definition = part_definition
         self.verification_ranges = verification_ranges
 
     def __repr__(self):
-        return '<{classname} part_definition={part_definition}>'.format(
-            classname=self.__class__.__name__,
-            part_definition=repr(self.part_definition),
-        )
+        return f'<{self.__class__.__name__} part_definition={repr(self.part_definition)}>'
 
     def get_length(self):
         return self.part_definition.get_length()
 
     def get_execution_step(self, execution_step_factory):
         return self.part_definition.get_execution_step(execution_step_factory)
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/emerge/planner/upload_subpart.py` & `b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/planner/upload_subpart.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 ######################################################################
 #
-# File: b2sdk/transfer/emerge/planner/upload_subpart.py
+# File: b2sdk/_internal/transfer/emerge/planner/upload_subpart.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import io
-
 from abc import ABCMeta, abstractmethod
 from functools import partial
 
-from b2sdk.download_dest import DownloadDestBytes
-from b2sdk.stream.chained import StreamOpener
-from b2sdk.stream.range import wrap_with_range
-from b2sdk.utils import hex_sha1_of_unlimited_stream
+from b2sdk._internal.stream.chained import StreamOpener
+from b2sdk._internal.stream.range import wrap_with_range
+from b2sdk._internal.utils import hex_sha1_of_unlimited_stream
 
 
 class BaseUploadSubpart(metaclass=ABCMeta):
     def __init__(self, outbound_source, relative_offset, length):
         self.outbound_source = outbound_source
         self.relative_offset = relative_offset
         self.length = length
@@ -46,34 +45,35 @@
 
     def is_hashable(self):
         return False
 
 
 class RemoteSourceUploadSubpart(BaseUploadSubpart):
     def __init__(self, *args, **kwargs):
-        super(RemoteSourceUploadSubpart, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._download_buffer_cache = None
 
     def get_subpart_id(self):
         return (self.outbound_source.file_id, self.relative_offset, self.length)
 
     def get_stream_opener(self, emerge_execution=None):
         if emerge_execution is None:
             raise RuntimeError('Cannot open remote source without emerge execution instance.')
         return CachedBytesStreamOpener(partial(self._download, emerge_execution))
 
     def _download(self, emerge_execution):
         url = emerge_execution.services.session.get_download_url_by_id(self.outbound_source.file_id)
         absolute_offset = self.outbound_source.offset + self.relative_offset
-        download_dest = DownloadDestBytes()
         range_ = (absolute_offset, absolute_offset + self.length - 1)
-        emerge_execution.services.download_manager.download_file_from_url(
-            url, download_dest, range_=range_, encryption=self.outbound_source.encryption
-        )
-        return download_dest.get_bytes_written()
+        with io.BytesIO() as bytes_io:
+            downloaded_file = emerge_execution.services.download_manager.download_file_from_url(
+                url, range_=range_, encryption=self.outbound_source.encryption
+            )
+            downloaded_file.save(bytes_io)
+            return bytes_io.getvalue()
 
 
 class LocalSourceUploadSubpart(BaseUploadSubpart):
     def get_subpart_id(self):
         with self._get_stream() as stream:
             sha1, _ = hex_sha1_of_unlimited_stream(stream)
             return sha1
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/emerge/write_intent.py` & `b2sdk-2.0.0/b2sdk/_internal/transfer/emerge/write_intent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 ######################################################################
 #
-# File: b2sdk/transfer/emerge/write_intent.py
+# File: b2sdk/_internal/transfer/emerge/write_intent.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
+from b2sdk._internal.utils import Sha1HexDigest
 
-class WriteIntent(object):
+
+class WriteIntent:
     """ Wrapper for outbound source that defines destination offset. """
 
     def __init__(self, outbound_source, destination_offset=0):
         """
-        :param b2sdk.v1.OutboundTransferSource outbound_source: data source (remote or local)
+        :param b2sdk.v2.OutboundTransferSource outbound_source: data source (remote or local)
         :param int destination_offset: point of start in destination file
         """
         if outbound_source.get_content_length() is None:
             raise ValueError('Cannot wrap outbound source of unknown length')
         self.outbound_source = outbound_source
         self.destination_offset = destination_offset
 
     def __repr__(self):
         return (
-            '<{classname} outbound_source={outbound_source} '
-            'destination_offset={destination_offset} id={id}>'
-        ).format(
-            classname=self.__class__.__name__,
-            outbound_source=repr(self.outbound_source),
-            destination_offset=self.destination_offset,
-            id=id(self),
+            f'<{self.__class__.__name__} outbound_source={repr(self.outbound_source)} '
+            f'destination_offset={self.destination_offset} id={id(self)}>'
         )
 
     @property
     def length(self):
         """ Length of the write intent.
 
         :rtype: int
@@ -59,23 +57,36 @@
     def is_upload(self):
         """ States if outbound source is local source and requires uploading.
 
         :rtype: bool
         """
         return self.outbound_source.is_upload()
 
+    def get_content_sha1(self) -> Sha1HexDigest | None:
+        """
+        Return a 40-character string containing the hex SHA1 checksum, which can be used as the `large_file_sha1` entry.
+
+        This method is only used if a large file is constructed from only a single source.  If that source's hash is known,
+        the result file's SHA1 checksum will be the same and can be copied.
+
+        If the source's sha1 is unknown and can't be calculated, `None` is returned.
+
+        :rtype str:
+        """
+        return self.outbound_source.get_content_sha1()
+
     @classmethod
     def wrap_sources_iterator(cls, outbound_sources_iterator):
         """ Helper that wraps outbound sources iterator with write intents.
 
         Can be used in cases similar to concatenate to automatically compute destination offsets
 
-        :param: iterator[b2sdk.v1.OutboundTransferSource] outbound_sources_iterator: iterator of outbound sources
+        :param: iterator[b2sdk.v2.OutboundTransferSource] outbound_sources_iterator: iterator of outbound sources
 
-        :rtype: generator[b2sdk.v1.WriteIntent]
+        :rtype: generator[b2sdk.v2.WriteIntent]
         """
         current_position = 0
         for outbound_source in outbound_sources_iterator:
             length = outbound_source.get_content_length()
             write_intent = WriteIntent(outbound_source, destination_offset=current_position)
             current_position += length
             yield write_intent
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/inbound/download_manager.py` & `b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/download_manager.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,150 +1,115 @@
 ######################################################################
 #
-# File: b2sdk/transfer/inbound/download_manager.py
+# File: b2sdk/_internal/transfer/inbound/download_manager.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import logging
-from typing import Optional
 
-from b2sdk.download_dest import DownloadDestProgressWrapper
-from b2sdk.encryption.setting import EncryptionSetting
-from b2sdk.progress import DoNothingProgressListener
-
-from b2sdk.exception import (
-    ChecksumMismatch,
+from b2sdk._internal.encryption.setting import EncryptionSetting
+from b2sdk._internal.exception import (
     InvalidRange,
-    TruncatedOutput,
 )
-from b2sdk.raw_api import SRC_LAST_MODIFIED_MILLIS
-from b2sdk.utils import B2TraceMetaAbstract
+from b2sdk._internal.progress import DoNothingProgressListener
+from b2sdk._internal.utils import B2TraceMetaAbstract
 
+from ...utils.thread_pool import ThreadPoolMixin
+from ..transfer_manager import TransferManager
+from .downloaded_file import DownloadedFile
 from .downloader.parallel import ParallelDownloader
 from .downloader.simple import SimpleDownloader
-from .file_metadata import FileMetadata
 
 logger = logging.getLogger(__name__)
 
 
-class DownloadManager(metaclass=B2TraceMetaAbstract):
+class DownloadManager(TransferManager, ThreadPoolMixin, metaclass=B2TraceMetaAbstract):
     """
     Handle complex actions around downloads to free raw_api from that responsibility.
     """
 
-    # how many chunks to break a downloaded file into
-    DEFAULT_MAX_STREAMS = 8
-
     # minimum size of a download chunk
     DEFAULT_MIN_PART_SIZE = 100 * 1024 * 1024
 
     # block size used when downloading file. If it is set to a high value,
     # progress reporting will be jumpy, if it's too low, it impacts CPU
     MIN_CHUNK_SIZE = 8192  # ~1MB file will show ~1% progress increment
     MAX_CHUNK_SIZE = 1024**2
 
-    def __init__(self, services):
+    PARALLEL_DOWNLOADER_CLASS = staticmethod(ParallelDownloader)
+    SIMPLE_DOWNLOADER_CLASS = staticmethod(SimpleDownloader)
+
+    def __init__(
+        self,
+        write_buffer_size: int | None = None,
+        check_hash: bool = True,
+        max_download_streams_per_file: int | None = None,
+        **kwargs
+    ):
         """
         Initialize the DownloadManager using the given services object.
-
-        :param b2sdk.v1.Services services:
         """
 
-        self.services = services
+        super().__init__(**kwargs)
         self.strategies = [
-            ParallelDownloader(
-                max_streams=self.DEFAULT_MAX_STREAMS,
+            self.PARALLEL_DOWNLOADER_CLASS(
                 min_part_size=self.DEFAULT_MIN_PART_SIZE,
                 min_chunk_size=self.MIN_CHUNK_SIZE,
-                max_chunk_size=self.MAX_CHUNK_SIZE,
+                max_chunk_size=max(self.MAX_CHUNK_SIZE, write_buffer_size or 0),
+                align_factor=write_buffer_size,
+                thread_pool=self._thread_pool,
+                check_hash=check_hash,
+                max_streams=max_download_streams_per_file,
             ),
-            # IOTDownloader(),  # TODO: curl -s httpbin.org/get | tee /dev/stderr 2>ble | sha1sum | cut -c -40
-            SimpleDownloader(
+            self.SIMPLE_DOWNLOADER_CLASS(
                 min_chunk_size=self.MIN_CHUNK_SIZE,
-                max_chunk_size=self.MAX_CHUNK_SIZE,
+                max_chunk_size=max(self.MAX_CHUNK_SIZE, write_buffer_size or 0),
+                align_factor=write_buffer_size,
+                thread_pool=self._thread_pool,
+                check_hash=check_hash,
             ),
         ]
+        self.write_buffer_size = write_buffer_size
+        self.check_hash = check_hash
 
     def download_file_from_url(
         self,
         url,
-        download_dest,
         progress_listener=None,
         range_=None,
-        encryption: Optional[EncryptionSetting] = None,
-    ):
+        encryption: EncryptionSetting | None = None,
+    ) -> DownloadedFile:
         """
         :param url: url from which the file should be downloaded
-        :param download_dest: where to put the file when it is downloaded
-        :param progress_listener: where to notify about progress downloading
+        :param progress_listener: where to notify about downloading progress
         :param range_: 2-element tuple containing data of http Range header
-        :param b2sdk.v1.EncryptionSetting encryption: encryption setting (``None`` if unknown)
+        :param b2sdk.v2.EncryptionSetting encryption: encryption setting (``None`` if unknown)
         """
         progress_listener = progress_listener or DoNothingProgressListener()
-        download_dest = DownloadDestProgressWrapper(download_dest, progress_listener)
         with self.services.session.download_file_from_url(
             url,
             range_=range_,
             encryption=encryption,
         ) as response:
-            metadata = FileMetadata.from_response(response)
+            download_version = self.services.api.download_version_factory.from_response_headers(
+                response.headers
+            )
             if range_ is not None:
                 # 2021-05-20: unfortunately for a read of a complete object server does not return the 'Content-Range' header
-                if (range_[1] - range_[0] + 1) != metadata.content_length:
-                    raise InvalidRange(metadata.content_length, range_)
-
-            mod_time_millis = int(
-                metadata.file_info.get(
-                    SRC_LAST_MODIFIED_MILLIS,
-                    response.headers['x-bz-upload-timestamp'],
-                )
-            )
+                if (range_[1] - range_[0] + 1) != download_version.content_length:
+                    raise InvalidRange(download_version.content_length, range_)
 
-            with download_dest.make_file_context(
-                metadata.file_id,
-                metadata.file_name,
-                metadata.content_length,
-                metadata.content_type,
-                metadata.content_sha1,
-                metadata.file_info,
-                mod_time_millis,
+            return DownloadedFile(
+                download_version=download_version,
+                download_manager=self,
                 range_=range_,
-            ) as file:
-
-                for strategy in self.strategies:
-                    if strategy.is_suitable(metadata, progress_listener):
-                        bytes_read, actual_sha1 = strategy.download(
-                            file,
-                            response,
-                            metadata,
-                            self.services.session,
-                            encryption=encryption,
-                        )
-                        break
-                else:
-                    assert False, 'no strategy suitable for download was found!'
-
-                self._validate_download(
-                    range_, bytes_read, actual_sha1, metadata
-                )  # raises exceptions
-                return metadata.as_info_dict()
-
-    @classmethod
-    def _validate_download(cls, range_, bytes_read, actual_sha1, metadata):
-        if range_ is None:
-            if bytes_read != metadata.content_length:
-                raise TruncatedOutput(bytes_read, metadata.content_length)
-
-            if metadata.content_sha1 != 'none' and actual_sha1 != metadata.content_sha1:
-                raise ChecksumMismatch(
-                    checksum_type='sha1',
-                    expected=metadata.content_sha1,
-                    actual=actual_sha1,
-                )
-        else:
-            desired_length = range_[1] - range_[0] + 1
-            if bytes_read != desired_length:
-                raise TruncatedOutput(bytes_read, desired_length)
+                response=response,
+                encryption=encryption,
+                progress_listener=progress_listener,
+                write_buffer_size=self.write_buffer_size,
+                check_hash=self.check_hash,
+            )
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/parallel.py` & `b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloader/parallel.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 ######################################################################
 #
-# File: b2sdk/transfer/inbound/downloader/parallel.py
+# File: b2sdk/_internal/transfer/inbound/downloader/parallel.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from abc import abstractmethod
-from typing import Optional
 import logging
-import hashlib
 import queue
 import threading
+from concurrent import futures
+from io import IOBase
+from time import perf_counter_ns
+
+from requests.models import Response
+
+from b2sdk._internal.encryption.setting import EncryptionSetting
+from b2sdk._internal.file_version import DownloadVersion
+from b2sdk._internal.session import B2Session
+from b2sdk._internal.utils.range_ import Range
 
 from .abstract import AbstractDownloader
-from .range import Range
-from b2sdk.encryption.setting import EncryptionSetting
+from .stats_collector import StatsCollector
 
 logger = logging.getLogger(__name__)
 
 
 class ParallelDownloader(AbstractDownloader):
     # situations to consider:
     #
@@ -40,55 +47,65 @@
     #      #######################################################################
     #      ^                                                                     ^
     #      |                                                                     |
     #      cloud file start                                         cloud file end
     #
     FINISH_HASHING_BUFFER_SIZE = 1024**2
 
-    def __init__(self, max_streams, min_part_size, *args, **kwargs):
+    def __init__(self, min_part_size: int, max_streams: int | None = None, **kwargs):
         """
         :param max_streams: maximum number of simultaneous streams
         :param min_part_size: minimum amount of data a single stream will retrieve, in bytes
         """
+        super().__init__(**kwargs)
         self.max_streams = max_streams
         self.min_part_size = min_part_size
-        super(ParallelDownloader, self).__init__(*args, **kwargs)
 
-    def is_suitable(self, metadata, progress_listener):
+    def is_suitable(self, download_version: DownloadVersion, allow_seeking: bool):
+        if not super().is_suitable(download_version, allow_seeking):
+            return False
         return self._get_number_of_streams(
-            metadata.content_length
-        ) >= 2 and metadata.content_length >= 2 * self.min_part_size
+            download_version.content_length
+        ) >= 2 and download_version.content_length >= 2 * self.min_part_size
 
     def _get_number_of_streams(self, content_length):
-        return min(self.max_streams, content_length // self.min_part_size) or 1
+        num_streams = content_length // self.min_part_size
+        if self.max_streams is not None:
+            num_streams = min(num_streams, self.max_streams)
+        else:
+            max_threadpool_workers = getattr(self._thread_pool, '_max_workers', None)
+            if max_threadpool_workers is not None:
+                num_streams = min(num_streams, max_threadpool_workers)
+        return num_streams
 
     def download(
-        self, file, response, metadata, session, encryption: Optional[EncryptionSetting] = None
+        self,
+        file: IOBase,
+        response: Response,
+        download_version: DownloadVersion,
+        session: B2Session,
+        encryption: EncryptionSetting | None = None,
     ):
         """
         Download a file from given url using parallel download sessions and stores it in the given download_destination.
-
-        :param file: an opened file-like object to write to
-        :param response: the response of the first request made to the cloud service with download intent
-        :return:
         """
-        remote_range = self._get_remote_range(response, metadata)
+        remote_range = self._get_remote_range(response, download_version)
         actual_size = remote_range.size()
         start_file_position = file.tell()
         parts_to_download = list(
             gen_parts(
                 remote_range,
                 Range(start_file_position, start_file_position + actual_size - 1),
-                part_count=self._get_number_of_streams(metadata.content_length),
+                part_count=self._get_number_of_streams(download_version.content_length),
             )
         )
 
         first_part = parts_to_download[0]
 
-        hasher = hashlib.sha1()
+        hasher = self._get_hasher()
 
         with WriterThread(file, max_queue_depth=len(parts_to_download) * 2) as writer:
             self._get_parts(
                 response,
                 session,
                 writer,
                 hasher,
@@ -97,15 +114,26 @@
                 self._get_chunk_size(actual_size),
                 encryption=encryption,
             )
         bytes_written = writer.total
 
         # At this point the hasher already consumed the data until the end of first stream.
         # Consume the rest of the file to complete the hashing process
-        self._finish_hashing(first_part, file, hasher, metadata.content_length)
+        if self._check_hash:
+            # we skip hashing if we would not check it - hasher object is actually a EmptyHasher instance
+            # but we avoid here reading whole file (except for the first part) from disk again
+            before_hash = perf_counter_ns()
+            self._finish_hashing(first_part, file, hasher, download_version.content_length)
+            after_hash = perf_counter_ns()
+            logger.info(
+                'download stats | %s | %s total: %.3f ms',
+                file,
+                'finish_hash',
+                (after_hash - before_hash) / 1000000,
+            )
 
         return bytes_written, hasher.hexdigest()
 
     def _finish_hashing(self, first_part, file, hasher, content_length):
         end_of_first_part = first_part.local_range.end + 1
         file.seek(end_of_first_part)
         file_read = file.read
@@ -127,39 +155,39 @@
             if stop:
                 break
 
     def _get_parts(
         self, response, session, writer, hasher, first_part, parts_to_download, chunk_size,
         encryption
     ):
-        stream = FirstPartDownloaderThread(
+        stream = self._thread_pool.submit(
+            download_first_part,
             response,
             hasher,
             session,
             writer,
             first_part,
             chunk_size,
             encryption=encryption,
         )
-        stream.start()
         streams = [stream]
 
         for part in parts_to_download:
-            stream = NonHashingDownloaderThread(
+            stream = self._thread_pool.submit(
+                download_non_first_part,
                 response.request.url,
                 session,
                 writer,
                 part,
                 chunk_size,
                 encryption=encryption,
             )
-            stream.start()
             streams.append(stream)
-        for stream in streams:
-            stream.join()
+
+        futures.wait(streams)
 
 
 class WriterThread(threading.Thread):
     """
     A thread responsible for keeping a queue of data chunks to write to a file-like object and for actually writing them down.
     Since a single thread is responsible for synchronization of the writes, we avoid a lot of issues between userspace and kernelspace
     that would normally require flushing buffers between the switches of the writer. That would kill performance and not synchronizing
@@ -182,167 +210,233 @@
     that might be 10 downloads, 8 producers, 1MB buffers, 2 buffers each = 8*2*10 = 160 MB (+ python buffers, operating system etc).
     """
 
     def __init__(self, file, max_queue_depth):
         self.file = file
         self.queue = queue.Queue(max_queue_depth)
         self.total = 0
-        super(WriterThread, self).__init__()
+        self.stats_collector = StatsCollector(str(self.file), 'writer', 'seek')
+        super().__init__()
 
     def run(self):
         file = self.file
         queue_get = self.queue.get
-        while 1:
-            shutdown, offset, data = queue_get()
-            if shutdown:
-                break
-            file.seek(offset)
-            file.write(data)
-            self.total += len(data)
+        stats_collector_read = self.stats_collector.read
+        stats_collector_other = self.stats_collector.other
+        stats_collector_write = self.stats_collector.write
+
+        with self.stats_collector.total:
+            while 1:
+                with stats_collector_read:
+                    shutdown, offset, data = queue_get()
+
+                if shutdown:
+                    break
+
+                with stats_collector_other:
+                    file.seek(offset)
+
+                with stats_collector_write:
+                    file.write(data)
+
+                self.total += len(data)
 
     def __enter__(self):
         self.start()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.queue.put((True, None, None))
         self.join()
+        self.stats_collector.report()
 
 
-class AbstractDownloaderThread(threading.Thread):
-    def __init__(
-        self,
-        session,
-        writer,
-        part_to_download,
-        chunk_size,
-        encryption: Optional[EncryptionSetting] = None,
-    ):
-        """
-        :param session: raw_api wrapper
-        :param writer: where to write data
-        :param part_to_download: PartToDownload object
-        :param chunk_size: internal buffer size to use for writing and hashing
-        """
-        self.session = session
-        self.writer = writer
-        self.part_to_download = part_to_download
-        self.chunk_size = chunk_size
-        self.encryption = encryption
-        super(AbstractDownloaderThread, self).__init__()
-
-    @abstractmethod
-    def run(self):
-        pass
-
-
-class FirstPartDownloaderThread(AbstractDownloaderThread):
-    def __init__(self, response, hasher, *args, **kwargs):
-        """
-        :param response: response of the original GET call
-        :param hasher: hasher object to feed to as the stream is written
-        """
-        self.response = response
-        self.hasher = hasher
-        super(FirstPartDownloaderThread, self).__init__(*args, **kwargs)
-
-    def run(self):
-        writer_queue_put = self.writer.queue.put
-        hasher_update = self.hasher.update
-        first_offset = self.part_to_download.local_range.start
-        last_offset = self.part_to_download.local_range.end + 1
-        actual_part_size = self.part_to_download.local_range.size()
-        starting_cloud_range = self.part_to_download.cloud_range
+def download_first_part(
+    response: Response,
+    hasher,
+    session: B2Session,
+    writer: WriterThread,
+    first_part: PartToDownload,
+    chunk_size: int,
+    encryption: EncryptionSetting | None = None,
+) -> None:
+    """
+    :param response: response of the original GET call
+    :param hasher: hasher object to feed to as the stream is written
+    :param session: B2 API session
+    :param writer: thread responsible for writing downloaded data
+    :param first_part: definition of the part to be downloaded
+    :param chunk_size: size (in bytes) of read data chunks
+    :param encryption: encryption mode, algorithm and key
+    """
+    # This function contains a loop that has heavy impact on performance.
+    # It has not been broken down to several small functions due to fear of
+    # performance overhead of calling a python function. Advanced performance optimization
+    # techniques are in use here, for example avoiding internal python getattr calls by
+    # caching function signatures in local variables. Most of this code was written in
+    # times where python 2.7 (or maybe even 2.6) had to be supported, so maybe some
+    # of those optimizations could be removed without affecting performance.
+    #
+    # Due to reports of hard to debug performance issues, this code has also been riddled
+    # with performance measurements. A known issue is GCP VMs which have more network speed
+    # than storage speed, but end users have different issues with network and storage.
+    # Basic tools to figure out where the time is being spent is a must for long-term
+    # maintainability.
+
+    writer_queue_put = writer.queue.put
+    hasher_update = hasher.update
+    first_offset = first_part.local_range.start
+    last_offset = first_part.local_range.end + 1
+    actual_part_size = first_part.local_range.size()
+    starting_cloud_range = first_part.cloud_range
+
+    bytes_read = 0
+    stop = False
+
+    stats_collector = StatsCollector(response.url, f'{first_offset}:{last_offset}', 'hash')
+    stats_collector_read = stats_collector.read
+    stats_collector_other = stats_collector.other
+    stats_collector_write = stats_collector.write
+
+    with stats_collector.total:
+        response_iterator = response.iter_content(chunk_size=chunk_size)
+
+        while True:
+            with stats_collector_read:
+                try:
+                    data = next(response_iterator)
+                except StopIteration:
+                    break
 
-        bytes_read = 0
-        stop = False
-        for data in self.response.iter_content(chunk_size=self.chunk_size):
             if first_offset + bytes_read + len(data) >= last_offset:
                 to_write = data[:last_offset - bytes_read]
                 stop = True
             else:
                 to_write = data
-            writer_queue_put((False, first_offset + bytes_read, to_write))
-            hasher_update(to_write)
+
+            with stats_collector_write:
+                writer_queue_put((False, first_offset + bytes_read, to_write))
+
+            with stats_collector_other:
+                hasher_update(to_write)
+
             bytes_read += len(to_write)
             if stop:
                 break
 
         # since we got everything we need from original response, close the socket and free the buffer
         # to avoid a timeout exception during hashing and other trouble
-        self.response.close()
+        response.close()
 
-        url = self.response.request.url
+        url = response.request.url
         tries_left = 5 - 1  # this is hardcoded because we are going to replace the entire retry interface soon, so we'll avoid deprecation here and keep it private
         while tries_left and bytes_read < actual_part_size:
             cloud_range = starting_cloud_range.subrange(
                 bytes_read, actual_part_size - 1
             )  # first attempt was for the whole file, but retries are bound correctly
             logger.debug(
                 'download attempts remaining: %i, bytes read already: %i. Getting range %s now.',
                 tries_left, bytes_read, cloud_range
             )
-            with self.session.download_file_from_url(
+            with session.download_file_from_url(
                 url,
                 cloud_range.as_tuple(),
-                encryption=self.encryption,
+                encryption=encryption,
             ) as response:
-                for to_write in response.iter_content(chunk_size=self.chunk_size):
-                    writer_queue_put((False, first_offset + bytes_read, to_write))
-                    hasher_update(to_write)
+                response_iterator = response.iter_content(chunk_size=chunk_size)
+
+                while True:
+                    with stats_collector_read:
+                        try:
+                            to_write = next(response_iterator)
+                        except StopIteration:
+                            break
+
+                    with stats_collector_write:
+                        writer_queue_put((False, first_offset + bytes_read, to_write))
+
+                    with stats_collector_other:
+                        hasher_update(to_write)
+
                     bytes_read += len(to_write)
             tries_left -= 1
 
+    stats_collector.report()
 
-class NonHashingDownloaderThread(AbstractDownloaderThread):
-    def __init__(self, url, *args, **kwargs):
-        """
-        :param url: url of the target file
-        """
-        self.url = url
-        super(NonHashingDownloaderThread, self).__init__(*args, **kwargs)
 
-    def run(self):
-        writer_queue_put = self.writer.queue.put
-        start_range = self.part_to_download.local_range.start
-        actual_part_size = self.part_to_download.local_range.size()
-        bytes_read = 0
-
-        starting_cloud_range = self.part_to_download.cloud_range
-
-        retries_left = 5  # this is hardcoded because we are going to replace the entire retry interface soon, so we'll avoid deprecation here and keep it private
-        while retries_left and bytes_read < actual_part_size:
-            cloud_range = starting_cloud_range.subrange(bytes_read, actual_part_size - 1)
-            logger.debug(
-                'download attempts remaining: %i, bytes read already: %i. Getting range %s now.',
-                retries_left, bytes_read, cloud_range
-            )
-            with self.session.download_file_from_url(
-                self.url,
+def download_non_first_part(
+    url: str,
+    session: B2Session,
+    writer: WriterThread,
+    part_to_download: PartToDownload,
+    chunk_size: int,
+    encryption: EncryptionSetting | None = None,
+) -> None:
+    """
+    :param url: download URL
+    :param session: B2 API session
+    :param writer: thread responsible for writing downloaded data
+    :param part_to_download: definition of the part to be downloaded
+    :param chunk_size: size (in bytes) of read data chunks
+    :param encryption: encryption mode, algorithm and key
+    """
+    writer_queue_put = writer.queue.put
+    start_range = part_to_download.local_range.start
+    actual_part_size = part_to_download.local_range.size()
+    bytes_read = 0
+
+    starting_cloud_range = part_to_download.cloud_range
+
+    retries_left = 5  # this is hardcoded because we are going to replace the entire retry interface soon, so we'll avoid deprecation here and keep it private
+    while retries_left and bytes_read < actual_part_size:
+        cloud_range = starting_cloud_range.subrange(bytes_read, actual_part_size - 1)
+        logger.debug(
+            'download attempts remaining: %i, bytes read already: %i. Getting range %s now.',
+            retries_left, bytes_read, cloud_range
+        )
+        stats_collector = StatsCollector(url, f'{cloud_range.start}:{cloud_range.end}', 'none')
+        stats_collector_read = stats_collector.read
+        stats_collector_write = stats_collector.write
+
+        with stats_collector.total:
+            with session.download_file_from_url(
+                url,
                 cloud_range.as_tuple(),
-                encryption=self.encryption,
+                encryption=encryption,
             ) as response:
-                for to_write in response.iter_content(chunk_size=self.chunk_size):
-                    writer_queue_put((False, start_range + bytes_read, to_write))
+                response_iterator = response.iter_content(chunk_size=chunk_size)
+
+                while True:
+                    with stats_collector_read:
+                        try:
+                            to_write = next(response_iterator)
+                        except StopIteration:
+                            break
+
+                    with stats_collector_write:
+                        writer_queue_put((False, start_range + bytes_read, to_write))
+
                     bytes_read += len(to_write)
             retries_left -= 1
 
+        stats_collector.report()
+
 
-class PartToDownload(object):
+class PartToDownload:
     """
     Hold the range of a file to download, and the range of the
     local file where it should be stored.
     """
 
     def __init__(self, cloud_range, local_range):
         self.cloud_range = cloud_range
         self.local_range = local_range
 
     def __repr__(self):
-        return 'PartToDownload(%s, %s)' % (self.cloud_range, self.local_range)
+        return f'PartToDownload({self.cloud_range}, {self.local_range})'
 
 
 def gen_parts(cloud_range, local_range, part_count):
     """
     Generate a sequence of PartToDownload to download a large file as
     a collection of parts.
     """
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/inbound/downloader/range.py` & `b2sdk-2.0.0/b2sdk/_internal/utils/range_.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 ######################################################################
 #
-# File: b2sdk/transfer/inbound/downloader/range.py
+# File: b2sdk/_internal/utils/range_.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 
-class Range(object):
+class Range:
     """
     HTTP ranges use an *inclusive* index at the end.
     """
 
     def __init__(self, start, end):
         assert 0 <= start <= end
         self.start = start
@@ -22,15 +23,17 @@
     @classmethod
     def from_header(cls, raw_range_header):
         """
         Factory method which returns an object constructed from Range http header.
 
         raw_range_header example: 'bytes=0-11'
         """
-        offsets = tuple(int(i) for i in raw_range_header.replace('bytes=', '').split('-'))
+        offsets = tuple(
+            int(i) for i in raw_range_header.replace('bytes', '').strip('= ').split('-')
+        )
         return cls(*offsets)
 
     def size(self):
         return self.end - self.start + 1
 
     def subrange(self, sub_start, sub_end):
         """
@@ -44,7 +47,10 @@
         return self.__class__(self.start + sub_start, self.start + sub_end)
 
     def as_tuple(self):
         return self.start, self.end
 
     def __repr__(self):
         return '%s(%d, %d)' % (self.__class__.__name__, self.start, self.end)
+
+    def __eq__(self, other):
+        return self.start == other.start and self.end == other.end
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/inbound/file_metadata.py` & `b2sdk-2.0.0/b2sdk/v1/file_metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 ######################################################################
 #
-# File: b2sdk/transfer/inbound/file_metadata.py
+# File: b2sdk/v1/file_metadata.py
 #
-# Copyright 2020 Backblaze Inc. All Rights Reserved.
+# Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
+import b2sdk.v2 as v2
 
-class FileMetadata(object):
+
+class FileMetadata:
     """
     Hold information about a file which is being downloaded.
     """
     UNVERIFIED_CHECKSUM_PREFIX = 'unverified:'
 
-    __slots__ = (
-        'file_id',
-        'file_name',
-        'content_type',
-        'content_length',
-        'content_sha1',
-        'content_sha1_verified',
-        'file_info',
-    )
-
     def __init__(
         self,
         file_id,
         file_name,
         content_type,
         content_length,
         content_sha1,
@@ -37,26 +30,14 @@
         self.file_id = file_id
         self.file_name = file_name
         self.content_type = content_type
         self.content_length = content_length
         self.content_sha1, self.content_sha1_verified = self._decode_content_sha1(content_sha1)
         self.file_info = file_info
 
-    @classmethod
-    def from_response(cls, response):
-        info = response.headers
-        return cls(
-            file_id=info['x-bz-file-id'],
-            file_name=info['x-bz-file-name'],
-            content_type=info['content-type'],
-            content_length=int(info['content-length']),
-            content_sha1=info['x-bz-content-sha1'],
-            file_info=dict((k[10:], info[k]) for k in info if k.startswith('x-bz-info-')),
-        )
-
     def as_info_dict(self):
         return {
             'fileId': self.file_id,
             'fileName': self.file_name,
             'contentType': self.content_type,
             'contentLength': self.content_length,
             'contentSha1': self._encode_content_sha1(self.content_sha1, self.content_sha1_verified),
@@ -68,9 +49,20 @@
         if content_sha1.startswith(cls.UNVERIFIED_CHECKSUM_PREFIX):
             return content_sha1[len(cls.UNVERIFIED_CHECKSUM_PREFIX):], False
         return content_sha1, True
 
     @classmethod
     def _encode_content_sha1(cls, content_sha1, content_sha1_verified):
         if not content_sha1_verified:
-            return '%s%s' % (cls.UNVERIFIED_CHECKSUM_PREFIX, content_sha1)
+            return f'{cls.UNVERIFIED_CHECKSUM_PREFIX}{content_sha1}'
         return content_sha1
+
+    @classmethod
+    def from_download_version(cls, download_version: v2.DownloadVersion):
+        return cls(
+            file_id=download_version.id_,
+            file_name=download_version.file_name,
+            content_type=download_version.content_type,
+            content_length=download_version.content_length,
+            content_sha1=download_version.content_sha1,
+            file_info=download_version.file_info,
+        )
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/outbound/copy_manager.py` & `b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/copy_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,88 +1,59 @@
 ######################################################################
 #
-# File: b2sdk/transfer/outbound/copy_manager.py
+# File: b2sdk/_internal/transfer/outbound/copy_manager.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-import concurrent.futures as futures
 import logging
-from typing import Optional
 
-from b2sdk.encryption.setting import EncryptionMode, EncryptionSetting, SSE_C_KEY_ID_FILE_INFO_KEY_NAME
-from b2sdk.exception import AlreadyFailed, SSECKeyIdMismatchInCopy
-from b2sdk.file_lock import FileRetentionSetting, LegalHold
-from b2sdk.raw_api import MetadataDirectiveMode
-from b2sdk.utils import B2TraceMetaAbstract
+from b2sdk._internal.encryption.setting import EncryptionMode, EncryptionSetting
+from b2sdk._internal.exception import AlreadyFailed, CopyArgumentsMismatch, SSECKeyIdMismatchInCopy
+from b2sdk._internal.file_lock import FileRetentionSetting, LegalHold
+from b2sdk._internal.http_constants import SSE_C_KEY_ID_FILE_INFO_KEY_NAME
+from b2sdk._internal.progress import AbstractProgressListener
+from b2sdk._internal.raw_api import MetadataDirectiveMode
+from b2sdk._internal.transfer.transfer_manager import TransferManager
+from b2sdk._internal.utils.thread_pool import ThreadPoolMixin
 
 logger = logging.getLogger(__name__)
 
 
-class CopyManager(metaclass=B2TraceMetaAbstract):
+class CopyManager(TransferManager, ThreadPoolMixin):
     """
     Handle complex actions around server side copy to free raw_api from that responsibility.
     """
 
     MAX_LARGE_FILE_SIZE = 10 * 1000 * 1000 * 1000 * 1000  # 10 TB
 
-    def __init__(self, services, max_copy_workers=10):
-        """
-        :param b2sdk.v1.Services services:
-        :param int max_copy_workers: a number of copy threads
-        """
-        self.services = services
-
-        self.copy_executor = None
-        self.max_workers = max_copy_workers
-
     @property
     def account_info(self):
         return self.services.session.account_info
 
-    def set_thread_pool_size(self, max_workers):
-        """
-        Set the size of the thread pool to use for uploads and downloads.
-
-        Must be called before any work starts, or the thread pool will get
-        the default size.
-
-        :param int max_workers: maximum allowed number of workers in a pool
-        """
-        if self.copy_executor is not None:
-            raise Exception('thread pool already created')
-        self.max_workers = max_workers
-
-    def get_thread_pool(self):
-        """
-        Return the thread pool executor to use for uploads and downloads.
-        """
-        if self.copy_executor is None:
-            self.copy_executor = futures.ThreadPoolExecutor(max_workers=self.max_workers)
-        return self.copy_executor
-
     def copy_file(
         self,
         copy_source,
         file_name,
         content_type,
         file_info,
         destination_bucket_id,
         progress_listener,
-        destination_encryption: Optional[EncryptionSetting] = None,
-        source_encryption: Optional[EncryptionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
+        destination_encryption: EncryptionSetting | None = None,
+        source_encryption: EncryptionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        file_retention: FileRetentionSetting | None = None,
     ):
         # Run small copies in the same thread pool as large file copies,
         # so that they share resources during a sync.
-        return self.get_thread_pool().submit(
+        return self._thread_pool.submit(
             self._copy_small_file,
             copy_source,
             file_name,
             content_type=content_type,
             file_info=file_info,
             destination_bucket_id=destination_bucket_id,
             progress_listener=progress_listener,
@@ -95,18 +66,18 @@
     def copy_part(
         self,
         large_file_id,
         part_copy_source,
         part_number,
         large_file_upload_state,
         finished_parts=None,
-        destination_encryption: Optional[EncryptionSetting] = None,
-        source_encryption: Optional[EncryptionSetting] = None,
+        destination_encryption: EncryptionSetting | None = None,
+        source_encryption: EncryptionSetting | None = None,
     ):
-        return self.get_thread_pool().submit(
+        return self._thread_pool.submit(
             self._copy_part,
             large_file_id,
             part_copy_source,
             part_number,
             large_file_upload_state,
             finished_parts=finished_parts,
             destination_encryption=destination_encryption,
@@ -116,30 +87,30 @@
     def _copy_part(
         self,
         large_file_id,
         part_copy_source,
         part_number,
         large_file_upload_state,
         finished_parts,
-        destination_encryption: Optional[EncryptionSetting],
-        source_encryption: Optional[EncryptionSetting],
+        destination_encryption: EncryptionSetting | None,
+        source_encryption: EncryptionSetting | None,
     ):
         """
         Copy a file part to started large file.
 
         :param :param str bucket_id: a bucket ID
-        :param file_id: a large file ID
-        :param b2sdk.v1.CopySourcePart copy_source_part: wrapper for copy source that represnts part range
-        :param b2sdk.v1.LargeFileUploadState large_file_upload_state: state object for progress reporting
+        :param large_file_id: a large file ID
+        :param b2sdk.v2.CopySource part_copy_source: copy source that represents a range (not necessarily a whole file)
+        :param b2sdk.v2.LargeFileUploadState large_file_upload_state: state object for progress reporting
                                                                       on large file upload
         :param dict,None finished_parts: dictionary of known finished parts, keys are part numbers,
-                                         values are instances of :class:`~b2sdk.v1.Part`
-        :param b2sdk.v1.EncryptionSetting destination_encryption: encryption settings for the destination
+                                         values are instances of :class:`~b2sdk.v2.Part`
+        :param b2sdk.v2.EncryptionSetting destination_encryption: encryption settings for the destination
                         (``None`` if unknown)
-        :param b2sdk.v1.EncryptionSetting source_encryption: encryption settings for the source
+        :param b2sdk.v2.EncryptionSetting source_encryption: encryption settings for the source
                         (``None`` if unknown)
         """
         # b2_copy_part doesn't need SSE-B2. Large file encryption is decided on b2_start_large_file.
         if destination_encryption is not None and destination_encryption.mode == EncryptionMode.SSE_B2:
             destination_encryption = None
 
         # Check if this part was uploaded before
@@ -170,71 +141,71 @@
     def _copy_small_file(
         self,
         copy_source,
         file_name,
         content_type,
         file_info,
         destination_bucket_id,
-        progress_listener,
-        destination_encryption: Optional[EncryptionSetting],
-        source_encryption: Optional[EncryptionSetting],
-        legal_hold: Optional[LegalHold] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
+        progress_listener: AbstractProgressListener,
+        destination_encryption: EncryptionSetting | None,
+        source_encryption: EncryptionSetting | None,
+        legal_hold: LegalHold | None = None,
+        file_retention: FileRetentionSetting | None = None,
     ):
-        with progress_listener:
-            progress_listener.set_total_bytes(copy_source.get_content_length() or 0)
+        progress_listener.set_total_bytes(copy_source.get_content_length() or 0)
 
-            bytes_range = copy_source.get_bytes_range()
+        bytes_range = copy_source.get_bytes_range()
 
-            if content_type is None:
-                if file_info is not None:
-                    raise ValueError('File info can be set only when content type is set')
-                metadata_directive = MetadataDirectiveMode.COPY
-            else:
-                if file_info is None:
-                    raise ValueError('File info can be not set only when content type is not set')
-                metadata_directive = MetadataDirectiveMode.REPLACE
-            metadata_directive, file_info, content_type = self.establish_sse_c_file_metadata(
-                metadata_directive=metadata_directive,
-                destination_file_info=file_info,
-                destination_content_type=content_type,
-                destination_server_side_encryption=destination_encryption,
-                source_server_side_encryption=source_encryption,
-                source_file_info=copy_source.source_file_info,
-                source_content_type=copy_source.source_content_type,
-            )
-            response = self.services.session.copy_file(
-                copy_source.file_id,
-                file_name,
-                bytes_range=bytes_range,
-                metadata_directive=metadata_directive,
-                content_type=content_type,
-                file_info=file_info,
-                destination_bucket_id=destination_bucket_id,
-                destination_server_side_encryption=destination_encryption,
-                source_server_side_encryption=source_encryption,
-                legal_hold=legal_hold,
-                file_retention=file_retention,
-            )
-            file_version = self.services.api.file_version_factory.from_api_response(response)
-            if progress_listener is not None:
-                progress_listener.bytes_completed(file_version.size)
+        if content_type is None:
+            if file_info is not None:
+                raise CopyArgumentsMismatch('File info can be set only when content type is set')
+            metadata_directive = MetadataDirectiveMode.COPY
+        else:
+            if file_info is None:
+                raise CopyArgumentsMismatch(
+                    'File info can be not set only when content type is not set'
+                )
+            metadata_directive = MetadataDirectiveMode.REPLACE
+        metadata_directive, file_info, content_type = self.establish_sse_c_file_metadata(
+            metadata_directive=metadata_directive,
+            destination_file_info=file_info,
+            destination_content_type=content_type,
+            destination_server_side_encryption=destination_encryption,
+            source_server_side_encryption=source_encryption,
+            source_file_info=copy_source.source_file_info,
+            source_content_type=copy_source.source_content_type,
+        )
+        response = self.services.session.copy_file(
+            copy_source.file_id,
+            file_name,
+            bytes_range=bytes_range,
+            metadata_directive=metadata_directive,
+            content_type=content_type,
+            file_info=file_info,
+            destination_bucket_id=destination_bucket_id,
+            destination_server_side_encryption=destination_encryption,
+            source_server_side_encryption=source_encryption,
+            legal_hold=legal_hold,
+            file_retention=file_retention,
+        )
+        file_version = self.services.api.file_version_factory.from_api_response(response)
+        progress_listener.bytes_completed(file_version.size)
 
         return file_version
 
     @classmethod
     def establish_sse_c_file_metadata(
         cls,
         metadata_directive: MetadataDirectiveMode,
-        destination_file_info: Optional[dict],
-        destination_content_type: Optional[str],
-        destination_server_side_encryption: Optional[EncryptionSetting],
-        source_server_side_encryption: Optional[EncryptionSetting],
-        source_file_info: Optional[dict],
-        source_content_type: Optional[str],
+        destination_file_info: dict | None,
+        destination_content_type: str | None,
+        destination_server_side_encryption: EncryptionSetting | None,
+        source_server_side_encryption: EncryptionSetting | None,
+        source_file_info: dict | None,
+        source_content_type: str | None,
     ):
         assert metadata_directive in (MetadataDirectiveMode.REPLACE, MetadataDirectiveMode.COPY)
 
         if metadata_directive == MetadataDirectiveMode.REPLACE:
             if destination_server_side_encryption:
                 destination_file_info = destination_server_side_encryption.add_key_id_to_file_info(
                     destination_file_info
@@ -253,18 +224,19 @@
             source_key_id = source_server_side_encryption.key.key_id
 
         if source_key_id == destination_key_id:
             return metadata_directive, destination_file_info, destination_content_type
 
         if source_file_info is None or source_content_type is None:
             raise SSECKeyIdMismatchInCopy(
-                'attempting to copy file using %s without providing source_file_info '
-                'and source_content_type for differing sse_c_key_ids: source="%s", '
-                'destination="%s"' %
-                (MetadataDirectiveMode.COPY, source_key_id, destination_key_id)
+                'attempting to copy file using {} without providing source_file_info '
+                'and source_content_type for differing sse_c_key_ids: source="{}", '
+                'destination="{}"'.format(
+                    MetadataDirectiveMode.COPY, source_key_id, destination_key_id
+                )
             )
 
         destination_file_info = source_file_info.copy()
         destination_file_info.pop(SSE_C_KEY_ID_FILE_INFO_KEY_NAME, None)
         if destination_server_side_encryption:
             destination_file_info = destination_server_side_encryption.add_key_id_to_file_info(
                 destination_file_info
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/outbound/copy_source.py` & `b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/copy_source.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 ######################################################################
 #
-# File: b2sdk/transfer/outbound/copy_source.py
+# File: b2sdk/_internal/transfer/outbound/copy_source.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from typing import Optional
-
-from b2sdk.encryption.setting import EncryptionSetting
-from b2sdk.transfer.outbound.outbound_source import OutboundTransferSource
+from b2sdk._internal.encryption.setting import EncryptionSetting
+from b2sdk._internal.http_constants import LARGE_FILE_SHA1
+from b2sdk._internal.transfer.outbound.outbound_source import OutboundTransferSource
 
 
 class CopySource(OutboundTransferSource):
     def __init__(
         self,
         file_id,
         offset=0,
         length=None,
-        encryption: Optional[EncryptionSetting] = None,
+        encryption: EncryptionSetting | None = None,
         source_file_info=None,
         source_content_type=None,
     ):
         if not length and offset > 0:
             raise ValueError('Cannot copy with non zero offset and unknown or zero length')
         self.file_id = file_id
         self.length = length
@@ -76,7 +76,13 @@
             self.file_id,
             range_offset,
             range_length,
             encryption=self.encryption,
             source_file_info=self.source_file_info,
             source_content_type=self.source_content_type
         )
+
+    def get_content_sha1(self):
+        if self.offset or self.length:
+            # this is a copy of only a range of the source, can't copy the SHA1
+            return None
+        return self.source_file_info.get(LARGE_FILE_SHA1)
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/outbound/large_file_upload_state.py` & `b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/large_file_upload_state.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 ######################################################################
 #
-# File: b2sdk/transfer/outbound/large_file_upload_state.py
+# File: b2sdk/_internal/transfer/outbound/large_file_upload_state.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import threading
 
 
-class LargeFileUploadState(object):
+class LargeFileUploadState:
     """
     Track the status of uploading a large file, accepting updates
     from the tasks that upload each of the parts.
 
     The aggregated progress is passed on to a ProgressListener that
     reports the progress for the file as a whole.
 
     This class is THREAD SAFE.
     """
 
     def __init__(self, file_progress_listener):
         """
-        :param b2sdk.v1.AbstractProgressListener file_progress_listener: a progress listener object to use. Use :py:class:`b2sdk.v1.DoNothingProgressListener` to disable.
+        :param b2sdk.v2.AbstractProgressListener file_progress_listener: a progress listener object to use. Use :py:class:`b2sdk.v2.DoNothingProgressListener` to disable.
         """
         self.lock = threading.RLock()
         self.error_message = None
         self.file_progress_listener = file_progress_listener
         self.part_number_to_part_state = {}
         self.bytes_completed = 0
 
@@ -39,15 +40,15 @@
         :param str message: an error message
         """
         with self.lock:
             self.error_message = message
 
     def has_error(self):
         """
-        Check whether an error occured.
+        Check whether an error occurred.
 
         :rtype: bool
         """
         with self.lock:
             return self.error_message is not None
 
     def get_error_message(self):
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/outbound/outbound_source.py` & `b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/outbound_source.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,58 @@
 ######################################################################
 #
-# File: b2sdk/transfer/outbound/outbound_source.py
+# File: b2sdk/_internal/transfer/outbound/outbound_source.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
 
+from b2sdk._internal.utils import Sha1HexDigest
+
 
 class OutboundTransferSource(metaclass=ABCMeta):
     """ Abstract class for defining outbound transfer sources.
 
     Supported outbound transfer sources are:
 
-    * :class:`b2sdk.v1.CopySource`
-    * :class:`b2sdk.v1.UploadSourceBytes`
-    * :class:`b2sdk.v1.UploadSourceLocalFile`
-    * :class:`b2sdk.v1.UploadSourceLocalFileRange`
-    * :class:`b2sdk.v1.UploadSourceStream`
-    * :class:`b2sdk.v1.UploadSourceStreamRange`
+    * :class:`b2sdk.v2.CopySource`
+    * :class:`b2sdk.v2.UploadSourceBytes`
+    * :class:`b2sdk.v2.UploadSourceLocalFile`
+    * :class:`b2sdk.v2.UploadSourceLocalFileRange`
+    * :class:`b2sdk.v2.UploadSourceStream`
+    * :class:`b2sdk.v2.UploadSourceStreamRange`
 
     """
 
     @abstractmethod
-    def get_content_length(self):
+    def get_content_length(self) -> int:
         """
-        Return the number of bytes of data in the file.
+        Returns the number of bytes of data in the file.
         """
 
     @abstractmethod
-    def is_upload(self):
-        """ Return if outbound source is an upload source.
-        :rtype bool:
+    def get_content_sha1(self) -> Sha1HexDigest | None:
+        """
+        Return a 40-character string containing the hex SHA1 checksum, which can be used as the `large_file_sha1` entry.
+
+        This method is only used if a large file is constructed from only a single source.  If that source's hash is known,
+        the result file's SHA1 checksum will be the same and can be copied.
+
+        If the source's sha1 is unknown and can't be calculated, `None` is returned.
         """
 
     @abstractmethod
-    def is_copy(self):
-        """ Return if outbound source is a copy source.
-        :rtype bool:
+    def is_upload(self) -> bool:
+        """
+        Returns True if outbound source is an upload source.
+        """
+
+    @abstractmethod
+    def is_copy(self) -> bool:
+        """
+        Returns True if outbound source is a copy source.
         """
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/outbound/progress_reporter.py` & `b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/progress_reporter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 ######################################################################
 #
-# File: b2sdk/transfer/outbound/progress_reporter.py
+# File: b2sdk/_internal/transfer/outbound/progress_reporter.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from b2sdk.progress import AbstractProgressListener
+from b2sdk._internal.progress import AbstractProgressListener
 
 
 class PartProgressReporter(AbstractProgressListener):
     """
     An adapter that listens to the progress of upload a part and
-    gives the information to a :py:class:`b2sdk.bucket.LargeFileUploadState`.
+    gives the information to a :py:class:`b2sdk._internal.transfer.outbound.large_file_upload_state.LargeFileUploadState`.
 
     Accepts absolute bytes_completed from the uploader, and reports
-    deltas to the :py:class:`b2sdk.bucket.LargeFileUploadState`.  The bytes_completed for the
+    deltas to the :py:class:`b2sdk._internal.transfer.outbound.large_file_upload_state.LargeFileUploadState`.  The bytes_completed for the
     part will drop back to 0 on a retry, which will result in a
     negative delta.
     """
 
     def __init__(self, large_file_upload_state, *args, **kwargs):
         """
-        :param b2sdk.bucket.LargeFileUploadState large_file_upload_state: object to relay the progress to
+        :param b2sdk._internal.transfer.outbound.large_file_upload_state.LargeFileUploadState large_file_upload_state: object to relay the progress to
         """
-        super(PartProgressReporter, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.large_file_upload_state = large_file_upload_state
         self.prev_byte_count = 0
 
     def bytes_completed(self, byte_count):
         self.large_file_upload_state.update_part_bytes(byte_count - self.prev_byte_count)
         self.prev_byte_count = byte_count
```

### Comparing `b2sdk-1.9.0/b2sdk/transfer/outbound/upload_manager.py` & `b2sdk-2.0.0/b2sdk/_internal/transfer/outbound/upload_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,118 +1,95 @@
 ######################################################################
 #
-# File: b2sdk/transfer/outbound/upload_manager.py
+# File: b2sdk/_internal/transfer/outbound/upload_manager.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import logging
-import concurrent.futures as futures
+from contextlib import ExitStack
+from typing import TYPE_CHECKING, TypeVar
 
-from typing import Optional
-
-from b2sdk.encryption.setting import EncryptionMode, EncryptionSetting
-from b2sdk.exception import (
+from b2sdk._internal.encryption.setting import EncryptionMode, EncryptionSetting
+from b2sdk._internal.exception import (
     AlreadyFailed,
     B2Error,
     MaxRetriesExceeded,
 )
-from b2sdk.file_lock import FileRetentionSetting, LegalHold
-from b2sdk.stream.progress import ReadingStreamWithProgress
-from b2sdk.stream.hashing import StreamWithHash
-from b2sdk.raw_api import HEX_DIGITS_AT_END
-from b2sdk.utils import B2TraceMetaAbstract
+from b2sdk._internal.file_lock import FileRetentionSetting, LegalHold
+from b2sdk._internal.http_constants import HEX_DIGITS_AT_END
+from b2sdk._internal.stream.hashing import StreamWithHash
+from b2sdk._internal.stream.progress import ReadingStreamWithProgress
 
+from ...utils.thread_pool import ThreadPoolMixin
+from ..transfer_manager import TransferManager
 from .progress_reporter import PartProgressReporter
 
 logger = logging.getLogger(__name__)
 
+if TYPE_CHECKING:
+    from b2sdk._internal.transfer.outbound.upload_source import AbstractUploadSource
+
+    _TypeUploadSource = TypeVar("_TypeUploadSource", bound=AbstractUploadSource)
 
-class UploadManager(metaclass=B2TraceMetaAbstract):
+
+class UploadManager(TransferManager, ThreadPoolMixin):
     """
     Handle complex actions around uploads to free raw_api from that responsibility.
     """
 
     MAX_UPLOAD_ATTEMPTS = 5
 
-    def __init__(self, services, max_upload_workers=10):
-        """
-        :param b2sdk.v1.Services services:
-        :param int max_upload_workers: a number of upload threads
-        """
-        self.services = services
-
-        self.upload_executor = None
-        self.max_workers = max_upload_workers
-
     @property
     def account_info(self):
         return self.services.session.account_info
 
-    def set_thread_pool_size(self, max_workers):
-        """
-        Set the size of the thread pool to use for uploads and downloads.
-
-        Must be called before any work starts, or the thread pool will get
-        the default size.
-
-        :param int max_workers: maximum allowed number of workers in a pool
-        """
-        if self.upload_executor is not None:
-            raise Exception('thread pool already created')
-        self.max_workers = max_workers
-
-    def get_thread_pool(self):
-        """
-        Return the thread pool executor to use for uploads and downloads.
-        """
-        if self.upload_executor is None:
-            self.upload_executor = futures.ThreadPoolExecutor(max_workers=self.max_workers)
-        return self.upload_executor
-
     def upload_file(
         self,
         bucket_id,
         upload_source,
         file_name,
         content_type,
         file_info,
         progress_listener,
-        encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
     ):
-        f = self.get_thread_pool().submit(
+        f = self._thread_pool.submit(
             self._upload_small_file,
             bucket_id,
             upload_source,
             file_name,
             content_type,
             file_info,
             progress_listener,
             encryption,
             file_retention,
             legal_hold,
+            custom_upload_timestamp=custom_upload_timestamp,
         )
         return f
 
     def upload_part(
         self,
         bucket_id,
         file_id,
-        part_upload_source,
+        part_upload_source: _TypeUploadSource,
         part_number,
         large_file_upload_state,
         finished_parts=None,
         encryption: EncryptionSetting = None,
     ):
-        f = self.get_thread_pool().submit(
+        f = self._thread_pool.submit(
             self._upload_part,
             bucket_id,
             file_id,
             part_upload_source,
             part_number,
             large_file_upload_state,
             finished_parts,
@@ -120,31 +97,31 @@
         )
         return f
 
     def _upload_part(
         self,
         bucket_id,
         file_id,
-        part_upload_source,
+        part_upload_source: _TypeUploadSource,
         part_number,
         large_file_upload_state,
         finished_parts,
         encryption: EncryptionSetting,
     ):
         """
         Upload a file part to started large file.
 
         :param :param str bucket_id: a bucket ID
         :param file_id: a large file ID
-        :param b2sdk.v1.UploadSourcePart upload_source_part: wrapper for upload source that reads only required range
-        :param b2sdk.v1.LargeFileUploadState large_file_upload_state: state object for progress reporting
+        :param b2sdk.v2.AbstractUploadSource part_upload_source: upload source that reads only required range
+        :param b2sdk.v2.LargeFileUploadState large_file_upload_state: state object for progress reporting
                                                                       on large file upload
         :param dict,None finished_parts: dictionary of known finished parts, keys are part numbers,
-                                         values are instances of :class:`~b2sdk.v1.Part`
-        :param b2sdk.v1.EncryptionSetting encryption: encryption setting (``None`` if unknown)
+                                         values are instances of :class:`~b2sdk.v2.Part`
+        :param b2sdk.v2.EncryptionSetting encryption: encryption setting (``None`` if unknown)
         """
 
         # b2_upload_part doesn't need SSE-B2. Large file encryption is decided on b2_start_large_file.
         if encryption is not None and encryption.mode == EncryptionMode.SSE_B2:
             encryption = None
 
         # Check if this part was uploaded before
@@ -157,22 +134,33 @@
             return {'contentSha1': part.content_sha1}
 
         # Set up a progress listener
         part_progress_listener = PartProgressReporter(large_file_upload_state)
 
         # Retry the upload as needed
         exception_list = []
-        for _ in range(self.MAX_UPLOAD_ATTEMPTS):
-            # if another part has already had an error there's no point in
-            # uploading this part
-            if large_file_upload_state.has_error():
-                raise AlreadyFailed(large_file_upload_state.get_error_message())
+        with ExitStack() as stream_guard:
+            part_stream = None
+
+            def close_stream_callback(stream):
+                if not stream.closed:
+                    stream.close()
+
+            for _ in range(self.MAX_UPLOAD_ATTEMPTS):
+                # if another part has already had an error there's no point in
+                # uploading this part
+                if large_file_upload_state.has_error():
+                    raise AlreadyFailed(large_file_upload_state.get_error_message())
+
+                try:
+                    # reuse the stream in case of retry
+                    part_stream = part_stream or part_upload_source.open()
+                    # register stream closing callback only when reading is finally concluded
+                    stream_guard.callback(close_stream_callback, part_stream)
 
-            try:
-                with part_upload_source.open() as part_stream:
                     content_length = part_upload_source.get_content_length()
                     input_stream = ReadingStreamWithProgress(
                         part_stream, part_progress_listener, length=content_length
                     )
                     if part_upload_source.is_sha1_known():
                         content_sha1 = part_upload_source.get_content_sha1()
                     else:
@@ -187,72 +175,70 @@
                         input_stream,
                         server_side_encryption=encryption,  # todo: client side encryption
                     )
                     if content_sha1 == HEX_DIGITS_AT_END:
                         content_sha1 = input_stream.hash
                     assert content_sha1 == response['contentSha1']
                     return response
-
-            except B2Error as e:
-                if not e.should_retry_upload():
-                    raise
-                exception_list.append(e)
-                self.account_info.clear_bucket_upload_data(bucket_id)
+                except B2Error as e:
+                    if not e.should_retry_upload():
+                        raise
+                    exception_list.append(e)
+                    self.account_info.clear_bucket_upload_data(bucket_id)
 
         large_file_upload_state.set_error(str(exception_list[-1]))
         raise MaxRetriesExceeded(self.MAX_UPLOAD_ATTEMPTS, exception_list)
 
     def _upload_small_file(
         self,
         bucket_id,
         upload_source,
         file_name,
         content_type,
         file_info,
         progress_listener,
-        encryption: Optional[EncryptionSetting] = None,
-        file_retention: Optional[FileRetentionSetting] = None,
-        legal_hold: Optional[LegalHold] = None,
+        encryption: EncryptionSetting | None = None,
+        file_retention: FileRetentionSetting | None = None,
+        legal_hold: LegalHold | None = None,
+        custom_upload_timestamp: int | None = None,
     ):
         content_length = upload_source.get_content_length()
         exception_info_list = []
         progress_listener.set_total_bytes(content_length)
-        with progress_listener:
-            for _ in range(self.MAX_UPLOAD_ATTEMPTS):
-                try:
-                    with upload_source.open() as file:
-                        input_stream = ReadingStreamWithProgress(
-                            file, progress_listener, length=content_length
-                        )
-                        if upload_source.is_sha1_known():
-                            content_sha1 = upload_source.get_content_sha1()
-                        else:
-                            input_stream = StreamWithHash(
-                                input_stream, stream_length=content_length
-                            )
-                            content_sha1 = HEX_DIGITS_AT_END
-                        # it is important that `len()` works on `input_stream`
-                        response = self.services.session.upload_file(
-                            bucket_id,
-                            file_name,
-                            len(input_stream),
-                            content_type,
-                            content_sha1,
-                            file_info,
-                            input_stream,
-                            server_side_encryption=encryption,  # todo: client side encryption
-                            file_retention=file_retention,
-                            legal_hold=legal_hold,
-                        )
-                        if content_sha1 == HEX_DIGITS_AT_END:
-                            content_sha1 = input_stream.hash
-                        assert content_sha1 == response[
-                            'contentSha1'], '%s != %s' % (content_sha1, response['contentSha1'])
-                        return self.services.api.file_version_factory.from_api_response(response)
+        for _ in range(self.MAX_UPLOAD_ATTEMPTS):
+            try:
+                with upload_source.open() as file:
+                    input_stream = ReadingStreamWithProgress(
+                        file, progress_listener, length=content_length
+                    )
+                    if upload_source.is_sha1_known():
+                        content_sha1 = upload_source.get_content_sha1()
+                    else:
+                        input_stream = StreamWithHash(input_stream, stream_length=content_length)
+                        content_sha1 = HEX_DIGITS_AT_END
+                    # it is important that `len()` works on `input_stream`
+                    response = self.services.session.upload_file(
+                        bucket_id,
+                        file_name,
+                        len(input_stream),
+                        content_type,
+                        content_sha1,
+                        file_info,
+                        input_stream,
+                        server_side_encryption=encryption,  # todo: client side encryption
+                        file_retention=file_retention,
+                        legal_hold=legal_hold,
+                        custom_upload_timestamp=custom_upload_timestamp,
+                    )
+                    if content_sha1 == HEX_DIGITS_AT_END:
+                        content_sha1 = input_stream.hash
+                    assert content_sha1 == 'do_not_verify' or content_sha1 == response[
+                        'contentSha1'], '{} != {}'.format(content_sha1, response['contentSha1'])
+                    return self.services.api.file_version_factory.from_api_response(response)
 
-                except B2Error as e:
-                    if not e.should_retry_upload():
-                        raise
-                    exception_info_list.append(e)
-                    self.account_info.clear_bucket_upload_data(bucket_id)
+            except B2Error as e:
+                if not e.should_retry_upload():
+                    raise
+                exception_info_list.append(e)
+                self.account_info.clear_bucket_upload_data(bucket_id)
 
         raise MaxRetriesExceeded(self.MAX_UPLOAD_ATTEMPTS, exception_info_list)
```

### Comparing `b2sdk-1.9.0/b2sdk/utils.py` & `b2sdk-2.0.0/b2sdk/_internal/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 ######################################################################
 #
-# File: b2sdk/utils.py
+# File: b2sdk/_internal/utils/__init__.py
 #
-# Copyright 2019 Backblaze Inc. All Rights Reserved.
+# Copyright 2022 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import base64
 import hashlib
+import logging
 import os
+import pathlib
 import platform
 import re
-import shutil
-import tempfile
-import concurrent.futures as futures
+import time
+from dataclasses import dataclass, field
 from decimal import Decimal
+from itertools import chain
+from typing import Any, Iterator, NewType, TypeVar
 from urllib.parse import quote, unquote_plus
 
-from logfury.v0_1 import DefaultTraceAbstractMeta, DefaultTraceMeta, limit_trace_arguments, disable_trace, trace_call
+from logfury.v1 import DefaultTraceAbstractMeta, DefaultTraceMeta, limit_trace_arguments, disable_trace, trace_call
 
+logger = logging.getLogger(__name__)
 
-def interruptible_get_result(future):
-    """
-    Wait for the result of a future in a way that can be interrupted
-    by a KeyboardInterrupt.
-
-    This is not necessary in Python 3, but is needed for Python 2.
-
-    :param future: a future to get result of
-    :type future: Future
-    """
-    while True:
-        try:
-            return future.result(timeout=1.0)
-        except futures.TimeoutError:
-            pass
+Sha1HexDigest = NewType('Sha1HexDigest', str)
+T = TypeVar('T')
+# TODO: When we drop Python 3.7 support, this should be replaced
+#   with typing.Protocol that exposes read method.
+ReadOnlyStream = Any
 
 
 def b2_url_encode(s):
     """
     URL-encode a unicode string to be sent to B2 in an HTTP header.
 
     :param s: a unicode string to encode
@@ -96,62 +91,117 @@
     start_of_last = (part_count - 1) * part_size
     last_part = (start_of_last, content_length - start_of_last)
     parts.append(last_part)
 
     return parts
 
 
-def hex_sha1_of_stream(input_stream, content_length):
+def update_digest_from_stream(digest: T, input_stream: ReadOnlyStream, content_length: int) -> T:
     """
-    Return the 40-character hex SHA1 checksum of the first content_length
-    bytes in the input stream.
+    Update and return `digest` with data read from `input_stream`
 
-    :param input_stream: stream object, which exposes read() method
+    :param digest: a digest object, which exposes an `update(bytes)` method
+    :param input_stream: stream object, which exposes a `read(int|None)` method
     :param content_length: expected length of the stream
     :type content_length: int
-    :rtype: str
     """
     remaining = content_length
     block_size = 1024 * 1024
-    digest = hashlib.sha1()
     while remaining != 0:
         to_read = min(remaining, block_size)
         data = input_stream.read(to_read)
         if len(data) != to_read:
             raise ValueError(
                 'content_length(%s) is more than the size of the file' % content_length
             )
         digest.update(data)
         remaining -= to_read
-    return digest.hexdigest()
+    return digest
 
 
-def hex_sha1_of_unlimited_stream(input_stream, limit=None):
-    block_size = 1024 * 1024
-    content_length = 0
-    digest = hashlib.sha1()
-    while True:
-        if limit is not None:
-            to_read = min(limit - content_length, block_size)
-        else:
-            to_read = block_size
-        data = input_stream.read(to_read)
-        data_len = len(data)
-        if data_len > 0:
-            digest.update(data)
-            content_length += data_len
-        if data_len < to_read:
-            return digest.hexdigest(), content_length
+def hex_sha1_of_stream(input_stream: ReadOnlyStream, content_length: int) -> Sha1HexDigest:
+    """
+    Return the 40-character hex SHA1 checksum of the first content_length
+    bytes in the input stream.
+
+    :param input_stream: stream object, which exposes read(int|None) method
+    :param content_length: expected length of the stream
+    :type content_length: int
+    :rtype: str
+    """
+    return Sha1HexDigest(
+        update_digest_from_stream(
+            hashlib.sha1(),
+            input_stream,
+            content_length,
+        ).hexdigest()
+    )
+
+
+@dataclass
+class IncrementalHexDigester:
+    """
+    Calculates digest of a stream or parts of it.
+    """
+    stream: ReadOnlyStream
+    digest: 'hashlib._Hash' = field(  # noqa (_Hash is a dynamic object)
+        default_factory=hashlib.sha1
+    )
+    read_bytes: int = 0
+    block_size: int = 1024 * 1024
+
+    @property
+    def hex_digest(self) -> Sha1HexDigest:
+        return Sha1HexDigest(self.digest.hexdigest())
+
+    def update_from_stream(
+        self,
+        limit: int | None = None,
+    ) -> Sha1HexDigest:
+        """
+        :param limit: How many new bytes try to read from the stream. Default None – read until nothing left.
+        """
+        offset = 0
+
+        while True:
+            if limit is not None:
+                to_read = min(limit - offset, self.block_size)
+            else:
+                to_read = self.block_size
+            data = self.stream.read(to_read)
+            data_len = len(data)
+            if data_len > 0:
+                self.digest.update(data)
+                self.read_bytes += data_len
+                offset += data_len
+            if data_len < to_read or to_read == 0:
+                break
+
+        return self.hex_digest
+
+
+def hex_sha1_of_unlimited_stream(
+    input_stream: ReadOnlyStream,
+    limit: int | None = None,
+) -> tuple[Sha1HexDigest, int]:
+    digester = IncrementalHexDigester(input_stream)
+    digester.update_from_stream(limit)
+    return digester.hex_digest, digester.read_bytes
+
+
+def hex_sha1_of_file(path_) -> Sha1HexDigest:
+    with open(path_, 'rb') as file:
+        return hex_sha1_of_unlimited_stream(file)[0]
 
 
-def hex_sha1_of_bytes(data: bytes) -> str:
+def hex_sha1_of_bytes(data: bytes) -> Sha1HexDigest:
     """
     Return the 40-character hex SHA1 checksum of the data.
     """
-    return hashlib.sha1(data).hexdigest()
+    return Sha1HexDigest(hashlib.sha1(data).hexdigest())
 
 
 def hex_md5_of_bytes(data: bytes) -> str:
     """
     Return the 32-character hex MD5 checksum of the data.
     """
     return hashlib.md5(data).hexdigest()
@@ -227,37 +277,53 @@
     :type local_path: str
     :rtype: int
     """
     mod_time = os.path.getmtime(local_path) * 1000
     return int(mod_time)
 
 
-def set_file_mtime(local_path, mod_time_millis):
+def is_special_file(path: str | pathlib.Path) -> bool:
+    """
+    Is the path a special file, such as /dev/null or stdout?
+
+    :param path: a "file" path
+    :return: True if the path is a special file
+    """
+    path_str = str(path)
+    return (
+        path == os.devnull or path_str.startswith('/dev/') or
+        platform.system() == 'Windows' and path_str.upper() in ('CON', 'NUL')
+    )
+
+
+def set_file_mtime(local_path: str | pathlib.Path, mod_time_millis: int) -> None:
     """
     Set modification time of a file in milliseconds.
 
     :param local_path: a file path
-    :type local_path: str
     :param mod_time_millis: time to be set
-    :type mod_time_millis: int
     """
     mod_time = mod_time_millis / 1000.0
 
     # We have to convert it this way to avoid differences when mtime
     # is read from the local file in the next iterations, and time is fetched
     # without rounding.
     # This is caused by floating point arithmetic as POSIX systems
     # represents mtime as floats and B2 as integers.
     # E.g. for 1093258377393, it would be converted to 1093258377.393
     # which is actually represented by 1093258377.3929998874664306640625.
     # When we save mtime and read it again, we will end up with 1093258377392.
     # See #617 for details.
     mod_time = float(Decimal('%.3f5' % mod_time))
 
-    os.utime(local_path, (mod_time, mod_time))
+    try:
+        os.utime(local_path, (mod_time, mod_time))
+    except OSError:
+        if not is_special_file(local_path):
+            raise
 
 
 def fix_windows_path_limit(path):
     """
     Prefix paths when running on Windows to overcome 260 character path length limit.
     See https://msdn.microsoft.com/en-us/library/windows/desktop/aa365247(v=vs.85).aspx#maxpath
 
@@ -276,32 +342,14 @@
         else:
             # relative path, don't alter
             return path
     else:
         return path
 
 
-class TempDir(object):
-    """
-    Context manager that creates and destroys a temporary directory.
-    """
-
-    def __enter__(self):
-        """
-        Return the unicode path to the temp dir.
-        """
-        dirpath_bytes = tempfile.mkdtemp()
-        self.dirpath = str(dirpath_bytes.replace('\\', '\\\\'))
-        return self.dirpath
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        shutil.rmtree(self.dirpath)
-        return None  # do not hide exception
-
-
 def _pick_scale_and_suffix(x):
     # suffixes for different scales
     suffixes = ' kMGTP'
 
     # We want to use the biggest suffix that makes sense.
     ref_digits = str(int(x))
     index = (len(ref_digits) - 1) // 3
@@ -406,15 +454,15 @@
     """
     Default class for tracers, to be set as
     a metaclass for abstract base classes.
     """
     pass
 
 
-class ConcurrentUsedAuthTokenGuard(object):
+class ConcurrentUsedAuthTokenGuard:
     """
     Context manager preventing two tokens being used simultaneously.
     Throws UploadTokenUsedConcurrently when unable to acquire a lock
     Sample usage:
 
     with ConcurrentUsedAuthTokenGuard(lock_for_token, token):
         # code that uses the token exclusively
@@ -422,21 +470,46 @@
 
     def __init__(self, lock, token):
         self.lock = lock
         self.token = token
 
     def __enter__(self):
         if not self.lock.acquire(False):
-            from b2sdk.exception import UploadTokenUsedConcurrently
+            from b2sdk._internal.exception import UploadTokenUsedConcurrently
             raise UploadTokenUsedConcurrently(self.token)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         try:
             self.lock.release()
         except RuntimeError:
             # guard against releasing a non-acquired lock
             pass
 
 
+def current_time_millis():
+    """
+    File times are in integer milliseconds, to avoid roundoff errors.
+    """
+    return int(round(time.time() * 1000))
+
+
+def iterator_peek(iterator: Iterator[T], count: int) -> tuple[list[T], Iterator[T]]:
+    """
+    Get up to the `count` first elements yielded by `iterator`.
+
+    The function will read `count` elements from `iterator` or less if the end is reached first.  Returns a tuple
+    consisting of a list of retrieved elements and an iterator equivalent to the input iterator.
+    """
+
+    ret = []
+    for _ in range(count):
+        try:
+            ret.append(next(iterator))
+        except StopIteration:
+            break
+
+    return ret, chain(ret, iterator)
+
+
 assert disable_trace
 assert limit_trace_arguments
 assert trace_call
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `b2sdk-1.9.0/b2sdk/v0/__init__.py` & `b2sdk-2.0.0/b2sdk/v0/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # File: b2sdk/v0/__init__.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 from b2sdk.v1 import *  # noqa
 from b2sdk.v0.account_info import AbstractAccountInfo, InMemoryAccountInfo, UrlPoolAccountInfo, SqliteAccountInfo
 from b2sdk.v0.api import B2Api
 from b2sdk.v0.bucket import Bucket
 from b2sdk.v0.bucket import BucketFactory
 from b2sdk.v0.sync import Synchronizer
```

### Comparing `b2sdk-1.9.0/b2sdk/v0/account_info.py` & `b2sdk-2.0.0/b2sdk/v0/account_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 # File: b2sdk/v0/account_info.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from b2sdk import version_utils
+from b2sdk._internal import version_utils
 from b2sdk import v1
 
 
-class OldAccountInfoMethods(object):
+class OldAccountInfoMethods:
     """ this class contains proxy methods for deprecated signatures renamed for consistency in mid-2019 """
 
     def get_account_id_or_app_key_id(self):
         """
         Return the application key ID used to authenticate.
 
         :rtype: str
@@ -43,15 +44,15 @@
         realm,
         allowed=None,
         application_key_id=None,
         s3_api_url=None,
     ):
         # we need to enumerate all the parameters and cannot just "*args, **kwargs" because
         # the deprecation decorator doesn't feel safe with the kwargs approach
-        return super(OldAccountInfoMethods, self).set_auth_data(
+        return super().set_auth_data(
             account_id,
             auth_token,
             api_url,
             download_url,
             minimum_part_size,
             application_key,
             realm,
```

### Comparing `b2sdk-1.9.0/b2sdk/v0/api.py` & `b2sdk-2.0.0/b2sdk/v0/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # File: b2sdk/v0/api.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 from .bucket import Bucket, BucketFactory
 from b2sdk import v1
 
 
 class B2Api(v1.B2Api):
     BUCKET_FACTORY_CLASS = staticmethod(BucketFactory)
```

### Comparing `b2sdk-1.9.0/b2sdk/v0/bucket.py` & `b2sdk-2.0.0/b2sdk/v0/bucket.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # File: b2sdk/v0/bucket.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 from b2sdk import v1
 
 
 class Bucket(v1.Bucket):
     def list_file_names(self, start_filename=None, max_entries=None, prefix=None):
         """
```

### Comparing `b2sdk-1.9.0/b2sdk/v0/exception.py` & `b2sdk-2.0.0/b2sdk/v0/exception.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 # File: b2sdk/v0/exception.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 B2Error = None  # calm down, pyflakes
 
 from b2sdk.v1.exception import *  # noqa
 
 v1DestFileNewer = DestFileNewer
 
 
 # override to retain old style __str__
 class DestFileNewer(v1DestFileNewer):
     def __str__(self):
-        return 'source file is older than destination: %s%s with a time of %s cannot be synced to %s%s with a time of %s, unless --skipNewer or --replaceNewer is provided' % (
+        return 'source file is older than destination: {}{} with a time of {} cannot be synced to {}{} with a time of {}, unless --skipNewer or --replaceNewer is provided'.format(
             self.source_prefix,
             self.source_file.name,
             self.source_file.latest_version().mod_time,
             self.dest_prefix,
             self.dest_file.name,
             self.dest_file.latest_version().mod_time,
         )
```

### Comparing `b2sdk-1.9.0/b2sdk/v0/sync.py` & `b2sdk-2.0.0/b2sdk/v0/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # File: b2sdk/v0/sync.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import logging
 
 from b2sdk.v1.exception import CommandError
 from b2sdk.v1.exception import DestFileNewer as DestFileNewerV1
 from b2sdk.v1 import trace_call
 from .exception import DestFileNewer
@@ -28,30 +29,29 @@
 class Synchronizer(SynchronizerV1):
     """
     This is wrapper for newer version and will return the v0 style exceptions
     """
 
     def __init__(self, *args, **kwargs):
         try:
-            super(Synchronizer, self).__init__(*args, **kwargs)
+            super().__init__(*args, **kwargs)
         except InvalidArgument as e:
-            raise CommandError('--%s %s' % (e.parameter_name, e.message))
+            raise CommandError(f'--{e.parameter_name} {e.message}')
 
     def _make_file_sync_actions(self, *args, **kwargs):
         try:
-            for i in super(Synchronizer, self)._make_file_sync_actions(*args, **kwargs):
-                yield i
+            yield from super()._make_file_sync_actions(*args, **kwargs)
         except DestFileNewerV1 as e:
             raise DestFileNewer(e.dest_file, e.source_file, e.dest_prefix, e.source_prefix)
 
     def sync_folders(self, *args, **kwargs):
         try:
-            super(Synchronizer, self).sync_folders(*args, **kwargs)
+            super().sync_folders(*args, **kwargs)
         except InvalidArgument as e:
-            raise CommandError('--%s %s' % (e.parameter_name, e.message))
+            raise CommandError(f'--{e.parameter_name} {e.message}')
         except IncompleteSync as e:
             raise CommandError(str(e))
 
 
 def get_synchronizer_from_args(
     args,
     max_workers,
@@ -118,17 +118,17 @@
 ):
     """
     This is deprecated. Use the new Synchronizer class.
     Yields a sequence of actions that will sync the destination
     folder to the source folder.
 
     :param source_folder: source folder object
-    :type source_folder: b2sdk.sync.folder.AbstractFolder
+    :type source_folder: b2sdk._internal.scan.folder.AbstractFolder
     :param dest_folder: destination folder object
-    :type dest_folder: b2sdk.sync.folder.AbstractFolder
+    :type dest_folder: b2sdk._internal.scan.folder.AbstractFolder
     :param args: an object which holds command line arguments
     :param now_millis: current time in milliseconds
     :type now_millis: int
     :param reporter: reporter object
     :param policies_manager: policies manager object
     :param encryption_settings_provider: encryption settings provider
     :type encryption_settings_provider: AbstractSyncEncryptionSettingsProvider
@@ -146,15 +146,15 @@
             dest_folder,
             now_millis,
             reporter,
             policies_manager=policies_manager,
             encryption_settings_provider=encryption_settings_provider
         )
     except InvalidArgument as e:
-        raise CommandError('--%s %s' % (e.parameter_name, e.message))
+        raise CommandError(f'--{e.parameter_name} {e.message}')
 
 
 @trace_call(logger)
 def sync_folders(
     source_folder,
     dest_folder,
     args,
@@ -171,17 +171,17 @@
     """
     This is deprecated. Use the new Synchronizer class.
 
     source is also in the destination.  Deletes any file versions
     in the destination older than history_days.
 
     :param source_folder: source folder object
-    :type source_folder: b2sdk.sync.folder.AbstractFolder
+    :type source_folder: b2sdk._internal.scan.folder.AbstractFolder
     :param dest_folder: destination folder object
-    :type dest_folder: b2sdk.sync.folder.AbstractFolder
+    :type dest_folder: b2sdk._internal.scan.folder.AbstractFolder
     :param args: an object which holds command line arguments
     :param now_millis: current time in milliseconds
     :type now_millis: int
     :param stdout: standard output file object
     :param no_progress: if True, do not show progress
     :type no_progress: bool
     :param max_workers: max number of workers
```

### Comparing `b2sdk-1.9.0/b2sdk/v1/__init__.py` & `b2sdk-2.0.0/b2sdk/v1/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,33 @@
 # File: b2sdk/v1/__init__.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from b2sdk._v2 import *  # noqa
+from b2sdk.v2 import *  # noqa
 from b2sdk.v1.account_info import (
     AbstractAccountInfo, InMemoryAccountInfo, UrlPoolAccountInfo, SqliteAccountInfo, StubAccountInfo
 )
 from b2sdk.v1.api import B2Api
+from b2sdk.v1.b2http import B2Http
 from b2sdk.v1.bucket import Bucket, BucketFactory
 from b2sdk.v1.cache import AbstractCache
+from b2sdk.v1.download_dest import (
+    AbstractDownloadDestination, DownloadDestLocalFile, PreSeekedDownloadDest, DownloadDestBytes,
+    DownloadDestProgressWrapper
+)
 from b2sdk.v1.exception import CommandError, DestFileNewer
+from b2sdk.v1.file_metadata import FileMetadata
 from b2sdk.v1.file_version import FileVersionInfo
 from b2sdk.v1.session import B2Session
 from b2sdk.v1.sync import (
     ScanPoliciesManager, DEFAULT_SCAN_MANAGER, zip_folders, Synchronizer, AbstractFolder,
-    LocalFolder, B2Folder, parse_sync_folder, File, B2File, FileVersion,
+    LocalFolder, B2Folder, parse_sync_folder, SyncReport, File, B2File, FileVersion,
     AbstractSyncEncryptionSettingsProvider
 )
+from b2sdk.v1.replication.monitoring import ReplicationMonitor
+
+B2RawApi = B2RawHTTPApi
```

### Comparing `b2sdk-1.9.0/b2sdk/v1/account_info.py` & `b2sdk-2.0.0/b2sdk/v1/account_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # File: b2sdk/v1/account_info.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 from abc import abstractmethod
 import inspect
 import logging
 import os
-from typing import Optional
 
-from b2sdk import _v2 as v2
-from b2sdk.account_info.sqlite_account_info import DEFAULT_ABSOLUTE_MINIMUM_PART_SIZE
-from b2sdk.utils import limit_trace_arguments
+from b2sdk import v2
+from b2sdk._internal.account_info.sqlite_account_info import DEFAULT_ABSOLUTE_MINIMUM_PART_SIZE
+from b2sdk._internal.utils import limit_trace_arguments
 
 logger = logging.getLogger(__name__)
 
 
 # Retain legacy get_minimum_part_size and facilitate for optional s3_api_url
 class OldAccountInfoMethods:
     REALM_URLS = v2.REALM_URLS
@@ -113,15 +113,15 @@
         """
         Return s3_api_url or raises MissingAccountData exception.
 
         :rtype: str
         """
         # Removed @abstractmethod decorators
 
-    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> Optional[str]:
+    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> str | None:
         """
         Look up the bucket name for the given bucket id.
         """
         # Removed @abstractmethod decorator
 
     def get_recommended_part_size(self):
         """
```

### Comparing `b2sdk-1.9.0/b2sdk/v1/cache.py` & `b2sdk-2.0.0/b2sdk/v1/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # File: b2sdk/v1/cache.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
-from typing import Optional
+from __future__ import annotations
 
-from b2sdk import _v2 as v2
+from b2sdk import v2
 
 
 class AbstractCache(v2.AbstractCache):
-    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> Optional[str]:
+    def get_bucket_name_or_none_from_bucket_id(self, bucket_id: str) -> str | None:
         return None
         # Removed @abstractmethod decorator
```

### Comparing `b2sdk-1.9.0/b2sdk/v1/exception.py` & `b2sdk-2.0.0/b2sdk/v1/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 # File: b2sdk/v1/exception.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from b2sdk._v2.exception import *  # noqa
+from b2sdk.v2.exception import *  # noqa
 v2DestFileNewer = DestFileNewer
 
 
 # This exception class is deprecated and should not be used in new designs
 class CommandError(B2Error):
     """
     b2 command error (user caused).  Accepts exactly one argument: message.
 
     We expect users of shell scripts will parse our ``__str__`` output.
     """
 
     def __init__(self, message):
-        super(CommandError, self).__init__()
+        super().__init__()
         self.message = message
 
     def __str__(self):
         return self.message
 
 
 class DestFileNewer(v2DestFileNewer):
@@ -33,15 +34,15 @@
         super(v2DestFileNewer, self).__init__()
         self.dest_file = dest_file
         self.source_file = source_file
         self.dest_prefix = dest_prefix
         self.source_prefix = source_prefix
 
     def __str__(self):
-        return 'source file is older than destination: %s%s with a time of %s cannot be synced to %s%s with a time of %s, unless a valid newer_file_mode is provided' % (
+        return 'source file is older than destination: {}{} with a time of {} cannot be synced to {}{} with a time of {}, unless a valid newer_file_mode is provided'.format(
             self.source_prefix,
             self.source_file.name,
             self.source_file.latest_version().mod_time,
             self.dest_prefix,
             self.dest_file.name,
             self.dest_file.latest_version().mod_time,
         )
```

### Comparing `b2sdk-1.9.0/b2sdk/v1/file_version.py` & `b2sdk-2.0.0/b2sdk/_internal/transfer/inbound/downloader/simple.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,138 +1,93 @@
 ######################################################################
 #
-# File: b2sdk/v1/file_version.py
+# File: b2sdk/_internal/transfer/inbound/downloader/simple.py
 #
-# Copyright 2021 Backblaze Inc. All Rights Reserved.
+# Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from typing import Optional
-import datetime
-import functools
+import logging
+from io import IOBase
 
-from b2sdk import _v2 as v2
-from ..raw_api import SRC_LAST_MODIFIED_MILLIS
-from . import api as v1api
+from requests.models import Response
 
+from b2sdk._internal.encryption.setting import EncryptionSetting
+from b2sdk._internal.file_version import DownloadVersion
+from b2sdk._internal.session import B2Session
 
-# Override to retain legacy class name, __init__ signature, slots
-# and old formatting methods
-class FileVersionInfo(v2.FileVersion):
-    __slots__ = ['_api']
+from .abstract import AbstractDownloader
 
-    LS_ENTRY_TEMPLATE = '%83s  %6s  %10s  %8s  %9d  %s'  # order is file_id, action, date, time, size, name
+logger = logging.getLogger(__name__)
 
-    def __init__(
+
+class SimpleDownloader(AbstractDownloader):
+
+    REQUIRES_SEEKING = False
+
+    def _download(
         self,
-        id_,
-        file_name,
-        size,
-        content_type,
-        content_sha1,
-        file_info,
-        upload_timestamp,
-        action,
-        content_md5=None,
-        server_side_encryption: Optional[v2.EncryptionSetting] = None,
-        file_retention: Optional[v2.FileRetentionSetting] = None,
-        legal_hold: Optional[v2.LegalHold] = None,
-        api: Optional['v1api.B2Api'] = None,
+        file: IOBase,
+        response: Response,
+        download_version: DownloadVersion,
+        session: B2Session,
+        encryption: EncryptionSetting | None = None,
     ):
-        self.id_ = id_
-        self.file_name = file_name
-        self.size = size
-        self.content_type = content_type
-        self.content_sha1 = content_sha1
-        self.content_md5 = content_md5
-        self.file_info = file_info or {}
-        self.upload_timestamp = upload_timestamp
-        self.action = action
-        self.server_side_encryption = server_side_encryption
-        self.legal_hold = legal_hold
-        self.file_retention = file_retention
-        self._api = api
-
-        if SRC_LAST_MODIFIED_MILLIS in self.file_info:
-            self.mod_time_millis = int(self.file_info[SRC_LAST_MODIFIED_MILLIS])
-        else:
-            self.mod_time_millis = self.upload_timestamp
-
-    @property
-    def api(self):
-        if self._api is None:
-            raise ValueError('"api" not set')
-        return self._api
-
-    def format_ls_entry(self):
-        dt = datetime.datetime.utcfromtimestamp(self.upload_timestamp / 1000)
-        date_str = dt.strftime('%Y-%m-%d')
-        time_str = dt.strftime('%H:%M:%S')
-        size = self.size or 0  # required if self.action == 'hide'
-        return self.LS_ENTRY_TEMPLATE % (
-            self.id_,
-            self.action,
-            date_str,
-            time_str,
-            size,
-            self.file_name,
-        )
+        actual_size = self._get_remote_range(response, download_version).size()
+        chunk_size = self._get_chunk_size(actual_size)
+
+        digest = self._get_hasher()
 
-    @classmethod
-    def format_folder_ls_entry(cls, name):
-        return cls.LS_ENTRY_TEMPLATE % ('-', '-', '-', '-', 0, name)
-
-
-def file_version_info_from_new_file_version(file_version: v2.FileVersion) -> FileVersionInfo:
-    return FileVersionInfo(
-        **{
-            att_name: getattr(file_version, att_name)
-            for att_name in [
-                'id_',
-                'file_name',
-                'size',
-                'content_type',
-                'content_sha1',
-                'file_info',
-                'upload_timestamp',
-                'action',
-                'content_md5',
-                'server_side_encryption',
-                'legal_hold',
-                'file_retention',
-                'api',
-            ]
-        }
-    )
-
-
-def translate_single_file_version(func):
-    @functools.wraps(func)
-    def inner(*a, **kw):
-        return file_version_info_from_new_file_version(func(*a, **kw))
-
-    return inner
-
-
-# override to return old style FileVersionInfo
-class FileVersionInfoFactory(v2.FileVersionFactory):
-
-    from_api_response = translate_single_file_version(v2.FileVersionFactory.from_api_response)
-    from_response_headers = translate_single_file_version(
-        v2.FileVersionFactory.from_response_headers
-    )
-
-
-def file_version_info_from_id_and_name(file_id_and_name: v2.FileIdAndName, api: 'v1api.B2Api'):
-    return FileVersionInfo(
-        id_=file_id_and_name.file_id,
-        file_name=file_id_and_name.file_name,
-        size=0,
-        content_type='unknown',
-        content_sha1='none',
-        file_info={},
-        upload_timestamp=0,
-        action='cancel',
-        api=api,
-    )
+        bytes_read = 0
+        for data in response.iter_content(chunk_size=chunk_size):
+            file.write(data)
+            digest.update(data)
+            bytes_read += len(data)
+
+        assert actual_size >= 1  # code below does `actual_size - 1`, but it should never reach that part with an empty file
+
+        # now, normally bytes_read == download_version.content_length, but sometimes there is a timeout
+        # or something and the server closes connection, while neither tcp or http have a problem
+        # with the truncated output, so we detect it here and try to continue
+
+        num_tries = 5  # this is hardcoded because we are going to replace the entire retry interface soon, so we'll avoid deprecation here and keep it private
+        retries_left = num_tries - 1
+        while retries_left and bytes_read < download_version.content_length:
+            new_range = self._get_remote_range(
+                response,
+                download_version,
+            ).subrange(bytes_read, actual_size - 1)
+            # original response is not closed at this point yet, as another layer is responsible for closing it, so a new socket might be allocated,
+            # but this is a very rare case and so it is not worth the optimization
+            logger.debug(
+                're-download attempts remaining: %i, bytes read already: %i. Getting range %s now.',
+                retries_left, bytes_read, new_range
+            )
+            with session.download_file_from_url(
+                response.request.url,
+                new_range.as_tuple(),
+                encryption=encryption,
+            ) as followup_response:
+                for data in followup_response.iter_content(
+                    chunk_size=self._get_chunk_size(actual_size)
+                ):
+                    file.write(data)
+                    digest.update(data)
+                    bytes_read += len(data)
+            retries_left -= 1
+        return bytes_read, digest.hexdigest()
+
+    def download(
+        self,
+        file: IOBase,
+        response: Response,
+        download_version: DownloadVersion,
+        session: B2Session,
+        encryption: EncryptionSetting | None = None,
+    ):
+        future = self._thread_pool.submit(
+            self._download, file, response, download_version, session, encryption
+        )
+        return future.result()
```

### Comparing `b2sdk-1.9.0/b2sdk/v1/session.py` & `b2sdk-2.0.0/b2sdk/v1/session.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,23 +3,44 @@
 # File: b2sdk/v1/session.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from b2sdk import _v2 as v2
+from b2sdk import v2
+from b2sdk.v2.exception import InvalidArgument
 from .account_info import SqliteAccountInfo
 
 
 # Override to use legacy signature of account_info.set_auth_data, especially the minimum_part_size argument
+# and to accept old-style raw_api argument
 class B2Session(v2.B2Session):
     SQLITE_ACCOUNT_INFO_CLASS = staticmethod(SqliteAccountInfo)
 
+    def __init__(
+        self,
+        account_info=None,
+        cache=None,
+        raw_api: v2.B2RawHTTPApi = None,
+        api_config: v2.B2HttpApiConfig | None = None
+    ):
+        if raw_api is not None and api_config is not None:
+            raise InvalidArgument(
+                'raw_api,api_config', 'Provide at most one of: raw_api, api_config'
+            )
+
+        if api_config is None:
+            api_config = v2.DEFAULT_HTTP_API_CONFIG
+        super().__init__(account_info=account_info, cache=cache, api_config=api_config)
+        if raw_api is not None:
+            self.raw_api = raw_api
+
     def authorize_account(self, realm, application_key_id, application_key):
         """
         Perform account authorization.
 
         :param str realm: a realm to authorize account in (usually just "production")
         :param str application_key_id: :term:`application key ID`
         :param str application_key: user's :term:`application key`
```

### Comparing `b2sdk-1.9.0/b2sdk/v1/sync/file.py` & `b2sdk-2.0.0/b2sdk/v1/sync/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,74 +3,73 @@
 # File: b2sdk/v1/sync/file.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
-
-from typing import List
+from __future__ import annotations
 
 from b2sdk.v1 import FileVersionInfo
-from b2sdk.raw_api import SRC_LAST_MODIFIED_MILLIS
+from b2sdk._internal.http_constants import SRC_LAST_MODIFIED_MILLIS
 
 
 # This whole module is here to retain legacy classes so they can be used in retained legacy exception
-class File(object):
+class File:
     """
     Hold information about one file in a folder.
 
     The name is relative to the folder in all cases.
 
     Files that have multiple versions (which only happens
     in B2, not in local folders) include information about
     all of the versions, most recent first.
     """
 
     __slots__ = ['name', 'versions']
 
-    def __init__(self, name, versions: List['FileVersion']):
+    def __init__(self, name, versions: list[FileVersion]):
         """
         :param str name: a relative file name
         :param List[FileVersion] versions: a list of file versions
         """
         self.name = name
         self.versions = versions
 
-    def latest_version(self) -> 'FileVersion':
+    def latest_version(self) -> FileVersion:
         """
         Return the latest file version.
         """
         return self.versions[0]
 
     def __repr__(self):
-        return '%s(%s, [%s])' % (
+        return '{}({}, [{}])'.format(
             self.__class__.__name__, self.name, ', '.join(repr(v) for v in self.versions)
         )
 
 
 class B2File(File):
     """
     Hold information about one file in a folder in B2 cloud.
     """
 
     __slots__ = ['name', 'versions']
 
-    def __init__(self, name, versions: List['FileVersion']):
+    def __init__(self, name, versions: list[FileVersion]):
         """
         :param str name: a relative file name
         :param List[FileVersion] versions: a list of file versions
         """
         super().__init__(name, versions)
 
-    def latest_version(self) -> 'FileVersion':
+    def latest_version(self) -> FileVersion:
         return super().latest_version()
 
 
-class FileVersion(object):
+class FileVersion:
     """
     Hold information about one version of a file.
     """
 
     __slots__ = ['id_', 'name', 'mod_time', 'action', 'size']
 
     def __init__(self, id_, file_name, mod_time, action, size):
@@ -90,15 +89,15 @@
         self.id_ = id_
         self.name = file_name
         self.mod_time = mod_time
         self.action = action
         self.size = size
 
     def __repr__(self):
-        return '%s(%s, %s, %s, %s)' % (
+        return '{}({}, {}, {}, {})'.format(
             self.__class__.__name__,
             repr(self.id_),
             repr(self.name),
             repr(self.mod_time),
             repr(self.action),
         )
```

### Comparing `b2sdk-1.9.0/b2sdk/v1/sync/file_to_path_translator.py` & `b2sdk-2.0.0/b2sdk/v1/sync/file_to_path_translator.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # File: b2sdk/v1/sync/file_to_path_translator.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from typing import Tuple
+from b2sdk import v2
 
-from b2sdk import _v2 as v2
-from .file import File, B2File, FileVersion, B2FileVersion
+from .file import B2File, B2FileVersion, File, FileVersion
 
 
 # The goal is to create v1.File objects together with v1.FileVersion objects from v2.SyncPath objects
 def make_files_from_paths(
     dest_path: v2.AbstractSyncPath, source_path: v2.AbstractSyncPath, sync_type: str
-) -> Tuple[File, File]:
+) -> tuple[File, File]:
     assert sync_type in ('b2-to-b2', 'b2-to-local', 'local-to-b2')
     sync_type_split = sync_type.split('-')
 
     dest_type = sync_type_split[-1]
     dest_file = _path_translation_map[dest_type](dest_path)
 
     source_type = sync_type_split[0]
@@ -47,15 +47,15 @@
 
 
 _path_translation_map = {'b2': _translate_b2_path_to_file, 'local': _translate_local_path_to_file}
 
 
 # The goal is to create v2.SyncPath objects from v1.File objects
 def make_paths_from_files(dest_file: File, source_file: File,
-                          sync_type: str) -> Tuple[v2.AbstractSyncPath, v2.AbstractSyncPath]:
+                          sync_type: str) -> tuple[v2.AbstractSyncPath, v2.AbstractSyncPath]:
     assert sync_type in ('b2-to-b2', 'b2-to-local', 'local-to-b2')
     sync_type_split = sync_type.split('-')
 
     dest_type = sync_type_split[-1]
     dest_path = _file_translation_map[dest_type](dest_file)
 
     source_type = sync_type_split[0]
```

### Comparing `b2sdk-1.9.0/b2sdk/v1/sync/folder.py` & `b2sdk-2.0.0/b2sdk/v1/sync/folder.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,35 +3,36 @@
 # File: b2sdk/v1/sync/folder.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 from abc import abstractmethod
 import functools
 
-from b2sdk import _v2 as v2
+from b2sdk import v2
 from .scan_policies import DEFAULT_SCAN_MANAGER, wrap_if_necessary
 from .. import exception
 
 
 def translate_errors(func):
     @functools.wraps(func)
     def wrapper(*a, **kw):
         try:
             return func(*a, **kw)
         except exception.NotADirectory as ex:
-            raise Exception('%s is not a directory' % (ex.path,))
+            raise Exception(f'{ex.path} is not a directory')
         except exception.UnableToCreateDirectory as ex:
-            raise Exception('unable to create directory %s' % (ex.path,))
+            raise Exception(f'unable to create directory {ex.path}')
         except exception.EmptyDirectory as ex:
             raise exception.CommandError(
-                'Directory %s is empty.  Use --allowEmptySource to sync anyway.' % (ex.path,)
+                f'Directory {ex.path} is empty.  Use --allowEmptySource to sync anyway.'
             )
 
     return wrapper
 
 
 # Override to change "policies_manager" default argument
 class AbstractFolder(v2.AbstractFolder):
@@ -42,14 +43,22 @@
 
 # override to retain "policies_manager" default argument,
 # and wrap policies_manager
 class B2Folder(v2.B2Folder, AbstractFolder):
     def all_files(self, reporter, policies_manager=DEFAULT_SCAN_MANAGER):
         return super().all_files(reporter, wrap_if_necessary(policies_manager))
 
+    def get_file_versions(self):
+        for file_version, _ in self.bucket.ls(
+            self.folder_name,
+            show_versions=True,
+            recursive=True,
+        ):
+            yield file_version
+
 
 # override to retain "policies_manager" default argument,
 # translate nice errors to old style Exceptions and CommandError
 # and wrap policies_manager
 class LocalFolder(v2.LocalFolder, AbstractFolder):
     @translate_errors
     def ensure_present(self):
```

### Comparing `b2sdk-1.9.0/b2sdk/v1/sync/folder_parser.py` & `b2sdk-2.0.0/b2sdk/v1/sync/folder_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 # File: b2sdk/v1/sync/folder_parser.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from b2sdk import _v2 as v2
+from b2sdk import v2
 from .. import exception
 
 from .folder import LocalFolder, B2Folder
 
 
 # Override to use v1 version of "LocalFolder" and "B2Folder" and raise old style CommandError
 def parse_sync_folder(folder_name, api):
```

### Comparing `b2sdk-1.9.0/b2sdk/v1/sync/scan_policies.py` & `b2sdk-2.0.0/b2sdk/v1/sync/scan_policies.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,24 @@
 # File: b2sdk/v1/sync/scan_policies.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
 import re
-from typing import Optional, Union, Iterable
+from typing import Iterable
 
 from .file import B2FileVersion
 from ..file_version import FileVersionInfo
 from .file_to_path_translator import _translate_local_path_to_file
-from b2sdk import _v2 as v2
-from b2sdk._v2 import exception as v2_exception  # noqa
-
-try:  # python 3.5 and 3.6 compatibility
-    regex_class = re.Pattern
-except AttributeError:
-    regex_class = re._pattern_type
+from b2sdk import v2
+from b2sdk.v2 import exception as v2_exception  # noqa
 
 
 # Override to retain old exceptions in __init__
 # and to provide interface for new should_exclude_* methods
 class ScanPoliciesManager(v2.ScanPoliciesManager):
     """
     Policy object used when scanning folders for syncing, used to decide
@@ -37,22 +33,22 @@
     Code that scans may optionally use should_exclude_directory() to test whether
     it can skip a directory completely and not bother listing the files and
     sub-directories in it.
     """
 
     def __init__(
         self,
-        exclude_dir_regexes: Iterable[Union[str, regex_class]] = tuple(),
-        exclude_file_regexes: Iterable[Union[str, regex_class]] = tuple(),
-        include_file_regexes: Iterable[Union[str, regex_class]] = tuple(),
+        exclude_dir_regexes: Iterable[str | re.Pattern] = tuple(),
+        exclude_file_regexes: Iterable[str | re.Pattern] = tuple(),
+        include_file_regexes: Iterable[str | re.Pattern] = tuple(),
         exclude_all_symlinks: bool = False,
-        exclude_modified_before: Optional[int] = None,
-        exclude_modified_after: Optional[int] = None,
-        exclude_uploaded_before: Optional[int] = None,
-        exclude_uploaded_after: Optional[int] = None,
+        exclude_modified_before: int | None = None,
+        exclude_modified_after: int | None = None,
+        exclude_uploaded_before: int | None = None,
+        exclude_uploaded_after: int | None = None,
     ):
         """
         :param exclude_dir_regexes: regexes to exclude directories
         :param exclude_file_regexes: regexes to exclude files
         :param include_file_regexes: regexes to include files
         :param exclude_all_symlinks: if True, exclude all symlinks
         :param exclude_modified_before: optionally exclude file versions (both local and b2) modified before (in millis)
@@ -132,18 +128,15 @@
 
 class ScanPoliciesManagerWrapper(v2.ScanPoliciesManager):
     def __init__(self, scan_policies_manager: ScanPoliciesManager):
         self.scan_policies_manager = scan_policies_manager
         self.exclude_all_symlinks = scan_policies_manager.exclude_all_symlinks
 
     def __repr__(self):
-        return "%s(%s)" % (
-            self.__class__.__name__,
-            self.scan_policies_manager,
-        )
+        return f"{self.__class__.__name__}({self.scan_policies_manager})"
 
     def should_exclude_local_path(self, local_path: v2.LocalSyncPath):
         if self.scan_policies_manager.should_exclude_file_version(
             _translate_local_path_to_file(local_path).latest_version()
         ):
             return True
         return self.scan_policies_manager.should_exclude_file(local_path.relative_path)
```

### Comparing `b2sdk-1.9.0/b2sdk/v1/sync/sync.py` & `b2sdk-2.0.0/b2sdk/v1/sync/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 # File: b2sdk/v1/sync/sync.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from b2sdk import _v2 as v2
-from b2sdk._v2 import exception as v2_exception
+from b2sdk import v2
+from b2sdk.v2 import exception as v2_exception
 from .file_to_path_translator import make_files_from_paths, make_paths_from_files
 from .scan_policies import DEFAULT_SCAN_MANAGER, wrap_if_necessary as scan_wrap_if_necessary
 from .encryption_provider import wrap_if_necessary as encryption_wrap_if_necessary
 from ..exception import DestFileNewer
 
 
 # Override to change "policies_manager" default argument
@@ -33,18 +34,27 @@
         dry_run=False,
         allow_empty_source=False,
         newer_file_mode=v2.NewerFileSyncMode.RAISE_ERROR,
         keep_days_or_delete=v2.KeepOrDeleteMode.NO_DELETE,
         compare_version_mode=v2.CompareVersionMode.MODTIME,
         compare_threshold=None,
         keep_days=None,
+        sync_policy_manager: v2.SyncPolicyManager = v2.POLICY_MANAGER,
     ):
         super().__init__(
-            max_workers, scan_wrap_if_necessary(policies_manager), dry_run, allow_empty_source,
-            newer_file_mode, keep_days_or_delete, compare_version_mode, compare_threshold, keep_days
+            max_workers,
+            scan_wrap_if_necessary(policies_manager),
+            dry_run,
+            allow_empty_source,
+            newer_file_mode,
+            keep_days_or_delete,
+            compare_version_mode,
+            compare_threshold,
+            keep_days,
+            sync_policy_manager,
         )
 
     def make_folder_sync_actions(
         self,
         source_folder,
         dest_folder,
         now_millis,
```

### Comparing `b2sdk-1.9.0/b2sdk/version_utils.py` & `b2sdk-2.0.0/b2sdk/_internal/version_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,91 +1,103 @@
 ######################################################################
 #
-# File: b2sdk/version_utils.py
+# File: b2sdk/_internal/version_utils.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from abc import ABCMeta, abstractmethod
-from functools import wraps
 import inspect
+import re
 import warnings
+from abc import ABCMeta, abstractmethod
+from functools import total_ordering, wraps
 
-from pkg_resources import parse_version
 from b2sdk.version import VERSION
 
 
+@total_ordering
+class _Version:
+    """
+    Rudimentary semver version parser.
+
+    It uses VERY naive parsing which is only supposed to produce a tuple, able to
+    compare major.minor.patch versions.
+    It does not support PEP 440 epoch, pre-releases, post-releases, local versions, etc.
+    """
+
+    def __init__(self, version: str):
+        self._raw = version
+        self._parsed = self._parse_version(version)
+
+    def __str__(self):
+        return self._raw
+
+    def __eq__(self, other):
+        return self._parsed == other._parsed
+
+    def __lt__(self, other):
+        return self._parsed < other._parsed
+
+    @classmethod
+    def _parse_version(cls, version: str) -> tuple[int, ...]:
+        if "!" in version:  # strip PEP 440 epoch
+            version = version.split("!", 1)[1]
+        return tuple(map(int, re.findall(r'\d+', version)))
+
+
 class AbstractVersionDecorator(metaclass=ABCMeta):
     WHAT = NotImplemented  # 'function', 'method', 'class' etc
 
     def __init__(self, changed_version, cutoff_version=None, reason='', current_version=None):
         """
         Changed_version, cutoff_version and current_version are version strings.
         """
         if current_version is None:  # this is for tests only
             current_version = VERSION  # TODO autodetect by going up the qualname tree and trying getattr(part, '__version__')
-        self.current_version = parse_version(current_version)  #: current version
+        self.current_version = _Version(current_version)  #: current version
         self.reason = reason
 
-        self.changed_version = parse_version(
+        self.changed_version = self._parse_if_not_none(
             changed_version
         )  #: version in which the decorator was added
         self.cutoff_version = self._parse_if_not_none(
             cutoff_version
         )  #: version in which the decorator (and something?) shall be removed
 
     @classmethod
     def _parse_if_not_none(cls, version):
         if version is None:
             return None
-        return parse_version(version)
+        return _Version(version)
 
     @abstractmethod
     def __call__(self, func):
         """
         The actual implementation of decorator. Needs self.source to be set before it's called.
         """
-        if self.cutoff_version is not None:
-            assert self.changed_version < self.cutoff_version, '%s decorator is set to start renaming %s %r starting at version %s and finishing in %s. It needs to start at a lower version and finish at a higher version.' % (
+        if self.cutoff_version and self.changed_version:
+            assert self.changed_version < self.cutoff_version, '{} decorator is set to start renaming {} {!r} starting at version {} and finishing in {}. It needs to start at a lower version and finish at a higher version.'.format(
                 self.__class__.__name__,
                 self.WHAT,
                 self.source,
                 self.changed_version,
                 self.cutoff_version,
             )
-            assert self.current_version < self.cutoff_version, '%s decorator is still used in version %s when old %s name %r was scheduled to be dropped in %s. It is time to remove the mapping.' % (
-                self.__class__.__name__,
-                self.current_version,
-                self.WHAT,
-                self.source,
-                self.cutoff_version,
-            )
 
 
 class AbstractDeprecator(AbstractVersionDecorator):
     ALTERNATIVE_DECORATOR = NotImplemented
 
     def __init__(self, target, *args, **kwargs):
         self.target = target
-        super(AbstractDeprecator, self).__init__(*args, **kwargs)
-
-    @abstractmethod
-    def __call__(self, func):
-        super(AbstractDeprecator, self).__call__(func)
-        assert self.changed_version <= self.current_version, '%s decorator indicates that the replacement of %s %r should take place in the future version %s, while the current version is %s. It looks like should be _discouraged_ at this point and not _deprecated_ yet. Consider using %r decorator instead.' % (
-            self.__class__.__name__,
-            self.WHAT,
-            self.source,
-            self.changed_version,
-            self.cutoff_version,
-            self.ALTERNATIVE_DECORATOR,
-        )
+        super().__init__(*args, **kwargs)
 
 
 class rename_argument(AbstractDeprecator):
     """
     Change the argument name to new one if old one is used, warns about deprecation in docs and through a warning.
 
     >>> @rename_argument('aaa', 'bbb', '0.1.0', '0.2.0')
@@ -98,42 +110,40 @@
     >>>
     """
     WHAT = 'argument'
     ALTERNATIVE_DECORATOR = 'discourage_argument'
 
     def __init__(self, source, *args, **kwargs):
         self.source = source
-        super(rename_argument, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     def __call__(self, func):
-        super(rename_argument, self).__call__(func)
+        super().__call__(func)
+        signature = inspect.signature(func)
+        has_target_arg = self.target in signature.parameters or any(
+            p.kind == p.VAR_KEYWORD for p in signature.parameters.values()
+        )
+        assert has_target_arg, f'{self.target!r} is not an argument of the decorated function so it cannot be remapped to from a deprecated parameter name'
 
         @wraps(func)
         def wrapper(*args, **kwargs):
-            message = '%r is not an argument of the decorated function so it cannot be remapped to from a deprecated parameter name' % (
-                self.target,
-            )
-            signature = inspect.getfullargspec(func)
-            assert self.target in signature.args or self.target in signature.kwonlyargs, message
-
             if self.source in kwargs:
-                assert self.target not in kwargs, 'both argument names were provided: %r (deprecated) and %r (new)' % (
+                assert self.target not in kwargs, 'both argument names were provided: {!r} (deprecated) and {!r} (new)'.format(
                     self.source, self.target
                 )
                 kwargs[self.target] = kwargs[self.source]
                 del kwargs[self.source]
+                info = f'{self.source!r} is a deprecated argument for {func.__name__!r} function/method - it was renamed to {self.target!r}'
+                if self.changed_version:
+                    info += f' in version {self.changed_version}'
+                if self.cutoff_version:
+                    info += f'. Support for the old name is going to be dropped in {self.cutoff_version}'
+
                 warnings.warn(
-                    '%r is a deprecated argument for %r function/method - it was renamed to %r in version %s. Support for the old name is going to be dropped in %s.'
-                    % (
-                        self.source,
-                        func.__name__,
-                        self.target,
-                        self.changed_version,
-                        self.cutoff_version,
-                    ),
+                    f"{info}.",
                     DeprecationWarning,
                 )
             return func(*args, **kwargs)
 
         return wrapper
 
 
@@ -154,25 +164,25 @@
     """
     WHAT = 'function'
     ALTERNATIVE_DECORATOR = 'discourage_function'
 
     def __init__(self, target, *args, **kwargs):
         if callable(target):
             target = target.__name__
-        super(rename_function, self).__init__(target, *args, **kwargs)
+        super().__init__(target, *args, **kwargs)
 
     def __call__(self, func):
         self.source = func.__name__
-        super(rename_function, self).__call__(func)
+        super().__call__(func)
 
         @wraps(func)
         def wrapper(*args, **kwargs):
             warnings.warn(
-                '%r is deprecated since version %s - it was moved to %r, please switch to use that. The proxy for the old name is going to be removed in %s.'
-                % (
+                '{!r} is deprecated since version {} - it was moved to {!r}, please switch to use that. The proxy for the old name is going to be removed in {}.'
+                .format(
                     func.__name__,
                     self.changed_version,
                     self.target,
                     self.cutoff_version,
                 ),
                 DeprecationWarning,
             )
```

### Comparing `b2sdk-1.9.0/test/unit/v1/test_copy_manager.py` & `b2sdk-2.0.0/b2sdk/v1/file_version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,150 +1,205 @@
 ######################################################################
 #
-# File: test/unit/v1/test_copy_manager.py
+# File: b2sdk/v1/file_version.py
 #
 # Copyright 2021 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+from __future__ import annotations
 
-from ..test_base import TestBase
-
-from .deps_exception import InvalidAuthToken, Unauthorized, SSECKeyIdMismatchInCopy
-from .deps import MetadataDirectiveMode
-from .deps import EncryptionAlgorithm, EncryptionSetting, EncryptionMode, EncryptionKey, SSE_NONE, SSE_B2_AES
-from b2sdk.transfer.outbound.copy_manager import CopyManager
-from b2sdk.encryption.setting import SSE_C_KEY_ID_FILE_INFO_KEY_NAME
-
-SSE_C_AES = EncryptionSetting(
-    mode=EncryptionMode.SSE_C,
-    algorithm=EncryptionAlgorithm.AES256,
-    key=EncryptionKey(secret=b'some_key', key_id='some-id'),
-)
-SSE_C_AES_2 = EncryptionSetting(
-    mode=EncryptionMode.SSE_C,
-    algorithm=EncryptionAlgorithm.AES256,
-    key=EncryptionKey(secret=b'some_other_key', key_id='some-id-2'),
-)
-
-
-class TestCopyManager(TestBase):
-    def test_establish_sse_c_replace(self):
-        file_info = {'some_key': 'some_value'}
-        content_type = 'text/plain'
-        metadata_directive, new_file_info, new_content_type = CopyManager.establish_sse_c_file_metadata(
-            MetadataDirectiveMode.REPLACE,
-            destination_file_info=file_info,
-            destination_content_type=content_type,
-            destination_server_side_encryption=SSE_C_AES,
-            source_server_side_encryption=SSE_C_AES_2,
-            source_file_info=None,
-            source_content_type=None,
-        )
-        self.assertEqual(
-            (
-                MetadataDirectiveMode.REPLACE, {
-                    'some_key': 'some_value',
-                    SSE_C_KEY_ID_FILE_INFO_KEY_NAME: 'some-id'
-                }, content_type
-            ), (metadata_directive, new_file_info, new_content_type)
-        )
-
-    def test_establish_sse_c_copy_no_enc(self):
-        file_info = {}
-        content_type = 'text/plain'
-        metadata_directive, new_file_info, new_content_type = CopyManager.establish_sse_c_file_metadata(
-            MetadataDirectiveMode.COPY,
-            destination_file_info=file_info,
-            destination_content_type=content_type,
-            destination_server_side_encryption=None,
-            source_server_side_encryption=None,
-            source_file_info=None,
-            source_content_type=None,
-        )
-        self.assertEqual(
-            (MetadataDirectiveMode.COPY, {}, content_type),
-            (metadata_directive, new_file_info, new_content_type)
-        )
-
-    def test_establish_sse_c_copy_b2(self):
-        file_info = {}
-        content_type = 'text/plain'
-        metadata_directive, new_file_info, new_content_type = CopyManager.establish_sse_c_file_metadata(
-            MetadataDirectiveMode.COPY,
-            destination_file_info=file_info,
-            destination_content_type=content_type,
-            destination_server_side_encryption=SSE_B2_AES,
-            source_server_side_encryption=None,
-            source_file_info=None,
-            source_content_type=None,
-        )
-        self.assertEqual(
-            (MetadataDirectiveMode.COPY, {}, content_type),
-            (metadata_directive, new_file_info, new_content_type)
-        )
-
-    def test_establish_sse_c_copy_same_key_id(self):
-        file_info = None
-        content_type = 'text/plain'
-        metadata_directive, new_file_info, new_content_type = CopyManager.establish_sse_c_file_metadata(
-            MetadataDirectiveMode.COPY,
-            destination_file_info=file_info,
-            destination_content_type=content_type,
-            destination_server_side_encryption=SSE_C_AES,
-            source_server_side_encryption=SSE_C_AES,
-            source_file_info=None,
-            source_content_type=None,
-        )
-        self.assertEqual(
-            (MetadataDirectiveMode.COPY, None, content_type),
-            (metadata_directive, new_file_info, new_content_type)
-        )
-
-    def test_establish_sse_c_copy_sources_given(self):
-        metadata_directive, new_file_info, new_content_type = CopyManager.establish_sse_c_file_metadata(
-            MetadataDirectiveMode.COPY,
-            destination_file_info=None,
-            destination_content_type=None,
-            destination_server_side_encryption=SSE_C_AES,
-            source_server_side_encryption=SSE_C_AES_2,
-            source_file_info={
-                'some_key': 'some_value',
-                SSE_C_KEY_ID_FILE_INFO_KEY_NAME: 'some-id-2'
-            },
-            source_content_type='text/plain',
-        )
-        self.assertEqual(
-            (
-                MetadataDirectiveMode.REPLACE, {
-                    'some_key': 'some_value',
-                    SSE_C_KEY_ID_FILE_INFO_KEY_NAME: 'some-id'
-                }, 'text/plain'
-            ), (metadata_directive, new_file_info, new_content_type)
-        )
-
-    def test_establish_sse_c_copy_sources_unknown(self):
-        for source_file_info, source_content_type in [
-            (None, None),
-            ({
-                'a': 'b'
-            }, None),
-            (None, 'text/plain'),
-        ]:
-            with self.subTest(
-                source_file_info=source_file_info, source_content_type=source_content_type
-            ):
-                with self.assertRaises(
-                    SSECKeyIdMismatchInCopy,
-                    'attempting to copy file using MetadataDirectiveMode.COPY without providing source_file_info '
-                    'and source_content_type for differing sse_c_key_ids: source="some-id-2", destination="some-id"'
-                ):
-                    CopyManager.establish_sse_c_file_metadata(
-                        MetadataDirectiveMode.COPY,
-                        destination_file_info=None,
-                        destination_content_type=None,
-                        destination_server_side_encryption=SSE_C_AES,
-                        source_server_side_encryption=SSE_C_AES_2,
-                        source_file_info=source_file_info,
-                        source_content_type=source_content_type,
-                    )
+from contextlib import suppress
+import datetime
+import functools
+
+from b2sdk import v2
+from . import api as v1api
+
+
+# Override to retain legacy class name, __init__ signature, slots
+# and old formatting methods
+# and to omit 'api' property when doing __eq__ and __repr__
+# and to make get_fresh_state return proper objects, even though v1.B2Api.get_file_info returns dicts
+class FileVersionInfo(v2.FileVersion):
+    __slots__ = ['_api']
+
+    LS_ENTRY_TEMPLATE = '%83s  %6s  %10s  %8s  %9d  %s'  # order is file_id, action, date, time, size, name
+
+    def __init__(
+        self,
+        id_,
+        file_name,
+        size,
+        content_type,
+        content_sha1,
+        file_info,
+        upload_timestamp,
+        action,
+        account_id: str | None = None,
+        bucket_id: str | None = None,
+        content_md5=None,
+        server_side_encryption: v2.EncryptionSetting | None = None,
+        file_retention: v2.FileRetentionSetting | None = None,
+        legal_hold: v2.LegalHold | None = None,
+        api: v1api.B2Api | None = None,
+        cache_control: str | None = None,
+        **kwargs
+    ):
+        self.id_ = id_
+        self.file_name = file_name
+        self.size = size and int(size)
+        self.content_type = content_type
+        self.content_sha1, self.content_sha1_verified = self._decode_content_sha1(content_sha1)
+        self.account_id = account_id
+        self.bucket_id = bucket_id
+        self.content_md5 = content_md5
+        self.file_info = file_info or {}
+        self.upload_timestamp = upload_timestamp
+        self.action = action
+        self.server_side_encryption = server_side_encryption
+        self.legal_hold = legal_hold
+        self.file_retention = file_retention
+        self._api = api
+        self.cache_control = cache_control
+        if self.cache_control is None:
+            self.cache_control = (file_info or {}).get('b2-cache-control')
+
+        # allow common tests to execute without hitting attributeerror
+
+        with suppress(KeyError):
+            del kwargs['replication_status']
+        self.replication_status = None
+        assert not kwargs  # after we get rid of everything we don't support in this apiver, this should be empty
+
+        if v2.SRC_LAST_MODIFIED_MILLIS in self.file_info:
+            self.mod_time_millis = int(self.file_info[v2.SRC_LAST_MODIFIED_MILLIS])
+        else:
+            self.mod_time_millis = self.upload_timestamp
+
+    @property
+    def api(self):
+        if self._api is None:
+            raise ValueError('"api" not set')
+        return self._api
+
+    def _all_slots(self):
+        all_slots = super()._all_slots()
+        all_slots.remove('api')
+        return all_slots
+
+    def format_ls_entry(self):
+        dt = datetime.datetime.utcfromtimestamp(self.upload_timestamp / 1000)
+        date_str = dt.strftime('%Y-%m-%d')
+        time_str = dt.strftime('%H:%M:%S')
+        size = self.size or 0  # required if self.action == 'hide'
+        return self.LS_ENTRY_TEMPLATE % (
+            self.id_,
+            self.action,
+            date_str,
+            time_str,
+            size,
+            self.file_name,
+        )
+
+    @classmethod
+    def format_folder_ls_entry(cls, name):
+        return cls.LS_ENTRY_TEMPLATE % ('-', '-', '-', '-', 0, name)
+
+    def get_fresh_state(self) -> FileVersionInfo:
+        """
+        Fetch all the information about this file version and return a new FileVersion object.
+        This method does NOT change the object it is called on.
+        """
+        return self.api.file_version_factory.from_api_response(self.api.get_file_info(self.id_))
+
+
+def file_version_info_from_new_file_version(file_version: v2.FileVersion) -> FileVersionInfo:
+    return FileVersionInfo(
+        **{
+            att_name: getattr(file_version, att_name)
+            for att_name in [
+                'id_',
+                'file_name',
+                'size',
+                'content_type',
+                'content_sha1',
+                'file_info',
+                'upload_timestamp',
+                'action',
+                'content_md5',
+                'server_side_encryption',
+                'legal_hold',
+                'file_retention',
+                'cache_control',
+                'api',
+            ]
+        }
+    )
+
+
+def translate_single_file_version(func):
+    @functools.wraps(func)
+    def inner(*a, **kw):
+        return file_version_info_from_new_file_version(func(*a, **kw))
+
+    return inner
+
+
+# override to return old style FileVersionInfo
+class FileVersionInfoFactory(v2.FileVersionFactory):
+
+    from_api_response = translate_single_file_version(v2.FileVersionFactory.from_api_response)
+
+    def from_response_headers(self, headers):
+
+        file_info = v2.DownloadVersionFactory.file_info_from_headers(headers)
+        return FileVersionInfo(
+            api=self.api,
+            id_=headers['x-bz-file-id'],
+            file_name=headers['x-bz-file-name'],
+            size=int(headers['content-length']),
+            content_type=headers['content-type'],
+            content_sha1=headers['x-bz-content-sha1'],
+            file_info=file_info,
+            upload_timestamp=int(headers['x-bz-upload-timestamp']),
+            action='upload',
+            content_md5=None,
+            server_side_encryption=v2.EncryptionSettingFactory.from_response_headers(headers),
+            file_retention=v2.FileRetentionSetting.from_response_headers(headers),
+            legal_hold=v2.LegalHold.from_response_headers(headers),
+            cache_control=headers['Cache-control'],
+        )
+
+
+def file_version_info_from_id_and_name(file_id_and_name: v2.FileIdAndName, api: v1api.B2Api):
+    return FileVersionInfo(
+        id_=file_id_and_name.file_id,
+        file_name=file_id_and_name.file_name,
+        size=0,
+        content_type='unknown',
+        content_sha1='none',
+        file_info={},
+        upload_timestamp=0,
+        action='cancel',
+        api=api,
+    )
+
+
+def file_version_info_from_download_version(download_version: v2.DownloadVersion):
+    return FileVersionInfo(
+        id_=download_version.id_,
+        file_name=download_version.file_name,
+        size=download_version.size,
+        content_type=download_version.content_type,
+        content_sha1=download_version.content_sha1,
+        file_info=download_version.file_info,
+        upload_timestamp=download_version.upload_timestamp,
+        action='upload',
+        content_md5=None,
+        server_side_encryption=download_version.server_side_encryption,
+        file_retention=download_version.file_retention,
+        legal_hold=download_version.legal_hold,
+        cache_control=download_version.cache_control,
+        api=download_version.api,
+    )
```

