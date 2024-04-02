# Comparing `tmp/tigeropen-3.1.9.tar.gz` & `tmp/tigeropen-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigeropen-3.1.9.tar", last modified: Mon Mar 18 09:54:47 2024, max compression
+gzip compressed data, was "tigeropen-3.2.0.tar", last modified: Tue Apr  2 03:14:12 2024, max compression
```

## Comparing `tigeropen-3.1.9.tar` & `tigeropen-3.2.0.tar`

### file list

```diff
@@ -1,226 +1,226 @@
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.434124 tigeropen-3.1.9/
--rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-3.1.9/MANIFEST.in
--rw-r--r--   0 sukai      (501) staff       (20)     7120 2024-03-18 09:54:47.433808 tigeropen-3.1.9/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-3.1.9/README.md
--rw-r--r--   0 sukai      (501) staff       (20)      137 2024-02-27 08:47:04.000000 tigeropen-3.1.9/requirements.txt
--rw-r--r--   0 sukai      (501) staff       (20)       38 2024-03-18 09:54:47.434188 tigeropen-3.1.9/setup.cfg
--rw-r--r--   0 sukai      (501) staff       (20)     1358 2024-01-19 03:27:35.000000 tigeropen-3.1.9/setup.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.390640 tigeropen-3.1.9/tests/
--rw-r--r--   0 sukai      (501) staff       (20)     2628 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tests/test_client_config.py
--rw-r--r--   0 sukai      (501) staff       (20)     2589 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tests/test_push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)     2856 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tests/test_utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.391165 tigeropen-3.1.9/tigeropen/
--rw-r--r--   0 sukai      (501) staff       (20)       91 2024-03-18 09:54:40.000000 tigeropen-3.1.9/tigeropen/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.393411 tigeropen-3.1.9/tigeropen/common/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.1.9/tigeropen/common/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.396171 tigeropen-3.1.9/tigeropen/common/consts/
--rw-r--r--   0 sukai      (501) staff       (20)     5171 2024-03-12 07:51:18.000000 tigeropen-3.1.9/tigeropen/common/consts/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    19289 2024-02-27 08:46:55.000000 tigeropen-3.1.9/tigeropen/common/consts/filter_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)    39797 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/common/consts/fundamental_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-3.1.9/tigeropen/common/consts/params.py
--rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/common/consts/push_destinations.py
--rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/common/consts/push_subscriptions.py
--rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-3.1.9/tigeropen/common/consts/push_types.py
--rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-3.1.9/tigeropen/common/consts/quote_keys.py
--rw-r--r--   0 sukai      (501) staff       (20)     3296 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/common/consts/service_types.py
--rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/common/consts/tick_constants.py
--rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-3.1.9/tigeropen/common/exceptions.py
--rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-3.1.9/tigeropen/common/model.py
--rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/common/request.py
--rw-r--r--   0 sukai      (501) staff       (20)      654 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/common/response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.398095 tigeropen-3.1.9/tigeropen/common/util/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.1.9/tigeropen/common/util/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/common/util/account_util.py
--rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/common/util/common_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     4032 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/common/util/contract_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     8379 2024-03-12 07:51:18.000000 tigeropen-3.1.9/tigeropen/common/util/order_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     3124 2024-03-12 07:51:18.000000 tigeropen-3.1.9/tigeropen/common/util/price_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     2709 2024-02-27 08:47:04.000000 tigeropen-3.1.9/tigeropen/common/util/signature_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-3.1.9/tigeropen/common/util/string_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-3.1.9/tigeropen/common/util/tick_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     1675 2024-02-27 08:47:04.000000 tigeropen-3.1.9/tigeropen/common/util/web_utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.399825 tigeropen-3.1.9/tigeropen/examples/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.1.9/tigeropen/examples/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/examples/client_config.py
--rw-r--r--   0 sukai      (501) staff       (20)     7026 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/examples/financial_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/examples/nasdaq100.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.400332 tigeropen-3.1.9/tigeropen/examples/option_helpers/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/examples/option_helpers/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/examples/option_helpers/helpers.py
--rw-r--r--   0 sukai      (501) staff       (20)    11453 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/examples/push_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    11030 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/examples/push_client_stomp_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    13724 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/examples/quote_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)     8386 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/examples/trade_client_demo.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.400565 tigeropen-3.1.9/tigeropen/fundamental/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.1.9/tigeropen/fundamental/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.400753 tigeropen-3.1.9/tigeropen/fundamental/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.1.9/tigeropen/fundamental/domain/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.401157 tigeropen-3.1.9/tigeropen/fundamental/request/
--rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-3.1.9/tigeropen/fundamental/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     7711 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/fundamental/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.402962 tigeropen-3.1.9/tigeropen/fundamental/response/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.1.9/tigeropen/fundamental/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-3.1.9/tigeropen/fundamental/response/corporate_dividend_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-3.1.9/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-3.1.9/tigeropen/fundamental/response/corporate_split_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      898 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/fundamental/response/dataframe_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/fundamental/response/financial_daily_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      972 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/fundamental/response/financial_exchange_rate_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/fundamental/response/financial_report_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/fundamental/response/industry_response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.403677 tigeropen-3.1.9/tigeropen/push/
--rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/push/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.405200 tigeropen-3.1.9/tigeropen/push/network/
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-3.1.9/tigeropen/push/network/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-3.1.9/tigeropen/push/network/connect.py
--rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-3.1.9/tigeropen/push/network/exception.py
--rw-r--r--   0 sukai      (501) staff       (20)     7566 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/push/network/listener.py
--rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-3.1.9/tigeropen/push/network/protocal.py
--rw-r--r--   0 sukai      (501) staff       (20)    31352 2024-02-27 08:47:04.000000 tigeropen-3.1.9/tigeropen/push/network/transport.py
--rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-3.1.9/tigeropen/push/network/utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.416142 tigeropen-3.1.9/tigeropen/push/pb/
--rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-3.1.9/tigeropen/push/pb/AssetData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1572 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/AssetData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1887 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/AssetData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      714 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/push/pb/KlineData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1446 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/push/pb/KlineData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1355 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/push/pb/KlineData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1238 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/push/pb/OptionTopData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2473 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/OptionTopData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3823 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/OptionTopData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     2051 2024-02-28 06:50:45.000000 tigeropen-3.1.9/tigeropen/push/pb/OrderStatusData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2662 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/OrderStatusData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4752 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/OrderStatusData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-3.1.9/tigeropen/push/pb/OrderTransactionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1729 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/OrderTransactionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2102 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/OrderTransactionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1117 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/push/pb/PositionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1824 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/PositionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2418 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/PositionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1089 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/push/pb/PushData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     4091 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/push/pb/PushData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3921 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/push/pb/PushData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-3.1.9/tigeropen/push/pb/QuoteBBOData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1702 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/QuoteBBOData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/QuoteBBOData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-3.1.9/tigeropen/push/pb/QuoteBasicData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3046 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/QuoteBasicData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3115 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/QuoteBasicData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     2303 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/push/pb/QuoteData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3573 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/QuoteData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4265 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/QuoteData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      433 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/push/pb/QuoteDepthData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1570 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/QuoteDepthData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1817 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/QuoteDepthData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      622 2024-03-06 07:57:50.000000 tigeropen-3.1.9/tigeropen/push/pb/Request.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2412 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/Request_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2457 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/Request_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-3.1.9/tigeropen/push/pb/Response.proto
--rw-r--r--   0 sukai      (501) staff       (20)     5105 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/push/pb/Response_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1917 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/push/pb/Response_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      781 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/push/pb/SocketCommon.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2129 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/push/pb/SocketCommon_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1584 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/push/pb/SocketCommon_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      411 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/push/pb/StockTopData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1631 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/StockTopData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1720 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/StockTopData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-3.1.9/tigeropen/push/pb/TradeTickData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1760 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/TradeTickData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2502 2024-03-06 08:28:03.000000 tigeropen-3.1.9/tigeropen/push/pb/TradeTickData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)        0 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/push/pb/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-3.1.9/tigeropen/push/pb/readme.md
--rw-r--r--   0 sukai      (501) staff       (20)      661 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/push/pb/trade_tick.py
--rw-r--r--   0 sukai      (501) staff       (20)     9466 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/push/pb/util.py
--rw-r--r--   0 sukai      (501) staff       (20)    19439 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/push/protobuf_push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)     9707 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/push/push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    28647 2024-03-18 09:47:36.000000 tigeropen-3.1.9/tigeropen/push/stomp_push_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.416512 tigeropen-3.1.9/tigeropen/quote/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.1.9/tigeropen/quote/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.418581 tigeropen-3.1.9/tigeropen/quote/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.1.9/tigeropen/quote/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/quote/domain/bar.py
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-3.1.9/tigeropen/quote/domain/capital_distribution.py
--rw-r--r--   0 sukai      (501) staff       (20)     9623 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/quote/domain/filter.py
--rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/quote/domain/market_status.py
--rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/quote/domain/quote_brief.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-3.1.9/tigeropen/quote/domain/stock_broker.py
--rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/quote/domain/tick.py
--rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/quote/domain/timeline.py
--rw-r--r--   0 sukai      (501) staff       (20)    83925 2024-03-18 09:54:40.000000 tigeropen-3.1.9/tigeropen/quote/quote_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.418949 tigeropen-3.1.9/tigeropen/quote/request/
--rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/quote/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    34912 2024-03-18 09:54:40.000000 tigeropen-3.1.9/tigeropen/quote/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.427348 tigeropen-3.1.9/tigeropen/quote/response/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.1.9/tigeropen/quote/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-3.1.9/tigeropen/quote/response/capital_distribution_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-3.1.9/tigeropen/quote/response/capital_flow_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      911 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/quote/response/fund_contracts_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-3.1.9/tigeropen/quote/response/future_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-3.1.9/tigeropen/quote/response/future_contract_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/quote/response/future_exchange_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1746 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/quote/response/future_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/quote/response/future_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-3.1.9/tigeropen/quote/response/future_trading_times_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      706 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/quote/response/kline_quota_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1805 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/quote/response/market_scanner_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/quote/response/market_status_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/quote/response/option_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-3.1.9/tigeropen/quote/response/option_chains_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1121 2024-03-18 09:34:43.000000 tigeropen-3.1.9/tigeropen/quote/response/option_expirations_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/quote/response/option_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/quote/response/option_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1599 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/quote/response/quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2469 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/quote/response/quote_brief_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      983 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/quote/response/quote_dataframe_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-3.1.9/tigeropen/quote/response/quote_delay_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/quote/response/quote_depth_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/quote/response/quote_grab_permission_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2730 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/quote/response/quote_hour_trading_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2410 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/quote/response/quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-3.1.9/tigeropen/quote/response/quote_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1152 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/quote/response/stock_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-3.1.9/tigeropen/quote/response/stock_broker_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4898 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/quote/response/stock_details_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/quote/response/stock_short_interest_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/quote/response/stock_trade_meta_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-3.1.9/tigeropen/quote/response/symbol_names_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      653 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/quote/response/symbols_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/quote/response/trading_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      802 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/quote/response/warrant_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      979 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/quote/response/warrant_filter_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    11281 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/tiger_open_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    16397 2024-03-06 07:57:50.000000 tigeropen-3.1.9/tigeropen/tiger_open_config.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.427868 tigeropen-3.1.9/tigeropen/trade/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.1.9/tigeropen/trade/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.429809 tigeropen-3.1.9/tigeropen/trade/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.1.9/tigeropen/trade/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    11655 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/trade/domain/account.py
--rw-r--r--   0 sukai      (501) staff       (20)     6154 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/trade/domain/contract.py
--rw-r--r--   0 sukai      (501) staff       (20)    11246 2024-03-12 07:51:18.000000 tigeropen-3.1.9/tigeropen/trade/domain/order.py
--rw-r--r--   0 sukai      (501) staff       (20)     2704 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/trade/domain/position.py
--rw-r--r--   0 sukai      (501) staff       (20)     3242 2024-02-27 08:46:55.000000 tigeropen-3.1.9/tigeropen/trade/domain/prime_account.py
--rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/trade/domain/profile.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.430399 tigeropen-3.1.9/tigeropen/trade/request/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.1.9/tigeropen/trade/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    35911 2024-03-12 07:51:18.000000 tigeropen-3.1.9/tigeropen/trade/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.433364 tigeropen-3.1.9/tigeropen/trade/response/
--rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-3.1.9/tigeropen/trade/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1120 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/trade/response/account_profile_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      949 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/trade/response/analytics_asset_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4426 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/trade/response/assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1608 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/trade/response/contracts_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/trade/response/forex_order_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1255 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/trade/response/order_id_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1278 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/trade/response/order_preview_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     8507 2024-03-12 07:51:18.000000 tigeropen-3.1.9/tigeropen/trade/response/orders_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     6199 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/trade/response/positions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-3.1.9/tigeropen/trade/response/prime_assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2539 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/trade/response/segment_fund_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1413 2024-01-19 03:27:35.000000 tigeropen-3.1.9/tigeropen/trade/response/transactions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    40884 2024-03-12 07:51:18.000000 tigeropen-3.1.9/tigeropen/trade/trade_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-03-18 09:54:47.391992 tigeropen-3.1.9/tigeropen.egg-info/
--rw-r--r--   0 sukai      (501) staff       (20)     7120 2024-03-18 09:54:47.000000 tigeropen-3.1.9/tigeropen.egg-info/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     8053 2024-03-18 09:54:47.000000 tigeropen-3.1.9/tigeropen.egg-info/SOURCES.txt
--rw-r--r--   0 sukai      (501) staff       (20)        1 2024-03-18 09:54:47.000000 tigeropen-3.1.9/tigeropen.egg-info/dependency_links.txt
--rw-r--r--   0 sukai      (501) staff       (20)      138 2024-03-18 09:54:47.000000 tigeropen-3.1.9/tigeropen.egg-info/requires.txt
--rw-r--r--   0 sukai      (501) staff       (20)       10 2024-03-18 09:54:47.000000 tigeropen-3.1.9/tigeropen.egg-info/top_level.txt
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.059547 tigeropen-3.2.0/
+-rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-3.2.0/MANIFEST.in
+-rw-r--r--   0 sukai      (501) staff       (20)     7120 2024-04-02 03:14:12.059273 tigeropen-3.2.0/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-3.2.0/README.md
+-rw-r--r--   0 sukai      (501) staff       (20)      137 2024-02-27 08:47:04.000000 tigeropen-3.2.0/requirements.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       38 2024-04-02 03:14:12.059610 tigeropen-3.2.0/setup.cfg
+-rw-r--r--   0 sukai      (501) staff       (20)     1358 2024-01-19 03:27:35.000000 tigeropen-3.2.0/setup.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.018771 tigeropen-3.2.0/tests/
+-rw-r--r--   0 sukai      (501) staff       (20)     2628 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tests/test_client_config.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2589 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tests/test_push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2856 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tests/test_utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.019318 tigeropen-3.2.0/tigeropen/
+-rw-r--r--   0 sukai      (501) staff       (20)       91 2024-04-02 03:14:04.000000 tigeropen-3.2.0/tigeropen/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.021243 tigeropen-3.2.0/tigeropen/common/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.0/tigeropen/common/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.023792 tigeropen-3.2.0/tigeropen/common/consts/
+-rw-r--r--   0 sukai      (501) staff       (20)     5171 2024-03-12 07:51:18.000000 tigeropen-3.2.0/tigeropen/common/consts/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    19289 2024-02-27 08:46:55.000000 tigeropen-3.2.0/tigeropen/common/consts/filter_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)    39797 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/common/consts/fundamental_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-3.2.0/tigeropen/common/consts/params.py
+-rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/common/consts/push_destinations.py
+-rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/common/consts/push_subscriptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-3.2.0/tigeropen/common/consts/push_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-3.2.0/tigeropen/common/consts/quote_keys.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3296 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/common/consts/service_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/common/consts/tick_constants.py
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-3.2.0/tigeropen/common/exceptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-3.2.0/tigeropen/common/model.py
+-rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/common/request.py
+-rw-r--r--   0 sukai      (501) staff       (20)      654 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/common/response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.025459 tigeropen-3.2.0/tigeropen/common/util/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.0/tigeropen/common/util/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/common/util/account_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/common/util/common_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4032 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/common/util/contract_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8379 2024-03-12 07:51:18.000000 tigeropen-3.2.0/tigeropen/common/util/order_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3124 2024-03-12 07:51:18.000000 tigeropen-3.2.0/tigeropen/common/util/price_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2709 2024-02-27 08:47:04.000000 tigeropen-3.2.0/tigeropen/common/util/signature_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-3.2.0/tigeropen/common/util/string_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-3.2.0/tigeropen/common/util/tick_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1675 2024-02-27 08:47:04.000000 tigeropen-3.2.0/tigeropen/common/util/web_utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.026975 tigeropen-3.2.0/tigeropen/examples/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.0/tigeropen/examples/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/examples/client_config.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7026 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/examples/financial_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/examples/nasdaq100.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.027343 tigeropen-3.2.0/tigeropen/examples/option_helpers/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/examples/option_helpers/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/examples/option_helpers/helpers.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11453 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/examples/push_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11030 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/examples/push_client_stomp_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    13724 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/examples/quote_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8386 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/examples/trade_client_demo.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.027520 tigeropen-3.2.0/tigeropen/fundamental/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.2.0/tigeropen/fundamental/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.027689 tigeropen-3.2.0/tigeropen/fundamental/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.2.0/tigeropen/fundamental/domain/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.028057 tigeropen-3.2.0/tigeropen/fundamental/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-3.2.0/tigeropen/fundamental/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7711 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/fundamental/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.029792 tigeropen-3.2.0/tigeropen/fundamental/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-3.2.0/tigeropen/fundamental/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-3.2.0/tigeropen/fundamental/response/corporate_dividend_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-3.2.0/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-3.2.0/tigeropen/fundamental/response/corporate_split_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      898 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/fundamental/response/dataframe_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/fundamental/response/financial_daily_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      972 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/fundamental/response/financial_exchange_rate_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/fundamental/response/financial_report_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/fundamental/response/industry_response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.030475 tigeropen-3.2.0/tigeropen/push/
+-rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/push/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.031663 tigeropen-3.2.0/tigeropen/push/network/
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-3.2.0/tigeropen/push/network/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-3.2.0/tigeropen/push/network/connect.py
+-rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-3.2.0/tigeropen/push/network/exception.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7566 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/push/network/listener.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-3.2.0/tigeropen/push/network/protocal.py
+-rw-r--r--   0 sukai      (501) staff       (20)    31352 2024-02-27 08:47:04.000000 tigeropen-3.2.0/tigeropen/push/network/transport.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-3.2.0/tigeropen/push/network/utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.043087 tigeropen-3.2.0/tigeropen/push/pb/
+-rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-3.2.0/tigeropen/push/pb/AssetData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1572 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/AssetData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1887 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/AssetData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      714 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/push/pb/KlineData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1446 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/push/pb/KlineData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1355 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/push/pb/KlineData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1238 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/push/pb/OptionTopData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2473 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/OptionTopData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3823 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/OptionTopData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     2051 2024-02-28 06:50:45.000000 tigeropen-3.2.0/tigeropen/push/pb/OrderStatusData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2662 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/OrderStatusData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4752 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/OrderStatusData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-3.2.0/tigeropen/push/pb/OrderTransactionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1729 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/OrderTransactionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2102 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/OrderTransactionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1117 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/push/pb/PositionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1824 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/PositionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2418 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/PositionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1089 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/push/pb/PushData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     4091 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/push/pb/PushData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3921 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/push/pb/PushData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-3.2.0/tigeropen/push/pb/QuoteBBOData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1702 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/QuoteBBOData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/QuoteBBOData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-3.2.0/tigeropen/push/pb/QuoteBasicData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3046 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/QuoteBasicData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3115 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/QuoteBasicData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     2303 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/push/pb/QuoteData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3573 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/QuoteData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4265 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/QuoteData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      433 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/push/pb/QuoteDepthData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1570 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/QuoteDepthData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1817 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/QuoteDepthData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      622 2024-03-06 07:57:50.000000 tigeropen-3.2.0/tigeropen/push/pb/Request.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2412 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/Request_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2457 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/Request_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-3.2.0/tigeropen/push/pb/Response.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     5105 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/push/pb/Response_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1917 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/push/pb/Response_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      781 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/push/pb/SocketCommon.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2129 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/push/pb/SocketCommon_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1584 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/push/pb/SocketCommon_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/push/pb/StockTopData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1631 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/StockTopData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1720 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/StockTopData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-3.2.0/tigeropen/push/pb/TradeTickData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1760 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/TradeTickData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2502 2024-03-06 08:28:03.000000 tigeropen-3.2.0/tigeropen/push/pb/TradeTickData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/push/pb/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-3.2.0/tigeropen/push/pb/readme.md
+-rw-r--r--   0 sukai      (501) staff       (20)      661 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/push/pb/trade_tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9466 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/push/pb/util.py
+-rw-r--r--   0 sukai      (501) staff       (20)    19439 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/push/protobuf_push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9707 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/push/push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    28647 2024-03-18 09:47:36.000000 tigeropen-3.2.0/tigeropen/push/stomp_push_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.043466 tigeropen-3.2.0/tigeropen/quote/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.0/tigeropen/quote/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.045524 tigeropen-3.2.0/tigeropen/quote/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.0/tigeropen/quote/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/quote/domain/bar.py
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-3.2.0/tigeropen/quote/domain/capital_distribution.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9623 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/quote/domain/filter.py
+-rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/quote/domain/market_status.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/quote/domain/quote_brief.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-3.2.0/tigeropen/quote/domain/stock_broker.py
+-rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/quote/domain/tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/quote/domain/timeline.py
+-rw-r--r--   0 sukai      (501) staff       (20)    84071 2024-04-02 03:14:04.000000 tigeropen-3.2.0/tigeropen/quote/quote_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.045959 tigeropen-3.2.0/tigeropen/quote/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/quote/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    35270 2024-04-02 03:14:04.000000 tigeropen-3.2.0/tigeropen/quote/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.053472 tigeropen-3.2.0/tigeropen/quote/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.0/tigeropen/quote/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-3.2.0/tigeropen/quote/response/capital_distribution_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-3.2.0/tigeropen/quote/response/capital_flow_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      911 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/quote/response/fund_contracts_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-3.2.0/tigeropen/quote/response/future_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-3.2.0/tigeropen/quote/response/future_contract_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/quote/response/future_exchange_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1746 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/quote/response/future_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/quote/response/future_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-3.2.0/tigeropen/quote/response/future_trading_times_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      706 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/quote/response/kline_quota_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1805 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/quote/response/market_scanner_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/quote/response/market_status_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/quote/response/option_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-3.2.0/tigeropen/quote/response/option_chains_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1121 2024-03-18 09:34:43.000000 tigeropen-3.2.0/tigeropen/quote/response/option_expirations_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/quote/response/option_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/quote/response/option_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1599 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/quote/response/quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2469 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/quote/response/quote_brief_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      983 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/quote/response/quote_dataframe_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-3.2.0/tigeropen/quote/response/quote_delay_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/quote/response/quote_depth_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/quote/response/quote_grab_permission_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2730 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/quote/response/quote_hour_trading_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2410 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/quote/response/quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-3.2.0/tigeropen/quote/response/quote_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1152 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/quote/response/stock_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-3.2.0/tigeropen/quote/response/stock_broker_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4898 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/quote/response/stock_details_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/quote/response/stock_short_interest_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/quote/response/stock_trade_meta_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-3.2.0/tigeropen/quote/response/symbol_names_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      653 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/quote/response/symbols_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/quote/response/trading_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      802 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/quote/response/warrant_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      979 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/quote/response/warrant_filter_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11281 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/tiger_open_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    16397 2024-03-06 07:57:50.000000 tigeropen-3.2.0/tigeropen/tiger_open_config.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.053857 tigeropen-3.2.0/tigeropen/trade/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-3.2.0/tigeropen/trade/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.055840 tigeropen-3.2.0/tigeropen/trade/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.0/tigeropen/trade/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11655 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/trade/domain/account.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6154 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/trade/domain/contract.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11246 2024-03-12 07:51:18.000000 tigeropen-3.2.0/tigeropen/trade/domain/order.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2704 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/trade/domain/position.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3242 2024-02-27 08:46:55.000000 tigeropen-3.2.0/tigeropen/trade/domain/prime_account.py
+-rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/trade/domain/profile.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.056386 tigeropen-3.2.0/tigeropen/trade/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-3.2.0/tigeropen/trade/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    35911 2024-03-12 07:51:18.000000 tigeropen-3.2.0/tigeropen/trade/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.058844 tigeropen-3.2.0/tigeropen/trade/response/
+-rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-3.2.0/tigeropen/trade/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1120 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/trade/response/account_profile_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      949 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/trade/response/analytics_asset_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4426 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/trade/response/assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1608 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/trade/response/contracts_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/trade/response/forex_order_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1255 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/trade/response/order_id_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1278 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/trade/response/order_preview_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8507 2024-03-12 07:51:18.000000 tigeropen-3.2.0/tigeropen/trade/response/orders_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6199 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/trade/response/positions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-3.2.0/tigeropen/trade/response/prime_assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2539 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/trade/response/segment_fund_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1413 2024-01-19 03:27:35.000000 tigeropen-3.2.0/tigeropen/trade/response/transactions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    40878 2024-04-02 03:14:04.000000 tigeropen-3.2.0/tigeropen/trade/trade_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2024-04-02 03:14:12.020148 tigeropen-3.2.0/tigeropen.egg-info/
+-rw-r--r--   0 sukai      (501) staff       (20)     7120 2024-04-02 03:14:11.000000 tigeropen-3.2.0/tigeropen.egg-info/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     8053 2024-04-02 03:14:11.000000 tigeropen-3.2.0/tigeropen.egg-info/SOURCES.txt
+-rw-r--r--   0 sukai      (501) staff       (20)        1 2024-04-02 03:14:11.000000 tigeropen-3.2.0/tigeropen.egg-info/dependency_links.txt
+-rw-r--r--   0 sukai      (501) staff       (20)      138 2024-04-02 03:14:11.000000 tigeropen-3.2.0/tigeropen.egg-info/requires.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       10 2024-04-02 03:14:11.000000 tigeropen-3.2.0/tigeropen.egg-info/top_level.txt
```

### Comparing `tigeropen-3.1.9/PKG-INFO` & `tigeropen-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 3.1.9
+Version: 3.2.0
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-3.1.9/README.md` & `tigeropen-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/setup.py` & `tigeropen-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tests/test_client_config.py` & `tigeropen-3.2.0/tests/test_client_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tests/test_push_client.py` & `tigeropen-3.2.0/tests/test_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tests/test_utils.py` & `tigeropen-3.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/consts/__init__.py` & `tigeropen-3.2.0/tigeropen/common/consts/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/consts/filter_fields.py` & `tigeropen-3.2.0/tigeropen/common/consts/filter_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/consts/fundamental_fields.py` & `tigeropen-3.2.0/tigeropen/common/consts/fundamental_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/consts/params.py` & `tigeropen-3.2.0/tigeropen/common/consts/params.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/consts/push_types.py` & `tigeropen-3.2.0/tigeropen/common/consts/push_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/consts/quote_keys.py` & `tigeropen-3.2.0/tigeropen/common/consts/quote_keys.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/consts/service_types.py` & `tigeropen-3.2.0/tigeropen/common/consts/service_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/consts/tick_constants.py` & `tigeropen-3.2.0/tigeropen/common/consts/tick_constants.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/model.py` & `tigeropen-3.2.0/tigeropen/common/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/request.py` & `tigeropen-3.2.0/tigeropen/common/request.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/response.py` & `tigeropen-3.2.0/tigeropen/common/response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/util/common_utils.py` & `tigeropen-3.2.0/tigeropen/common/util/common_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/util/contract_utils.py` & `tigeropen-3.2.0/tigeropen/common/util/contract_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/util/order_utils.py` & `tigeropen-3.2.0/tigeropen/common/util/order_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/util/price_util.py` & `tigeropen-3.2.0/tigeropen/common/util/price_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/util/signature_utils.py` & `tigeropen-3.2.0/tigeropen/common/util/signature_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/util/string_utils.py` & `tigeropen-3.2.0/tigeropen/common/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/util/tick_util.py` & `tigeropen-3.2.0/tigeropen/common/util/tick_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/common/util/web_utils.py` & `tigeropen-3.2.0/tigeropen/common/util/web_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/examples/client_config.py` & `tigeropen-3.2.0/tigeropen/examples/client_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/examples/financial_demo.py` & `tigeropen-3.2.0/tigeropen/examples/financial_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/examples/nasdaq100.py` & `tigeropen-3.2.0/tigeropen/examples/nasdaq100.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/examples/option_helpers/helpers.py` & `tigeropen-3.2.0/tigeropen/examples/option_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/examples/push_client_demo.py` & `tigeropen-3.2.0/tigeropen/examples/push_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/examples/push_client_stomp_demo.py` & `tigeropen-3.2.0/tigeropen/examples/push_client_stomp_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/examples/quote_client_demo.py` & `tigeropen-3.2.0/tigeropen/examples/quote_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/examples/trade_client_demo.py` & `tigeropen-3.2.0/tigeropen/examples/trade_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/fundamental/request/model.py` & `tigeropen-3.2.0/tigeropen/fundamental/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/fundamental/response/corporate_dividend_response.py` & `tigeropen-3.2.0/tigeropen/fundamental/response/corporate_dividend_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/fundamental/response/corporate_earnings_calendar_response.py` & `tigeropen-3.2.0/tigeropen/fundamental/response/corporate_earnings_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/fundamental/response/corporate_split_response.py` & `tigeropen-3.2.0/tigeropen/fundamental/response/corporate_split_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/fundamental/response/dataframe_response.py` & `tigeropen-3.2.0/tigeropen/fundamental/response/dataframe_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/fundamental/response/financial_daily_response.py` & `tigeropen-3.2.0/tigeropen/fundamental/response/financial_daily_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/fundamental/response/financial_exchange_rate_response.py` & `tigeropen-3.2.0/tigeropen/fundamental/response/financial_exchange_rate_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/fundamental/response/financial_report_response.py` & `tigeropen-3.2.0/tigeropen/fundamental/response/financial_report_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/fundamental/response/industry_response.py` & `tigeropen-3.2.0/tigeropen/fundamental/response/industry_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/__init__.py` & `tigeropen-3.2.0/tigeropen/push/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/network/connect.py` & `tigeropen-3.2.0/tigeropen/push/network/connect.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/network/exception.py` & `tigeropen-3.2.0/tigeropen/push/network/exception.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/network/listener.py` & `tigeropen-3.2.0/tigeropen/push/network/listener.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/network/protocal.py` & `tigeropen-3.2.0/tigeropen/push/network/protocal.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/network/transport.py` & `tigeropen-3.2.0/tigeropen/push/network/transport.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/network/utils.py` & `tigeropen-3.2.0/tigeropen/push/network/utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/AssetData.proto` & `tigeropen-3.2.0/tigeropen/push/pb/AssetData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/AssetData_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/AssetData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/AssetData_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/AssetData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/KlineData.proto` & `tigeropen-3.2.0/tigeropen/push/pb/KlineData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/KlineData_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/KlineData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/KlineData_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/KlineData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/OptionTopData.proto` & `tigeropen-3.2.0/tigeropen/push/pb/OptionTopData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/OptionTopData_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/OptionTopData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/OptionTopData_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/OptionTopData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/OrderStatusData.proto` & `tigeropen-3.2.0/tigeropen/push/pb/OrderStatusData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/OrderStatusData_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/OrderStatusData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/OrderStatusData_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/OrderStatusData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/OrderTransactionData.proto` & `tigeropen-3.2.0/tigeropen/push/pb/OrderTransactionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/OrderTransactionData_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/OrderTransactionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/OrderTransactionData_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/OrderTransactionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/PositionData.proto` & `tigeropen-3.2.0/tigeropen/push/pb/PositionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/PositionData_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/PositionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/PositionData_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/PositionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/PushData.proto` & `tigeropen-3.2.0/tigeropen/push/pb/PushData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/PushData_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/PushData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/PushData_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/PushData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/QuoteBBOData_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/QuoteBBOData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/QuoteBBOData_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/QuoteBBOData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/QuoteBasicData.proto` & `tigeropen-3.2.0/tigeropen/push/pb/QuoteBasicData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/QuoteBasicData_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/QuoteBasicData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/QuoteBasicData_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/QuoteBasicData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/QuoteData.proto` & `tigeropen-3.2.0/tigeropen/push/pb/QuoteData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/QuoteData_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/QuoteData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/QuoteData_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/QuoteData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/QuoteDepthData_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/QuoteDepthData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/QuoteDepthData_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/QuoteDepthData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/Request.proto` & `tigeropen-3.2.0/tigeropen/push/pb/Request.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/Request_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/Request_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/Request_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/Request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/Response_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/Response_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/Response_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/Response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/SocketCommon.proto` & `tigeropen-3.2.0/tigeropen/push/pb/SocketCommon.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/SocketCommon_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/SocketCommon_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/SocketCommon_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/SocketCommon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/StockTopData_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/StockTopData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/StockTopData_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/StockTopData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/TradeTickData.proto` & `tigeropen-3.2.0/tigeropen/push/pb/TradeTickData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/TradeTickData_pb2.py` & `tigeropen-3.2.0/tigeropen/push/pb/TradeTickData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/TradeTickData_pb2.pyi` & `tigeropen-3.2.0/tigeropen/push/pb/TradeTickData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/trade_tick.py` & `tigeropen-3.2.0/tigeropen/push/pb/trade_tick.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/pb/util.py` & `tigeropen-3.2.0/tigeropen/push/pb/util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/protobuf_push_client.py` & `tigeropen-3.2.0/tigeropen/push/protobuf_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/push_client.py` & `tigeropen-3.2.0/tigeropen/push/push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/push/stomp_push_client.py` & `tigeropen-3.2.0/tigeropen/push/stomp_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/domain/filter.py` & `tigeropen-3.2.0/tigeropen/quote/domain/filter.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/domain/quote_brief.py` & `tigeropen-3.2.0/tigeropen/quote/domain/quote_brief.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/domain/stock_broker.py` & `tigeropen-3.2.0/tigeropen/quote/domain/stock_broker.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/quote_client.py` & `tigeropen-3.2.0/tigeropen/quote/quote_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -653,20 +653,21 @@
             if response.is_success():
                 return response.expirations
             else:
                 raise ApiException(response.code, response.message)
 
         return None
 
-    def get_option_chain(self, symbol, expiry, option_filter=None, **kwargs):
+    def get_option_chain(self, symbol, expiry, option_filter=None, return_greek_value=None, **kwargs):
         """
         query option chain with filter
         :param symbol: underlying stock symbol
         :param expiry: expiration date ( like '2021-06-18' or 1560484800000 )
         :param option_filter: option filter conditions, tigeropen.quote.domain.filter.OptionFilter
+        :param return_greek_value: return greek value or not, bool
         :param kwargs: optional. specify option_filter parameters directly without option_filer,
                         like: open_interest_min=100, delta_min=0.1
         :return: pandas.DataFrame，the columns are as follows：
             identifier: option identifier
             symbol: underlying stock symbol
             expiry: option expiration date. timestamp in millisecond, like 1560484800000
             strike: strike price
@@ -689,15 +690,15 @@
         else:
             param.expiry = expiry
         params.contracts = [param]
         if option_filter:
             params.option_filter = option_filter
         elif kwargs:
             params.option_filter = OptionFilter(**kwargs)
-
+        params.return_greek_value = return_greek_value
         params.lang = get_enum_value(self._lang)
         params.version = OPEN_API_SERVICE_VERSION_V3
         request = OpenApiRequest(OPTION_CHAIN, biz_model=params)
         response_content = self.__fetch_data(request)
         if response_content:
             response = OptionChainsResponse()
             response.parse_response_content(response_content)
```

### Comparing `tigeropen-3.1.9/tigeropen/quote/request/model.py` & `tigeropen-3.2.0/tigeropen/quote/request/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -786,14 +786,15 @@
 
 
 class OptionChainParams(BaseParams):
     def __init__(self):
         super(OptionChainParams, self).__init__()
         self._contracts = None
         self._option_filter = None
+        self._return_greek_value = None
 
     @property
     def contracts(self):
         return self._contracts
 
     @contracts.setter
     def contracts(self, value):
@@ -803,23 +804,33 @@
     def option_filter(self):
         return self._option_filter
 
     @option_filter.setter
     def option_filter(self, value):
         self._option_filter = value
 
+    @property
+    def return_greek_value(self):
+        return self._return_greek_value
+
+    @return_greek_value.setter
+    def return_greek_value(self, value):
+        self._return_greek_value = value
+
     def to_openapi_dict(self):
         params = super().to_openapi_dict()
         params.update({'option_basic': list()})
 
         if self.contracts:
             for contract in self.contracts:
                 params['option_basic'].append(contract.to_openapi_dict())
         if self.option_filter:
             params['option_filter'] = self.option_filter.to_dict()
+        if self.return_greek_value is not None:
+            params['return_greek_value'] = self.return_greek_value
         return params
 
 
 class TradingCalendarParams(BaseParams):
     def __init__(self):
         super().__init__()
         self._market = None
```

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/capital_distribution_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/capital_distribution_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/capital_flow_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/capital_flow_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/fund_contracts_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/fund_contracts_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/future_briefs_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/future_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/future_contract_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/future_contract_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/future_exchange_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/future_exchange_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/future_quote_bar_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/future_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/future_quote_ticks_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/future_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/future_trading_times_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/future_trading_times_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/kline_quota_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/kline_quota_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/market_scanner_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/market_scanner_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/market_status_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/market_status_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/option_briefs_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/option_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/option_chains_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/option_chains_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/option_expirations_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/option_expirations_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/option_quote_bar_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/option_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/option_quote_ticks_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/option_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/quote_bar_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/quote_brief_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/quote_brief_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/quote_dataframe_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/quote_dataframe_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/quote_delay_briefs_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/quote_delay_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/quote_depth_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/quote_depth_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/quote_grab_permission_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/quote_grab_permission_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/quote_hour_trading_timeline_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/quote_hour_trading_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/quote_ticks_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/quote_timeline_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/quote_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/stock_briefs_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/stock_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/stock_broker_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/stock_broker_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/stock_details_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/stock_details_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/stock_short_interest_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/stock_short_interest_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/stock_trade_meta_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/stock_trade_meta_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/symbol_names_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/symbol_names_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/symbols_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/symbols_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/trading_calendar_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/trading_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/warrant_briefs_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/warrant_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/quote/response/warrant_filter_response.py` & `tigeropen-3.2.0/tigeropen/quote/response/warrant_filter_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/tiger_open_client.py` & `tigeropen-3.2.0/tigeropen/tiger_open_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/tiger_open_config.py` & `tigeropen-3.2.0/tigeropen/tiger_open_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/domain/account.py` & `tigeropen-3.2.0/tigeropen/trade/domain/account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/domain/contract.py` & `tigeropen-3.2.0/tigeropen/trade/domain/contract.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/domain/order.py` & `tigeropen-3.2.0/tigeropen/trade/domain/order.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/domain/position.py` & `tigeropen-3.2.0/tigeropen/trade/domain/position.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/domain/prime_account.py` & `tigeropen-3.2.0/tigeropen/trade/domain/prime_account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/request/model.py` & `tigeropen-3.2.0/tigeropen/trade/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/response/__init__.py` & `tigeropen-3.2.0/tigeropen/trade/response/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/response/account_profile_response.py` & `tigeropen-3.2.0/tigeropen/trade/response/account_profile_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/response/analytics_asset_response.py` & `tigeropen-3.2.0/tigeropen/trade/response/analytics_asset_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/response/assets_response.py` & `tigeropen-3.2.0/tigeropen/trade/response/assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/response/contracts_response.py` & `tigeropen-3.2.0/tigeropen/trade/response/contracts_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/response/forex_order_response.py` & `tigeropen-3.2.0/tigeropen/trade/response/forex_order_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/response/order_id_response.py` & `tigeropen-3.2.0/tigeropen/trade/response/order_id_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/response/order_preview_response.py` & `tigeropen-3.2.0/tigeropen/trade/response/order_preview_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/response/orders_response.py` & `tigeropen-3.2.0/tigeropen/trade/response/orders_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/response/positions_response.py` & `tigeropen-3.2.0/tigeropen/trade/response/positions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/response/prime_assets_response.py` & `tigeropen-3.2.0/tigeropen/trade/response/prime_assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/response/segment_fund_response.py` & `tigeropen-3.2.0/tigeropen/trade/response/segment_fund_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/response/transactions_response.py` & `tigeropen-3.2.0/tigeropen/trade/response/transactions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-3.1.9/tigeropen/trade/trade_client.py` & `tigeropen-3.2.0/tigeropen/trade/trade_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,16 @@
         :param account:
         :return: AccountProfile 对象, 有如下属性：
             account： 交易账户
             capability： 账户类型(CASH:现金账户, MGRN: Reg T 保证金账户, PMGRN: 投资组合保证金)
             status： 账户状态(New, Funded, Open, Pending, Abandoned, Rejected, Closed, Unknown)
         """
         params = AccountsParams()
-        params.account = account if account else self._account
+        if account:
+            params.account = account
         params.lang = get_enum_value(self._lang)
         request = OpenApiRequest(ACCOUNTS, biz_model=params)
         response_content = self.__fetch_data(request)
         if response_content:
             response = ProfilesResponse()
             response.parse_response_content(response_content)
             if response.is_success():
```

### Comparing `tigeropen-3.1.9/tigeropen.egg-info/PKG-INFO` & `tigeropen-3.2.0/tigeropen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 3.1.9
+Version: 3.2.0
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-3.1.9/tigeropen.egg-info/SOURCES.txt` & `tigeropen-3.2.0/tigeropen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

