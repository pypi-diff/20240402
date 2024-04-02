# Comparing `tmp/roc_dingo-1.4.0.tar.gz` & `tmp/roc_dingo-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roc_dingo-1.4.0.tar", max compression
+gzip compressed data, was "roc_dingo-1.4.1.tar", max compression
```

## Comparing `roc_dingo-1.4.0.tar` & `roc_dingo-1.4.1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rwxr-xr-x   0        0        0    21863 2024-03-29 14:56:15.046382 roc_dingo-1.4.0/LICENSE
--rw-r--r--   0        0        0     2173 2024-03-29 14:56:15.046382 roc_dingo-1.4.0/README.md
--rw-r--r--   0        0        0     1203 2024-03-29 14:56:15.050382 roc_dingo-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      113 2024-03-29 14:56:15.050382 roc_dingo-1.4.0/roc/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 14:56:15.170387 roc_dingo-1.4.0/roc/dingo/__init__.py
--rw-r--r--   0        0        0    28270 2024-03-29 14:56:15.050382 roc_dingo-1.4.0/roc/dingo/commands.py
--rw-r--r--   0        0        0    13629 2024-03-29 14:56:15.054382 roc_dingo-1.4.0/roc/dingo/constants.py
--rw-r--r--   0        0        0     7319 2024-03-29 14:56:15.054382 roc_dingo-1.4.0/roc/dingo/descriptor.json
--rw-r--r--   0        0        0      945 2024-03-29 14:56:15.054382 roc_dingo-1.4.0/roc/dingo/exceptions.py
--rw-r--r--   0        0        0      682 2024-03-29 14:56:15.054382 roc_dingo-1.4.0/roc/dingo/models/__init__.py
--rw-r--r--   0        0        0    11964 2024-03-29 14:56:15.054382 roc_dingo-1.4.0/roc/dingo/models/data.py
--rw-r--r--   0        0        0     6109 2024-03-29 14:56:15.054382 roc_dingo-1.4.0/roc/dingo/models/file.py
--rw-r--r--   0        0        0     6989 2024-03-29 14:56:15.054382 roc_dingo-1.4.0/roc/dingo/models/packet.py
--rw-r--r--   0        0        0      747 2024-03-29 14:56:15.054382 roc_dingo-1.4.0/roc/dingo/models/versions/README.rst
--rw-r--r--   0        0        0      265 2024-03-29 14:56:15.054382 roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0025_create_view_anomalies_per_day.sql
--rw-r--r--   0        0        0      118 2024-03-29 14:56:15.054382 roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0025_create_view_total_events.sql
--rw-r--r--   0        0        0     6079 2024-03-29 14:56:15.054382 roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0025_insert_into_anomalies.sql
--rw-r--r--   0        0        0      342 2024-03-29 14:56:15.054382 roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0026_create_view_anomalies_per_day.sql
--rw-r--r--   0        0        0      695 2024-03-29 14:56:15.054382 roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0026_create_view_rpw_events_per_day.sql
--rw-r--r--   0        0        0    27905 2024-03-29 14:56:15.054382 roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0026_insert_into_events.sql
--rw-r--r--   0        0        0      693 2024-03-29 14:56:15.054382 roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0027_modifiy_view_rpw_events_per_day.sql
--rw-r--r--   0        0        0      396 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0028__downgrade.sql
--rw-r--r--   0        0        0      478 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0028__upgrade.sql
--rw-r--r--   0        0        0     2018 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0029__downgrade.sql
--rw-r--r--   0        0        0     2940 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0029__upgrade.sql
--rw-r--r--   0        0        0     5825 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0001_initial_.py
--rw-r--r--   0        0        0     8958 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0004_modify_file_log.py
--rw-r--r--   0        0        0      823 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0005_rename_column_type_to_level.py
--rw-r--r--   0        0        0     1208 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0006_add_is_removed_.py
--rw-r--r--   0        0        0     1014 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0007_add_error_log_.py
--rw-r--r--   0        0        0      728 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0008_remove_date_.py
--rw-r--r--   0        0        0      610 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0009_add_bia_.py
--rw-r--r--   0        0        0     1567 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0010_add_view_.py
--rw-r--r--   0        0        0     3355 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0011_update_packet_.py
--rw-r--r--   0        0        0     5719 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0012_add_data_.py
--rw-r--r--   0        0        0      957 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0013_fix_db_.py
--rw-r--r--   0        0        0     1555 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0014_add_solohk_.py
--rw-r--r--   0        0        0     1525 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0015_add_processqueue_.py
--rw-r--r--   0        0        0     4015 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0016_add_kcoeffbiacur.py
--rw-r--r--   0        0        0     1526 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0017_add_efecsevents_.py
--rw-r--r--   0        0        0     1698 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0018a_task_delivered.py
--rw-r--r--   0        0        0     1101 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0018b_add_product_to_file_log.py
--rw-r--r--   0        0        0     6781 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0019_modify_views_per_date.py
--rw-r--r--   0        0        0     2786 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0020_rm_biacurrtablehfr_.py
--rw-r--r--   0        0        0     1134 2024-03-29 14:56:15.058382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0021_add_retrieved_time_.py
--rw-r--r--   0        0        0     1732 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0022_add_to_update_flag_to_filelog_.py
--rw-r--r--   0        0        0     1629 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0023_add_hfrtimelog_.py
--rw-r--r--   0        0        0     1750 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0024_add_invalidpacketlog_.py
--rw-r--r--   0        0        0     2043 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0025_add_anomalies.py
--rw-r--r--   0        0        0     3640 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0026_add_table_events.py
--rw-r--r--   0        0        0      988 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0027_modify_view_rpw_events_per_day_.py
--rw-r--r--   0        0        0     2586 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0028_modify_sbm_log_status_retrieved_.py
--rw-r--r--   0        0        0     2501 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0029_tm_log_partitioning_.py
--rw-r--r--   0        0        0     1227 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0030_add_packet_acq_time_.py
--rw-r--r--   0        0        0      937 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/tasks/__init__.py
--rw-r--r--   0        0        0     6755 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/tasks/check_file_in_db.py
--rw-r--r--   0        0        0     7225 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/tasks/check_soar.py
--rw-r--r--   0        0        0     4898 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/tasks/clear.py
--rw-r--r--   0        0        0    11043 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/tasks/db_to_solohk.py
--rw-r--r--   0        0        0     8653 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/tasks/efecs_to_db.py
--rw-r--r--   0        0        0    35119 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/tasks/event_to_db.py
--rw-r--r--   0        0        0     5800 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/tasks/export.py
--rw-r--r--   0        0        0     4177 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/tasks/file_handler.py
--rw-r--r--   0        0        0    34078 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/tasks/l0_to_db.py
--rw-r--r--   0        0        0    23467 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/tasks/l0_to_hfrtimelog.py
--rw-r--r--   0        0        0    27739 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/tasks/log_file_to_db.py
--rw-r--r--   0        0        0     6857 2024-03-29 14:56:15.062382 roc_dingo-1.4.0/roc/dingo/tasks/parse_file_tree.py
--rw-r--r--   0        0        0     4480 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tasks/search_for_update.py
--rw-r--r--   0        0        0     3730 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tasks/search_missing_parents_files.py
--rw-r--r--   0        0        0    12897 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tasks/solohk_to_db.py
--rw-r--r--   0        0        0     5520 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tasks/store_delivered.py
--rw-r--r--   0        0        0    10615 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tasks/store_public_filename.py
--rw-r--r--   0        0        0     6190 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tasks/update_parents_in_db.py
--rw-r--r--   0        0        0    11328 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tasks/update_sbm_log_retrieved.py
--rw-r--r--   0        0        0     5385 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tasks/update_utc_time.py
--rw-r--r--   0        0        0        0 2024-03-29 14:56:15.174387 roc_dingo-1.4.0/roc/dingo/templates/__init__.py
--rw-r--r--   0        0        0      386 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/templates/solo_hk_xml.tpl
--rw-r--r--   0        0        0        0 2024-03-29 14:56:15.174387 roc_dingo-1.4.0/roc/dingo/tests/__init__.py
--rw-r--r--   0        0        0     5076 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_data_files_2020_08.dat
--rw-r--r--   0        0        0     2496 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_data_files_2020_08_19.dat
--rw-r--r--   0        0        0     5220 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_data_files_all.dat
--rw-r--r--   0        0        0    59454 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_data_files_all_dump.yml
--rw-r--r--   0        0        0     1005 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_data_files_missing_parents.dat
--rw-r--r--   0        0        0     6856 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_data_files_public_filename.dat
--rw-r--r--   0        0        0      930 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_data_files_warning_state.dat
--rw-r--r--   0        0        0       81 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_data_old_removed_file.dat
--rw-r--r--   0        0        0      411 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_dir_list_2020_08.dat
--rw-r--r--   0        0        0      101 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_dir_list_2020_08_18.dat
--rw-r--r--   0        0        0      101 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_dir_list_2020_08_19.dat
--rw-r--r--   0        0        0      248 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_dir_list_all.dat
--rw-r--r--   0        0        0      306 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_sk_files_1.dat
--rw-r--r--   0        0        0     3656 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_sk_files_1_dump.yml
--rw-r--r--   0        0        0      362 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_sk_files_2.dat
--rw-r--r--   0        0        0        0 2024-03-29 14:56:15.174387 roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/__init__.py
--rw-r--r--   0        0        0    17669 2024-03-29 14:56:15.066383 roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_check_file_in_db.py
--rw-r--r--   0        0        0    10685 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_parse_file_tree.py
--rw-r--r--   0        0        0     5207 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_search_missing_parents_files.py
--rw-r--r--   0        0        0     3711 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_store_archived.py
--rw-r--r--   0        0        0     3359 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_store_delivered.py
--rw-r--r--   0        0        0     3175 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_store_public_filename.py
--rw-r--r--   0        0        0     7632 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_to_db.py
--rw-r--r--   0        0        0     6714 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_to_update_files.py
--rw-r--r--   0        0        0      122 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_solohk_to_db.py
--rw-r--r--   0        0        0        0 2024-03-29 14:56:15.174387 roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/__init__.py
--rw-r--r--   0        0        0     2680 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_check_soar.py
--rw-r--r--   0        0        0     4025 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_efecs_to_db.py
--rw-r--r--   0        0        0        0 2024-03-29 14:56:15.174387 roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_event_to_db.py
--rw-r--r--   0        0        0     7773 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_l0_to_db.py
--rw-r--r--   0        0        0     4242 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_l0_to_hfrtimelog.py
--rw-r--r--   0        0        0     5844 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_logfile_to_rocdb.py
--rw-r--r--   0        0        0     4193 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_logfile_update.py
--rw-r--r--   0        0        0     4708 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_store_delivered.py
--rw-r--r--   0        0        0    10011 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_update_sbm_log_retrieved.py
--rw-r--r--   0        0        0     9919 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test_dingo.py
--rw-r--r--   0        0        0     4124 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tests/test_log_file.py
--rw-r--r--   0        0        0    22296 2024-03-29 14:56:15.070383 roc_dingo-1.4.0/roc/dingo/tools.py
--rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 roc_dingo-1.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0    21863 2024-03-29 14:56:15.046382 roc_dingo-1.4.1/LICENSE
+-rw-r--r--   0        0        0     2173 2024-03-29 14:56:15.046382 roc_dingo-1.4.1/README.md
+-rw-r--r--   0        0        0     1202 2024-04-02 13:39:49.236694 roc_dingo-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      113 2024-03-29 14:56:15.050382 roc_dingo-1.4.1/roc/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:39:49.368700 roc_dingo-1.4.1/roc/dingo/__init__.py
+-rw-r--r--   0        0        0    28270 2024-03-29 14:56:15.050382 roc_dingo-1.4.1/roc/dingo/commands.py
+-rw-r--r--   0        0        0    13629 2024-03-29 14:56:15.054382 roc_dingo-1.4.1/roc/dingo/constants.py
+-rw-r--r--   0        0        0     7317 2024-04-02 13:39:49.236694 roc_dingo-1.4.1/roc/dingo/descriptor.json
+-rw-r--r--   0        0        0      945 2024-03-29 14:56:15.054382 roc_dingo-1.4.1/roc/dingo/exceptions.py
+-rw-r--r--   0        0        0      682 2024-03-29 14:56:15.054382 roc_dingo-1.4.1/roc/dingo/models/__init__.py
+-rw-r--r--   0        0        0    11964 2024-03-29 14:56:15.054382 roc_dingo-1.4.1/roc/dingo/models/data.py
+-rw-r--r--   0        0        0     6109 2024-03-29 14:56:15.054382 roc_dingo-1.4.1/roc/dingo/models/file.py
+-rw-r--r--   0        0        0     6989 2024-03-29 14:56:15.054382 roc_dingo-1.4.1/roc/dingo/models/packet.py
+-rw-r--r--   0        0        0      747 2024-03-29 14:56:15.054382 roc_dingo-1.4.1/roc/dingo/models/versions/README.rst
+-rw-r--r--   0        0        0      265 2024-03-29 14:56:15.054382 roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0025_create_view_anomalies_per_day.sql
+-rw-r--r--   0        0        0      118 2024-03-29 14:56:15.054382 roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0025_create_view_total_events.sql
+-rw-r--r--   0        0        0     6079 2024-03-29 14:56:15.054382 roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0025_insert_into_anomalies.sql
+-rw-r--r--   0        0        0      342 2024-03-29 14:56:15.054382 roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0026_create_view_anomalies_per_day.sql
+-rw-r--r--   0        0        0      695 2024-03-29 14:56:15.054382 roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0026_create_view_rpw_events_per_day.sql
+-rw-r--r--   0        0        0    27905 2024-03-29 14:56:15.054382 roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0026_insert_into_events.sql
+-rw-r--r--   0        0        0      693 2024-03-29 14:56:15.054382 roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0027_modifiy_view_rpw_events_per_day.sql
+-rw-r--r--   0        0        0      396 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0028__downgrade.sql
+-rw-r--r--   0        0        0      478 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0028__upgrade.sql
+-rw-r--r--   0        0        0     2018 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0029__downgrade.sql
+-rw-r--r--   0        0        0     2940 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0029__upgrade.sql
+-rw-r--r--   0        0        0     5825 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0001_initial_.py
+-rw-r--r--   0        0        0     8958 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0004_modify_file_log.py
+-rw-r--r--   0        0        0      823 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0005_rename_column_type_to_level.py
+-rw-r--r--   0        0        0     1208 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0006_add_is_removed_.py
+-rw-r--r--   0        0        0     1014 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0007_add_error_log_.py
+-rw-r--r--   0        0        0      728 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0008_remove_date_.py
+-rw-r--r--   0        0        0      610 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0009_add_bia_.py
+-rw-r--r--   0        0        0     1567 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0010_add_view_.py
+-rw-r--r--   0        0        0     3355 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0011_update_packet_.py
+-rw-r--r--   0        0        0     5719 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0012_add_data_.py
+-rw-r--r--   0        0        0      957 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0013_fix_db_.py
+-rw-r--r--   0        0        0     1555 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0014_add_solohk_.py
+-rw-r--r--   0        0        0     1525 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0015_add_processqueue_.py
+-rw-r--r--   0        0        0     4015 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0016_add_kcoeffbiacur.py
+-rw-r--r--   0        0        0     1526 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0017_add_efecsevents_.py
+-rw-r--r--   0        0        0     1698 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0018a_task_delivered.py
+-rw-r--r--   0        0        0     1101 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0018b_add_product_to_file_log.py
+-rw-r--r--   0        0        0     6781 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0019_modify_views_per_date.py
+-rw-r--r--   0        0        0     2786 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0020_rm_biacurrtablehfr_.py
+-rw-r--r--   0        0        0     1134 2024-03-29 14:56:15.058382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0021_add_retrieved_time_.py
+-rw-r--r--   0        0        0     1732 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0022_add_to_update_flag_to_filelog_.py
+-rw-r--r--   0        0        0     1629 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0023_add_hfrtimelog_.py
+-rw-r--r--   0        0        0     1750 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0024_add_invalidpacketlog_.py
+-rw-r--r--   0        0        0     2043 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0025_add_anomalies.py
+-rw-r--r--   0        0        0     3640 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0026_add_table_events.py
+-rw-r--r--   0        0        0      988 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0027_modify_view_rpw_events_per_day_.py
+-rw-r--r--   0        0        0     2586 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0028_modify_sbm_log_status_retrieved_.py
+-rw-r--r--   0        0        0     2501 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0029_tm_log_partitioning_.py
+-rw-r--r--   0        0        0     1227 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0030_add_packet_acq_time_.py
+-rw-r--r--   0        0        0      937 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/tasks/__init__.py
+-rw-r--r--   0        0        0     6755 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/tasks/check_file_in_db.py
+-rw-r--r--   0        0        0     7225 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/tasks/check_soar.py
+-rw-r--r--   0        0        0     4898 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/tasks/clear.py
+-rw-r--r--   0        0        0    11043 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/tasks/db_to_solohk.py
+-rw-r--r--   0        0        0     8653 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/tasks/efecs_to_db.py
+-rw-r--r--   0        0        0    35119 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/tasks/event_to_db.py
+-rw-r--r--   0        0        0     5800 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/tasks/export.py
+-rw-r--r--   0        0        0     4177 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/tasks/file_handler.py
+-rw-r--r--   0        0        0    34078 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/tasks/l0_to_db.py
+-rw-r--r--   0        0        0    23467 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/tasks/l0_to_hfrtimelog.py
+-rw-r--r--   0        0        0    27739 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/tasks/log_file_to_db.py
+-rw-r--r--   0        0        0     6857 2024-03-29 14:56:15.062382 roc_dingo-1.4.1/roc/dingo/tasks/parse_file_tree.py
+-rw-r--r--   0        0        0     4480 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tasks/search_for_update.py
+-rw-r--r--   0        0        0     3730 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tasks/search_missing_parents_files.py
+-rw-r--r--   0        0        0    12897 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tasks/solohk_to_db.py
+-rw-r--r--   0        0        0     5520 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tasks/store_delivered.py
+-rw-r--r--   0        0        0    10615 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tasks/store_public_filename.py
+-rw-r--r--   0        0        0     6190 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tasks/update_parents_in_db.py
+-rw-r--r--   0        0        0    11520 2024-04-02 13:39:49.236694 roc_dingo-1.4.1/roc/dingo/tasks/update_sbm_log_retrieved.py
+-rw-r--r--   0        0        0     5385 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tasks/update_utc_time.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:39:49.380700 roc_dingo-1.4.1/roc/dingo/templates/__init__.py
+-rw-r--r--   0        0        0      386 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/templates/solo_hk_xml.tpl
+-rw-r--r--   0        0        0        0 2024-04-02 13:39:49.380700 roc_dingo-1.4.1/roc/dingo/tests/__init__.py
+-rw-r--r--   0        0        0     5076 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_data_files_2020_08.dat
+-rw-r--r--   0        0        0     2496 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_data_files_2020_08_19.dat
+-rw-r--r--   0        0        0     5220 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_data_files_all.dat
+-rw-r--r--   0        0        0    59454 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_data_files_all_dump.yml
+-rw-r--r--   0        0        0     1005 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_data_files_missing_parents.dat
+-rw-r--r--   0        0        0     6856 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_data_files_public_filename.dat
+-rw-r--r--   0        0        0      930 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_data_files_warning_state.dat
+-rw-r--r--   0        0        0       81 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_data_old_removed_file.dat
+-rw-r--r--   0        0        0      411 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_dir_list_2020_08.dat
+-rw-r--r--   0        0        0      101 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_dir_list_2020_08_18.dat
+-rw-r--r--   0        0        0      101 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_dir_list_2020_08_19.dat
+-rw-r--r--   0        0        0      248 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_dir_list_all.dat
+-rw-r--r--   0        0        0      306 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_sk_files_1.dat
+-rw-r--r--   0        0        0     3670 2024-04-02 13:39:49.240694 roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_sk_files_1_dump.yml
+-rw-r--r--   0        0        0      362 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_sk_files_2.dat
+-rw-r--r--   0        0        0        0 2024-04-02 13:39:49.384700 roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/__init__.py
+-rw-r--r--   0        0        0    17669 2024-03-29 14:56:15.066383 roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_check_file_in_db.py
+-rw-r--r--   0        0        0    10685 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_parse_file_tree.py
+-rw-r--r--   0        0        0     5207 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_search_missing_parents_files.py
+-rw-r--r--   0        0        0     3711 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_store_archived.py
+-rw-r--r--   0        0        0     3359 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_store_delivered.py
+-rw-r--r--   0        0        0     3175 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_store_public_filename.py
+-rw-r--r--   0        0        0     7632 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_to_db.py
+-rw-r--r--   0        0        0     6714 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_to_update_files.py
+-rw-r--r--   0        0        0      122 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_solohk_to_db.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:39:49.384700 roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/__init__.py
+-rw-r--r--   0        0        0     2680 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_check_soar.py
+-rw-r--r--   0        0        0     4025 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_efecs_to_db.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:39:49.384700 roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_event_to_db.py
+-rw-r--r--   0        0        0     7773 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_l0_to_db.py
+-rw-r--r--   0        0        0     4242 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_l0_to_hfrtimelog.py
+-rw-r--r--   0        0        0     5844 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_logfile_to_rocdb.py
+-rw-r--r--   0        0        0     4193 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_logfile_update.py
+-rw-r--r--   0        0        0     4708 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_store_delivered.py
+-rw-r--r--   0        0        0    10011 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_update_sbm_log_retrieved.py
+-rw-r--r--   0        0        0     9919 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test_dingo.py
+-rw-r--r--   0        0        0     4124 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tests/test_log_file.py
+-rw-r--r--   0        0        0    22296 2024-03-29 14:56:15.070383 roc_dingo-1.4.1/roc/dingo/tools.py
+-rw-r--r--   0        0        0     3382 1970-01-01 00:00:00.000000 roc_dingo-1.4.1/PKG-INFO
```

### Comparing `roc_dingo-1.4.0/LICENSE` & `roc_dingo-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/README.md` & `roc_dingo-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/pyproject.toml` & `roc_dingo-1.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [build-system]
-requires = ["setuptools==54", "wheel", "poetry==1.1.8", "poetry-core==1.0.4"]
+requires = ["setuptools<60", "wheel", "poetry", "poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 skip-string-normalization = true
 line-length = 79
 include = "\\.pyi?$"
 exclude = "/(\n    \\.git\n  | \\.hg\n  | \\.mypy_cache\n  | \\.tox\n  | \\.venv\n  | _build\n  | buck-out\n  | build\n  | dist\n)/\n"
 
 [tool.poetry]
 name = "roc-dingo"
-version = "1.4.0"
+version = "1.4.1"
 readme = "README.md"
 license = "CeCILL-C"
 repository = "https://gitlab.obspm.fr/ROC/Pipelines/Plugins/DINGO"
 description = "Data INgestOr (DINGO) plugin is used to ingest data into the ROC pipeline database"
 authors = [ "ROC Team <roc.support@sympa.obspm.fr>"]
 exclude = [ "bump_descriptor.py",]
 [[tool.poetry.packages]]
 include = "roc"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 numpy = "!=1.19.5"
 astropy = '^5.2'
 pandas = "^1.1.3"
+h5py = "^3.7"
 spacepy = ">=0.5,<1.0"
 xmltodict = ">=0.12,<1.0"
 spice_manager = {version ="^1.1.0"}
 "poppy-core" =  {version = ">=0.9.4"}
 "poppy-pop" = {version = ">=0.7.5"}
 "roc-idb" = {version = "^1.0"}
 "roc-rpl" = {version = "^1.0"}
```

### Comparing `roc_dingo-1.4.0/roc/dingo/commands.py` & `roc_dingo-1.4.1/roc/dingo/commands.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/constants.py` & `roc_dingo-1.4.1/roc/dingo/constants.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/descriptor.json` & `roc_dingo-1.4.1/roc/dingo/descriptor.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'release'": "{'version': '1.4.1', 'date': '2024-04-02', 'modification': 'Hotfix in "*

 * *              "update_sbm_retrieved task'}"}*

```diff
@@ -4,19 +4,19 @@
         "identifier": "roc.dingo",
         "name": "Data Ingestor",
         "project": "RODP"
     },
     "release": {
         "author": "ROC Team <roc.support@sympa.obspm.fr>",
         "contact": "roc.support@sympa.obspm.fr",
-        "date": "2024-03-28",
+        "date": "2024-04-02",
         "institute": "LESIA",
-        "modification": "Update db model and add tasks for sbm",
+        "modification": "Hotfix in update_sbm_retrieved task",
         "url": "https://gitlab.obspm.fr/ROC/Pipelines/Plugins/DINGO",
-        "version": "1.4.0"
+        "version": "1.4.1"
     },
     "tasks": [
         {
             "category": "Database handling",
             "description": "Clear content of ROC database.",
             "inputs": {},
             "name": "clear_rocdb",
```

### Comparing `roc_dingo-1.4.0/roc/dingo/exceptions.py` & `roc_dingo-1.4.1/roc/dingo/exceptions.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/__init__.py` & `roc_dingo-1.4.1/roc/dingo/models/__init__.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/data.py` & `roc_dingo-1.4.1/roc/dingo/models/data.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/file.py` & `roc_dingo-1.4.1/roc/dingo/models/file.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/packet.py` & `roc_dingo-1.4.1/roc/dingo/models/packet.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/README.rst` & `roc_dingo-1.4.1/roc/dingo/models/versions/README.rst`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0025_insert_into_anomalies.sql` & `roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0025_insert_into_anomalies.sql`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0026_create_view_rpw_events_per_day.sql` & `roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0026_create_view_rpw_events_per_day.sql`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0026_insert_into_events.sql` & `roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0026_insert_into_events.sql`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0027_modifiy_view_rpw_events_per_day.sql` & `roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0027_modifiy_view_rpw_events_per_day.sql`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0029__downgrade.sql` & `roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0029__downgrade.sql`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/SQL/roc_dingo_0029__upgrade.sql` & `roc_dingo-1.4.1/roc/dingo/models/versions/SQL/roc_dingo_0029__upgrade.sql`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0001_initial_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0001_initial_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0004_modify_file_log.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0004_modify_file_log.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0005_rename_column_type_to_level.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0005_rename_column_type_to_level.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0006_add_is_removed_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0006_add_is_removed_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0007_add_error_log_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0007_add_error_log_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0008_remove_date_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0008_remove_date_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0009_add_bia_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0009_add_bia_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0010_add_view_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0010_add_view_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0011_update_packet_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0011_update_packet_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0012_add_data_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0012_add_data_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0013_fix_db_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0013_fix_db_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0014_add_solohk_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0014_add_solohk_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0015_add_processqueue_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0015_add_processqueue_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0016_add_kcoeffbiacur.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0016_add_kcoeffbiacur.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0017_add_efecsevents_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0017_add_efecsevents_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0018a_task_delivered.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0018a_task_delivered.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0018b_add_product_to_file_log.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0018b_add_product_to_file_log.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0019_modify_views_per_date.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0019_modify_views_per_date.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0020_rm_biacurrtablehfr_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0020_rm_biacurrtablehfr_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0021_add_retrieved_time_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0021_add_retrieved_time_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0022_add_to_update_flag_to_filelog_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0022_add_to_update_flag_to_filelog_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0023_add_hfrtimelog_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0023_add_hfrtimelog_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0024_add_invalidpacketlog_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0024_add_invalidpacketlog_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0025_add_anomalies.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0025_add_anomalies.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0026_add_table_events.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0026_add_table_events.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0027_modify_view_rpw_events_per_day_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0027_modify_view_rpw_events_per_day_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0028_modify_sbm_log_status_retrieved_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0028_modify_sbm_log_status_retrieved_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0029_tm_log_partitioning_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0029_tm_log_partitioning_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/models/versions/roc_dingo_0030_add_packet_acq_time_.py` & `roc_dingo-1.4.1/roc/dingo/models/versions/roc_dingo_0030_add_packet_acq_time_.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/__init__.py` & `roc_dingo-1.4.1/roc/dingo/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/check_file_in_db.py` & `roc_dingo-1.4.1/roc/dingo/tasks/check_file_in_db.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/check_soar.py` & `roc_dingo-1.4.1/roc/dingo/tasks/check_soar.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/clear.py` & `roc_dingo-1.4.1/roc/dingo/tasks/clear.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/db_to_solohk.py` & `roc_dingo-1.4.1/roc/dingo/tasks/db_to_solohk.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/efecs_to_db.py` & `roc_dingo-1.4.1/roc/dingo/tasks/efecs_to_db.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/event_to_db.py` & `roc_dingo-1.4.1/roc/dingo/tasks/event_to_db.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/export.py` & `roc_dingo-1.4.1/roc/dingo/tasks/export.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/file_handler.py` & `roc_dingo-1.4.1/roc/dingo/tasks/file_handler.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/l0_to_db.py` & `roc_dingo-1.4.1/roc/dingo/tasks/l0_to_db.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/l0_to_hfrtimelog.py` & `roc_dingo-1.4.1/roc/dingo/tasks/l0_to_hfrtimelog.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/log_file_to_db.py` & `roc_dingo-1.4.1/roc/dingo/tasks/log_file_to_db.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/parse_file_tree.py` & `roc_dingo-1.4.1/roc/dingo/tasks/parse_file_tree.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/search_for_update.py` & `roc_dingo-1.4.1/roc/dingo/tasks/search_for_update.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/search_missing_parents_files.py` & `roc_dingo-1.4.1/roc/dingo/tasks/search_missing_parents_files.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/solohk_to_db.py` & `roc_dingo-1.4.1/roc/dingo/tasks/solohk_to_db.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/store_delivered.py` & `roc_dingo-1.4.1/roc/dingo/tasks/store_delivered.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/store_public_filename.py` & `roc_dingo-1.4.1/roc/dingo/tasks/store_public_filename.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/update_parents_in_db.py` & `roc_dingo-1.4.1/roc/dingo/tasks/update_parents_in_db.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/update_sbm_log_retrieved.py` & `roc_dingo-1.4.1/roc/dingo/tasks/update_sbm_log_retrieved.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
                 self.end_time))
 
         results = query_db(self.session, model,
                            filters=(and_(*filters) if filters else None),
                            tryouts=self.tryouts,
                            wait=self.wait,
                            limit=self.limit,
+                           order_by=model.utc_time,
                            to_dict='records')
 
         n_rec = len(results)
         logger.info(f'{n_rec} SBM event(s) found in pipeline.sbm_log')
         if n_rec == 0:
             return
 
@@ -127,15 +128,15 @@
 
             # Retrieve SBM event science packets from pipeline.TmLog table
             current_sbm_tm = self.query_sbm_tm_data(current_sbm_type,
                                                       current_sbm_start, current_sbm_end)
             n_pkt = len(current_sbm_tm)
             logger.info(f'{n_pkt} SBM{current_sbm_type} packets '
                         f'retrieved from pipeline.tm_log for event occurred at '
-                        f'{current_sbm_utc}')
+                        f'{current_sbm_utc}\t [{n_rec - i - 1}]')
 
             # Compute info from SBM science packet data
             # and update sbm_log.retrieved column
             current_sbm_stats = self.update_sbm_log(current_sbm_type,
                                                     current_sbm_tm,
                                                     current_sbm)
 
@@ -270,16 +271,21 @@
 
         # Update retrieved column in pipeline.sbm_log table with
         # this information
         retrieved = {'size': int(total_size),
                      'percent': total_percent,
                      'info': sbm_info}
 
+        if retrieved_time:
+            retrieved_time = max(retrieved_time)
+        else:
+            retrieved_time = None
+
         stmt = update(model). \
-            values(retrieved=retrieved, retrieved_time=max(retrieved_time)). \
+            values(retrieved=retrieved, retrieved_time=retrieved_time). \
             where(model.id == sbm_log_data['id'])
         self.session.execute(stmt)
 
         return sbm_info
 
     @staticmethod
     def get_sbm_sci_pkt_names(sbm_type: int, no_comp=False):
```

### Comparing `roc_dingo-1.4.0/roc/dingo/tasks/update_utc_time.py` & `roc_dingo-1.4.1/roc/dingo/tasks/update_utc_time.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_data_files_2020_08.dat` & `roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_data_files_2020_08.dat`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_data_files_2020_08_19.dat` & `roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_data_files_2020_08_19.dat`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_data_files_all.dat` & `roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_data_files_all.dat`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_data_files_all_dump.yml` & `roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_data_files_all_dump.yml`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_data_files_missing_parents.dat` & `roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_data_files_missing_parents.dat`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_data_files_public_filename.dat` & `roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_data_files_public_filename.dat`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_data_files_warning_state.dat` & `roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_data_files_warning_state.dat`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/data-tasks/roc_sk_files_1_dump.yml` & `roc_dingo-1.4.1/roc/dingo/tests/data-tasks/roc_sk_files_1_dump.yml`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
   author: ''
   basename: solo_ANC_soc-flown-att_20201228T101703-20201228T102157_V01.bc
   product: solo_ANC_soc-flown-att_20201228T101703-20201228T102157
   creation_time: '2021-01-28T08:18:24'
   dataset_id: null
   descr: ''
   dirname: ck
-  end_time: '2020-12-28T10:21:57'
+  end_time: '2020-12-28T10:21:57.388000'
   error_log: ''
   is_archived: false
   is_latest: true
   is_removed: false
   level: SK
   parents: []
   sha: ''
   size: 14336
-  start_time: '2020-12-28T10:17:03'
+  start_time: '2020-12-28T10:17:03.387000'
   state: OK
   status: Terminated
   url: https://rpw.lesia.obspm.fr/roc/data/private/solo/soc/spice/kernels//ck/solo_ANC_soc-flown-att_20201228T101703-20201228T102157_V01.bc
   validity_end: null
   validity_start: null
   version: '01'
   is_delivered: False
```

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_check_file_in_db.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_check_file_in_db.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_parse_file_tree.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_parse_file_tree.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_search_missing_parents_files.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_search_missing_parents_files.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_store_archived.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_store_archived.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_store_delivered.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_store_delivered.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_store_public_filename.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_store_public_filename.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_to_db.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_to_db.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-1-tasks/test_log_file_to_update_files.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-1-tasks/test_log_file_to_update_files.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_check_soar.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_check_soar.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_efecs_to_db.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_efecs_to_db.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_l0_to_db.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_l0_to_db.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_l0_to_hfrtimelog.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_l0_to_hfrtimelog.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_logfile_to_rocdb.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_logfile_to_rocdb.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_logfile_update.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_logfile_update.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_store_delivered.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_store_delivered.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test-2-commands/test_update_sbm_log_retrieved.py` & `roc_dingo-1.4.1/roc/dingo/tests/test-2-commands/test_update_sbm_log_retrieved.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test_dingo.py` & `roc_dingo-1.4.1/roc/dingo/tests/test_dingo.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tests/test_log_file.py` & `roc_dingo-1.4.1/roc/dingo/tests/test_log_file.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/roc/dingo/tools.py` & `roc_dingo-1.4.1/roc/dingo/tools.py`

 * *Files identical despite different names*

### Comparing `roc_dingo-1.4.0/PKG-INFO` & `roc_dingo-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: roc-dingo
-Version: 1.4.0
+Version: 1.4.1
 Summary: Data INgestOr (DINGO) plugin is used to ingest data into the ROC pipeline database
 Home-page: https://gitlab.obspm.fr/ROC/Pipelines/Plugins/DINGO
 License: CECILL-C
 Author: ROC Team
 Author-email: roc.support@sympa.obspm.fr
 Requires-Python: >=3.8,<4
 Classifier: License :: CeCILL-C Free Software License Agreement (CECILL-C)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: astropy (>=5.2,<6.0)
+Requires-Dist: h5py (>=3.7,<4.0)
 Requires-Dist: numpy (!=1.19.5)
 Requires-Dist: pandas (>=1.1.3,<2.0.0)
 Requires-Dist: poppy-core (>=0.9.4)
 Requires-Dist: poppy-pop (>=0.7.5)
 Requires-Dist: roc-idb (>=1.0,<2.0)
 Requires-Dist: roc-rpl (>=1.0,<2.0)
 Requires-Dist: spacepy (>=0.5,<1.0)
```

