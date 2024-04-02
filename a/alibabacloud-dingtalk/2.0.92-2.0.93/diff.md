# Comparing `tmp/alibabacloud_dingtalk-2.0.92.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.92.tar", last modified: Tue Mar 26 02:54:03 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.93.tar", last modified: Tue Apr  2 10:37:19 2024, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.92.tar` & `alibabacloud_dingtalk-2.0.93.tar`

### file list

```diff
@@ -1,421 +1,425 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/
--rw-r--r--   0 root         (0) root         (0)   115749 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3832 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2544 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     2629 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8552 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15045 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ai_interaction_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17374 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ai_interaction_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    19132 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ai_interaction_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ai_paa_s_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38246 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    50325 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22974 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   168107 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    45004 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26721 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    95304 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   142688 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   199802 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   385200 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60886 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bay_max_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bay_max_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5222 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bay_max_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4059 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bay_max_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   250056 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   651741 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bizfinance_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64166 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bizfinance_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    91975 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bizfinance_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9614 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9792 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161860 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   394680 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41039 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78198 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   236838 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10276 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   119949 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   143446 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   199904 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   122524 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   328156 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   412861 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41482 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33392 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44364 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30172 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/cool_ops_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8944 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/cool_ops_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14272 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/cool_ops_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/credit_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/credit_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5652 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/credit_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10226 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/credit_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   252718 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   604351 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7215 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    45878 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   499475 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148230 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13874 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15755 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54091 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64765 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    80337 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   259804 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   315211 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   213190 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   379351 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/dpaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/dpaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19496 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/dpaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25936 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/dpaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   190495 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   557050 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   850115 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   113146 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   120009 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18589 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   378556 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   527163 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161906 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   305557 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17280 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28173 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/flashmsg_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35856 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/flashmsg_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    52698 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/flashmsg_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4825 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4965 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9402 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   134962 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18223 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68862 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   119412 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   136559 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   208354 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   303006 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   368637 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24693 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33051 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89450 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   671658 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   913856 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152590 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   105975 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   131540 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9852 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14026 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/mail_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/mail_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5150 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/mail_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4229 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/mail_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22736 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148979 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   170469 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    52481 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/notable_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/notable_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25614 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/notable_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31620 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/notable_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34360 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42471 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7167 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89094 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   161460 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   120360 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    57967 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    68049 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   265120 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   409387 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10808 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4409 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25740 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43482 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169147 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94300 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   103368 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93324 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   146182 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44633 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   386598 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   538012 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25740 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    94517 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   346388 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53470 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    87250 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28049 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70520 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152094 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15723 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21167 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17009 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73122 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   128823 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   107789 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33103 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40753 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20146 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   128063 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8155 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41320 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42730 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   194138 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   406923 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   488736 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   727920 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4320 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3832 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13944 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2024-03-26 02:54:03.000000 alibabacloud_dingtalk-2.0.92/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/
+-rw-r--r--   0 root         (0) root         (0)   117264 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3844 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2556 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     2641 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15045 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_interaction_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17374 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_interaction_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    19132 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_interaction_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_paa_s_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38246 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    50325 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22974 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   168107 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    45004 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26721 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    95304 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   142688 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   204138 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   393347 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60886 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bay_max_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bay_max_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5222 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bay_max_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4059 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bay_max_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   250270 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   651992 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    67784 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    97238 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9614 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9792 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161860 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   394680 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41039 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78198 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   236838 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   119949 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   143446 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   199904 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   122524 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   328156 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   412861 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41482 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33392 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44364 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30172 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19630 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25937 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_ops_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8944 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_ops_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14272 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_ops_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/credit_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/credit_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5652 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/credit_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10226 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/credit_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   252718 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   604351 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7215 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    45878 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   499475 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148230 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15755 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54091 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64765 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    80337 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   259804 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   315211 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   213190 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   379351 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dpaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dpaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19496 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dpaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25936 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dpaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   190495 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   557050 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   850115 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   113146 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   120009 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18589 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   378556 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   527163 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161906 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   305557 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17280 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28173 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmsg_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35856 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmsg_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    52698 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmsg_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4825 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9402 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   134962 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18223 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68862 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   119612 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   136559 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   208354 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   303006 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   368637 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24693 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33051 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89450 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   671658 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   913856 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152590 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   105975 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   131540 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9852 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14026 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/mail_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/mail_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/mail_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4229 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/mail_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22736 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148979 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   170469 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    52481 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/notable_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/notable_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25614 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/notable_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31620 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/notable_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34360 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42471 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7167 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89094 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   161460 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   120360 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    57967 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    68049 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   265120 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   409387 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10808 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4409 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25740 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43482 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169147 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94300 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   103368 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93324 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   146182 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44633 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   386598 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   538012 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25740 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    94517 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   346388 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53470 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    87250 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28049 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70520 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152094 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15723 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21167 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17009 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    73122 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   129616 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   107789 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33103 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40753 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20146 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   128063 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8155 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41320 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42730 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   194138 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   407479 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   488736 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   727920 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3844 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14081 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-02 10:37:19.000000 alibabacloud_dingtalk-2.0.93/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-04-02 10:37:18.000000 alibabacloud_dingtalk-2.0.93/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.92/ChangeLog.md` & `alibabacloud_dingtalk-2.0.93/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-03-26 Version: 2.0.92
+- Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
+
 2024-03-21 Version: 2.0.91
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-03-20 Version: 2.0.90
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-03-18 Version: 2.0.89
```

### Comparing `alibabacloud_dingtalk-2.0.92/LICENSE` & `alibabacloud_dingtalk-2.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/PKG-INFO` & `alibabacloud_dingtalk-2.0.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.92
+Version: 2.0.93
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolApp_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_dingtalk-2.0.92/README-CN.md` & `alibabacloud_dingtalk-2.0.93/README-CN.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolApp_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_dingtalk-2.0.92/README.md` & `alibabacloud_dingtalk-2.0.93/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolApp_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ai_interaction_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_interaction_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ai_interaction_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_interaction_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ai_paa_s_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_paa_s_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ai_paa_s_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ai_paa_s_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1811,14 +1811,112 @@
         self,
         request: dingtalkattendance__1__0_models.GetClosingAccountsRequest,
     ) -> dingtalkattendance__1__0_models.GetClosingAccountsResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkattendance__1__0_models.GetClosingAccountsHeaders()
         return await self.get_closing_accounts_with_options_async(request, headers, runtime)
 
+    def get_columnvals_with_options(
+        self,
+        request: dingtalkattendance__1__0_models.GetColumnvalsRequest,
+        headers: dingtalkattendance__1__0_models.GetColumnvalsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkattendance__1__0_models.GetColumnvalsResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.column_id_list):
+            body['columnIdList'] = request.column_id_list
+        if not UtilClient.is_unset(request.from_date):
+            body['fromDate'] = request.from_date
+        if not UtilClient.is_unset(request.to_date):
+            body['toDate'] = request.to_date
+        if not UtilClient.is_unset(request.user_ids):
+            body['userIds'] = request.user_ids
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetColumnvals',
+            version='attendance_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/attendance/columnValues/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkattendance__1__0_models.GetColumnvalsResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_columnvals_with_options_async(
+        self,
+        request: dingtalkattendance__1__0_models.GetColumnvalsRequest,
+        headers: dingtalkattendance__1__0_models.GetColumnvalsHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkattendance__1__0_models.GetColumnvalsResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.column_id_list):
+            body['columnIdList'] = request.column_id_list
+        if not UtilClient.is_unset(request.from_date):
+            body['fromDate'] = request.from_date
+        if not UtilClient.is_unset(request.to_date):
+            body['toDate'] = request.to_date
+        if not UtilClient.is_unset(request.user_ids):
+            body['userIds'] = request.user_ids
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetColumnvals',
+            version='attendance_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/attendance/columnValues/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkattendance__1__0_models.GetColumnvalsResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_columnvals(
+        self,
+        request: dingtalkattendance__1__0_models.GetColumnvalsRequest,
+    ) -> dingtalkattendance__1__0_models.GetColumnvalsResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkattendance__1__0_models.GetColumnvalsHeaders()
+        return self.get_columnvals_with_options(request, headers, runtime)
+
+    async def get_columnvals_async(
+        self,
+        request: dingtalkattendance__1__0_models.GetColumnvalsRequest,
+    ) -> dingtalkattendance__1__0_models.GetColumnvalsResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkattendance__1__0_models.GetColumnvalsHeaders()
+        return await self.get_columnvals_with_options_async(request, headers, runtime)
+
     def get_leave_records_with_options(
         self,
         request: dingtalkattendance__1__0_models.GetLeaveRecordsRequest,
         headers: dingtalkattendance__1__0_models.GetLeaveRecordsHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkattendance__1__0_models.GetLeaveRecordsResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4591,14 +4591,289 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetClosingAccountsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetColumnvalsHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
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
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class GetColumnvalsRequest(TeaModel):
+    def __init__(
+        self,
+        column_id_list: List[str] = None,
+        from_date: int = None,
+        to_date: int = None,
+        user_ids: List[str] = None,
+    ):
+        self.column_id_list = column_id_list
+        self.from_date = from_date
+        self.to_date = to_date
+        self.user_ids = user_ids
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
+        if self.column_id_list is not None:
+            result['columnIdList'] = self.column_id_list
+        if self.from_date is not None:
+            result['fromDate'] = self.from_date
+        if self.to_date is not None:
+            result['toDate'] = self.to_date
+        if self.user_ids is not None:
+            result['userIds'] = self.user_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('columnIdList') is not None:
+            self.column_id_list = m.get('columnIdList')
+        if m.get('fromDate') is not None:
+            self.from_date = m.get('fromDate')
+        if m.get('toDate') is not None:
+            self.to_date = m.get('toDate')
+        if m.get('userIds') is not None:
+            self.user_ids = m.get('userIds')
+        return self
+
+
+class GetColumnvalsResponseBodyResultColumnDataColumnValues(TeaModel):
+    def __init__(
+        self,
+        date: int = None,
+        value: str = None,
+    ):
+        self.date = date
+        self.value = value
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
+        if self.date is not None:
+            result['date'] = self.date
+        if self.value is not None:
+            result['value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('date') is not None:
+            self.date = m.get('date')
+        if m.get('value') is not None:
+            self.value = m.get('value')
+        return self
+
+
+class GetColumnvalsResponseBodyResultColumnData(TeaModel):
+    def __init__(
+        self,
+        column_values: List[GetColumnvalsResponseBodyResultColumnDataColumnValues] = None,
+        fixed_value: str = None,
+        id: int = None,
+    ):
+        self.column_values = column_values
+        self.fixed_value = fixed_value
+        self.id = id
+
+    def validate(self):
+        if self.column_values:
+            for k in self.column_values:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['columnValues'] = []
+        if self.column_values is not None:
+            for k in self.column_values:
+                result['columnValues'].append(k.to_map() if k else None)
+        if self.fixed_value is not None:
+            result['fixedValue'] = self.fixed_value
+        if self.id is not None:
+            result['id'] = self.id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.column_values = []
+        if m.get('columnValues') is not None:
+            for k in m.get('columnValues'):
+                temp_model = GetColumnvalsResponseBodyResultColumnDataColumnValues()
+                self.column_values.append(temp_model.from_map(k))
+        if m.get('fixedValue') is not None:
+            self.fixed_value = m.get('fixedValue')
+        if m.get('id') is not None:
+            self.id = m.get('id')
+        return self
+
+
+class GetColumnvalsResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        column_data: List[GetColumnvalsResponseBodyResultColumnData] = None,
+        user_id: str = None,
+    ):
+        self.column_data = column_data
+        self.user_id = user_id
+
+    def validate(self):
+        if self.column_data:
+            for k in self.column_data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['columnData'] = []
+        if self.column_data is not None:
+            for k in self.column_data:
+                result['columnData'].append(k.to_map() if k else None)
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.column_data = []
+        if m.get('columnData') is not None:
+            for k in m.get('columnData'):
+                temp_model = GetColumnvalsResponseBodyResultColumnData()
+                self.column_data.append(temp_model.from_map(k))
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class GetColumnvalsResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: List[GetColumnvalsResponseBodyResult] = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['result'] = []
+        if self.result is not None:
+            for k in self.result:
+                result['result'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.result = []
+        if m.get('result') is not None:
+            for k in m.get('result'):
+                temp_model = GetColumnvalsResponseBodyResult()
+                self.result.append(temp_model.from_map(k))
+        return self
+
+
+class GetColumnvalsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetColumnvalsResponseBody = None,
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
+            temp_model = GetColumnvalsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetLeaveRecordsHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bay_max_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bay_max_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bay_max_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bay_max_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5295,14 +5295,16 @@
             body['operatorId'] = request.operator_id
         if not UtilClient.is_unset(request.receipt_id):
             body['receiptId'] = request.receipt_id
         if not UtilClient.is_unset(request.voucher_code):
             body['voucherCode'] = request.voucher_code
         if not UtilClient.is_unset(request.voucher_id):
             body['voucherId'] = request.voucher_id
+        if not UtilClient.is_unset(request.voucher_no):
+            body['voucherNo'] = request.voucher_no
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
@@ -5340,14 +5342,16 @@
             body['operatorId'] = request.operator_id
         if not UtilClient.is_unset(request.receipt_id):
             body['receiptId'] = request.receipt_id
         if not UtilClient.is_unset(request.voucher_code):
             body['voucherCode'] = request.voucher_code
         if not UtilClient.is_unset(request.voucher_id):
             body['voucherId'] = request.voucher_id
+        if not UtilClient.is_unset(request.voucher_no):
+            body['voucherNo'] = request.voucher_no
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
```

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -18219,21 +18219,23 @@
         self,
         account_period: str = None,
         action_type: str = None,
         operator_id: str = None,
         receipt_id: str = None,
         voucher_code: str = None,
         voucher_id: str = None,
+        voucher_no: str = None,
     ):
         self.account_period = account_period
         self.action_type = action_type
         self.operator_id = operator_id
         self.receipt_id = receipt_id
         self.voucher_code = voucher_code
         self.voucher_id = voucher_id
+        self.voucher_no = voucher_no
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -18248,14 +18250,16 @@
             result['operatorId'] = self.operator_id
         if self.receipt_id is not None:
             result['receiptId'] = self.receipt_id
         if self.voucher_code is not None:
             result['voucherCode'] = self.voucher_code
         if self.voucher_id is not None:
             result['voucherId'] = self.voucher_id
+        if self.voucher_no is not None:
+            result['voucherNo'] = self.voucher_no
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('accountPeriod') is not None:
             self.account_period = m.get('accountPeriod')
         if m.get('actionType') is not None:
@@ -18264,14 +18268,16 @@
             self.operator_id = m.get('operatorId')
         if m.get('receiptId') is not None:
             self.receipt_id = m.get('receiptId')
         if m.get('voucherCode') is not None:
             self.voucher_code = m.get('voucherCode')
         if m.get('voucherId') is not None:
             self.voucher_id = m.get('voucherId')
+        if m.get('voucherNo') is not None:
+            self.voucher_no = m.get('voucherNo')
         return self
 
 
 class UpdateReceiptVoucherStatusResponseBody(TeaModel):
     def __init__(
         self,
         result: bool = None,
```

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bizfinance_2_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_2_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,94 @@
         self,
         request: dingtalkbizfinance__2__0_models.BatchDeleteReceiptRequest,
     ) -> dingtalkbizfinance__2__0_models.BatchDeleteReceiptResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkbizfinance__2__0_models.BatchDeleteReceiptHeaders()
         return await self.batch_delete_receipt_with_options_async(request, headers, runtime)
 
+    def batch_sync_bank_receipt_with_options(
+        self,
+        request: dingtalkbizfinance__2__0_models.BatchSyncBankReceiptRequest,
+        headers: dingtalkbizfinance__2__0_models.BatchSyncBankReceiptHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkbizfinance__2__0_models.BatchSyncBankReceiptResponse:
+        UtilClient.validate_model(request)
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=UtilClient.to_array(request.body)
+        )
+        params = open_api_models.Params(
+            action='BatchSyncBankReceipt',
+            version='bizfinance_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/bizfinance/receipts/batchSync',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkbizfinance__2__0_models.BatchSyncBankReceiptResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def batch_sync_bank_receipt_with_options_async(
+        self,
+        request: dingtalkbizfinance__2__0_models.BatchSyncBankReceiptRequest,
+        headers: dingtalkbizfinance__2__0_models.BatchSyncBankReceiptHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkbizfinance__2__0_models.BatchSyncBankReceiptResponse:
+        UtilClient.validate_model(request)
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=UtilClient.to_array(request.body)
+        )
+        params = open_api_models.Params(
+            action='BatchSyncBankReceipt',
+            version='bizfinance_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/bizfinance/receipts/batchSync',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkbizfinance__2__0_models.BatchSyncBankReceiptResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def batch_sync_bank_receipt(
+        self,
+        request: dingtalkbizfinance__2__0_models.BatchSyncBankReceiptRequest,
+    ) -> dingtalkbizfinance__2__0_models.BatchSyncBankReceiptResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkbizfinance__2__0_models.BatchSyncBankReceiptHeaders()
+        return self.batch_sync_bank_receipt_with_options(request, headers, runtime)
+
+    async def batch_sync_bank_receipt_async(
+        self,
+        request: dingtalkbizfinance__2__0_models.BatchSyncBankReceiptRequest,
+    ) -> dingtalkbizfinance__2__0_models.BatchSyncBankReceiptResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkbizfinance__2__0_models.BatchSyncBankReceiptHeaders()
+        return await self.batch_sync_bank_receipt_with_options_async(request, headers, runtime)
+
     def get_category_with_options(
         self,
         request: dingtalkbizfinance__2__0_models.GetCategoryRequest,
         headers: dingtalkbizfinance__2__0_models.GetCategoryHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkbizfinance__2__0_models.GetCategoryResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/bizfinance_2_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/bizfinance_2_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,195 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = BatchDeleteReceiptResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class BatchSyncBankReceiptHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
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
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class BatchSyncBankReceiptRequestBody(TeaModel):
+    def __init__(
+        self,
+        file_download_url: str = None,
+        file_name: str = None,
+        message_id: str = None,
+        message_id_type: str = None,
+    ):
+        self.file_download_url = file_download_url
+        self.file_name = file_name
+        self.message_id = message_id
+        self.message_id_type = message_id_type
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
+        if self.file_download_url is not None:
+            result['fileDownloadUrl'] = self.file_download_url
+        if self.file_name is not None:
+            result['fileName'] = self.file_name
+        if self.message_id is not None:
+            result['messageId'] = self.message_id
+        if self.message_id_type is not None:
+            result['messageIdType'] = self.message_id_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('fileDownloadUrl') is not None:
+            self.file_download_url = m.get('fileDownloadUrl')
+        if m.get('fileName') is not None:
+            self.file_name = m.get('fileName')
+        if m.get('messageId') is not None:
+            self.message_id = m.get('messageId')
+        if m.get('messageIdType') is not None:
+            self.message_id_type = m.get('messageIdType')
+        return self
+
+
+class BatchSyncBankReceiptRequest(TeaModel):
+    def __init__(
+        self,
+        body: List[BatchSyncBankReceiptRequestBody] = None,
+    ):
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            for k in self.body:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['body'] = []
+        if self.body is not None:
+            for k in self.body:
+                result['body'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.body = []
+        if m.get('body') is not None:
+            for k in m.get('body'):
+                temp_model = BatchSyncBankReceiptRequestBody()
+                self.body.append(temp_model.from_map(k))
+        return self
+
+
+class BatchSyncBankReceiptResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: bool = None,
+    ):
+        self.result = result
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
+        if self.result is not None:
+            result['result'] = self.result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            self.result = m.get('result')
+        return self
+
+
+class BatchSyncBankReceiptResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: BatchSyncBankReceiptResponseBody = None,
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
+            temp_model = BatchSyncBankReceiptResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetCategoryHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/cool_ops_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_ops_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/cool_ops_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/cool_ops_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/credit_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/credit_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/credit_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/credit_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/dpaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dpaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/dpaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/dpaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/flashmsg_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmsg_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/flashmsg_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/flashmsg_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1929,42 +1929,48 @@
         return self
 
 
 class HrbrainImportLabelInventoryRequestBody(TeaModel):
     def __init__(
         self,
         extend_info: Dict[str, Any] = None,
+        name: str = None,
         period: str = None,
         work_no: str = None,
     ):
         self.extend_info = extend_info
+        self.name = name
         self.period = period
         self.work_no = work_no
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.extend_info is not None:
             result['extendInfo'] = self.extend_info
+        if self.name is not None:
+            result['name'] = self.name
         if self.period is not None:
             result['period'] = self.period
         if self.work_no is not None:
             result['workNo'] = self.work_no
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('extendInfo') is not None:
             self.extend_info = m.get('extendInfo')
+        if m.get('name') is not None:
+            self.name = m.get('name')
         if m.get('period') is not None:
             self.period = m.get('period')
         if m.get('workNo') is not None:
             self.work_no = m.get('workNo')
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/mail_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/mail_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/mail_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/mail_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/notable_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/notable_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/notable_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/notable_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2969,23 +2969,25 @@
         catering_type: str = None,
         check_in_time: str = None,
         check_out_time: str = None,
         depart_time: str = None,
         destination_city: str = None,
         destination_city_code: str = None,
         destination_station: str = None,
+        destination_terminal_building: str = None,
         detail_amount: str = None,
         hotel_address: str = None,
         hotel_city: str = None,
         hotel_location: SyncTripOrderRequestOrderDetailsHotelLocation = None,
         hotel_name: str = None,
         open_consumer_info: List[SyncTripOrderRequestOrderDetailsOpenConsumerInfo] = None,
         origin_city: str = None,
         origin_city_code: str = None,
         origin_station: str = None,
+        origin_terminal_building: str = None,
         room_count: int = None,
         seat_info: str = None,
         service_type: str = None,
         sub_supply_logo: str = None,
         sub_supply_name: str = None,
         taxi_type: str = None,
         telephone: str = None,
@@ -2999,23 +3001,25 @@
         self.catering_type = catering_type
         self.check_in_time = check_in_time
         self.check_out_time = check_out_time
         self.depart_time = depart_time
         self.destination_city = destination_city
         self.destination_city_code = destination_city_code
         self.destination_station = destination_station
+        self.destination_terminal_building = destination_terminal_building
         self.detail_amount = detail_amount
         self.hotel_address = hotel_address
         self.hotel_city = hotel_city
         self.hotel_location = hotel_location
         self.hotel_name = hotel_name
         self.open_consumer_info = open_consumer_info
         self.origin_city = origin_city
         self.origin_city_code = origin_city_code
         self.origin_station = origin_station
+        self.origin_terminal_building = origin_terminal_building
         self.room_count = room_count
         self.seat_info = seat_info
         self.service_type = service_type
         self.sub_supply_logo = sub_supply_logo
         self.sub_supply_name = sub_supply_name
         self.taxi_type = taxi_type
         self.telephone = telephone
@@ -3054,14 +3058,16 @@
             result['departTime'] = self.depart_time
         if self.destination_city is not None:
             result['destinationCity'] = self.destination_city
         if self.destination_city_code is not None:
             result['destinationCityCode'] = self.destination_city_code
         if self.destination_station is not None:
             result['destinationStation'] = self.destination_station
+        if self.destination_terminal_building is not None:
+            result['destinationTerminalBuilding'] = self.destination_terminal_building
         if self.detail_amount is not None:
             result['detailAmount'] = self.detail_amount
         if self.hotel_address is not None:
             result['hotelAddress'] = self.hotel_address
         if self.hotel_city is not None:
             result['hotelCity'] = self.hotel_city
         if self.hotel_location is not None:
@@ -3074,14 +3080,16 @@
                 result['openConsumerInfo'].append(k.to_map() if k else None)
         if self.origin_city is not None:
             result['originCity'] = self.origin_city
         if self.origin_city_code is not None:
             result['originCityCode'] = self.origin_city_code
         if self.origin_station is not None:
             result['originStation'] = self.origin_station
+        if self.origin_terminal_building is not None:
+            result['originTerminalBuilding'] = self.origin_terminal_building
         if self.room_count is not None:
             result['roomCount'] = self.room_count
         if self.seat_info is not None:
             result['seatInfo'] = self.seat_info
         if self.service_type is not None:
             result['serviceType'] = self.service_type
         if self.sub_supply_logo is not None:
@@ -3118,14 +3126,16 @@
             self.depart_time = m.get('departTime')
         if m.get('destinationCity') is not None:
             self.destination_city = m.get('destinationCity')
         if m.get('destinationCityCode') is not None:
             self.destination_city_code = m.get('destinationCityCode')
         if m.get('destinationStation') is not None:
             self.destination_station = m.get('destinationStation')
+        if m.get('destinationTerminalBuilding') is not None:
+            self.destination_terminal_building = m.get('destinationTerminalBuilding')
         if m.get('detailAmount') is not None:
             self.detail_amount = m.get('detailAmount')
         if m.get('hotelAddress') is not None:
             self.hotel_address = m.get('hotelAddress')
         if m.get('hotelCity') is not None:
             self.hotel_city = m.get('hotelCity')
         if m.get('hotelLocation') is not None:
@@ -3140,14 +3150,16 @@
                 self.open_consumer_info.append(temp_model.from_map(k))
         if m.get('originCity') is not None:
             self.origin_city = m.get('originCity')
         if m.get('originCityCode') is not None:
             self.origin_city_code = m.get('originCityCode')
         if m.get('originStation') is not None:
             self.origin_station = m.get('originStation')
+        if m.get('originTerminalBuilding') is not None:
+            self.origin_terminal_building = m.get('originTerminalBuilding')
         if m.get('roomCount') is not None:
             self.room_count = m.get('roomCount')
         if m.get('seatInfo') is not None:
             self.seat_info = m.get('seatInfo')
         if m.get('serviceType') is not None:
             self.service_type = m.get('serviceType')
         if m.get('subSupplyLogo') is not None:
```

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,15 @@
         choice: str = None,
         common_biz_type: str = None,
         component_id: str = None,
         content: str = None,
         data_source: FormDataSource = None,
         disabled: bool = None,
         duration: bool = None,
+        duration_label: str = None,
         format: str = None,
         formula: str = None,
         invisible: bool = None,
         label: str = None,
         limit: int = None,
         link: str = None,
         max_length: int = None,
@@ -236,14 +237,15 @@
         self.choice = choice
         self.common_biz_type = common_biz_type
         self.component_id = component_id
         self.content = content
         self.data_source = data_source
         self.disabled = disabled
         self.duration = duration
+        self.duration_label = duration_label
         self.format = format
         self.formula = formula
         self.invisible = invisible
         self.label = label
         self.limit = limit
         self.link = link
         self.max_length = max_length
@@ -308,14 +310,16 @@
             result['content'] = self.content
         if self.data_source is not None:
             result['dataSource'] = self.data_source.to_map()
         if self.disabled is not None:
             result['disabled'] = self.disabled
         if self.duration is not None:
             result['duration'] = self.duration
+        if self.duration_label is not None:
+            result['durationLabel'] = self.duration_label
         if self.format is not None:
             result['format'] = self.format
         if self.formula is not None:
             result['formula'] = self.formula
         if self.invisible is not None:
             result['invisible'] = self.invisible
         if self.label is not None:
@@ -386,14 +390,16 @@
         if m.get('dataSource') is not None:
             temp_model = FormDataSource()
             self.data_source = temp_model.from_map(m['dataSource'])
         if m.get('disabled') is not None:
             self.disabled = m.get('disabled')
         if m.get('duration') is not None:
             self.duration = m.get('duration')
+        if m.get('durationLabel') is not None:
+            self.duration_label = m.get('durationLabel')
         if m.get('format') is not None:
             self.format = m.get('format')
         if m.get('formula') is not None:
             self.formula = m.get('formula')
         if m.get('invisible') is not None:
             self.invisible = m.get('invisible')
         if m.get('label') is not None:
@@ -3527,33 +3533,39 @@
             self.name = m.get('name')
         return self
 
 
 class GetProcessCodeByNameResponseBodyResult(TeaModel):
     def __init__(
         self,
+        gmt_modified: str = None,
         process_code: str = None,
     ):
+        self.gmt_modified = gmt_modified
         self.process_code = process_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.gmt_modified is not None:
+            result['gmtModified'] = self.gmt_modified
         if self.process_code is not None:
             result['processCode'] = self.process_code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('gmtModified') is not None:
+            self.gmt_modified = m.get('gmtModified')
         if m.get('processCode') is not None:
             self.process_code = m.get('processCode')
         return self
 
 
 class GetProcessCodeByNameResponseBody(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.92
+Version: 2.0.93
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/dingtalk-activity_1_0,aiInteraction_1_0,aiPaaS_1_0,algo_1_0,alitest_1_0,alitrip_1_0,apaas_1_0,appMarket_1_0,ats_1_0,attendance_1_0,badge_1_0,bayMax_1_0,baymax_2_0,bipaas_1_0,bizfinance_1_0,bizfinance_2_0,blackboard_1_0,calendar_1_0,calendar_2_0,carbon_1_0,card_1_0,checkIn_1_0,chengfeng_1_0,conference_1_0,connector_1_0,contact_1_0,content_1_0,contract_1_0,convFile_1_0,convStorage_1_0,coolApp_1_0,coolOps_1_0,credit_1_0,crm_1_0,crm_2_0,customerService_1_0,datacenter_1_0,delivery_1_0,devicemng_1_0,dingmi_1_0,dingPhone_1_0,dingsport_1_0,diot_1_0,doc_1_0,doc_2_0,dpaas_1_0,drive_1_0,drive_2_0,edu_1_0,esign_1_0,event_1_0,event_2_0,exclusive_1_0,finance_1_0,flashmeeting_1_0,flashmsg_1_0,gateway_1_0,groupBlackboard_1_0,h5package_1_0,hrbrain_1_0,hrm_1_0,im_1_0,im_2_0,impaas_1_0,industry_1_0,integration_1_0,liandanlu_1_0,link_1_0,live_1_0,liveActivities_1_0,mail_1_0,manufacturing_1_0,media_1_0,medical_1_0,microApp_1_0,miniapp_1_0,notable_1_0,oauth2_1_0,occupationauth_1_0,office_1_0,okr_1_0,orgCulture_1_0,ow_1_0,package_1_0,pedia_1_0,project_1_0,projectIntegration_1_0,rcsCall_1_0,report_1_0,resident_1_0,robot_1_0,rooms_1_0,search_1_0,serviceGroup_1_0,setting_1_0,smartDevice_1_0,snsStorage_1_0,storage_1_0,storage_2_0,swform_1_0,theone_1_0,todo_1_0,trade_1_0,trajectory_1_0,transcribe_1_0,trip_1_0,village_1_0,waterMark_1_0,watt_1_0,wiki_1_0,wiki_2_0,wms_1_0,workbench_1_0,workflow_1_0,workrecord_1_0,yida_1_0,yunShu_1_0,esign_1_1,esign_2_0,h3yun_1_0,jzcrm_1_0,soke_1_0/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_dingtalk-2.0.92/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.93/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,17 @@
 alibabacloud_dingtalk/content_1_0/models.py
 alibabacloud_dingtalk/contract_1_0/__init__.py
 alibabacloud_dingtalk/contract_1_0/client.py
 alibabacloud_dingtalk/contract_1_0/models.py
 alibabacloud_dingtalk/conv_file_1_0/__init__.py
 alibabacloud_dingtalk/conv_file_1_0/client.py
 alibabacloud_dingtalk/conv_file_1_0/models.py
+alibabacloud_dingtalk/cool_app_1_0/__init__.py
+alibabacloud_dingtalk/cool_app_1_0/client.py
+alibabacloud_dingtalk/cool_app_1_0/models.py
 alibabacloud_dingtalk/cool_ops_1_0/__init__.py
 alibabacloud_dingtalk/cool_ops_1_0/client.py
 alibabacloud_dingtalk/cool_ops_1_0/models.py
 alibabacloud_dingtalk/credit_1_0/__init__.py
 alibabacloud_dingtalk/credit_1_0/client.py
 alibabacloud_dingtalk/credit_1_0/models.py
 alibabacloud_dingtalk/crm_1_0/__init__.py
```

### Comparing `alibabacloud_dingtalk-2.0.92/setup.py` & `alibabacloud_dingtalk-2.0.93/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 26/03/2024
+Created on 02/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

