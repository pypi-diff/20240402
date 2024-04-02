# Comparing `tmp/ANX-0.7.0.tar.gz` & `tmp/ANX-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANX-0.7.0.tar", last modified: Tue Mar 12 14:41:30 2024, max compression
+gzip compressed data, was "ANX-0.7.1.tar", last modified: Tue Apr  2 02:36:45 2024, max compression
```

## Comparing `ANX-0.7.0.tar` & `ANX-0.7.1.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.543734 ANX-0.7.0/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.503437 ANX-0.7.0/ANX.egg-info/
--rw-r--r--   0 1a         (501) staff       (20)      125 2024-03-12 14:41:30.000000 ANX-0.7.0/ANX.egg-info/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)     4860 2024-03-12 14:41:30.000000 ANX-0.7.0/ANX.egg-info/SOURCES.txt
--rw-r--r--   0 1a         (501) staff       (20)        1 2024-03-12 14:41:30.000000 ANX-0.7.0/ANX.egg-info/dependency_links.txt
--rw-r--r--   0 1a         (501) staff       (20)      108 2024-03-12 14:41:30.000000 ANX-0.7.0/ANX.egg-info/requires.txt
--rw-r--r--   0 1a         (501) staff       (20)       10 2024-03-12 14:41:30.000000 ANX-0.7.0/ANX.egg-info/top_level.txt
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.504988 ANX-0.7.0/AndroidQQ/
--rw-r--r--   0 1a         (501) staff       (20)    33802 2024-03-12 14:39:25.000000 ANX-0.7.0/AndroidQQ/Android.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.505651 ANX-0.7.0/AndroidQQ/Echo/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/Echo/Tcp.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/Echo/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     3881 2024-03-12 14:40:27.000000 ANX-0.7.0/AndroidQQ/Tcp.py
--rw-r--r--   0 1a         (501) staff       (20)       71 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.508649 ANX-0.7.0/AndroidQQ/http/
--rw-r--r--   0 1a         (501) staff       (20)     2017 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/http/ClientKey.py
--rw-r--r--   0 1a         (501) staff       (20)      119 2024-03-05 18:40:23.000000 ANX-0.7.0/AndroidQQ/http/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1961 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/http/accounts.py
--rw-r--r--   0 1a         (501) staff       (20)     3760 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/http/friends.py
--rw-r--r--   0 1a         (501) staff       (20)     6591 2024-03-05 18:40:23.000000 ANX-0.7.0/AndroidQQ/http/game_credit.py
--rw-r--r--   0 1a         (501) staff       (20)      422 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/http/headers.py
--rw-r--r--   0 1a         (501) staff       (20)     7078 2024-02-14 09:03:34.000000 ANX-0.7.0/AndroidQQ/http/level.py
--rw-r--r--   0 1a         (501) staff       (20)     9985 2024-02-13 12:05:01.000000 ANX-0.7.0/AndroidQQ/http/music.py
--rw-r--r--   0 1a         (501) staff       (20)     1539 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/http/qqsignin.py
--rw-r--r--   0 1a         (501) staff       (20)     1279 2024-03-01 14:47:52.000000 ANX-0.7.0/AndroidQQ/http/weishi.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.508960 ANX-0.7.0/AndroidQQ/im/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.509058 ANX-0.7.0/AndroidQQ/im/oidb/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.509453 ANX-0.7.0/AndroidQQ/im/oidb/OidbSvc_0xc96/
--rw-r--r--   0 1a         (501) staff       (20)     2797 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)       34 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/OidbSvc_0xc96/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.510061 ANX-0.7.0/AndroidQQ/im/oidb/cmd0x88d/
--rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/cmd0x88d/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2139 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.511143 ANX-0.7.0/AndroidQQ/im/oidb/cmd0x922/
--rw-r--r--   0 1a         (501) staff       (20)     1343 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/cmd0x922/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1542 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.511733 ANX-0.7.0/AndroidQQ/im/oidb/cmd0xeb8/
--rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/cmd0xeb8/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1872 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.512285 ANX-0.7.0/AndroidQQ/im/oidb/oidb_0xc05/
--rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/oidb_0xc05/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2603 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.513132 ANX-0.7.0/AndroidQQ/im/oidb/oidb_sso/
--rw-r--r--   0 1a         (501) staff       (20)       27 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/oidb_sso/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1468 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.513644 ANX-0.7.0/AndroidQQ/im/oidb/qqconnect/
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/qqconnect/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2618 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.514833 ANX-0.7.0/AndroidQQ/im/oidb/scanlogin/
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/scanlogin/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1385 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.515175 ANX-0.7.0/AndroidQQ/log/
--rw-r--r--   0 1a         (501) staff       (20)       33 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/log/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.519005 ANX-0.7.0/AndroidQQ/pack/
--rw-r--r--   0 1a         (501) staff       (20)      395 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/Heartbeat_Alive.py
--rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py
--rw-r--r--   0 1a         (501) staff       (20)      733 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py
--rw-r--r--   0 1a         (501) staff       (20)     1368 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/OidbSvc_0x88d_1.py
--rw-r--r--   0 1a         (501) staff       (20)      986 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/OidbSvc_0xc05.py
--rw-r--r--   0 1a         (501) staff       (20)     1141 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/OidbSvc_0xc96.py
--rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/OidbSvc_0xeb8.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.521224 ANX-0.7.0/AndroidQQ/pack/SQQzoneSvc/
--rw-r--r--   0 1a         (501) staff       (20)       94 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/SQQzoneSvc/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1124 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/SQQzoneSvc/delUgc.py
--rw-r--r--   0 1a         (501) staff       (20)     2637 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/SQQzoneSvc/like.py
--rw-r--r--   0 1a         (501) staff       (20)     2631 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/SQQzoneSvc/publishmood.py
--rw-r--r--   0 1a         (501) staff       (20)     2152 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py
--rw-r--r--   0 1a         (501) staff       (20)     1116 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/StatSvc_register.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.521760 ANX-0.7.0/AndroidQQ/pack/SummaryCard/
--rw-r--r--   0 1a         (501) staff       (20)     1349 2024-03-07 10:14:41.000000 ANX-0.7.0/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/SummaryCard/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      402 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1383 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/friendlist.py
--rw-r--r--   0 1a         (501) staff       (20)      543 2024-03-06 13:46:02.000000 ANX-0.7.0/AndroidQQ/pack/test.py
--rw-r--r--   0 1a         (501) staff       (20)    46467 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.522786 ANX-0.7.0/AndroidQQ/proto/
--rw-r--r--   0 1a         (501) staff       (20)     4301 2024-02-12 04:07:38.000000 ANX-0.7.0/AndroidQQ/proto/IM_r_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)       67 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/proto/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1308 2023-10-29 17:25:21.000000 ANX-0.7.0/AndroidQQ/proto/wtlogin_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.526055 ANX-0.7.0/AndroidQQ/struct/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.527576 ANX-0.7.0/AndroidQQ/struct/Avatarlnfo/
--rw-r--r--   0 1a         (501) staff       (20)      444 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/Avatarlnfo/DestQQHeadInfo.py
--rw-r--r--   0 1a         (501) staff       (20)     1061 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      853 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py
--rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py
--rw-r--r--   0 1a         (501) staff       (20)     1028 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/Avatarlnfo/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      894 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/MessageSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.528669 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_COMM/
--rw-r--r--   0 1a         (501) staff       (20)      373 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_COMM/UgcRightInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_COMM/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.531804 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/
--rw-r--r--   0 1a         (501) staff       (20)       70 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     3064 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py
--rw-r--r--   0 1a         (501) staff       (20)     1565 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py
--rw-r--r--   0 1a         (501) staff       (20)      565 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py
--rw-r--r--   0 1a         (501) staff       (20)      895 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py
--rw-r--r--   0 1a         (501) staff       (20)     1789 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)      451 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_arkshare.py
--rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py
--rw-r--r--   0 1a         (501) staff       (20)      728 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py
--rw-r--r--   0 1a         (501) staff       (20)      249 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_user.py
--rw-r--r--   0 1a         (501) staff       (20)     1163 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.534247 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_OPERATION/
--rw-r--r--   0 1a         (501) staff       (20)      479 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_OPERATION/Source.py
--rw-r--r--   0 1a         (501) staff       (20)      187 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_OPERATION/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      656 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py
--rw-r--r--   0 1a         (501) staff       (20)     1161 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py
--rw-r--r--   0 1a         (501) staff       (20)     1300 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py
--rw-r--r--   0 1a         (501) staff       (20)      560 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)     3031 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py
--rw-r--r--   0 1a         (501) staff       (20)      503 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)      594 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/OidbSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.536704 ANX-0.7.0/AndroidQQ/struct/QMF_PROTOCAL/
--rw-r--r--   0 1a         (501) staff       (20)      504 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/QMF_PROTOCAL/QmfBusiControl.py
--rw-r--r--   0 1a         (501) staff       (20)      630 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      714 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py
--rw-r--r--   0 1a         (501) staff       (20)      526 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py
--rw-r--r--   0 1a         (501) staff       (20)     1180 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py
--rw-r--r--   0 1a         (501) staff       (20)      489 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/QMF_PROTOCAL/RetryInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       87 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/QMF_PROTOCAL/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.537026 ANX-0.7.0/AndroidQQ/struct/QQService/
--rw-r--r--   0 1a         (501) staff       (20)     1112 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      878 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/QQService/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1115 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/StatSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.537919 ANX-0.7.0/AndroidQQ/struct/SummaryCard/
--rw-r--r--   0 1a         (501) staff       (20)     2861 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py
--rw-r--r--   0 1a         (501) staff       (20)      493 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/SummaryCard/UserLocaleInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       61 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/SummaryCard/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)    15568 2024-03-05 18:40:23.000000 ANX-0.7.0/AndroidQQ/struct/Tlv.py
--rw-r--r--   0 1a         (501) staff       (20)     4784 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/Tlv_res.py
--rw-r--r--   0 1a         (501) staff       (20)      131 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.538439 ANX-0.7.0/AndroidQQ/struct/cooperation/
--rw-r--r--   0 1a         (501) staff       (20)       23 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/cooperation/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.539215 ANX-0.7.0/AndroidQQ/struct/cooperation/qzone/
--rw-r--r--   0 1a         (501) staff       (20)     4558 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/cooperation/qzone/WNSStream.py
--rw-r--r--   0 1a         (501) staff       (20)       26 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/cooperation/qzone/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.539452 ANX-0.7.0/AndroidQQ/struct/feedcomponent/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/feedcomponent/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1482 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/feedcomponent/model.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.539874 ANX-0.7.0/AndroidQQ/struct/friendlist/
--rw-r--r--   0 1a         (501) staff       (20)     2842 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/friendlist/AddFriendReq.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/friendlist/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     7428 2024-03-07 10:14:48.000000 ANX-0.7.0/AndroidQQ/struct/head.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.540560 ANX-0.7.0/AndroidQQ/struct/push/
--rw-r--r--   0 1a         (501) staff       (20)     3536 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/push/SvcReqRegister.py
--rw-r--r--   0 1a         (501) staff       (20)     2084 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/push/SvcRespRegister.py
--rw-r--r--   0 1a         (501) staff       (20)       31 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/struct/push/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)    27313 2024-03-05 18:40:23.000000 ANX-0.7.0/AndroidQQ/struct/wtlogin.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.541643 ANX-0.7.0/AndroidQQ/utils/
--rw-r--r--   0 1a         (501) staff       (20)       20 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/utils/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      523 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/utils/build_device.py
--rw-r--r--   0 1a         (501) staff       (20)     1140 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/utils/ecdh.py
--rw-r--r--   0 1a         (501) staff       (20)     1379 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/utils/sso_server.py
--rw-r--r--   0 1a         (501) staff       (20)      735 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/utils/tool.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.541845 ANX-0.7.0/AndroidQQ/wlogin_sdk/
--rw-r--r--   0 1a         (501) staff       (20)       25 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/wlogin_sdk/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-03-12 14:41:30.542054 ANX-0.7.0/AndroidQQ/wlogin_sdk/request/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.0/AndroidQQ/wlogin_sdk/request/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      125 2024-03-12 14:41:30.542346 ANX-0.7.0/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)       34 2023-08-04 12:41:32.000000 ANX-0.7.0/README.md
--rw-r--r--   0 1a         (501) staff       (20)       38 2024-03-12 14:41:30.543819 ANX-0.7.0/setup.cfg
--rw-r--r--   0 1a         (501) staff       (20)      573 2024-03-12 14:41:29.000000 ANX-0.7.0/setup.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.151862 ANX-0.7.1/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.114578 ANX-0.7.1/ANX.egg-info/
+-rw-r--r--   0 1a         (501) staff       (20)      125 2024-04-02 02:36:45.000000 ANX-0.7.1/ANX.egg-info/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)     4860 2024-04-02 02:36:45.000000 ANX-0.7.1/ANX.egg-info/SOURCES.txt
+-rw-r--r--   0 1a         (501) staff       (20)        1 2024-04-02 02:36:45.000000 ANX-0.7.1/ANX.egg-info/dependency_links.txt
+-rw-r--r--   0 1a         (501) staff       (20)      108 2024-04-02 02:36:45.000000 ANX-0.7.1/ANX.egg-info/requires.txt
+-rw-r--r--   0 1a         (501) staff       (20)       10 2024-04-02 02:36:45.000000 ANX-0.7.1/ANX.egg-info/top_level.txt
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.115198 ANX-0.7.1/AndroidQQ/
+-rw-r--r--   0 1a         (501) staff       (20)    33802 2024-03-12 14:39:25.000000 ANX-0.7.1/AndroidQQ/Android.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.115683 ANX-0.7.1/AndroidQQ/Echo/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/Echo/Tcp.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/Echo/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     4035 2024-04-02 02:29:47.000000 ANX-0.7.1/AndroidQQ/Tcp.py
+-rw-r--r--   0 1a         (501) staff       (20)       71 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.119131 ANX-0.7.1/AndroidQQ/http/
+-rw-r--r--   0 1a         (501) staff       (20)     2017 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/http/ClientKey.py
+-rw-r--r--   0 1a         (501) staff       (20)      119 2024-03-05 18:40:23.000000 ANX-0.7.1/AndroidQQ/http/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1961 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/http/accounts.py
+-rw-r--r--   0 1a         (501) staff       (20)     3760 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/http/friends.py
+-rw-r--r--   0 1a         (501) staff       (20)     6591 2024-03-05 18:40:23.000000 ANX-0.7.1/AndroidQQ/http/game_credit.py
+-rw-r--r--   0 1a         (501) staff       (20)      422 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/http/headers.py
+-rw-r--r--   0 1a         (501) staff       (20)     7078 2024-03-17 04:57:20.000000 ANX-0.7.1/AndroidQQ/http/level.py
+-rw-r--r--   0 1a         (501) staff       (20)     9985 2024-02-13 12:05:01.000000 ANX-0.7.1/AndroidQQ/http/music.py
+-rw-r--r--   0 1a         (501) staff       (20)     1539 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/http/qqsignin.py
+-rw-r--r--   0 1a         (501) staff       (20)     1279 2024-03-01 14:47:52.000000 ANX-0.7.1/AndroidQQ/http/weishi.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.119424 ANX-0.7.1/AndroidQQ/im/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.119612 ANX-0.7.1/AndroidQQ/im/oidb/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.120050 ANX-0.7.1/AndroidQQ/im/oidb/OidbSvc_0xc96/
+-rw-r--r--   0 1a         (501) staff       (20)     2797 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)       34 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/OidbSvc_0xc96/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.120625 ANX-0.7.1/AndroidQQ/im/oidb/cmd0x88d/
+-rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/cmd0x88d/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2139 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.121643 ANX-0.7.1/AndroidQQ/im/oidb/cmd0x922/
+-rw-r--r--   0 1a         (501) staff       (20)     1343 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/cmd0x922/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1542 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.122185 ANX-0.7.1/AndroidQQ/im/oidb/cmd0xeb8/
+-rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/cmd0xeb8/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1872 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.122698 ANX-0.7.1/AndroidQQ/im/oidb/oidb_0xc05/
+-rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/oidb_0xc05/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2603 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.123221 ANX-0.7.1/AndroidQQ/im/oidb/oidb_sso/
+-rw-r--r--   0 1a         (501) staff       (20)       27 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/oidb_sso/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1468 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.123735 ANX-0.7.1/AndroidQQ/im/oidb/qqconnect/
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/qqconnect/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2618 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.124441 ANX-0.7.1/AndroidQQ/im/oidb/scanlogin/
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/scanlogin/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1385 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.124740 ANX-0.7.1/AndroidQQ/log/
+-rw-r--r--   0 1a         (501) staff       (20)       33 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/log/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.128646 ANX-0.7.1/AndroidQQ/pack/
+-rw-r--r--   0 1a         (501) staff       (20)      395 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/Heartbeat_Alive.py
+-rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py
+-rw-r--r--   0 1a         (501) staff       (20)      733 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py
+-rw-r--r--   0 1a         (501) staff       (20)     1368 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/OidbSvc_0x88d_1.py
+-rw-r--r--   0 1a         (501) staff       (20)      986 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/OidbSvc_0xc05.py
+-rw-r--r--   0 1a         (501) staff       (20)     1141 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/OidbSvc_0xc96.py
+-rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/OidbSvc_0xeb8.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.130620 ANX-0.7.1/AndroidQQ/pack/SQQzoneSvc/
+-rw-r--r--   0 1a         (501) staff       (20)       94 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/SQQzoneSvc/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1124 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/SQQzoneSvc/delUgc.py
+-rw-r--r--   0 1a         (501) staff       (20)     2637 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/SQQzoneSvc/like.py
+-rw-r--r--   0 1a         (501) staff       (20)     2631 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/SQQzoneSvc/publishmood.py
+-rw-r--r--   0 1a         (501) staff       (20)     2152 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1116 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/StatSvc_register.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.130977 ANX-0.7.1/AndroidQQ/pack/SummaryCard/
+-rw-r--r--   0 1a         (501) staff       (20)     1349 2024-03-07 10:14:41.000000 ANX-0.7.1/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/SummaryCard/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      402 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1383 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/friendlist.py
+-rw-r--r--   0 1a         (501) staff       (20)      543 2024-03-06 13:46:02.000000 ANX-0.7.1/AndroidQQ/pack/test.py
+-rw-r--r--   0 1a         (501) staff       (20)    46467 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.132435 ANX-0.7.1/AndroidQQ/proto/
+-rw-r--r--   0 1a         (501) staff       (20)     4301 2024-02-12 04:07:38.000000 ANX-0.7.1/AndroidQQ/proto/IM_r_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)       67 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/proto/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1308 2023-10-29 17:25:21.000000 ANX-0.7.1/AndroidQQ/proto/wtlogin_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.136115 ANX-0.7.1/AndroidQQ/struct/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.138068 ANX-0.7.1/AndroidQQ/struct/Avatarlnfo/
+-rw-r--r--   0 1a         (501) staff       (20)      444 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/Avatarlnfo/DestQQHeadInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1061 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      853 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py
+-rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py
+-rw-r--r--   0 1a         (501) staff       (20)     1028 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/Avatarlnfo/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      894 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/MessageSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.138703 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_COMM/
+-rw-r--r--   0 1a         (501) staff       (20)      373 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_COMM/UgcRightInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_COMM/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.141833 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/
+-rw-r--r--   0 1a         (501) staff       (20)       70 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     3064 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py
+-rw-r--r--   0 1a         (501) staff       (20)     1565 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py
+-rw-r--r--   0 1a         (501) staff       (20)      565 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      895 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py
+-rw-r--r--   0 1a         (501) staff       (20)     1789 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)      451 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/s_arkshare.py
+-rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py
+-rw-r--r--   0 1a         (501) staff       (20)      728 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py
+-rw-r--r--   0 1a         (501) staff       (20)      249 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/s_user.py
+-rw-r--r--   0 1a         (501) staff       (20)     1163 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.143845 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_OPERATION/
+-rw-r--r--   0 1a         (501) staff       (20)      479 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_OPERATION/Source.py
+-rw-r--r--   0 1a         (501) staff       (20)      187 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_OPERATION/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      656 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py
+-rw-r--r--   0 1a         (501) staff       (20)     1161 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py
+-rw-r--r--   0 1a         (501) staff       (20)     1300 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py
+-rw-r--r--   0 1a         (501) staff       (20)      560 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)     3031 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py
+-rw-r--r--   0 1a         (501) staff       (20)      503 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)      594 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/OidbSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.146293 ANX-0.7.1/AndroidQQ/struct/QMF_PROTOCAL/
+-rw-r--r--   0 1a         (501) staff       (20)      504 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/QMF_PROTOCAL/QmfBusiControl.py
+-rw-r--r--   0 1a         (501) staff       (20)      630 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      714 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py
+-rw-r--r--   0 1a         (501) staff       (20)      526 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1180 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py
+-rw-r--r--   0 1a         (501) staff       (20)      489 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/QMF_PROTOCAL/RetryInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       87 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/QMF_PROTOCAL/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.146674 ANX-0.7.1/AndroidQQ/struct/QQService/
+-rw-r--r--   0 1a         (501) staff       (20)     1112 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      878 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/QQService/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1115 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/StatSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.147423 ANX-0.7.1/AndroidQQ/struct/SummaryCard/
+-rw-r--r--   0 1a         (501) staff       (20)     2861 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py
+-rw-r--r--   0 1a         (501) staff       (20)      493 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/SummaryCard/UserLocaleInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       61 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/SummaryCard/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)    15568 2024-03-05 18:40:23.000000 ANX-0.7.1/AndroidQQ/struct/Tlv.py
+-rw-r--r--   0 1a         (501) staff       (20)     4784 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/Tlv_res.py
+-rw-r--r--   0 1a         (501) staff       (20)      131 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.147823 ANX-0.7.1/AndroidQQ/struct/cooperation/
+-rw-r--r--   0 1a         (501) staff       (20)       23 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/cooperation/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.148532 ANX-0.7.1/AndroidQQ/struct/cooperation/qzone/
+-rw-r--r--   0 1a         (501) staff       (20)     4558 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/cooperation/qzone/WNSStream.py
+-rw-r--r--   0 1a         (501) staff       (20)       26 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/cooperation/qzone/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.148928 ANX-0.7.1/AndroidQQ/struct/feedcomponent/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/feedcomponent/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1482 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/feedcomponent/model.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.149324 ANX-0.7.1/AndroidQQ/struct/friendlist/
+-rw-r--r--   0 1a         (501) staff       (20)     2842 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/friendlist/AddFriendReq.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/friendlist/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     7428 2024-03-07 10:14:48.000000 ANX-0.7.1/AndroidQQ/struct/head.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.149863 ANX-0.7.1/AndroidQQ/struct/push/
+-rw-r--r--   0 1a         (501) staff       (20)     3536 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/push/SvcReqRegister.py
+-rw-r--r--   0 1a         (501) staff       (20)     2084 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/push/SvcRespRegister.py
+-rw-r--r--   0 1a         (501) staff       (20)       31 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/struct/push/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)    27313 2024-03-05 18:40:23.000000 ANX-0.7.1/AndroidQQ/struct/wtlogin.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.151056 ANX-0.7.1/AndroidQQ/utils/
+-rw-r--r--   0 1a         (501) staff       (20)       20 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/utils/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      523 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/utils/build_device.py
+-rw-r--r--   0 1a         (501) staff       (20)     1140 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/utils/ecdh.py
+-rw-r--r--   0 1a         (501) staff       (20)     1379 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/utils/sso_server.py
+-rw-r--r--   0 1a         (501) staff       (20)      735 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/utils/tool.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.151238 ANX-0.7.1/AndroidQQ/wlogin_sdk/
+-rw-r--r--   0 1a         (501) staff       (20)       25 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/wlogin_sdk/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 02:36:45.151440 ANX-0.7.1/AndroidQQ/wlogin_sdk/request/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.1/AndroidQQ/wlogin_sdk/request/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      125 2024-04-02 02:36:45.151671 ANX-0.7.1/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)       34 2023-08-04 12:41:32.000000 ANX-0.7.1/README.md
+-rw-r--r--   0 1a         (501) staff       (20)       38 2024-04-02 02:36:45.151955 ANX-0.7.1/setup.cfg
+-rw-r--r--   0 1a         (501) staff       (20)      573 2024-04-02 02:36:35.000000 ANX-0.7.1/setup.py
```

### Comparing `ANX-0.7.0/ANX.egg-info/SOURCES.txt` & `ANX-0.7.1/ANX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/Android.py` & `ANX-0.7.1/AndroidQQ/Android.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/Tcp.py` & `ANX-0.7.1/AndroidQQ/Tcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,17 +95,20 @@
         host = random_item['1']
         port = random_item['2']
     else:
         # 没初始化ip列表前用这个快速连接
         host = '36.155.245.16'
         port = 8080
 
-    if len(proxy) == 2:
+    if len(proxy) >= 2:
         # 对于需要设置代理的客户端，创建一个配置了代理的socket对象
-        socks.set_default_proxy(socks.SOCKS5, proxy[0], proxy[1])
+        if len(proxy) == 2:
+            socks.set_default_proxy(socks.SOCKS5, proxy[0], proxy[1])
+        else:
+            socks.set_default_proxy(socks.SOCKS5, proxy[0], proxy[1], username=proxy[2], password=proxy[3])
         client = socks.socksocket()
     else:
         # 不需要代理的客户端，使用普通的socket对象
         client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
     try:
         client.connect((host, port))
```

### Comparing `ANX-0.7.0/AndroidQQ/http/ClientKey.py` & `ANX-0.7.1/AndroidQQ/http/ClientKey.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/http/accounts.py` & `ANX-0.7.1/AndroidQQ/http/accounts.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/http/friends.py` & `ANX-0.7.1/AndroidQQ/http/friends.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/http/game_credit.py` & `ANX-0.7.1/AndroidQQ/http/game_credit.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/http/level.py` & `ANX-0.7.1/AndroidQQ/http/level.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/http/music.py` & `ANX-0.7.1/AndroidQQ/http/music.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/http/qqsignin.py` & `ANX-0.7.1/AndroidQQ/http/qqsignin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/http/weishi.py` & `ANX-0.7.1/AndroidQQ/http/weishi.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py` & `ANX-0.7.1/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py` & `ANX-0.7.1/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py` & `ANX-0.7.1/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py` & `ANX-0.7.1/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py` & `ANX-0.7.1/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py` & `ANX-0.7.1/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py` & `ANX-0.7.1/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py` & `ANX-0.7.1/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py` & `ANX-0.7.1/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py` & `ANX-0.7.1/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py` & `ANX-0.7.1/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/pack/OidbSvc_0x88d_1.py` & `ANX-0.7.1/AndroidQQ/pack/OidbSvc_0x88d_1.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/pack/OidbSvc_0xc05.py` & `ANX-0.7.1/AndroidQQ/pack/OidbSvc_0xc05.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/pack/OidbSvc_0xc96.py` & `ANX-0.7.1/AndroidQQ/pack/OidbSvc_0xc96.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/pack/OidbSvc_0xeb8.py` & `ANX-0.7.1/AndroidQQ/pack/OidbSvc_0xeb8.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/pack/SQQzoneSvc/delUgc.py` & `ANX-0.7.1/AndroidQQ/pack/SQQzoneSvc/delUgc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/pack/SQQzoneSvc/like.py` & `ANX-0.7.1/AndroidQQ/pack/SQQzoneSvc/like.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/pack/SQQzoneSvc/publishmood.py` & `ANX-0.7.1/AndroidQQ/pack/SQQzoneSvc/publishmood.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py` & `ANX-0.7.1/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/pack/StatSvc_register.py` & `ANX-0.7.1/AndroidQQ/pack/StatSvc_register.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py` & `ANX-0.7.1/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/pack/friendlist.py` & `ANX-0.7.1/AndroidQQ/pack/friendlist.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/pack/test.py` & `ANX-0.7.1/AndroidQQ/pack/test.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py` & `ANX-0.7.1/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/proto/IM_r_pb2.py` & `ANX-0.7.1/AndroidQQ/proto/IM_r_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/proto/wtlogin_pb2.py` & `ANX-0.7.1/AndroidQQ/proto/wtlogin_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py` & `ANX-0.7.1/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py` & `ANX-0.7.1/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py` & `ANX-0.7.1/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/Avatarlnfo/__init__.py` & `ANX-0.7.1/AndroidQQ/struct/Avatarlnfo/__init__.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/MessageSvc.py` & `ANX-0.7.1/AndroidQQ/struct/MessageSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py` & `ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py` & `ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py` & `ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py` & `ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py` & `ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py` & `ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py` & `ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py` & `ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py` & `ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py` & `ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py` & `ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py` & `ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py` & `ANX-0.7.1/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/OidbSvc.py` & `ANX-0.7.1/AndroidQQ/struct/OidbSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py` & `ANX-0.7.1/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py` & `ANX-0.7.1/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py` & `ANX-0.7.1/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py` & `ANX-0.7.1/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py` & `ANX-0.7.1/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/QQService/__init__.py` & `ANX-0.7.1/AndroidQQ/struct/QQService/__init__.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/StatSvc.py` & `ANX-0.7.1/AndroidQQ/struct/StatSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py` & `ANX-0.7.1/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/Tlv.py` & `ANX-0.7.1/AndroidQQ/struct/Tlv.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/Tlv_res.py` & `ANX-0.7.1/AndroidQQ/struct/Tlv_res.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/cooperation/qzone/WNSStream.py` & `ANX-0.7.1/AndroidQQ/struct/cooperation/qzone/WNSStream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/feedcomponent/model.py` & `ANX-0.7.1/AndroidQQ/struct/feedcomponent/model.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/friendlist/AddFriendReq.py` & `ANX-0.7.1/AndroidQQ/struct/friendlist/AddFriendReq.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/head.py` & `ANX-0.7.1/AndroidQQ/struct/head.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/push/SvcReqRegister.py` & `ANX-0.7.1/AndroidQQ/struct/push/SvcReqRegister.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/push/SvcRespRegister.py` & `ANX-0.7.1/AndroidQQ/struct/push/SvcRespRegister.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/struct/wtlogin.py` & `ANX-0.7.1/AndroidQQ/struct/wtlogin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/utils/build_device.py` & `ANX-0.7.1/AndroidQQ/utils/build_device.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/utils/ecdh.py` & `ANX-0.7.1/AndroidQQ/utils/ecdh.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/utils/sso_server.py` & `ANX-0.7.1/AndroidQQ/utils/sso_server.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/AndroidQQ/utils/tool.py` & `ANX-0.7.1/AndroidQQ/utils/tool.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.0/setup.py` & `ANX-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 setuptools.setup(
     name='ANX',
-    version='0.7.0',
+    version='0.7.1',
     url='https://github.com/grayrail000/AndroidQQ',
     packages=setuptools.find_packages(),
     license='',
     author='1x',
     author_email='',
     description='',
     install_requires=[
```

