# Comparing `tmp/netbox-device-support-plugin-0.0.8.tar.gz` & `tmp/netbox-device-support-plugin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-device-support-plugin-0.0.8.tar", last modified: Tue Nov 21 12:33:31 2023, max compression
+gzip compressed data, was "netbox-device-support-plugin-0.0.9.tar", last modified: Tue Nov 21 12:51:45 2023, max compression
```

## Comparing `netbox-device-support-plugin-0.0.8.tar` & `netbox-device-support-plugin-0.0.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:31.061225 netbox-device-support-plugin-0.0.8/
--rw-r--r--   0 vsts      (1001) docker     (127)     1068 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)       58 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    13514 2023-11-21 12:33:31.061225 netbox-device-support-plugin-0.0.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    12867 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:31.057225 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (127)      678 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2448 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:31.057225 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/api/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3192 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/api/serializers.py
--rw-r--r--   0 vsts      (1001) docker     (127)      407 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/api/urls.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/api/views.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5438 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/filtersets.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12196 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/forms.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:31.057225 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/management/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:31.057225 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39500 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:31.057225 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/migrations/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35472 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/models.py
--rw-r--r--   0 vsts      (1001) docker     (127)      537 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/navigation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4954 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/tables.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5150 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:31.053225 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:31.057225 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/
--rw-r--r--   0 vsts      (1001) docker     (127)     6651 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/cisco_device_support.html
--rw-r--r--   0 vsts      (1001) docker     (127)     4524 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:31.057225 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/
--rw-r--r--   0 vsts      (1001) docker     (127)      832 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      896 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1078 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      888 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1038 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1030 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      966 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)     1046 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:31.057225 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/fortinet/
--rw-r--r--   0 vsts      (1001) docker     (127)     4709 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:31.061225 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2960 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1585 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/urls.py
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2491 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/views.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:33:31.061225 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    13514 2023-11-21 12:33:31.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2205 2023-11-21 12:33:31.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-21 12:33:31.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-21 12:33:30.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       29 2023-11-21 12:33:31.000000 netbox-device-support-plugin-0.0.8/netbox_device_support_plugin.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2023-11-21 12:33:31.061225 netbox-device-support-plugin-0.0.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1570 2023-11-21 12:33:09.000000 netbox-device-support-plugin-0.0.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1068 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)       58 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    13514 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    12867 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.780943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (127)      678 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2448 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.780943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/api/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3199 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/api/serializers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      415 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/api/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1239 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/api/views.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5438 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/filtersets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12196 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/forms.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.780943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/management/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39500 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35472 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/models.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      537 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/navigation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4954 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/tables.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5150 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.776943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6651 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/cisco_device_support.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     4524 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/
+-rw-r--r--   0 vsts      (1001) docker     (127)      832 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      896 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1078 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      888 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1038 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1030 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      966 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)     1046 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/fortinet/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4709 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2960 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1585 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2491 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/views.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-21 12:51:45.784943 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    13514 2023-11-21 12:51:45.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2205 2023-11-21 12:51:45.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-21 12:51:45.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-21 12:51:45.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       29 2023-11-21 12:51:45.000000 netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2023-11-21 12:51:45.788943 netbox-device-support-plugin-0.0.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1570 2023-11-21 12:51:14.000000 netbox-device-support-plugin-0.0.9/setup.py
```

### Comparing `netbox-device-support-plugin-0.0.8/LICENSE` & `netbox-device-support-plugin-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/PKG-INFO` & `netbox-device-support-plugin-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-device-support-plugin
-Version: 0.0.8
+Version: 0.0.9
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-device-support-plugin-0.0.8/README.md` & `netbox-device-support-plugin-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/__init__.py` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/admin.py` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/api/serializers.py` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/api/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             "last_updated",
         ]
         # fmt: on
 
 
 #### Fortinet Support #######################################################################################
 
-
+"""
 class FortinetDeviceSupportSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:netbox_device_support_plugin-api:fortinetdevicesupport-detail"
     )
 
     device = NestedDeviceSerializer()
 
@@ -68,7 +68,8 @@
         # fmt: off
         fields = [
             "id", "url", "display", "name", "device", "pid", "serial", "recommended_release",
             "desired_release", "current_release", "desired_release_status", "current_release_status",
             "tags", "custom_fields", "created", "last_updated",
         ]
         # fmt: on
+"""
```

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/api/views.py` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/api/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,11 +22,13 @@
     serializer_class = CiscoDeviceTypeSupportSerializer
     filterset_class = filtersets.CiscoDeviceTypeSupportFilterSet
 
 
 #### Fortinet Support #######################################################################################
 
 
+"""
 class FortinetDeviceSupportViewSet(NetBoxModelViewSet):
     queryset = models.FortinetDeviceSupport.objects.all().prefetch_related("device")
     serializer_class = FortinetDeviceSupportSerializer
     filterset_class = filtersets.FortinetDeviceSupportFilterSet
+"""
```

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/filtersets.py` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/forms.py` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/management/commands/sync_cisco_support_data.py`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/models.py` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/models.py`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/navigation.py` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/tables.py` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/template_content.py` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/cisco_device_support.html` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/cisco_device_support.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/cisco_device_type_support.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_contract_coverage_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_partner_contract_coverage_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eorfa_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eos_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eoscr_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eosm_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvca_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_eosvs_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/cisco/inc/device_type_last_day_support_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templates/fortinet/fortinet_device_support.html`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/templatetags/filters.py` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/urls.py` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin/views.py` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin/views.py`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin.egg-info/PKG-INFO` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-device-support-plugin
-Version: 0.0.8
+Version: 0.0.9
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-device-support-plugin-0.0.8/netbox_device_support_plugin.egg-info/SOURCES.txt` & `netbox-device-support-plugin-0.0.9/netbox_device_support_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-device-support-plugin-0.0.8/setup.py` & `netbox-device-support-plugin-0.0.9/setup.py`

 * *Files identical despite different names*

