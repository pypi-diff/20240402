# Comparing `tmp/graas-observability-utility-1.5.2.tar.gz` & `tmp/graas-observability-utility-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graas-observability-utility-1.5.2.tar", last modified: Mon Apr  1 07:33:14 2024, max compression
+gzip compressed data, was "graas-observability-utility-1.5.3.tar", last modified: Tue Apr  2 06:35:16 2024, max compression
```

## Comparing `graas-observability-utility-1.5.2.tar` & `graas-observability-utility-1.5.3.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-01 07:33:14.006223 graas-observability-utility-1.5.2/
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       43 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/MANIFEST.in
--rw-r--r--   0 priyanka  (1003) priyanka  (1003)      856 2024-04-01 07:33:14.006223 graas-observability-utility-1.5.2/PKG-INFO
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      565 2023-11-02 10:15:21.000000 graas-observability-utility-1.5.2/README.md
-drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-01 07:33:13.978224 graas-observability-utility-1.5.2/graas_observability_utility.egg-info/
--rw-r--r--   0 priyanka  (1003) priyanka  (1003)      856 2024-04-01 07:33:13.000000 graas-observability-utility-1.5.2/graas_observability_utility.egg-info/PKG-INFO
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4595 2024-04-01 07:33:13.000000 graas-observability-utility-1.5.2/graas_observability_utility.egg-info/SOURCES.txt
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        1 2024-04-01 07:33:13.000000 graas-observability-utility-1.5.2/graas_observability_utility.egg-info/dependency_links.txt
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       11 2024-04-01 07:33:13.000000 graas-observability-utility-1.5.2/graas_observability_utility.egg-info/requires.txt
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       16 2024-04-01 07:33:13.000000 graas-observability-utility-1.5.2/graas_observability_utility.egg-info/top_level.txt
-drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-01 07:33:13.978224 graas-observability-utility-1.5.2/graas_utilities/
-drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-01 07:33:14.006223 graas-observability-utility-1.5.2/graas_utilities/Schema/
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4031 2024-03-31 17:37:11.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Product_Performance_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2438 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Sponsored_Brands_Attributed_Purchases_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5106 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Sponsored_Brands_Campaign_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5005 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Sponsored_Display_Advertised_Product_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3585 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Sponsored_Display_Campaign_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3548 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Sponsored_Products_Advertised_Product_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3482 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Sponsored_Products_Campaign_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1873 2024-03-31 17:16:07.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Store_Key_Metrics_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2962 2024-03-31 17:16:11.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Store_Key_Metrics_Hourly_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1561 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2631 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Flipkart_PLA_Campaign_Seller_Portal_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2226 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Flipkart_PLA_Consolidated_FSN_seller_Portal_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2188 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Flipkart_Search_Traffic_Report_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1488 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_Customers_Insight_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3619 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_Keywords_Onsite_daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5758 2024-03-31 17:34:03.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_Product_Performance_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1694 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_Product_Sponsored_Affiliate_Report_Daily_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5961 2024-03-31 17:21:42.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_Store_Key_Metrics_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     9612 2024-03-28 09:12:35.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_mkp_onsite_campaign_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3866 2024-01-08 08:41:17.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_offsite_campaign_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4668 2024-03-28 06:38:57.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_onsite_campaign_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3926 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Keywords_Onsite_daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3505 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Key_Metrics_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3208 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Trends_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1833 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_BundleDeal_Overview_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1229 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Bundle_Deal_Trends_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1628 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1251 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Trends_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2994 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Detailed_Overview_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1148 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Trends_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2001 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Voucher_Performance_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1095 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Voucher_Trends_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5890 2024-04-01 07:30:32.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Product_Overview_Daily_Monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     6341 2024-03-31 17:16:52.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Product_Overview_Hourly_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     6387 2024-04-01 07:33:01.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Product_Performance_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2479 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Store_Metrics_Paid_Orders_Daily_monthly_report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1429 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     8670 2024-03-31 17:14:17.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_mkp_onsite_campaign_daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5456 2024-03-28 06:39:02.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_onsite_campaign_daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3500 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_store_Metrics_Placed_Order_Hourly_Daily_report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1531 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2362 2024-03-31 17:13:34.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Tokopedia_Product_Overview_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3318 2024-03-31 17:39:27.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Tokopedia_Product_Performance_Daily_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4650 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Daily_monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4115 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Monthly_Report.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        0 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/__init__.py
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      577 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/amount_currency_code_object.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1785 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/graas_amazon_campaigns.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1301 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/graas_flipkart_campaigns.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1306 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_affiliate_report_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1794 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_deals_overview_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2318 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_deals_trends_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1294 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_offsite_campaigns.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1499 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_onsite_keywords.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2141 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_product_campaign_performance.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2700 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_shop_stats_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1554 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_shop_stats_hourly.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2454 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_traffic_overview_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1330 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_traffic_overview_hourly.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1851 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_voucher_performance_daily.json
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        0 2023-11-27 05:46:40.000000 graas-observability-utility-1.5.2/graas_utilities/__init__.py
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5651 2024-04-01 05:38:14.000000 graas-observability-utility-1.5.2/graas_utilities/configs.py
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      751 2024-03-26 06:37:57.000000 graas-observability-utility-1.5.2/graas_utilities/ref_Resolver.py
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3717 2024-04-01 05:39:58.000000 graas-observability-utility-1.5.2/graas_utilities/validation.py
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       38 2024-04-01 07:33:14.006223 graas-observability-utility-1.5.2/setup.cfg
--rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1307 2024-04-01 07:33:09.000000 graas-observability-utility-1.5.2/setup.py
+drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-02 06:35:16.757076 graas-observability-utility-1.5.3/
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       43 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/MANIFEST.in
+-rw-r--r--   0 priyanka  (1003) priyanka  (1003)      856 2024-04-02 06:35:16.757076 graas-observability-utility-1.5.3/PKG-INFO
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      565 2023-11-02 10:15:21.000000 graas-observability-utility-1.5.3/README.md
+drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-02 06:35:16.725082 graas-observability-utility-1.5.3/graas_observability_utility.egg-info/
+-rw-r--r--   0 priyanka  (1003) priyanka  (1003)      856 2024-04-02 06:35:16.000000 graas-observability-utility-1.5.3/graas_observability_utility.egg-info/PKG-INFO
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4595 2024-04-02 06:35:16.000000 graas-observability-utility-1.5.3/graas_observability_utility.egg-info/SOURCES.txt
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        1 2024-04-02 06:35:16.000000 graas-observability-utility-1.5.3/graas_observability_utility.egg-info/dependency_links.txt
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       11 2024-04-02 06:35:16.000000 graas-observability-utility-1.5.3/graas_observability_utility.egg-info/requires.txt
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       16 2024-04-02 06:35:16.000000 graas-observability-utility-1.5.3/graas_observability_utility.egg-info/top_level.txt
+drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-02 06:35:16.725082 graas-observability-utility-1.5.3/graas_utilities/
+drwxrwxr-x   0 priyanka  (1003) priyanka  (1003)        0 2024-04-02 06:35:16.753077 graas-observability-utility-1.5.3/graas_utilities/Schema/
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4031 2024-03-31 17:37:11.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Product_Performance_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2438 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Sponsored_Brands_Attributed_Purchases_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5106 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Sponsored_Brands_Campaign_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5005 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Sponsored_Display_Advertised_Product_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3585 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Sponsored_Display_Campaign_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3548 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Sponsored_Products_Advertised_Product_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3482 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Sponsored_Products_Campaign_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1873 2024-03-31 17:16:07.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Store_Key_Metrics_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2962 2024-03-31 17:16:11.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Store_Key_Metrics_Hourly_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1561 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2631 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Flipkart_PLA_Campaign_Seller_Portal_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2226 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Flipkart_PLA_Consolidated_FSN_seller_Portal_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2188 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Flipkart_Search_Traffic_Report_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1488 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_Customers_Insight_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3619 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_Keywords_Onsite_daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5758 2024-03-31 17:34:03.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_Product_Performance_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1694 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_Product_Sponsored_Affiliate_Report_Daily_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5961 2024-03-31 17:21:42.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_Store_Key_Metrics_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     9612 2024-03-28 09:12:35.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_mkp_onsite_campaign_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3866 2024-01-08 08:41:17.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_offsite_campaign_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4668 2024-03-28 06:38:57.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_onsite_campaign_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3926 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Keywords_Onsite_daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3505 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Key_Metrics_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3208 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Trends_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1833 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_BundleDeal_Overview_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1229 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Bundle_Deal_Trends_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1628 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1251 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Trends_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2994 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Detailed_Overview_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1148 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Trends_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2001 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Voucher_Performance_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1095 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Voucher_Trends_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5893 2024-04-02 06:34:52.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Product_Overview_Daily_Monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     6341 2024-03-31 17:16:52.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Product_Overview_Hourly_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     6387 2024-04-02 05:01:52.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Product_Performance_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2479 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Store_Metrics_Paid_Orders_Daily_monthly_report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1429 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     8670 2024-03-31 17:14:17.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_mkp_onsite_campaign_daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5456 2024-03-28 06:39:02.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_onsite_campaign_daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3500 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_store_Metrics_Placed_Order_Hourly_Daily_report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1531 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2362 2024-03-31 17:13:34.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Tokopedia_Product_Overview_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3318 2024-03-31 17:39:27.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Tokopedia_Product_Performance_Daily_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4650 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Daily_monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     4115 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Monthly_Report.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        0 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/__init__.py
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      577 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/amount_currency_code_object.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1785 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/graas_amazon_campaigns.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1301 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/graas_flipkart_campaigns.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1306 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_affiliate_report_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1794 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_deals_overview_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2318 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_deals_trends_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1294 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_offsite_campaigns.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1499 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_onsite_keywords.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2141 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_product_campaign_performance.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2700 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_shop_stats_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1554 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_shop_stats_hourly.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     2454 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_traffic_overview_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1330 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_traffic_overview_hourly.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1851 2023-12-24 13:53:23.000000 graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_voucher_performance_daily.json
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)        0 2023-11-27 05:46:40.000000 graas-observability-utility-1.5.3/graas_utilities/__init__.py
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     5651 2024-04-01 05:38:14.000000 graas-observability-utility-1.5.3/graas_utilities/configs.py
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)      751 2024-03-26 06:37:57.000000 graas-observability-utility-1.5.3/graas_utilities/ref_Resolver.py
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     3717 2024-04-01 05:39:58.000000 graas-observability-utility-1.5.3/graas_utilities/validation.py
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)       38 2024-04-02 06:35:16.757076 graas-observability-utility-1.5.3/setup.cfg
+-rw-rw-r--   0 priyanka  (1003) priyanka  (1003)     1307 2024-04-02 06:35:10.000000 graas-observability-utility-1.5.3/setup.py
```

### Comparing `graas-observability-utility-1.5.2/PKG-INFO` & `graas-observability-utility-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graas-observability-utility
-Version: 1.5.2
+Version: 1.5.3
 Summary: A small wrapper around data observability
 Home-page: https://bitbucket.org/shoptimizeanalytics/graas-observability-utility
 Author: Graas
 Author-email: priyanka.patel@graas.ai
 Keywords: utility
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `graas-observability-utility-1.5.2/README.md` & `graas-observability-utility-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_observability_utility.egg-info/PKG-INFO` & `graas-observability-utility-1.5.3/graas_observability_utility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graas-observability-utility
-Version: 1.5.2
+Version: 1.5.3
 Summary: A small wrapper around data observability
 Home-page: https://bitbucket.org/shoptimizeanalytics/graas-observability-utility
 Author: Graas
 Author-email: priyanka.patel@graas.ai
 Keywords: utility
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `graas-observability-utility-1.5.2/graas_observability_utility.egg-info/SOURCES.txt` & `graas-observability-utility-1.5.3/graas_observability_utility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Product_Performance_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Product_Performance_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Sponsored_Brands_Attributed_Purchases_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Sponsored_Brands_Attributed_Purchases_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Sponsored_Brands_Campaign_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Sponsored_Brands_Campaign_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Sponsored_Display_Advertised_Product_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Sponsored_Display_Advertised_Product_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Sponsored_Display_Campaign_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Sponsored_Display_Campaign_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Sponsored_Products_Advertised_Product_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Sponsored_Products_Advertised_Product_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Sponsored_Products_Campaign_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Sponsored_Products_Campaign_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Store_Key_Metrics_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Store_Key_Metrics_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Store_Key_Metrics_Hourly_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Store_Key_Metrics_Hourly_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Amazon_Traffic_Metrics_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Flipkart_PLA_Campaign_Seller_Portal_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Flipkart_PLA_Campaign_Seller_Portal_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Flipkart_PLA_Consolidated_FSN_seller_Portal_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Flipkart_PLA_Consolidated_FSN_seller_Portal_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Flipkart_Search_Traffic_Report_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Flipkart_Search_Traffic_Report_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_Customers_Insight_monthly_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_Customers_Insight_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_Keywords_Onsite_daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_Keywords_Onsite_daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_Product_Performance_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_Product_Performance_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_Product_Sponsored_Affiliate_Report_Daily_monthly_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_Product_Sponsored_Affiliate_Report_Daily_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_Store_Key_Metrics_monthly_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_Store_Key_Metrics_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_mkp_onsite_campaign_monthly_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_mkp_onsite_campaign_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_offsite_campaign_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_offsite_campaign_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Lazada_onsite_campaign_monthly_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Lazada_onsite_campaign_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Keywords_Onsite_daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Keywords_Onsite_daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Key_Metrics_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Key_Metrics_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Trends_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Add_On_Deal_Trends_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_BundleDeal_Overview_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_BundleDeal_Overview_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Bundle_Deal_Trends_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Bundle_Deal_Trends_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Trends_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Flash_Deals_Trends_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Detailed_Overview_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Detailed_Overview_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Trends_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Shipping_Fee_Promotion_Trends_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Voucher_Performance_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Voucher_Performance_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Marketing_Voucher_Trends_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Marketing_Voucher_Trends_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Product_Overview_Daily_Monthly_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Product_Overview_Daily_Monthly_Report.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999937996031746%*

 * *Differences: {"'properties'": "{'result': {'items': {'properties': {'Buyers_Paid_Order': {'type': 'integer'}, "*

 * *                 "'Units_Paid_Order': {'type': 'integer'}, 'Items_Paid': {'type': 'integer'}}}}}"}*

```diff
@@ -15,15 +15,15 @@
             "type": "string"
         },
         "result": {
             "items": {
                 "properties": {
                     "Buyers_Paid_Order": {
                         "description": "Number of buyers who paid for the order",
-                        "type": "string"
+                        "type": "integer"
                     },
                     "Buyers_Placed_Order": {
                         "description": "Total number of buyers who placed an order",
                         "type": "integer"
                     },
                     "Conversion_Rate_Add_to_Cart": {
                         "description": "Conversion rate from product view to adding to cart as a percentage",
@@ -41,15 +41,15 @@
                         "description": "Date of the report in the format 'MM-DD-YYYY'",
                         "format": "dd-MM-yyyy",
                         "pattern": "[0-9]{2}-[0-9]{2}-[1-2][0-9]{3}",
                         "type": "string"
                     },
                     "Items_Paid": {
                         "description": "Number of items paid for in the order",
-                        "type": "string"
+                        "type": "integer"
                     },
                     "Items_Placed": {
                         "description": "Total number of items placed in orders",
                         "type": "integer"
                     },
                     "Items_Visited": {
                         "description": "Total number of items visited",
@@ -121,15 +121,15 @@
                     },
                     "Units_Add_to_Cart": {
                         "description": "Total number of units added to the cart for the product",
                         "type": "integer"
                     },
                     "Units_Paid_Order": {
                         "description": "Number of units paid for in the order",
-                        "type": "string"
+                        "type": "integer"
                     },
                     "Units_Placed_Order": {
                         "description": "Total number of units placed in orders",
                         "type": "integer"
                     }
                 },
                 "required": [
```

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Product_Overview_Hourly_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Product_Overview_Hourly_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Product_Performance_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Product_Performance_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Store_Metrics_Paid_Orders_Daily_monthly_report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Store_Metrics_Paid_Orders_Daily_monthly_report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_Traffic_Overview_Daily_Monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_mkp_onsite_campaign_daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_mkp_onsite_campaign_daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_onsite_campaign_daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_onsite_campaign_daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Shopee_store_Metrics_Placed_Order_Hourly_Daily_report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Shopee_store_Metrics_Placed_Order_Hourly_Daily_report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Tokopedia_Customer_Insight_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Tokopedia_Product_Overview_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Tokopedia_Product_Overview_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Tokopedia_Product_Performance_Daily_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Tokopedia_Product_Performance_Daily_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Daily_monthly_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Daily_monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Monthly_Report.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/Tokopedia_Store_Key_Metrics_Monthly_Report.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/amount_currency_code_object.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/amount_currency_code_object.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/graas_amazon_campaigns.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/graas_amazon_campaigns.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/graas_flipkart_campaigns.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/graas_flipkart_campaigns.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_affiliate_report_daily.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_affiliate_report_daily.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_deals_overview_daily.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_deals_overview_daily.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_deals_trends_daily.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_deals_trends_daily.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_offsite_campaigns.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_offsite_campaigns.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_onsite_keywords.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_onsite_keywords.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_product_campaign_performance.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_product_campaign_performance.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_shop_stats_daily.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_shop_stats_daily.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_shop_stats_hourly.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_shop_stats_hourly.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_traffic_overview_daily.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_traffic_overview_daily.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_traffic_overview_hourly.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_traffic_overview_hourly.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/Schema/graas_mkp_voucher_performance_daily.json` & `graas-observability-utility-1.5.3/graas_utilities/Schema/graas_mkp_voucher_performance_daily.json`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/configs.py` & `graas-observability-utility-1.5.3/graas_utilities/configs.py`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/ref_Resolver.py` & `graas-observability-utility-1.5.3/graas_utilities/ref_Resolver.py`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/graas_utilities/validation.py` & `graas-observability-utility-1.5.3/graas_utilities/validation.py`

 * *Files identical despite different names*

### Comparing `graas-observability-utility-1.5.2/setup.py` & `graas-observability-utility-1.5.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 	'Programming Language :: Python :: 3.3', 
 	'Programming Language :: Python :: 3.4', 
 	'Programming Language :: Python :: 3.8', 
 	]
 
 # calling the setup function 
 setup(name='graas-observability-utility', 
-	version='1.5.2', 
+	version='1.5.3', 
 	description='A small wrapper around data observability', 
 	# long_description=long_description, 
 	url='https://bitbucket.org/shoptimizeanalytics/graas-observability-utility', 
 	author='Graas', 
 	author_email='priyanka.patel@graas.ai', 
 	# license='MIT',
     packages=find_packages(),
```

