# Comparing `tmp/mns-scheduler-1.0.1.6.tar.gz` & `tmp/mns-scheduler-1.0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.1.6.tar", last modified: Sat Mar 23 11:44:51 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.1.7.tar", last modified: Tue Apr  2 12:07:33 2024, max compression
```

## Comparing `mns-scheduler-1.0.1.6.tar` & `mns-scheduler-1.0.1.7.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.584140 mns-scheduler-1.0.1.6/
--rw-rw-rw-   0        0        0       62 2024-03-23 11:44:51.583143 mns-scheduler-1.0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.552226 mns-scheduler-1.0.1.6/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.6/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.555218 mns-scheduler-1.0.1.6/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.6/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2023-12-22 04:57:03.000000 mns-scheduler-1.0.1.6/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.556215 mns-scheduler-1.0.1.6/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15238 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.6/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20673 2024-01-13 06:13:31.000000 mns-scheduler-1.0.1.6/mns_scheduler/company_info/company_info_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.557212 mns-scheduler-1.0.1.6/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.558210 mns-scheduler-1.0.1.6/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     2440 2024-03-22 08:13:08.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.560204 mns-scheduler-1.0.1.6/mns_scheduler/concept/em/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/em/__init__.py
--rw-rw-rw-   0        0        0     4993 2023-12-22 05:01:59.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2023-12-22 05:01:59.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2335 2023-12-22 05:01:59.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.560204 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.561202 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/app/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.562199 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0    10290 2024-03-21 16:17:01.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.563197 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/symbol/__init__.py
--rw-rw-rw-   0        0        0     1928 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8263 2024-03-22 07:44:40.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.565191 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/web/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/web/__init__.py
--rw-rw-rw-   0        0        0     4996 2024-03-21 16:54:33.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-03-21 16:54:56.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.566188 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/wen_cai/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.567185 mns-scheduler-1.0.1.6/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-02-28 08:33:00.000000 mns-scheduler-1.0.1.6/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.568183 mns-scheduler-1.0.1.6/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.569180 mns-scheduler-1.0.1.6/mns_scheduler/ipo/
--rw-rw-rw-   0        0        0      163 2024-01-08 10:50:26.000000 mns-scheduler-1.0.1.6/mns_scheduler/ipo/__init__.py
--rw-rw-rw-   0        0        0      387 2024-01-08 10:59:33.000000 mns-scheduler-1.0.1.6/mns_scheduler/ipo/auto_ipo_buy_api.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.569180 mns-scheduler-1.0.1.6/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.571175 mns-scheduler-1.0.1.6/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-01-09 10:50:36.000000 mns-scheduler-1.0.1.6/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7028 2024-01-09 10:50:05.000000 mns-scheduler-1.0.1.6/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.572172 mns-scheduler-1.0.1.6/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5650 2024-01-02 01:13:30.000000 mns-scheduler-1.0.1.6/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.572172 mns-scheduler-1.0.1.6/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.573169 mns-scheduler-1.0.1.6/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.574167 mns-scheduler-1.0.1.6/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.6/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     7550 2024-01-13 04:24:42.000000 mns-scheduler-1.0.1.6/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.575164 mns-scheduler-1.0.1.6/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.6/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.6/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.576161 mns-scheduler-1.0.1.6/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.6/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0     3859 2024-01-13 06:26:06.000000 mns-scheduler-1.0.1.6/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.577159 mns-scheduler-1.0.1.6/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.6/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     8850 2024-02-28 02:05:19.000000 mns-scheduler-1.0.1.6/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.578156 mns-scheduler-1.0.1.6/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2023-12-17 03:50:52.000000 mns-scheduler-1.0.1.6/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.581148 mns-scheduler-1.0.1.6/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2023-12-17 13:29:39.000000 mns-scheduler-1.0.1.6/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17269 2024-03-09 09:58:27.000000 mns-scheduler-1.0.1.6/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-01-04 12:05:04.000000 mns-scheduler-1.0.1.6/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.6/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7490 2024-01-11 03:30:22.000000 mns-scheduler-1.0.1.6/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.582145 mns-scheduler-1.0.1.6/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.6/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    13443 2024-03-22 08:08:32.000000 mns-scheduler-1.0.1.6/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-03-23 03:12:05.000000 mns-scheduler-1.0.1.6/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:44:51.583143 mns-scheduler-1.0.1.6/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-03-23 11:44:51.000000 mns-scheduler-1.0.1.6/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2948 2024-03-23 11:44:51.000000 mns-scheduler-1.0.1.6/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 11:44:51.000000 mns-scheduler-1.0.1.6/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-03-23 11:44:51.000000 mns-scheduler-1.0.1.6/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-23 11:44:51.584140 mns-scheduler-1.0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-03-23 11:44:34.000000 mns-scheduler-1.0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.222881 mns-scheduler-1.0.1.7/
+-rw-rw-rw-   0        0        0       62 2024-04-02 12:07:33.221884 mns-scheduler-1.0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.189905 mns-scheduler-1.0.1.7/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.7/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.192896 mns-scheduler-1.0.1.7/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.7/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2023-12-22 04:57:03.000000 mns-scheduler-1.0.1.7/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.193894 mns-scheduler-1.0.1.7/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    15238 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.7/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20673 2024-03-26 12:36:46.000000 mns-scheduler-1.0.1.7/mns_scheduler/company_info/company_info_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.194891 mns-scheduler-1.0.1.7/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.195889 mns-scheduler-1.0.1.7/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     2440 2024-03-22 08:13:08.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.197884 mns-scheduler-1.0.1.7/mns_scheduler/concept/em/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/em/__init__.py
+-rw-rw-rw-   0        0        0     4993 2023-12-22 05:01:59.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2023-12-22 05:01:59.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2335 2023-12-22 05:01:59.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.198881 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.198881 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/app/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.199878 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0    10290 2024-03-21 16:17:01.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.201873 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/symbol/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/symbol/__init__.py
+-rw-rw-rw-   0        0        0     1928 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8263 2024-03-22 07:44:40.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.202870 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/web/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/web/__init__.py
+-rw-rw-rw-   0        0        0     4996 2024-03-21 16:54:33.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-03-21 16:54:56.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.203868 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/wen_cai/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.205925 mns-scheduler-1.0.1.7/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-02-28 08:33:00.000000 mns-scheduler-1.0.1.7/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.206924 mns-scheduler-1.0.1.7/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.207921 mns-scheduler-1.0.1.7/mns_scheduler/ipo/
+-rw-rw-rw-   0        0        0      163 2024-01-08 10:50:26.000000 mns-scheduler-1.0.1.7/mns_scheduler/ipo/__init__.py
+-rw-rw-rw-   0        0        0      387 2024-01-08 10:59:33.000000 mns-scheduler-1.0.1.7/mns_scheduler/ipo/auto_ipo_buy_api.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.207921 mns-scheduler-1.0.1.7/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.209916 mns-scheduler-1.0.1.7/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-01-09 10:50:36.000000 mns-scheduler-1.0.1.7/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7028 2024-01-09 10:50:05.000000 mns-scheduler-1.0.1.7/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.210913 mns-scheduler-1.0.1.7/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5654 2024-03-29 10:48:40.000000 mns-scheduler-1.0.1.7/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.210913 mns-scheduler-1.0.1.7/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.211911 mns-scheduler-1.0.1.7/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.211911 mns-scheduler-1.0.1.7/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.7/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     7591 2024-04-02 11:59:52.000000 mns-scheduler-1.0.1.7/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.212908 mns-scheduler-1.0.1.7/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.7/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.7/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.213905 mns-scheduler-1.0.1.7/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.7/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0     3859 2024-01-13 06:26:06.000000 mns-scheduler-1.0.1.7/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.214903 mns-scheduler-1.0.1.7/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.7/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     8850 2024-04-01 01:27:55.000000 mns-scheduler-1.0.1.7/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.215900 mns-scheduler-1.0.1.7/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2023-12-17 03:50:52.000000 mns-scheduler-1.0.1.7/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.219890 mns-scheduler-1.0.1.7/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2023-12-17 13:29:39.000000 mns-scheduler-1.0.1.7/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17269 2024-03-09 09:58:27.000000 mns-scheduler-1.0.1.7/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-01-04 12:05:04.000000 mns-scheduler-1.0.1.7/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2023-12-19 00:49:10.000000 mns-scheduler-1.0.1.7/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7490 2024-01-11 03:30:22.000000 mns-scheduler-1.0.1.7/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.220886 mns-scheduler-1.0.1.7/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.1.7/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    13443 2024-03-22 08:08:32.000000 mns-scheduler-1.0.1.7/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-03-23 03:12:05.000000 mns-scheduler-1.0.1.7/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:07:33.221884 mns-scheduler-1.0.1.7/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-04-02 12:07:33.000000 mns-scheduler-1.0.1.7/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2948 2024-04-02 12:07:33.000000 mns-scheduler-1.0.1.7/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 12:07:33.000000 mns-scheduler-1.0.1.7/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-02 12:07:33.000000 mns-scheduler-1.0.1.7/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 12:07:33.222881 mns-scheduler-1.0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-04-02 12:06:50.000000 mns-scheduler-1.0.1.7/setup.py
```

### Comparing `mns-scheduler-1.0.1.6/README.md` & `mns-scheduler-1.0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.1.7/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.1.7/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.1.7/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py` & `mns-scheduler-1.0.1.7/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/concept/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.1.7/mns_scheduler/concept/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/concept/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.1.7/mns_scheduler/concept/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/concept/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.1.7/mns_scheduler/concept/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py` & `mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py` & `mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.1.7/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.1.7/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.1.7/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.1.7/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.1.7/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.1.7/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.1.7/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         mongodb_util.create_index(db_name, [("symbol", 1), ("date", 1)])
         logger.info("创建索引成功:{}", db_name)
     except BaseException as e:
         logger.warning("创建索引异常:{}", e)
 
 
 if __name__ == '__main__':
-    sync_all_daily_data('daily', 'qfq', 'stock_qfq_daily', None, None)
-    sync_all_daily_data('weekly', 'qfq', 'stock_qfq_weekly', None, None)
+    # sync_all_daily_data('daily', 'qfq', 'stock_qfq_daily', None, None)
+    # sync_all_daily_data('weekly', 'qfq', 'stock_qfq_weekly', None, None)
     sync_all_daily_data('monthly', 'qfq', 'stock_qfq_monthly', None, None)
 
     # sync_all_daily_data('monthly', '1990-12-19', 'qfq', 'stock_qfq_monthly', None, None)
     # sync_all_daily_data('daily', '1990-12-19', 'qfq', 'stock_qfq_daily', '2023-10-31', None)
     # sync_all_daily_data('weekly', '1990-12-19', 'qfq', 'stock_qfq_weekly', '2023-10-15', None)
     # sync_all_daily_data('monthly', '1990-12-19', 'qfq', 'stock_qfq_monthly', '2023-09-30', None)
```

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.1.7/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,15 @@
     now_date = datetime.now()
     str_day = now_date.strftime('%Y-%m-%d')
     str_now_date = now_date.strftime('%Y-%m-%d %H:%M:%S')
     new_data_df['create_day'] = str_day
     new_data_df['create_time'] = str_now_date
     new_data_df.loc[:, "create_day"] = str_day
     new_data_df.loc[:, "create_time"] = str_now_date
+    new_data_df.loc[:, "valid"] = False
     new_data_df = new_data_df[["_id",
                                "plate_code",
                                "plate_name",
                                "heat_score",
                                "index_class",
                                "sync_str_day",
                                "sync_str_time",
```

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.1.7/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.1.7/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.1.7/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.1.7/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.1.7/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.1.7/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.1.7/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.1.7/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.1.7/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.1.7/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.1.7/mns_scheduler/zz_task/data_sync_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.1.7/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.1.6/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.1.7/mns_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

