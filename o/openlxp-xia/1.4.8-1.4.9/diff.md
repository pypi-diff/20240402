# Comparing `tmp/openlxp-xia-1.4.8.tar.gz` & `tmp/openlxp-xia-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlxp-xia-1.4.8.tar", last modified: Tue Mar 19 18:03:33 2024, max compression
+gzip compressed data, was "openlxp-xia-1.4.9.tar", last modified: Tue Apr  2 19:55:39 2024, max compression
```

## Comparing `openlxp-xia-1.4.8.tar` & `openlxp-xia-1.4.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-03-19 18:03:33.761057 openlxp-xia-1.4.8/
--rw-r--r--   0 kjijo      (502) staff       (20)     4930 2024-03-19 18:03:33.761293 openlxp-xia-1.4.8/PKG-INFO
--rw-r--r--   0 kjijo      (502) staff       (20)     4064 2023-12-15 21:25:01.000000 openlxp-xia-1.4.8/README.md
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-03-19 18:03:33.672216 openlxp-xia-1.4.8/enviroment_name/
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-03-19 18:03:33.712645 openlxp-xia-1.4.8/enviroment_name/bin/
--rw-r--r--   0 kjijo      (502) staff       (20)     1199 2023-09-07 16:15:28.000000 openlxp-xia-1.4.8/enviroment_name/bin/activate_this.py
--rwxr-xr-x   0 kjijo      (502) staff       (20)      232 2023-09-07 16:16:08.000000 openlxp-xia-1.4.8/enviroment_name/bin/django-admin.py
--rwxr-xr-x   0 kjijo      (502) staff       (20)      701 2023-09-07 17:57:27.000000 openlxp-xia-1.4.8/enviroment_name/bin/rst2html.py
--rwxr-xr-x   0 kjijo      (502) staff       (20)      821 2023-09-07 17:57:27.000000 openlxp-xia-1.4.8/enviroment_name/bin/rst2html4.py
--rwxr-xr-x   0 kjijo      (502) staff       (20)     1189 2023-09-07 17:57:27.000000 openlxp-xia-1.4.8/enviroment_name/bin/rst2html5.py
--rwxr-xr-x   0 kjijo      (502) staff       (20)      898 2023-09-07 17:57:27.000000 openlxp-xia-1.4.8/enviroment_name/bin/rst2latex.py
--rwxr-xr-x   0 kjijo      (502) staff       (20)      706 2023-09-07 17:57:27.000000 openlxp-xia-1.4.8/enviroment_name/bin/rst2man.py
--rwxr-xr-x   0 kjijo      (502) staff       (20)      871 2023-09-07 17:57:27.000000 openlxp-xia-1.4.8/enviroment_name/bin/rst2odt.py
--rwxr-xr-x   0 kjijo      (502) staff       (20)     1833 2023-09-07 17:57:27.000000 openlxp-xia-1.4.8/enviroment_name/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 kjijo      (502) staff       (20)      708 2023-09-07 17:57:27.000000 openlxp-xia-1.4.8/enviroment_name/bin/rst2pseudoxml.py
--rwxr-xr-x   0 kjijo      (502) staff       (20)      744 2023-09-07 17:57:27.000000 openlxp-xia-1.4.8/enviroment_name/bin/rst2s5.py
--rwxr-xr-x   0 kjijo      (502) staff       (20)      978 2023-09-07 17:57:27.000000 openlxp-xia-1.4.8/enviroment_name/bin/rst2xetex.py
--rwxr-xr-x   0 kjijo      (502) staff       (20)      709 2023-09-07 17:57:27.000000 openlxp-xia-1.4.8/enviroment_name/bin/rst2xml.py
--rwxr-xr-x   0 kjijo      (502) staff       (20)      777 2023-09-07 17:57:27.000000 openlxp-xia-1.4.8/enviroment_name/bin/rstpep2html.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-03-19 18:03:33.716899 openlxp-xia-1.4.8/openlxp_xia/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-09-07 15:25:44.000000 openlxp-xia-1.4.8/openlxp_xia/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)     1945 2024-03-19 17:51:29.000000 openlxp-xia-1.4.8/openlxp_xia/admin.py
--rw-r--r--   0 kjijo      (502) staff       (20)      147 2024-03-19 17:51:38.000000 openlxp-xia-1.4.8/openlxp_xia/apps.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-03-19 18:03:33.723968 openlxp-xia-1.4.8/openlxp_xia/management/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-03-19 17:50:28.000000 openlxp-xia-1.4.8/openlxp_xia/management/__init__.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-03-19 18:03:33.728941 openlxp-xia-1.4.8/openlxp_xia/management/commands/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-03-19 17:50:28.000000 openlxp-xia-1.4.8/openlxp_xia/management/commands/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)     4718 2024-03-19 17:50:28.000000 openlxp-xia-1.4.8/openlxp_xia/management/commands/load_supplemental_metadata.py
--rw-r--r--   0 kjijo      (502) staff       (20)     4403 2024-03-19 17:50:28.000000 openlxp-xia-1.4.8/openlxp_xia/management/commands/load_target_metadata.py
--rw-r--r--   0 kjijo      (502) staff       (20)    12029 2024-03-19 17:50:28.000000 openlxp-xia-1.4.8/openlxp_xia/management/commands/transform_source_metadata.py
--rw-r--r--   0 kjijo      (502) staff       (20)     5116 2024-03-19 17:50:28.000000 openlxp-xia-1.4.8/openlxp_xia/management/commands/validate_source_metadata.py
--rw-r--r--   0 kjijo      (502) staff       (20)     7956 2024-03-19 17:50:28.000000 openlxp-xia-1.4.8/openlxp_xia/management/commands/validate_target_metadata.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-03-19 18:03:33.731940 openlxp-xia-1.4.8/openlxp_xia/management/utils/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-03-19 17:50:28.000000 openlxp-xia-1.4.8/openlxp_xia/management/utils/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)     1394 2024-03-19 17:50:28.000000 openlxp-xia-1.4.8/openlxp_xia/management/utils/model_help.py
--rw-r--r--   0 kjijo      (502) staff       (20)     9840 2024-03-19 17:50:28.000000 openlxp-xia-1.4.8/openlxp_xia/management/utils/xia_internal.py
--rw-r--r--   0 kjijo      (502) staff       (20)     2087 2024-03-19 17:50:28.000000 openlxp-xia-1.4.8/openlxp_xia/management/utils/xis_client.py
--rw-r--r--   0 kjijo      (502) staff       (20)     5119 2024-03-19 18:02:36.000000 openlxp-xia-1.4.8/openlxp_xia/management/utils/xss_client.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-03-19 18:03:33.736719 openlxp-xia-1.4.8/openlxp_xia/migrations/
--rw-r--r--   0 kjijo      (502) staff       (20)     7683 2023-09-07 15:25:44.000000 openlxp-xia-1.4.8/openlxp_xia/migrations/0001_initial.py
--rw-r--r--   0 kjijo      (502) staff       (20)     1726 2023-12-15 21:25:01.000000 openlxp-xia-1.4.8/openlxp_xia/migrations/0002_use_xss.py
--rw-r--r--   0 kjijo      (502) staff       (20)      487 2023-12-15 21:25:01.000000 openlxp-xia-1.4.8/openlxp_xia/migrations/0003_xisconfiguration_xis_api_key.py
--rw-r--r--   0 kjijo      (502) staff       (20)      444 2023-12-15 21:25:01.000000 openlxp-xia-1.4.8/openlxp_xia/migrations/0004_alter_xiaconfiguration_xss_api.py
--rw-r--r--   0 kjijo      (502) staff       (20)      454 2023-12-15 21:25:01.000000 openlxp-xia-1.4.8/openlxp_xia/migrations/0005_alter_xisconfiguration_xis_api_key.py
--rw-r--r--   0 kjijo      (502) staff       (20)     1452 2023-12-15 21:25:19.000000 openlxp-xia-1.4.8/openlxp_xia/migrations/0006_auto_20230907_1642.py
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-09-07 15:25:44.000000 openlxp-xia-1.4.8/openlxp_xia/migrations/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)    12526 2024-03-19 18:02:28.000000 openlxp-xia-1.4.8/openlxp_xia/models.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-03-19 18:03:33.757681 openlxp-xia-1.4.8/openlxp_xia/tests/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-09-07 15:25:44.000000 openlxp-xia-1.4.8/openlxp_xia/tests/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)    17232 2023-09-07 15:25:44.000000 openlxp-xia-1.4.8/openlxp_xia/tests/test_setup.py
--rw-r--r--   0 kjijo      (502) staff       (20)    27386 2023-09-07 15:25:44.000000 openlxp-xia-1.4.8/openlxp_xia/tests/test_xia_command_intergration.py
--rw-r--r--   0 kjijo      (502) staff       (20)    33612 2023-09-07 15:25:44.000000 openlxp-xia-1.4.8/openlxp_xia/tests/test_xia_command_unit.py
--rw-r--r--   0 kjijo      (502) staff       (20)     1120 2023-12-15 21:25:01.000000 openlxp-xia-1.4.8/openlxp_xia/tests/test_xia_models_integration.py
--rw-r--r--   0 kjijo      (502) staff       (20)    12993 2023-12-15 21:25:01.000000 openlxp-xia-1.4.8/openlxp_xia/tests/test_xia_models_unit.py
--rw-r--r--   0 kjijo      (502) staff       (20)      710 2023-09-07 15:25:44.000000 openlxp-xia-1.4.8/openlxp_xia/tests/test_xia_utils_integration.py
--rw-r--r--   0 kjijo      (502) staff       (20)    22425 2023-12-15 21:25:01.000000 openlxp-xia-1.4.8/openlxp_xia/tests/test_xia_utils_unit.py
--rw-r--r--   0 kjijo      (502) staff       (20)      761 2024-03-19 17:51:53.000000 openlxp-xia-1.4.8/openlxp_xia/urls.py
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-09-07 15:25:44.000000 openlxp-xia-1.4.8/openlxp_xia/views.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-03-19 18:03:33.723345 openlxp-xia-1.4.8/openlxp_xia.egg-info/
--rw-r--r--   0 kjijo      (502) staff       (20)     4930 2024-03-19 18:03:33.000000 openlxp-xia-1.4.8/openlxp_xia.egg-info/PKG-INFO
--rw-r--r--   0 kjijo      (502) staff       (20)     2232 2024-03-19 18:03:33.000000 openlxp-xia-1.4.8/openlxp_xia.egg-info/SOURCES.txt
--rw-r--r--   0 kjijo      (502) staff       (20)        1 2024-03-19 18:03:33.000000 openlxp-xia-1.4.8/openlxp_xia.egg-info/dependency_links.txt
--rw-r--r--   0 kjijo      (502) staff       (20)       78 2024-03-19 18:03:33.000000 openlxp-xia-1.4.8/openlxp_xia.egg-info/requires.txt
--rw-r--r--   0 kjijo      (502) staff       (20)       48 2024-03-19 18:03:33.000000 openlxp-xia-1.4.8/openlxp_xia.egg-info/top_level.txt
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-03-19 18:03:33.760638 openlxp-xia-1.4.8/openlxp_xia_project/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-09-07 15:25:44.000000 openlxp-xia-1.4.8/openlxp_xia_project/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)      415 2023-09-07 15:25:44.000000 openlxp-xia-1.4.8/openlxp_xia_project/asgi.py
--rw-r--r--   0 kjijo      (502) staff       (20)     4538 2024-03-19 17:59:48.000000 openlxp-xia-1.4.8/openlxp_xia_project/settings.py
--rw-r--r--   0 kjijo      (502) staff       (20)      761 2023-09-07 15:25:44.000000 openlxp-xia-1.4.8/openlxp_xia_project/urls.py
--rw-r--r--   0 kjijo      (502) staff       (20)      415 2023-09-07 15:25:44.000000 openlxp-xia-1.4.8/openlxp_xia_project/wsgi.py
--rw-r--r--   0 kjijo      (502) staff       (20)     1043 2024-03-19 18:03:33.761745 openlxp-xia-1.4.8/setup.cfg
--rw-r--r--   0 kjijo      (502) staff       (20)       95 2023-09-07 15:25:44.000000 openlxp-xia-1.4.8/setup.py
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-04-02 19:55:39.753851 openlxp-xia-1.4.9/
+-rw-r--r--   0 kjijo      (502) staff       (20)     4930 2024-04-02 19:55:39.754144 openlxp-xia-1.4.9/PKG-INFO
+-rw-r--r--   0 kjijo      (502) staff       (20)     4064 2023-12-15 21:25:01.000000 openlxp-xia-1.4.9/README.md
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-04-02 19:55:39.642926 openlxp-xia-1.4.9/enviroment_name/
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-04-02 19:55:39.693330 openlxp-xia-1.4.9/enviroment_name/bin/
+-rw-r--r--   0 kjijo      (502) staff       (20)     1199 2023-09-07 16:15:28.000000 openlxp-xia-1.4.9/enviroment_name/bin/activate_this.py
+-rwxr-xr-x   0 kjijo      (502) staff       (20)      232 2023-09-07 16:16:08.000000 openlxp-xia-1.4.9/enviroment_name/bin/django-admin.py
+-rwxr-xr-x   0 kjijo      (502) staff       (20)      701 2023-09-07 17:57:27.000000 openlxp-xia-1.4.9/enviroment_name/bin/rst2html.py
+-rwxr-xr-x   0 kjijo      (502) staff       (20)      821 2023-09-07 17:57:27.000000 openlxp-xia-1.4.9/enviroment_name/bin/rst2html4.py
+-rwxr-xr-x   0 kjijo      (502) staff       (20)     1189 2023-09-07 17:57:27.000000 openlxp-xia-1.4.9/enviroment_name/bin/rst2html5.py
+-rwxr-xr-x   0 kjijo      (502) staff       (20)      898 2023-09-07 17:57:27.000000 openlxp-xia-1.4.9/enviroment_name/bin/rst2latex.py
+-rwxr-xr-x   0 kjijo      (502) staff       (20)      706 2023-09-07 17:57:27.000000 openlxp-xia-1.4.9/enviroment_name/bin/rst2man.py
+-rwxr-xr-x   0 kjijo      (502) staff       (20)      871 2023-09-07 17:57:27.000000 openlxp-xia-1.4.9/enviroment_name/bin/rst2odt.py
+-rwxr-xr-x   0 kjijo      (502) staff       (20)     1833 2023-09-07 17:57:27.000000 openlxp-xia-1.4.9/enviroment_name/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 kjijo      (502) staff       (20)      708 2023-09-07 17:57:27.000000 openlxp-xia-1.4.9/enviroment_name/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 kjijo      (502) staff       (20)      744 2023-09-07 17:57:27.000000 openlxp-xia-1.4.9/enviroment_name/bin/rst2s5.py
+-rwxr-xr-x   0 kjijo      (502) staff       (20)      978 2023-09-07 17:57:27.000000 openlxp-xia-1.4.9/enviroment_name/bin/rst2xetex.py
+-rwxr-xr-x   0 kjijo      (502) staff       (20)      709 2023-09-07 17:57:27.000000 openlxp-xia-1.4.9/enviroment_name/bin/rst2xml.py
+-rwxr-xr-x   0 kjijo      (502) staff       (20)      777 2023-09-07 17:57:27.000000 openlxp-xia-1.4.9/enviroment_name/bin/rstpep2html.py
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-04-02 19:55:39.721049 openlxp-xia-1.4.9/openlxp_xia/
+-rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-09-07 15:25:44.000000 openlxp-xia-1.4.9/openlxp_xia/__init__.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     1945 2024-03-19 17:51:29.000000 openlxp-xia-1.4.9/openlxp_xia/admin.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      147 2024-03-19 17:51:38.000000 openlxp-xia-1.4.9/openlxp_xia/apps.py
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-04-02 19:55:39.723078 openlxp-xia-1.4.9/openlxp_xia/management/
+-rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-03-19 17:50:28.000000 openlxp-xia-1.4.9/openlxp_xia/management/__init__.py
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-04-02 19:55:39.725939 openlxp-xia-1.4.9/openlxp_xia/management/commands/
+-rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-03-19 17:50:28.000000 openlxp-xia-1.4.9/openlxp_xia/management/commands/__init__.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     4718 2024-03-19 17:50:28.000000 openlxp-xia-1.4.9/openlxp_xia/management/commands/load_supplemental_metadata.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     4403 2024-03-19 17:50:28.000000 openlxp-xia-1.4.9/openlxp_xia/management/commands/load_target_metadata.py
+-rw-r--r--   0 kjijo      (502) staff       (20)    12029 2024-03-19 17:50:28.000000 openlxp-xia-1.4.9/openlxp_xia/management/commands/transform_source_metadata.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     5116 2024-03-19 17:50:28.000000 openlxp-xia-1.4.9/openlxp_xia/management/commands/validate_source_metadata.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     7956 2024-03-19 17:50:28.000000 openlxp-xia-1.4.9/openlxp_xia/management/commands/validate_target_metadata.py
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-04-02 19:55:39.728295 openlxp-xia-1.4.9/openlxp_xia/management/utils/
+-rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-03-19 17:50:28.000000 openlxp-xia-1.4.9/openlxp_xia/management/utils/__init__.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     1452 2024-04-02 18:31:02.000000 openlxp-xia-1.4.9/openlxp_xia/management/utils/model_help.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     9840 2024-03-19 17:50:28.000000 openlxp-xia-1.4.9/openlxp_xia/management/utils/xia_internal.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     2115 2024-03-29 15:44:20.000000 openlxp-xia-1.4.9/openlxp_xia/management/utils/xis_client.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     5119 2024-03-19 18:02:36.000000 openlxp-xia-1.4.9/openlxp_xia/management/utils/xss_client.py
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-04-02 19:55:39.743998 openlxp-xia-1.4.9/openlxp_xia/migrations/
+-rw-r--r--   0 kjijo      (502) staff       (20)     7683 2023-09-07 15:25:44.000000 openlxp-xia-1.4.9/openlxp_xia/migrations/0001_initial.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     1726 2023-12-15 21:25:01.000000 openlxp-xia-1.4.9/openlxp_xia/migrations/0002_use_xss.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      487 2023-12-15 21:25:01.000000 openlxp-xia-1.4.9/openlxp_xia/migrations/0003_xisconfiguration_xis_api_key.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      444 2023-12-15 21:25:01.000000 openlxp-xia-1.4.9/openlxp_xia/migrations/0004_alter_xiaconfiguration_xss_api.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      454 2023-12-15 21:25:01.000000 openlxp-xia-1.4.9/openlxp_xia/migrations/0005_alter_xisconfiguration_xis_api_key.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     1452 2023-12-15 21:25:19.000000 openlxp-xia-1.4.9/openlxp_xia/migrations/0006_auto_20230907_1642.py
+-rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-09-07 15:25:44.000000 openlxp-xia-1.4.9/openlxp_xia/migrations/__init__.py
+-rw-r--r--   0 kjijo      (502) staff       (20)    13584 2024-03-29 16:09:23.000000 openlxp-xia-1.4.9/openlxp_xia/models.py
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-04-02 19:55:39.750022 openlxp-xia-1.4.9/openlxp_xia/tests/
+-rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-09-07 15:25:44.000000 openlxp-xia-1.4.9/openlxp_xia/tests/__init__.py
+-rw-r--r--   0 kjijo      (502) staff       (20)    17232 2023-09-07 15:25:44.000000 openlxp-xia-1.4.9/openlxp_xia/tests/test_setup.py
+-rw-r--r--   0 kjijo      (502) staff       (20)    27386 2023-09-07 15:25:44.000000 openlxp-xia-1.4.9/openlxp_xia/tests/test_xia_command_intergration.py
+-rw-r--r--   0 kjijo      (502) staff       (20)    33612 2023-09-07 15:25:44.000000 openlxp-xia-1.4.9/openlxp_xia/tests/test_xia_command_unit.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     1120 2023-12-15 21:25:01.000000 openlxp-xia-1.4.9/openlxp_xia/tests/test_xia_models_integration.py
+-rw-r--r--   0 kjijo      (502) staff       (20)    12993 2023-12-15 21:25:01.000000 openlxp-xia-1.4.9/openlxp_xia/tests/test_xia_models_unit.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      710 2023-09-07 15:25:44.000000 openlxp-xia-1.4.9/openlxp_xia/tests/test_xia_utils_integration.py
+-rw-r--r--   0 kjijo      (502) staff       (20)    22425 2023-12-15 21:25:01.000000 openlxp-xia-1.4.9/openlxp_xia/tests/test_xia_utils_unit.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      761 2024-03-19 17:51:53.000000 openlxp-xia-1.4.9/openlxp_xia/urls.py
+-rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-09-07 15:25:44.000000 openlxp-xia-1.4.9/openlxp_xia/views.py
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-04-02 19:55:39.722729 openlxp-xia-1.4.9/openlxp_xia.egg-info/
+-rw-r--r--   0 kjijo      (502) staff       (20)     4930 2024-04-02 19:55:39.000000 openlxp-xia-1.4.9/openlxp_xia.egg-info/PKG-INFO
+-rw-r--r--   0 kjijo      (502) staff       (20)     2232 2024-04-02 19:55:39.000000 openlxp-xia-1.4.9/openlxp_xia.egg-info/SOURCES.txt
+-rw-r--r--   0 kjijo      (502) staff       (20)        1 2024-04-02 19:55:39.000000 openlxp-xia-1.4.9/openlxp_xia.egg-info/dependency_links.txt
+-rw-r--r--   0 kjijo      (502) staff       (20)       78 2024-04-02 19:55:39.000000 openlxp-xia-1.4.9/openlxp_xia.egg-info/requires.txt
+-rw-r--r--   0 kjijo      (502) staff       (20)       48 2024-04-02 19:55:39.000000 openlxp-xia-1.4.9/openlxp_xia.egg-info/top_level.txt
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-04-02 19:55:39.752960 openlxp-xia-1.4.9/openlxp_xia_project/
+-rw-r--r--   0 kjijo      (502) staff       (20)        0 2023-09-07 15:25:44.000000 openlxp-xia-1.4.9/openlxp_xia_project/__init__.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      415 2023-09-07 15:25:44.000000 openlxp-xia-1.4.9/openlxp_xia_project/asgi.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     4538 2024-03-19 17:59:48.000000 openlxp-xia-1.4.9/openlxp_xia_project/settings.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      761 2023-09-07 15:25:44.000000 openlxp-xia-1.4.9/openlxp_xia_project/urls.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      415 2023-09-07 15:25:44.000000 openlxp-xia-1.4.9/openlxp_xia_project/wsgi.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     1043 2024-04-02 19:55:39.754685 openlxp-xia-1.4.9/setup.cfg
+-rw-r--r--   0 kjijo      (502) staff       (20)       95 2023-09-07 15:25:44.000000 openlxp-xia-1.4.9/setup.py
```

### Comparing `openlxp-xia-1.4.8/PKG-INFO` & `openlxp-xia-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlxp-xia
-Version: 1.4.8
+Version: 1.4.9
 Summary: Sample installable XIA
 Home-page: https://github.com/OpenLXP/openlxp-xia/
 Author: OpenLXP
 Author-email: openlxphost@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `openlxp-xia-1.4.8/README.md` & `openlxp-xia-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/enviroment_name/bin/activate_this.py` & `openlxp-xia-1.4.9/enviroment_name/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/enviroment_name/bin/rst2html.py` & `openlxp-xia-1.4.9/enviroment_name/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/enviroment_name/bin/rst2html4.py` & `openlxp-xia-1.4.9/enviroment_name/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/enviroment_name/bin/rst2html5.py` & `openlxp-xia-1.4.9/enviroment_name/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/enviroment_name/bin/rst2latex.py` & `openlxp-xia-1.4.9/enviroment_name/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/enviroment_name/bin/rst2man.py` & `openlxp-xia-1.4.9/enviroment_name/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/enviroment_name/bin/rst2odt.py` & `openlxp-xia-1.4.9/enviroment_name/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/enviroment_name/bin/rst2odt_prepstyles.py` & `openlxp-xia-1.4.9/enviroment_name/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/enviroment_name/bin/rst2pseudoxml.py` & `openlxp-xia-1.4.9/enviroment_name/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/enviroment_name/bin/rst2s5.py` & `openlxp-xia-1.4.9/enviroment_name/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/enviroment_name/bin/rst2xetex.py` & `openlxp-xia-1.4.9/enviroment_name/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/enviroment_name/bin/rst2xml.py` & `openlxp-xia-1.4.9/enviroment_name/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/enviroment_name/bin/rstpep2html.py` & `openlxp-xia-1.4.9/enviroment_name/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/admin.py` & `openlxp-xia-1.4.9/openlxp_xia/admin.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/management/commands/load_supplemental_metadata.py` & `openlxp-xia-1.4.9/openlxp_xia/management/commands/load_supplemental_metadata.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/management/commands/load_target_metadata.py` & `openlxp-xia-1.4.9/openlxp_xia/management/commands/load_target_metadata.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/management/commands/transform_source_metadata.py` & `openlxp-xia-1.4.9/openlxp_xia/management/commands/transform_source_metadata.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/management/commands/validate_source_metadata.py` & `openlxp-xia-1.4.9/openlxp_xia/management/commands/validate_source_metadata.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/management/commands/validate_target_metadata.py` & `openlxp-xia-1.4.9/openlxp_xia/management/commands/validate_target_metadata.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/management/utils/model_help.py` & `openlxp-xia-1.4.9/openlxp_xia/management/utils/model_help.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import html
 import bleach
 import logging
 from confusable_homoglyphs import categories, confusables
 
 logger = logging.getLogger('dict_config_logger')
 
 
@@ -14,14 +15,15 @@
     :return: dict"""
 
     # iterate over dict
     for key in rdata:
         # if string, clean
         if isinstance(rdata[key], str):
             rdata[key] = bleach.clean(rdata[key], tags={}, strip=True)
+            rdata[key] = html.unescape(rdata)
         # if dict, enter dict
         if isinstance(rdata[key], dict):
             rdata[key] = bleach_data_to_json(rdata[key])
 
     return rdata
```

### Comparing `openlxp-xia-1.4.8/openlxp_xia/management/utils/xia_internal.py` & `openlxp-xia-1.4.9/openlxp_xia/management/utils/xia_internal.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/management/utils/xis_client.py` & `openlxp-xia-1.4.9/openlxp_xia/management/utils/xis_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,26 +30,26 @@
 def posting_metadata_ledger_to_xis(renamed_data):
     """This function post data to XIS and returns the XIS response to
             XIA load_target_metadata() """
     headers = {'Content-Type': 'application/json'}
 
     xis_response = requests.post(url=get_xis_metadata_api_endpoint(),
                                  data=renamed_data, headers=headers,
-                                 auth=TokenAuth())
+                                 auth=TokenAuth(), verify=False)
     return xis_response
 
 
 def posting_supplemental_metadata_to_xis(renamed_data):
     """This function post data to XIS and returns the XIS response to
             XIA load_target_metadata() """
     headers = {'Content-Type': 'application/json'}
 
     xis_response = requests.post(
         url=get_xis_supplemental_metadata_api_endpoint(), data=renamed_data,
-        headers=headers, auth=TokenAuth())
+        headers=headers, auth=TokenAuth(), verify=False)
     return xis_response
 
 
 class TokenAuth(AuthBase):
     """Attaches HTTP Authentication Header to the given Request object."""
 
     def __call__(self, r, token_name='token'):
```

### Comparing `openlxp-xia-1.4.8/openlxp_xia/management/utils/xss_client.py` & `openlxp-xia-1.4.9/openlxp_xia/management/utils/xss_client.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/migrations/0001_initial.py` & `openlxp-xia-1.4.9/openlxp_xia/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/migrations/0002_use_xss.py` & `openlxp-xia-1.4.9/openlxp_xia/migrations/0002_use_xss.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/migrations/0006_auto_20230907_1642.py` & `openlxp-xia-1.4.9/openlxp_xia/migrations/0006_auto_20230907_1642.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/models.py` & `openlxp-xia-1.4.9/openlxp_xia/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import uuid
 
 import requests
 from django.db import models
 from django.forms import ValidationError
 from django.core.validators import RegexValidator
 from django.urls import reverse
+from django.utils import timezone
 from openlxp_xia.management.utils.model_help import confusable_homoglyphs_check
 from openlxp_xia.management.utils.model_help import bleach_data_to_json
 from model_utils.models import TimeStampedModel
 
 logger = logging.getLogger('dict_config_logger')
 
 
@@ -184,16 +185,27 @@
     target_metadata_validation_date = models.DateTimeField(blank=True,
                                                            null=True)
     target_metadata_validation_status = models.CharField(
         max_length=10, blank=True, choices=METADATA_VALIDATION_CHOICES)
 
     def clean(self):
         source_data = self.source_metadata
+        # Checking for confusable hologlyphs 
         data_checked = confusable_homoglyphs_check(source_data)
-        self.source_metadata = bleach_data_to_json(data_checked)
+        if not data_checked:
+            # If data check failed setting metadata to inactive
+            self.record_lifecycle_status = "Inactive"
+            self.metadata_record_inactivation_date=timezone.now()
+            raise ValidationError('Data Fails validation and cannot be saved further')
+        # cleaning metadata using bleach 
+        self.source_metadata = bleach_data_to_json(source_data)
+
+    def save(self, *args, **kwargs):
+        MetadataLedger.clean()
+        return super(MetadataLedger, self).save(*args, **kwargs)
 
 
 class SupplementalLedger(TimeStampedModel):
     """Model for Supplemental Metadata """
 
     RECORD_ACTIVATION_STATUS_CHOICES = [('Active', 'A'), ('Inactive', 'I')]
     RECORD_TRANSMISSION_STATUS_CHOICES = [('Successful', 'S'), ('Failed', 'F'),
@@ -226,17 +238,28 @@
     supplemental_metadata_transmission_status = models.CharField(
         max_length=10, blank=True, default='Ready',
         choices=RECORD_TRANSMISSION_STATUS_CHOICES)
     supplemental_metadata_transmission_status_code = models.IntegerField(
         blank=True, null=True)
 
     def clean(self):
-        supplemental_data = self.supplemental_metadata
-        data_checked = confusable_homoglyphs_check(supplemental_data)
-        self.supplemental_metadata = bleach_data_to_json(data_checked)
+        source_data = self.supplemental_metadata
+        # Checking for confusable hologlyphs 
+        data_checked = confusable_homoglyphs_check(source_data)
+        if not data_checked:
+            # If data check failed setting metadata to inactive
+            self.record_lifecycle_status = "Inactive"
+            self.metadata_record_inactivation_date=timezone.now()
+            raise ValidationError('Data Fails validation and cannot be saved further')
+        # cleaning metadata using bleach 
+        self.source_metadata = bleach_data_to_json(source_data)
+
+    def save(self, *args, **kwargs):
+        MetadataLedger.clean()
+        return super(MetadataLedger, self).save(*args, **kwargs)
 
 
 class MetadataFieldOverwrite(TimeStampedModel):
     """Model for taking list of fields name and it's values for overwriting
     field values in Source metadata"""
 
     DATATYPE_CHOICES = (
```

### Comparing `openlxp-xia-1.4.8/openlxp_xia/tests/test_setup.py` & `openlxp-xia-1.4.9/openlxp_xia/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/tests/test_xia_command_intergration.py` & `openlxp-xia-1.4.9/openlxp_xia/tests/test_xia_command_intergration.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/tests/test_xia_command_unit.py` & `openlxp-xia-1.4.9/openlxp_xia/tests/test_xia_command_unit.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/tests/test_xia_models_integration.py` & `openlxp-xia-1.4.9/openlxp_xia/tests/test_xia_models_integration.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/tests/test_xia_models_unit.py` & `openlxp-xia-1.4.9/openlxp_xia/tests/test_xia_models_unit.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/tests/test_xia_utils_integration.py` & `openlxp-xia-1.4.9/openlxp_xia/tests/test_xia_utils_integration.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/tests/test_xia_utils_unit.py` & `openlxp-xia-1.4.9/openlxp_xia/tests/test_xia_utils_unit.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia/urls.py` & `openlxp-xia-1.4.9/openlxp_xia/urls.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia.egg-info/PKG-INFO` & `openlxp-xia-1.4.9/openlxp_xia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlxp-xia
-Version: 1.4.8
+Version: 1.4.9
 Summary: Sample installable XIA
 Home-page: https://github.com/OpenLXP/openlxp-xia/
 Author: OpenLXP
 Author-email: openlxphost@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `openlxp-xia-1.4.8/openlxp_xia.egg-info/SOURCES.txt` & `openlxp-xia-1.4.9/openlxp_xia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia_project/settings.py` & `openlxp-xia-1.4.9/openlxp_xia_project/settings.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/openlxp_xia_project/urls.py` & `openlxp-xia-1.4.9/openlxp_xia_project/urls.py`

 * *Files identical despite different names*

### Comparing `openlxp-xia-1.4.8/setup.cfg` & `openlxp-xia-1.4.9/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = openlxp-xia
-version = 1.4.8
+version = 1.4.9
 description = Sample installable XIA
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/OpenLXP/openlxp-xia/
 author = OpenLXP
 author_email = openlxphost@gmail.com
 license = MIT
```

