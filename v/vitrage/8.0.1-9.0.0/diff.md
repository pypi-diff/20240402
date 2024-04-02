# Comparing `tmp/vitrage-8.0.1.tar.gz` & `tmp/vitrage-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vitrage-8.0.1.tar", last modified: Wed Mar 16 09:00:27 2022, max compression
+gzip compressed data, was "vitrage-9.0.0.tar", last modified: Tue Aug  2 10:18:15 2022, max compression
```

## Comparing `vitrage-8.0.1.tar` & `vitrage-9.0.0.tar`

### file list

```diff
@@ -1,1204 +1,1206 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.622536 vitrage-8.0.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2022-03-16 08:59:56.000000 vitrage-8.0.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2022-03-16 08:59:56.000000 vitrage-8.0.1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5450 2022-03-16 09:00:27.000000 vitrage-8.0.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2022-03-16 08:59:56.000000 vitrage-8.0.1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    58483 2022-03-16 09:00:27.000000 vitrage-8.0.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2022-03-16 08:59:56.000000 vitrage-8.0.1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-03-16 08:59:56.000000 vitrage-8.0.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2310 2022-03-16 09:00:27.622536 vitrage-8.0.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1038 2022-03-16 08:59:56.000000 vitrage-8.0.1/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.502531 vitrage-8.0.1/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1743 2022-03-16 08:59:56.000000 vitrage-8.0.1/devstack/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2022-03-16 08:59:56.000000 vitrage-8.0.1/devstack/apache-vitrage.template
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2022-03-16 08:59:56.000000 vitrage-8.0.1/devstack/override-defaults
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13231 2022-03-16 08:59:56.000000 vitrage-8.0.1/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1525 2022-03-16 08:59:56.000000 vitrage-8.0.1/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.502531 vitrage-8.0.1/devstack/upgrade/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2022-03-16 08:59:56.000000 vitrage-8.0.1/devstack/upgrade/settings
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1122 2022-03-16 08:59:56.000000 vitrage-8.0.1/devstack/upgrade/shutdhown.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3315 2022-03-16 08:59:56.000000 vitrage-8.0.1/devstack/upgrade/upgrade.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.502531 vitrage-8.0.1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.502531 vitrage-8.0.1/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.502531 vitrage-8.0.1/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.502531 vitrage-8.0.1/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/cli/vitrage-purge-data.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/cli/vitrage-status.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2952 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.502531 vitrage-8.0.1/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      828 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.506532 vitrage-8.0.1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11711 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/add-new-datasource.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4866 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/alarm-severity-config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1025 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/cetus_datasource.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3149 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3602 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/datasource-snmp-parsing-support.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/devstack-installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16929 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/entity_equivalence_use_cases.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4010 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/high-scale.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/host_high_memory_consumption.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.510532 vitrage-8.0.1/doc/source/contributor/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   205286 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/images/add_aodh_alarm_flow.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13261 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/images/add_aodh_alarm_graph.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   221898 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/images/add_nova_instance_flow.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13562 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/images/add_nova_instance_graph.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26304 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/images/complex_rca_graph.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   234474 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/images/low_level_design.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   216665 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/images/nagios_causes_deduced_flow.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20911 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/images/nagios_causes_deduced_graph.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   125468 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/images/osprofiler-html-output.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   197574 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/images/rca_flow.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19438 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/images/rca_graph.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    99836 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/images/vitrage-ha-vision.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   172861 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/images/vitrage_graph_architecture.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1861 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/k8s_datasource.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3098 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/kapacitor-datasource.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/keycloak-config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49512 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual-tests.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.510532 vitrage-8.0.1/doc/source/contributor/manual_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/switch_and_nic.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.514532 vitrage-8.0.1/doc/source/contributor/manual_tests/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v1_template.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v2_definition_template.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v2_equivalence.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1809 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v2_high_cpu_load.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v2_host_down.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v2_with_include.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v2_with_invalid_include.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      885 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v2_with_params.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v2_wrong.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v3_execute_mistral.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v3_high_mem_consumption.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      466 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v3_with_default_params.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v3_with_params.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/test_web_server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/manual_tests/workflow1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/mistral-config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/ml-jaccard_correlation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4038 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/nagios-config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2898 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/nagios-devstack-installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7156 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/not_operator_support.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10486 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/not_operator_support_v2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3807 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/notifier-snmp-plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3394 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/notifier-webhook-plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/nova-config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1133 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/nova-notifier.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/profiler-config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4764 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/prometheus-datasource.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5195 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/resource-state-config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10166 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/scenario-evaluator.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4019 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/static-config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16208 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/template_validation_status_code.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5923 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/templates-loading-v2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6067 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/templates-loading.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1127 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/tmfapi639-datasource.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50462 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/vitrage-api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4578 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/vitrage-first_steps.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4288 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/vitrage-graph-design.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9772 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/vitrage-ha-and-history-vision.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25954 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/vitrage-template-format-v2.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20962 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/vitrage-templates.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2940 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/vitrage-use-cases.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3713 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/zabbix_vitrage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/contributor/zaqar_notifier.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3381 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.514532 vitrage-8.0.1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      957 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/install/get_started.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5527 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/install/install-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/install/install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/install/next-steps.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2022-03-16 08:59:56.000000 vitrage-8.0.1/doc/source/install/verify.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.486531 vitrage-8.0.1/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.514532 vitrage-8.0.1/etc/vitrage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/README-vitrage.conf.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1952 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/api-paste.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.518532 vitrage-8.0.1/etc/vitrage/datasources_values/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/aodh.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/cetus.cluster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/cetus.pod.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1120 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/cinder.volume.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/collectd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/default.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/doctor.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1372 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/heat.stack.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/kapacitor.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/monasca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/nagios.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/network.interface.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/neutron.network.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/neutron.port.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/nova.host.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/nova.instance.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/nova.zone.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/openstack.cluster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/prometheus.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/static.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/static_physical.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/switch.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/trove.cluster.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/trove.instance.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/vitrage.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/datasources_values/zabbix.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.518532 vitrage-8.0.1/etc/vitrage/templates.sample/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2675 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/templates.sample/database_cluster_capacity_autoscaling.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1859 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/templates.sample/host_down_scenarios.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1868 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/templates.sample/host_high_cpu_load_scenarios.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/vitrage-config-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2022-03-16 08:59:56.000000 vitrage-8.0.1/etc/vitrage/vitrage-policy-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2022-03-16 08:59:56.000000 vitrage-8.0.1/initial.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.486531 vitrage-8.0.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.530532 vitrage-8.0.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/SNMP_notifier-5c46505b3043b58f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/Vitrage_ID-93737ff7b7ced8e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/add-upgrade-check-framework-166ba1c7e266953e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/add_service_list-d8e28adabc26f1cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/add_status-c5b13941c3ce978e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/add_template_versions-5476a446705b43d2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/add_zaqar_notifier-63de714384091ce5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/alarm-and-rca-history-0c4c513c98fdc426.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/alarm_count_api-057138c8e0a36443.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/aodh_extended_alarm_support-327bb589311da440.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/aodh_gnocchi_thresh_alarm-a529ec4f50f3cb0c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/cetus-datasource-0c8297005ac6ca92.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/cinder-default-version-9dfcb941996e32ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/collectd-datasource-a730f06aff840c8f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/collector-cache-limitations-4eedef1c7664f5b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/collector-removal-fd805c6298d66eb0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/collector-service-5848f96896f97d50.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/database-migrations-ffca2f9f3283f2a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/datasource-scaffold-2f5ee6f0d9f83099.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/definition_templates-6c2c10bb3e6912a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/deprecate-json-formatted-policy-file-6a1e9b690fdbc132.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/deprecate-keystone_client-region-option-b3f30100370a5471.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/deprecate-static-physical-datasource-ab0094620c05d0ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/doctor-datasource-59ee5b2afb677ab4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/drop-py-2-7-6add89c8aeb58399.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/entity-equivalence-44c0da4cf3b5bc7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/event_persistor-1b0b4563cc219915.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/graph-fast-failover-e2d0a62f18ab27f7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/health-check-api-19f180a104c7fa29.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/improve_tempest_tests-3e77197dfae4ad62.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/introduce-template-version-55bca9fc4e7d138f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/kapacitor_datasource-c0c9563bb52ff1f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/keycloak_auth_support-cf8c2c504b3ddd5b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/kubernetes-datasource-12af0f9caac1b21b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/machine_learning_service-da9700e6c6fa61b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/mock-datasource-1c9b427bc16f4a59.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1123 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/monasca-datasource-9ca61922ef14c2a8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/multi_tenancy_support-feb3d2d4f8014b66.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/nested_stacks-fddbfa1f79b2ef43.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/not_operator_for_templates-f1e4c517236ca54e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/nova-versioned-notifications-3c5ff450b9fe69f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/ocata-prelude-9b64d68bc898f7ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/osprofiler-784098daab42a150.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/parallel_evaluation-db8660ef3ff5b864.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/performance-bug-fixes-a2b5e85ee37bba93.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/persist_overlapping_scenarios-d426dffdf3d11094.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/policies-in-code-dd3f1490f7f5b3eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/prometheus-enhancement-b9dc2ef5705d1000.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/prometheus_datasource-65c72bc8e7ec7622.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/queens-prelude-a00e64274e8e64be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/refactor-execute-mistral-action-fc0fac84c07e1784.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/remove-static-physical-datasource-e8e70158f453cff1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/remove_end_messages-e92e7b41a52c61cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/resource_count-1e3184e5f1f413ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/resource_list_query-b3fbcbe01090f64a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/rewrite-aodh-datasource-4968c32c1c5b81f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/rocky-prelude-24ec92aedd5d8266.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/services-management-improvements-899c011e57002e84.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      223 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/snmp_parsing-1a5c4645ce832ee3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/sql_integration-c33342d100492ceb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/static-datasource-changes-914f9a16ad7e46ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/static-datasource-refactoring-2cc7569fafbe65c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/stein-prelude-5e6f583803807d84.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/support-aodh-notifications-cc495f3bc137099d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/support-get-changes-in-static-datasource-02715226f103455d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/support-mistral-13618b516699a1c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/support-networkx-version-2-8d47034b6b278137.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/support-template-functions-dcb2d2e1e63e9a5d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/support-template-parameters-f9552fef4fc66122.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/support_alarm_show_api-0b001dd185e2e523.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/support_high_scale-fa1053f06954aed7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/support_mark_down_for_instance-179b04c693f17787.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/support_overwrite_when_adding_template-f6795771ae0eff8e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/support_template_show_and_add_by_name-a73455f462175160.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/template-type-4587ad6a39130170.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/template_crud-91baea2ed68291f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/template_regex-8cb58f5e4438c11a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/template_version_3-cd8a0775b2f2e7cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/tmfapi639_datasource-bcae9474430ae5a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/trove-datasource-2aa7a88ff20aff8c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/notes/webhooks-139aeaaab7119302.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.530532 vitrage-8.0.1/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.530532 vitrage-8.0.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.530532 vitrage-8.0.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/source/_templates/.placeholder
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2661 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      885 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-03-16 08:59:56.000000 vitrage-8.0.1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1355 2022-03-16 08:59:56.000000 vitrage-8.0.1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2293 2022-03-16 09:00:27.622536 vitrage-8.0.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-03-16 08:59:56.000000 vitrage-8.0.1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2022-03-16 08:59:56.000000 vitrage-8.0.1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.530532 vitrage-8.0.1/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.530532 vitrage-8.0.1/tools/datasource-scaffold/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/datasource-scaffold/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/datasource-scaffold/cookiecutter.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/datasource-scaffold/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.534533 vitrage-8.0.1/tools/datasource-scaffold/sample/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1820 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/datasource-scaffold/sample/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1855 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/datasource-scaffold/sample/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2558 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/datasource-scaffold/sample/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.534533 vitrage-8.0.1/tools/datasource-scaffold/{{cookiecutter.name}}/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2031 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/datasource-scaffold/{{cookiecutter.name}}/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1985 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/datasource-scaffold/{{cookiecutter.name}}/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2897 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/datasource-scaffold/{{cookiecutter.name}}/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.534533 vitrage-8.0.1/tools/load_generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/load_generator/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11806 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/load_generator/computes.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5389 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/load_generator/load_generator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8583 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/load_generator/notification_info.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.534533 vitrage-8.0.1/tools/load_generator/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2165 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/load_generator/templates/port_0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2165 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/load_generator/templates/port_1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2165 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/load_generator/templates/port_2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2164 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/load_generator/templates/port_3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2165 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/load_generator/templates/port_4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/load_generator/templates/vm_0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/load_generator/templates/vm_1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/load_generator/templates/vm_2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/load_generator/templates/vm_3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2022-03-16 08:59:56.000000 vitrage-8.0.1/tools/load_generator/templates/vm_4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2670 2022-03-16 08:59:56.000000 vitrage-8.0.1/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.534533 vitrage-8.0.1/vitrage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.538533 vitrage-8.0.1/vitrage/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4522 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/app.wsgi
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.538533 vitrage-8.0.1/vitrage/api/controllers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1420 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/rest.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1103 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/root.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.538533 vitrage-8.0.1/vitrage/api/controllers/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2404 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/v1/alarm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3157 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/v1/alarm_base.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2999 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/v1/count.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2246 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/v1/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/v1/history.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2249 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/v1/rca.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4220 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/v1/resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/v1/root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1647 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/v1/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1381 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/v1/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9160 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/v1/template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5294 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/v1/topology.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4740 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/controllers/v1/webhook.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4039 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/hooks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api/policy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.538533 vitrage-8.0.1/vitrage/api_handler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api_handler/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.542533 vitrage-8.0.1/vitrage/api_handler/apis/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api_handler/apis/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5709 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api_handler/apis/alarm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4616 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api_handler/apis/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2758 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api_handler/apis/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api_handler/apis/operational.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3062 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api_handler/apis/rca.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api_handler/apis/resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4944 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api_handler/apis/template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8272 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api_handler/apis/topology.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5459 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/api_handler/apis/webhook.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.542533 vitrage-8.0.1/vitrage/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/cli/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/cli/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1371 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/cli/graph.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/cli/machine_learning.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/cli/notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/cli/persistor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      931 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/cli/snmp_parsing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1278 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/cli/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1892 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/cli/storage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.542533 vitrage-8.0.1/vitrage/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2318 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5961 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1186 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/exception.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.542533 vitrage-8.0.1/vitrage/common/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1274 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3030 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/policies/alarms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1023 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/policies/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1343 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/policies/rca.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2577 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/policies/resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/policies/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1031 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/policies/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2166 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/policies/template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/policies/topology.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2286 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/policies/webhook.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4719 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/common/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.542533 vitrage-8.0.1/vitrage/coordination/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/coordination/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3992 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/coordination/coordination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/coordination/service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.546533 vitrage-8.0.1/vitrage/datasources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2358 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4899 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/alarm_driver_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/alarm_properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2410 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/alarm_transformer_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.546533 vitrage-8.0.1/vitrage/datasources/aodh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1683 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/aodh/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14147 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/aodh/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/aodh/properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6720 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/aodh/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.546533 vitrage-8.0.1/vitrage/datasources/ceilometer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1785 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/ceilometer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14986 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/ceilometer/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1690 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/ceilometer/properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6882 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/ceilometer/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.546533 vitrage-8.0.1/vitrage/datasources/cetus/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/cetus/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/cetus/cetus_driver_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.546533 vitrage-8.0.1/vitrage/datasources/cetus/cluster/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1609 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/cetus/cluster/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1722 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/cetus/cluster/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3863 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/cetus/cluster/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.546533 vitrage-8.0.1/vitrage/datasources/cetus/pod/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1577 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/cetus/pod/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1418 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/cetus/pod/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3777 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/cetus/pod/transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/cetus/properties.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.546533 vitrage-8.0.1/vitrage/datasources/cinder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/cinder/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.546533 vitrage-8.0.1/vitrage/datasources/cinder/volume/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1617 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/cinder/volume/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2381 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/cinder/volume/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/cinder/volume/properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7509 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/cinder/volume/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.546533 vitrage-8.0.1/vitrage/datasources/collectd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/collectd/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.550533 vitrage-8.0.1/vitrage/datasources/collectd/collectd_vitrage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/collectd/collectd_vitrage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/collectd/collectd_vitrage/getsigchld.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5179 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/collectd/collectd_vitrage/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1259 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/collectd/collectd_vitrage/readme
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4170 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/collectd/collectd_vitrage/vitrageplugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3887 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/collectd/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1947 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/collectd/mapper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      878 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/collectd/properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4587 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/collectd/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.550533 vitrage-8.0.1/vitrage/datasources/consistency/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      609 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/consistency/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2251 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/consistency/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.550533 vitrage-8.0.1/vitrage/datasources/doctor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/doctor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4625 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/doctor/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/doctor/properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4142 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/doctor/transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4459 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/driver_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.550533 vitrage-8.0.1/vitrage/datasources/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/heat/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.550533 vitrage-8.0.1/vitrage/datasources/heat/stack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1588 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/heat/stack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5719 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/heat/stack/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/heat/stack/properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5854 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/heat/stack/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.550533 vitrage-8.0.1/vitrage/datasources/kapacitor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1696 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/kapacitor/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.550533 vitrage-8.0.1/vitrage/datasources/kapacitor/auxiliary/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3448 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/kapacitor/auxiliary/kapacitor_vitrage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3242 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/kapacitor/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3396 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/kapacitor/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      943 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/kapacitor/properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4179 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/kapacitor/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.550533 vitrage-8.0.1/vitrage/datasources/kubernetes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1823 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/kubernetes/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2671 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/kubernetes/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/kubernetes/properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4313 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/kubernetes/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.550533 vitrage-8.0.1/vitrage/datasources/monasca/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1817 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/monasca/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2553 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/monasca/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      907 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/monasca/properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3487 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/monasca/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.550533 vitrage-8.0.1/vitrage/datasources/nagios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2078 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nagios/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3041 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nagios/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3738 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nagios/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4436 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nagios/parser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nagios/properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3910 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nagios/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.554533 vitrage-8.0.1/vitrage/datasources/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/neutron/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/neutron/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.554533 vitrage-8.0.1/vitrage/datasources/neutron/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1614 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/neutron/network/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1856 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/neutron/network/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4657 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/neutron/network/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.554533 vitrage-8.0.1/vitrage/datasources/neutron/port/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1564 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/neutron/port/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2199 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/neutron/port/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7103 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/neutron/port/transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1180 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/neutron/properties.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.554533 vitrage-8.0.1/vitrage/datasources/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nova/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.554533 vitrage-8.0.1/vitrage/datasources/nova/host/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1546 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nova/host/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1214 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nova/host/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3403 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nova/host/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.554533 vitrage-8.0.1/vitrage/datasources/nova/instance/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1604 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nova/instance/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4991 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nova/instance/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3184 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nova/instance/field_extractor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5708 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nova/instance/transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nova/nova_driver_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nova/properties.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.554533 vitrage-8.0.1/vitrage/datasources/nova/zone/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1576 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nova/zone/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1400 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nova/zone/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5426 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/nova/zone/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.554533 vitrage-8.0.1/vitrage/datasources/prometheus/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2090 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/prometheus/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15542 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/prometheus/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1821 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/prometheus/properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4237 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/prometheus/transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/resource_transformer_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.554533 vitrage-8.0.1/vitrage/datasources/static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4524 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/static/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7444 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/static/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4634 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/static/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.554533 vitrage-8.0.1/vitrage/datasources/tmfapi639/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1974 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/tmfapi639/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1866 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/tmfapi639/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3293 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/tmfapi639/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3482 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/tmfapi639/transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12953 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/transformer_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.558534 vitrage-8.0.1/vitrage/datasources/trove/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/trove/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.558534 vitrage-8.0.1/vitrage/datasources/trove/cluster/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1847 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/trove/cluster/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1930 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/trove/cluster/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3436 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/trove/cluster/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.558534 vitrage-8.0.1/vitrage/datasources/trove/instance/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1854 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/trove/instance/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1814 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/trove/instance/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3265 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/trove/instance/transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/trove/properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3511 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/trove/trove_driver_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1624 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.558534 vitrage-8.0.1/vitrage/datasources/zabbix/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2064 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/zabbix/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.558534 vitrage-8.0.1/vitrage/datasources/zabbix/auxiliary/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/zabbix/auxiliary/readme
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3710 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/zabbix/auxiliary/zabbix_vitrage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7007 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/zabbix/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1678 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/zabbix/properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4973 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/datasources/zabbix/transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.558534 vitrage-8.0.1/vitrage/entity_graph/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1555 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.558534 vitrage-8.0.1/vitrage/entity_graph/consistency/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/consistency/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6054 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/consistency/consistency_enforcer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6877 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/driver_exec.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8349 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/graph_init.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4345 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/graph_persistency.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.558534 vitrage-8.0.1/vitrage/entity_graph/mappings/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/mappings/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1509 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/mappings/alarm_handler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10450 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/mappings/datasource_info_mapper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/mappings/handler_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/mappings/operational_alarm_severity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/mappings/operational_resource_state.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1574 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/mappings/resource_handler.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.562534 vitrage-8.0.1/vitrage/entity_graph/processor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/processor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1037 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/processor/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8954 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/processor/notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15733 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/processor/processor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3462 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/processor/processor_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3496 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/processor/transformer_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2977 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14393 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/entity_graph/workers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.562534 vitrage-8.0.1/vitrage/evaluator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      931 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.562534 vitrage-8.0.1/vitrage/evaluator/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      903 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/actions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6657 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/actions/action_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1059 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/actions/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7696 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/actions/evaluator_event_transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2741 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/actions/notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1972 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/actions/priority_tools.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.562534 vitrage-8.0.1/vitrage/evaluator/actions/recipes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/actions/recipes/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/actions/recipes/action_steps.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2260 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/actions/recipes/add_causal_relationship.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1673 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/actions/recipes/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/actions/recipes/execute_mistral.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2222 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/actions/recipes/mark_down.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2511 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/actions/recipes/raise_alarm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/actions/recipes/set_state.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1192 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6078 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/condition.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/equivalence_repository.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26439 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/scenario_evaluator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8342 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/scenario_repository.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3076 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_data.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.562534 vitrage-8.0.1/vitrage/evaluator/template_db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5292 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_db/template_repository.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1181 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_fields.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.562534 vitrage-8.0.1/vitrage/evaluator/template_functions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_functions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2644 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_functions/function_resolver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.562534 vitrage-8.0.1/vitrage/evaluator/template_functions/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1691 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_functions/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5471 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_functions/v2/functions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.566534 vitrage-8.0.1/vitrage/evaluator/template_loading/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_loading/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2269 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_loading/equivalence_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_loading/props_converter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7109 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_loading/scenario_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3245 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_loading/subgraph_builder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6308 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_loading/template_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5753 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_loading/template_loader_v3.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.566534 vitrage-8.0.1/vitrage/evaluator/template_loading/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_loading/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1327 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_loading/v1/action_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_loading/v1/execute_mistral_loader.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.566534 vitrage-8.0.1/vitrage/evaluator/template_loading/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_loading/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1514 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_loading/v3/action_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_loading/v3/raise_alarm_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1307 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_schema_factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6042 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_schemas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.566534 vitrage-8.0.1/vitrage/evaluator/template_validation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3102 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1772 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.566534 vitrage-8.0.1/vitrage/evaluator/template_validation/content/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2722 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4250 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/template_content_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5226 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/template_content_validator_v3.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.566534 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2785 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/add_causal_relationship_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8241 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/definitions_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1837 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/execute_mistral_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1563 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/get_param_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/mark_down_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1054 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/metadata_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2083 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/raise_alarm_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7286 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/scenario_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1902 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/set_state_validator.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.570534 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2285 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v2/execute_mistral_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1505 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v2/get_param_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1565 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/content/v2/metadata_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5745 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/status_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11734 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/template_syntax_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4580 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/evaluator/template_validation/template_syntax_validator_v3.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.570534 vitrage-8.0.1/vitrage/graph/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/graph/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.570534 vitrage-8.0.1/vitrage/graph/algo_driver/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/graph/algo_driver/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3101 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/graph/algo_driver/algorithm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7507 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/graph/algo_driver/networkx_algorithm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12077 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/graph/algo_driver/sub_graph_matching.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.570534 vitrage-8.0.1/vitrage/graph/driver/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/graph/driver/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5063 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/graph/driver/elements.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12340 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/graph/driver/graph.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13096 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/graph/driver/networkx_graph.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2270 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/graph/driver/notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1641 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/graph/filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3502 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/graph/query.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4466 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/graph/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.570534 vitrage-8.0.1/vitrage/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5180 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3738 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/keystone_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.570534 vitrage-8.0.1/vitrage/machine_learning/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/machine_learning/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.570534 vitrage-8.0.1/vitrage/machine_learning/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/machine_learning/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      807 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/machine_learning/plugins/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.570534 vitrage-8.0.1/vitrage/machine_learning/plugins/jaccard_correlation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1430 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/machine_learning/plugins/jaccard_correlation/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1930 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/machine_learning/plugins/jaccard_correlation/accumulation_persistor_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2958 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/machine_learning/plugins/jaccard_correlation/alarm_data_accumulator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3756 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/machine_learning/plugins/jaccard_correlation/alarm_processor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3146 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/machine_learning/plugins/jaccard_correlation/correlation_collection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4510 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/machine_learning/plugins/jaccard_correlation/correlation_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3204 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/machine_learning/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2857 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/messaging.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.570534 vitrage-8.0.1/vitrage/middleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/middleware/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5361 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/middleware/basic_and_keystone_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7662 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/middleware/keycloak.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.570534 vitrage-8.0.1/vitrage/notifier/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.570534 vitrage-8.0.1/vitrage/notifier/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.574534 vitrage-8.0.1/vitrage/notifier/plugins/aodh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/aodh/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3734 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/aodh/aodh_notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1039 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.574534 vitrage-8.0.1/vitrage/notifier/plugins/mistral/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/mistral/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2722 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/mistral/mistral_notifier.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.574534 vitrage-8.0.1/vitrage/notifier/plugins/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/nova/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2933 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/nova/nova_notifier.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.574534 vitrage-8.0.1/vitrage/notifier/plugins/snmp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1391 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/snmp/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/snmp/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2852 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/snmp/snmp_notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6969 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/snmp/snmp_sender.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.574534 vitrage-8.0.1/vitrage/notifier/plugins/webhook/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      973 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/webhook/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/webhook/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6440 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/webhook/webhook.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.574534 vitrage-8.0.1/vitrage/notifier/plugins/zaqar/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/zaqar/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1373 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/plugins/zaqar/zaqar_notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3795 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/notifier/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4214 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7714 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/os_clients.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.574534 vitrage-8.0.1/vitrage/persistency/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/persistency/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8015 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/persistency/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3164 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/rpc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.574534 vitrage-8.0.1/vitrage/snmp_parsing/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/snmp_parsing/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      689 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/snmp_parsing/properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6415 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/snmp_parsing/service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.574534 vitrage-8.0.1/vitrage/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1932 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8354 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/storage/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18087 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/storage/history_facade.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17640 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/storage/impl_sqlalchemy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.574534 vitrage-8.0.1/vitrage/storage/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/storage/sqlalchemy/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.574534 vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3021 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1084 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/alembic.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.574534 vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/alembic_migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/alembic_migrations/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/alembic_migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2369 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/alembic_migrations/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/alembic_migrations/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.578534 vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/alembic_migrations/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9428 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/alembic_migrations/versions/4e44c9414dff_initial_migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/alembic_migrations/versions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10796 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/storage/sqlalchemy/models.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.578534 vitrage-8.0.1/vitrage/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4909 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.578534 vitrage-8.0.1/vitrage/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.578534 vitrage-8.0.1/vitrage/tests/functional/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6820 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api/test_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.578534 vitrage-8.0.1/vitrage/tests/functional/api/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2591 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api/v1/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6961 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api/v1/test_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1297 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api/v1/test_health.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4508 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api/v1/test_keycloak.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5877 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api/v1/test_noauth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3122 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api/v1/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2598 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api/v1/test_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1536 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api/v1/test_template_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.578534 vitrage-8.0.1/vitrage/tests/functional/api_handler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api_handler/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    29960 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api_handler/test_apis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12220 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api_handler/test_templates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2778 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api_handler/test_templates_v2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2485 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/api_handler/test_templates_v3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2389 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.578534 vitrage-8.0.1/vitrage/tests/functional/datasources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.578534 vitrage-8.0.1/vitrage/tests/functional/datasources/aodh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/aodh/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4063 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/aodh/test_aodh.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.578534 vitrage-8.0.1/vitrage/tests/functional/datasources/ceilometer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/ceilometer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4102 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/ceilometer/test_ceilometer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.578534 vitrage-8.0.1/vitrage/tests/functional/datasources/cinder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/cinder/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3922 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/cinder/test_cinder_volume.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.578534 vitrage-8.0.1/vitrage/tests/functional/datasources/collectd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/collectd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9277 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/collectd/test_collectd.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.582535 vitrage-8.0.1/vitrage/tests/functional/datasources/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/heat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4189 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/heat/test_heat_stack.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.582535 vitrage-8.0.1/vitrage/tests/functional/datasources/listener_service/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/listener_service/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2416 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/listener_service/test_listener_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.582535 vitrage-8.0.1/vitrage/tests/functional/datasources/nagios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/nagios/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3734 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/nagios/test_nagios.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.582535 vitrage-8.0.1/vitrage/tests/functional/datasources/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/neutron/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/neutron/test_neutron_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/neutron/test_neutron_port.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.582535 vitrage-8.0.1/vitrage/tests/functional/datasources/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/nova/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/nova/test_nova_datasources.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.582535 vitrage-8.0.1/vitrage/tests/functional/datasources/trove/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/trove/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3645 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/datasources/trove/test_trove_instance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.582535 vitrage-8.0.1/vitrage/tests/functional/entity_graph/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/entity_graph/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.582535 vitrage-8.0.1/vitrage/tests/functional/entity_graph/consistency/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/entity_graph/consistency/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14775 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/entity_graph/consistency/test_consistency.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.582535 vitrage-8.0.1/vitrage/tests/functional/entity_graph/graph_persistor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/entity_graph/graph_persistor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4018 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/entity_graph/graph_persistor/test_graph_persistor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.582535 vitrage-8.0.1/vitrage/tests/functional/entity_graph/processor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/entity_graph/processor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1605 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/entity_graph/processor/test_processor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.582535 vitrage-8.0.1/vitrage/tests/functional/entity_graph/states/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/entity_graph/states/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2639 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/entity_graph/states/test_datasource_info_mapper.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.582535 vitrage-8.0.1/vitrage/tests/functional/evaluator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/evaluator/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15003 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/evaluator/test_action_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    71082 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/evaluator/test_scenario_evaluator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2629 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/functional/test_configuration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.582535 vitrage-8.0.1/vitrage/tests/mocks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/mocks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1416 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/mocks/entity_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8308 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/mocks/graph_generator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22849 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/mocks/mock_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.586535 vitrage-8.0.1/vitrage/tests/mocks/mock_graph_datasource/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2079 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/mocks/mock_graph_datasource/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4320 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/mocks/mock_graph_datasource/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/mocks/mock_graph_datasource/transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8860 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/mocks/mock_transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29737 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/mocks/trace_generator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4597 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/mocks/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.494531 vitrage-8.0.1/vitrage/tests/resources/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.586535 vitrage-8.0.1/vitrage/tests/resources/datasources_values/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/datasources_values/default.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.586535 vitrage-8.0.1/vitrage/tests/resources/datasources_values/erroneous_values/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/datasources_values/erroneous_values/default.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/datasources_values/erroneous_values/nagios.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/datasources_values/erroneous_values/nova.host.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1552 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/datasources_values/erroneous_values/nova.instance.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/datasources_values/nagios.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/datasources_values/nova.host.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/datasources_values/nova.instance.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/datasources_values/nova.zone.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/datasources_values/vitrage.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.586535 vitrage-8.0.1/vitrage/tests/resources/kapacitor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/kapacitor/kapacitor_conf.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.586535 vitrage-8.0.1/vitrage/tests/resources/kubernetes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/kubernetes/kubernetes_config.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.494531 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.590535 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_aodh_update_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_collectd_update_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_consistency_update_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_doctor_update_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_host_snapshot_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4611 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_inst_snapshot_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_inst_snapshot_static.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_inst_update_legacy_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3829 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_inst_update_versioned_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_kapacitor_update_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_kubernetes_snapshot_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_nagios_snapshot_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_nagios_snapshot_static.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5366 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_prometheus_update_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_stack_snapshot_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1175 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_stack_update_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_static_snapshot_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_static_snapshot_static.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      453 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_trove_cluster_snapshot_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_trove_instance_snapshot_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_volume_snapshot_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_volume_update_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_zabbix_snapshot_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_zone_snapshot_dynamic.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.590535 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/edges/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/edges/attached.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/edges/contains.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/edges/on.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.590535 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1290 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_aodh_snapshot_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1289 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_aodh_update_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_collectd_update_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_doctor_update_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_host_snapshot_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_host_snapshot_static.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_inst_snapshot_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_inst_snapshot_static.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_kapacitor_update_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_prometheus_update_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_zone_snapshot_dynamic.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_zone_snapshot_static.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.590535 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      612 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/cinder.volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/neutron.network.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/neutron.port.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/nova.host.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/nova.instance.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/nova.zone.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/openstack-cluster.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/tripleo.controller.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/vitrage.alarm.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/zabbix.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.590535 vitrage-8.0.1/vitrage/tests/resources/nagios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26541 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/nagios/nagios-mock.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/nagios/nagios_conf.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.594535 vitrage-8.0.1/vitrage/tests/resources/prometheus/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/prometheus/prometheus_conf.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.594535 vitrage-8.0.1/vitrage/tests/resources/snmp_notifier/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/snmp_notifier/alarm_oid_mapping.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/snmp_notifier/dests.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/snmp_notifier/oid_tree_with_severity_mapping.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/snmp_notifier/oid_tree_without_severity_mapping.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.594535 vitrage-8.0.1/vitrage/tests/resources/snmp_parsing/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/snmp_parsing/snmp_parsing_conf.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.594535 vitrage-8.0.1/vitrage/tests/resources/static_datasources/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.594535 vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.594535 vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/added_resources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/added_resources/static.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.594535 vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/baseline/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/baseline/static.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.594535 vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/changed_resources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/changed_resources/static.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.594535 vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/deleted_resources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/deleted_resources/static.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.594535 vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/mixed_changes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/mixed_changes/static.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/switch_to_host_datasource.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/switch_to_switch_datasource.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1318 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/static_datasources/switch_to_host.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/static_datasources/switch_to_host_datasource.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/static_datasources/switch_to_switch_datasource.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.494531 vitrage-8.0.1/vitrage/tests/resources/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.594535 vitrage-8.0.1/vitrage/tests/resources/templates/consistency/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/consistency/deduced_alarm_on_instance.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.494531 vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.594535 vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/definition_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/definition_templates/basic_def_template.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1081 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/definition_templates/large_def_template.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/definition_templates/single_entity.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/definition_templates/with_include.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/definition_templates/with_scenarios.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.594535 vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/templates/basic_with_include.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/templates/basic_with_include_that_doesnt_exist.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/templates/basic_with_two_includes.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/templates/include_with_empty_name.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      399 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/templates/no_definitions_only_include.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      976 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/templates/only_using_def_template_definitions.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/templates/with_conflicting_include_entities.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.494531 vitrage-8.0.1/vitrage/tests/resources/templates/equivalences_dup/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.594535 vitrage-8.0.1/vitrage/tests/resources/templates/equivalences_dup/dup-in-multi-def/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/equivalences_dup/dup-in-multi-def/multi.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.594535 vitrage-8.0.1/vitrage/tests/resources/templates/equivalences_dup/dup-in-multi-file/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/equivalences_dup/dup-in-multi-file/first.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/equivalences_dup/dup-in-multi-file/second.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.598535 vitrage-8.0.1/vitrage/tests/resources/templates/equivalences_dup/dup-in-one-def/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/equivalences_dup/dup-in-one-def/one.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.598535 vitrage-8.0.1/vitrage/tests/resources/templates/equivalent_scenarios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/equivalent_scenarios/basic.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.598535 vitrage-8.0.1/vitrage/tests/resources/templates/equivalent_scenarios/equivalences/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/equivalent_scenarios/equivalences/basic.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.598535 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      850 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/causal_basic.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1167 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/complex_and_or_operator_deduced_alarm.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1571 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/complex_not_operator_deduced_alarm.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.598535 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1266 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/complex1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/complex2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1273 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/complex_not.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1289 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/complex_not_unsupported.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/not_edge_unsupported.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1025 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/not_or_unsupported.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/not_or_unsupported2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/one_edge.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/one_vertex.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/simple_and.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1191 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/simple_and2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/simple_or.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/simple_or2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/simple_or3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1259 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/simple_or_unsupported.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1486 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/deduced_alarm.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1117 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/deduced_state.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1250 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/deduced_state_2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/high_availability.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/simple_not_operator_deduced_alarm.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/simple_or_operator_deduced_alarm.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.598535 vitrage-8.0.1/vitrage/tests/resources/templates/general/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/general/bad_yaml.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/general/basic.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.598535 vitrage-8.0.1/vitrage/tests/resources/templates/general/equivalences/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/general/equivalences/basic.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1497 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/general/host_high_cpu_load_to_instance_cpu_suboptimal.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.602535 vitrage-8.0.1/vitrage/tests/resources/templates/not_operator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/not_operator/basic_correct_not_condition.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/not_operator/basic_incorrect_not_condition.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/not_operator/complicated_correct_not_condition.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/not_operator/complicated_incorrect_not_condition.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.602535 vitrage-8.0.1/vitrage/tests/resources/templates/parameters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1001 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/parameters/v2_with_extra_param_def.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/parameters/v2_with_missing_param_def.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      885 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/parameters/v2_with_params.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/parameters/v2_without_params.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/parameters/v3_with_extra_param_def.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      511 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/parameters/v3_with_missing_param_def.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/parameters/v3_with_params.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.602535 vitrage-8.0.1/vitrage/tests/resources/templates/regex/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/regex/basic_regex.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/regex/basic_regex_for_fail.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/regex/faulty_regex.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/regex/regex_for_exact_match.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.602535 vitrage-8.0.1/vitrage/tests/resources/templates/v3_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1567 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/v3_templates/valid_actions.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/v3_templates/valid_conditions.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.602535 vitrage-8.0.1/vitrage/tests/resources/templates/version/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/version/invalid_version.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/version/no_version.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.602535 vitrage-8.0.1/vitrage/tests/resources/templates/version/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/version/v1/v1_execute_mistral.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/version/v1/version1.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.602535 vitrage-8.0.1/vitrage/tests/resources/templates/version/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      667 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/version/v2/v2_execute_mistral.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/version/v2/v2_standard.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/templates/version/v2/v2_with_func.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.602535 vitrage-8.0.1/vitrage/tests/resources/zabbix/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/resources/zabbix/zabbix_conf.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.602535 vitrage-8.0.1/vitrage/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.602535 vitrage-8.0.1/vitrage/tests/unit/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/cli/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1186 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/cli/test_status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.602535 vitrage-8.0.1/vitrage/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2808 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/common/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.606536 vitrage-8.0.1/vitrage/tests/unit/datasources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.606536 vitrage-8.0.1/vitrage/tests/unit/datasources/aodh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/aodh/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5517 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/aodh/aodh_transformer_base_test.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/aodh/mock_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35245 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/aodh/test_aodh_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6231 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/aodh/test_aodh_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.606536 vitrage-8.0.1/vitrage/tests/unit/datasources/ceilometer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/ceilometer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5634 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/ceilometer/ceilometer_transformer_base_test.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/ceilometer/mock_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15691 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/ceilometer/test_ceilometer_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6500 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/ceilometer/test_ceilometer_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.606536 vitrage-8.0.1/vitrage/tests/unit/datasources/cetus/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/cetus/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7407 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/cetus/test_cetus_cluster_transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7199 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/cetus/test_cetus_pod_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.606536 vitrage-8.0.1/vitrage/tests/unit/datasources/cinder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/cinder/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9674 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/cinder/test_cinder_volume_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.606536 vitrage-8.0.1/vitrage/tests/unit/datasources/collectd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/collectd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3203 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/collectd/test_collectd_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4748 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/collectd/test_collectd_transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3118 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/collectd/test_mapper.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.606536 vitrage-8.0.1/vitrage/tests/unit/datasources/consistency/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/consistency/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3911 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/consistency/test_consistency_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.606536 vitrage-8.0.1/vitrage/tests/unit/datasources/doctor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/doctor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5072 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/doctor/test_doctor_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4753 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/doctor/test_doctor_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.606536 vitrage-8.0.1/vitrage/tests/unit/datasources/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/heat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9278 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/heat/test_heat_stack_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.606536 vitrage-8.0.1/vitrage/tests/unit/datasources/kapacitor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/kapacitor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3530 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/kapacitor/test_kapacitor_configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4533 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/kapacitor/test_kapacitor_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7182 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/kapacitor/test_kapacitor_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.606536 vitrage-8.0.1/vitrage/tests/unit/datasources/kubernetes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6600 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/kubernetes/test_kubernetes_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.610536 vitrage-8.0.1/vitrage/tests/unit/datasources/nagios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/nagios/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1563 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/nagios/mock_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1625 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/nagios/nagios_base_test.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8277 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/nagios/test_nagios_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23434 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/nagios/test_nagios_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3244 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/nagios/test_nagios_parser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8290 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/nagios/test_nagios_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.610536 vitrage-8.0.1/vitrage/tests/unit/datasources/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/neutron/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.610536 vitrage-8.0.1/vitrage/tests/unit/datasources/neutron/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/neutron/network/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/neutron/network/test_neutron_network_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.610536 vitrage-8.0.1/vitrage/tests/unit/datasources/neutron/port/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/neutron/port/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/neutron/port/test_neutron_port_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.610536 vitrage-8.0.1/vitrage/tests/unit/datasources/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/nova/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9942 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/nova/base_nova_instance_transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2050 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/nova/test_instance_transformer_legacy_notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5020 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/nova/test_instance_transformer_snapshot_events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/nova/test_instance_transformer_versioned_notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9001 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/nova/test_nova_host_transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3120 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/nova/test_nova_instance_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10187 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/nova/test_nova_zone_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.610536 vitrage-8.0.1/vitrage/tests/unit/datasources/prometheus/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/prometheus/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8442 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/prometheus/test_prometheus_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6042 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/prometheus/test_prometheus_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.610536 vitrage-8.0.1/vitrage/tests/unit/datasources/static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/static/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8180 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/static/test_static_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5948 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/static/test_static_transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4500 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/test_alarm_transformer_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7859 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/test_datasource_update_method.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/test_transformer_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.610536 vitrage-8.0.1/vitrage/tests/unit/datasources/tmfapi639/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/tmfapi639/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4825 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/tmfapi639/test_tmfapi639_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.610536 vitrage-8.0.1/vitrage/tests/unit/datasources/trove/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/trove/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5734 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/trove/test_trove_cluster_transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5740 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/trove/test_trove_instance_transformer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.614536 vitrage-8.0.1/vitrage/tests/unit/datasources/zabbix/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/zabbix/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1547 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/zabbix/mock_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3629 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/zabbix/test_zabbix_configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16899 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/zabbix/test_zabbix_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7777 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/zabbix/test_zabbix_transformer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1486 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/datasources/zabbix/zabbix_base_test.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.614536 vitrage-8.0.1/vitrage/tests/unit/entity_graph/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/entity_graph/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8324 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/entity_graph/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.614536 vitrage-8.0.1/vitrage/tests/unit/entity_graph/processor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/entity_graph/processor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2255 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/entity_graph/processor/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4998 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/entity_graph/processor/test_entity_graph.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18598 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/entity_graph/processor/test_processor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.614536 vitrage-8.0.1/vitrage/tests/unit/entity_graph/states/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/entity_graph/states/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11911 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/entity_graph/states/test_datasource_info_mapper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2582 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/entity_graph/test_processor_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2647 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/entity_graph/test_transformer_manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.614536 vitrage-8.0.1/vitrage/tests/unit/evaluator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.614536 vitrage-8.0.1/vitrage/tests/unit/evaluator/recipes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/recipes/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3399 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/recipes/test_add_causal_relationship_recipe.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2750 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/recipes/test_execute_mistral.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3117 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/recipes/test_mark_down.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4148 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/recipes/test_raise_alarm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3167 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/recipes/test_set_state_recipe.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.614536 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_functions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_functions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2243 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_functions/test_template_functions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.614536 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_loading/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_loading/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18579 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_loading/test_template_loading_v3.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.614536 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_loading/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_loading/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2088 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_loading/v2/test_template_loader.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.618536 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.618536 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3710 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4314 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/base_test_execute_mistral_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15528 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/test_template_content_validator.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.618536 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4005 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/test_add_causal_relationship_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3666 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/test_execute_mistral_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2109 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/test_mark_down_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2799 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/test_metadata_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1656 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/test_parameters_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3279 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/test_raise_alarm_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2884 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/test_set_state_validator.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.618536 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4374 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v2/test_execute_mistral_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2428 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v2/test_metadata_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8206 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v2/test_parameters_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3047 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/test_def_template_syntax_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12443 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/test_template_syntax_validator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12629 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/test_template_validator_v3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5316 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/test_condition.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2327 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/test_equivalence_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1599 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/test_equivalence_repository.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/test_scenario_evaluator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7568 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/test_scenario_repository.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16532 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/evaluator/test_template_loader.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.618536 vitrage-8.0.1/vitrage/tests/unit/graph/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/graph/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7891 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/graph/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25549 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/graph/test_graph.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    63886 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/graph/test_graph_algo.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.618536 vitrage-8.0.1/vitrage/tests/unit/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7585 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/hacking/test_hacking.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.618536 vitrage-8.0.1/vitrage/tests/unit/machine_learning/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/machine_learning/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.618536 vitrage-8.0.1/vitrage/tests/unit/machine_learning/jaccard_correlation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/machine_learning/jaccard_correlation/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14159 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/machine_learning/jaccard_correlation/test_jaccard_correlation.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.618536 vitrage-8.0.1/vitrage/tests/unit/notifier/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/notifier/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.622536 vitrage-8.0.1/vitrage/tests/unit/notifier/snmp_notifier/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/notifier/snmp_notifier/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/notifier/snmp_notifier/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2651 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/notifier/snmp_notifier/test_snmp_notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4313 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/notifier/snmp_notifier/test_snmp_sender_with_severity_map.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3071 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/notifier/snmp_notifier/test_snmp_sender_without_severity_map.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8079 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/notifier/test_notifier.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.622536 vitrage-8.0.1/vitrage/tests/unit/snmp_parsing/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/snmp_parsing/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6059 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/snmp_parsing/test_snmp_parsing.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.622536 vitrage-8.0.1/vitrage/tests/unit/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4161 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/tests/unit/storage/test_migrations.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.622536 vitrage-8.0.1/vitrage/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1324 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2078 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/utils/datetime.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/utils/evaluator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2015 2022-03-16 08:59:56.000000 vitrage-8.0.1/vitrage/utils/file.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-16 09:00:27.538533 vitrage-8.0.1/vitrage.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2310 2022-03-16 09:00:27.000000 vitrage-8.0.1/vitrage.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52003 2022-03-16 09:00:27.000000 vitrage-8.0.1/vitrage.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-16 09:00:27.000000 vitrage-8.0.1/vitrage.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2022-03-16 09:00:27.000000 vitrage-8.0.1/vitrage.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-16 09:00:27.000000 vitrage-8.0.1/vitrage.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2022-03-16 09:00:27.000000 vitrage-8.0.1/vitrage.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2022-03-16 09:00:27.000000 vitrage-8.0.1/vitrage.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2022-03-16 09:00:27.000000 vitrage-8.0.1/vitrage.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.227531 vitrage-9.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2022-08-02 10:17:31.000000 vitrage-9.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      985 2022-08-02 10:17:31.000000 vitrage-9.0.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5485 2022-08-02 10:18:14.000000 vitrage-9.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2022-08-02 10:17:31.000000 vitrage-9.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    58650 2022-08-02 10:18:14.000000 vitrage-9.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2022-08-02 10:17:31.000000 vitrage-9.0.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-08-02 10:17:31.000000 vitrage-9.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2210 2022-08-02 10:18:15.227531 vitrage-9.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1038 2022-08-02 10:17:31.000000 vitrage-9.0.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.039530 vitrage-9.0.0/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1743 2022-08-02 10:17:31.000000 vitrage-9.0.0/devstack/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2022-08-02 10:17:31.000000 vitrage-9.0.0/devstack/apache-vitrage.template
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2022-08-02 10:17:31.000000 vitrage-9.0.0/devstack/override-defaults
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13231 2022-08-02 10:17:31.000000 vitrage-9.0.0/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1525 2022-08-02 10:17:31.000000 vitrage-9.0.0/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.039530 vitrage-9.0.0/devstack/upgrade/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2022-08-02 10:17:31.000000 vitrage-9.0.0/devstack/upgrade/settings
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1122 2022-08-02 10:17:31.000000 vitrage-9.0.0/devstack/upgrade/shutdhown.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3315 2022-08-02 10:17:31.000000 vitrage-9.0.0/devstack/upgrade/upgrade.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.039530 vitrage-9.0.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.039530 vitrage-9.0.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.039530 vitrage-9.0.0/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.039530 vitrage-9.0.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/cli/vitrage-purge-data.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/cli/vitrage-status.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2952 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.039530 vitrage-9.0.0/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      828 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.051530 vitrage-9.0.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11711 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/add-new-datasource.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4866 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/alarm-severity-config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1025 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/cetus_datasource.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3149 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3602 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/datasource-snmp-parsing-support.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/devstack-installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16929 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/entity_equivalence_use_cases.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4010 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/high-scale.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/host_high_memory_consumption.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.055530 vitrage-9.0.0/doc/source/contributor/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   205286 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/images/add_aodh_alarm_flow.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13261 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/images/add_aodh_alarm_graph.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   221898 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/images/add_nova_instance_flow.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13562 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/images/add_nova_instance_graph.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26304 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/images/complex_rca_graph.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   234474 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/images/low_level_design.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   216665 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/images/nagios_causes_deduced_flow.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20911 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/images/nagios_causes_deduced_graph.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   125468 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/images/osprofiler-html-output.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   197574 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/images/rca_flow.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19438 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/images/rca_graph.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    99836 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/images/vitrage-ha-vision.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   172861 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/images/vitrage_graph_architecture.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1861 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/k8s_datasource.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3098 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/kapacitor-datasource.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/keycloak-config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49512 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual-tests.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.059530 vitrage-9.0.0/doc/source/contributor/manual_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/switch_and_nic.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.059530 vitrage-9.0.0/doc/source/contributor/manual_tests/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v1_template.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v2_definition_template.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v2_equivalence.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1809 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v2_high_cpu_load.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v2_host_down.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v2_with_include.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v2_with_invalid_include.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      885 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v2_with_params.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v2_wrong.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v3_execute_mistral.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v3_high_mem_consumption.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      466 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v3_with_default_params.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v3_with_params.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/test_web_server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/manual_tests/workflow1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      942 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/mistral-config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/ml-jaccard_correlation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4038 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/nagios-config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2898 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/nagios-devstack-installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7156 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/not_operator_support.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10486 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/not_operator_support_v2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3807 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/notifier-snmp-plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3394 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/notifier-webhook-plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/nova-config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1133 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/nova-notifier.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/profiler-config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4764 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/prometheus-datasource.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5195 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/resource-state-config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10166 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/scenario-evaluator.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4019 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/static-config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16208 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/template_validation_status_code.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5923 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/templates-loading-v2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6067 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/templates-loading.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1127 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/tmfapi639-datasource.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50462 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/vitrage-api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4578 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/vitrage-first_steps.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4288 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/vitrage-graph-design.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9772 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/vitrage-ha-and-history-vision.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25954 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/vitrage-template-format-v2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20962 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/vitrage-templates.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2940 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/vitrage-use-cases.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3713 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/zabbix_vitrage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/contributor/zaqar_notifier.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3381 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.063530 vitrage-9.0.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      957 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/install/get_started.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5527 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/install/install-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/install/install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/install/next-steps.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2022-08-02 10:17:31.000000 vitrage-9.0.0/doc/source/install/verify.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.011530 vitrage-9.0.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.063530 vitrage-9.0.0/etc/vitrage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/README-vitrage.conf.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1952 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/api-paste.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.067530 vitrage-9.0.0/etc/vitrage/datasources_values/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/aodh.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/cetus.cluster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/cetus.pod.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1120 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/cinder.volume.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/collectd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/default.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/doctor.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1372 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/heat.stack.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/kapacitor.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/monasca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/nagios.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/network.interface.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/neutron.network.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/neutron.port.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/nova.host.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/nova.instance.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/nova.zone.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/openstack.cluster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/prometheus.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/static.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/static_physical.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/switch.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/trove.cluster.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/trove.instance.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/vitrage.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      767 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/datasources_values/zabbix.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.067530 vitrage-9.0.0/etc/vitrage/templates.sample/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2675 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/templates.sample/database_cluster_capacity_autoscaling.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1859 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/templates.sample/host_down_scenarios.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1868 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/templates.sample/host_high_cpu_load_scenarios.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/vitrage-config-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2022-08-02 10:17:31.000000 vitrage-9.0.0/etc/vitrage/vitrage-policy-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2022-08-02 10:17:31.000000 vitrage-9.0.0/initial.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.011530 vitrage-9.0.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.087530 vitrage-9.0.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/SNMP_notifier-5c46505b3043b58f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/Vitrage_ID-93737ff7b7ced8e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/add-upgrade-check-framework-166ba1c7e266953e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/add_service_list-d8e28adabc26f1cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/add_status-c5b13941c3ce978e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/add_template_versions-5476a446705b43d2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/add_zaqar_notifier-63de714384091ce5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/alarm-and-rca-history-0c4c513c98fdc426.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/alarm_count_api-057138c8e0a36443.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/aodh_extended_alarm_support-327bb589311da440.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/aodh_gnocchi_thresh_alarm-a529ec4f50f3cb0c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/cetus-datasource-0c8297005ac6ca92.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/cinder-default-version-9dfcb941996e32ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/collectd-datasource-a730f06aff840c8f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/collector-cache-limitations-4eedef1c7664f5b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/collector-removal-fd805c6298d66eb0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/collector-service-5848f96896f97d50.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/database-migrations-ffca2f9f3283f2a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/datasource-scaffold-2f5ee6f0d9f83099.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/definition_templates-6c2c10bb3e6912a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/deprecate-json-formatted-policy-file-6a1e9b690fdbc132.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/deprecate-keystone_client-region-option-b3f30100370a5471.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/deprecate-static-physical-datasource-ab0094620c05d0ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/doctor-datasource-59ee5b2afb677ab4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/drop-py-2-7-6add89c8aeb58399.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/drop-python-3-6-and-3-7-ca06b475787d017d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/entity-equivalence-44c0da4cf3b5bc7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/event_persistor-1b0b4563cc219915.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/graph-fast-failover-e2d0a62f18ab27f7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/health-check-api-19f180a104c7fa29.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/improve_tempest_tests-3e77197dfae4ad62.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/introduce-template-version-55bca9fc4e7d138f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/kapacitor_datasource-c0c9563bb52ff1f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/keycloak_auth_support-cf8c2c504b3ddd5b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/kubernetes-datasource-12af0f9caac1b21b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/machine_learning_service-da9700e6c6fa61b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/mock-datasource-1c9b427bc16f4a59.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1123 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/monasca-datasource-9ca61922ef14c2a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/multi_tenancy_support-feb3d2d4f8014b66.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/nested_stacks-fddbfa1f79b2ef43.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/not_operator_for_templates-f1e4c517236ca54e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/nova-versioned-notifications-3c5ff450b9fe69f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/ocata-prelude-9b64d68bc898f7ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/osprofiler-784098daab42a150.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/parallel_evaluation-db8660ef3ff5b864.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/performance-bug-fixes-a2b5e85ee37bba93.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/persist_overlapping_scenarios-d426dffdf3d11094.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/policies-in-code-dd3f1490f7f5b3eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/prometheus-enhancement-b9dc2ef5705d1000.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/prometheus_datasource-65c72bc8e7ec7622.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/queens-prelude-a00e64274e8e64be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/refactor-execute-mistral-action-fc0fac84c07e1784.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/remove-static-physical-datasource-e8e70158f453cff1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/remove_end_messages-e92e7b41a52c61cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/resource_count-1e3184e5f1f413ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/resource_list_query-b3fbcbe01090f64a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/rewrite-aodh-datasource-4968c32c1c5b81f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/rocky-prelude-24ec92aedd5d8266.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/services-management-improvements-899c011e57002e84.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      223 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/snmp_parsing-1a5c4645ce832ee3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/sql_integration-c33342d100492ceb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/static-datasource-changes-914f9a16ad7e46ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/static-datasource-refactoring-2cc7569fafbe65c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/stein-prelude-5e6f583803807d84.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/support-aodh-notifications-cc495f3bc137099d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/support-get-changes-in-static-datasource-02715226f103455d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/support-mistral-13618b516699a1c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/support-networkx-version-2-8d47034b6b278137.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/support-template-functions-dcb2d2e1e63e9a5d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/support-template-parameters-f9552fef4fc66122.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/support_alarm_show_api-0b001dd185e2e523.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/support_high_scale-fa1053f06954aed7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/support_mark_down_for_instance-179b04c693f17787.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/support_overwrite_when_adding_template-f6795771ae0eff8e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/support_template_show_and_add_by_name-a73455f462175160.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/template-type-4587ad6a39130170.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/template_crud-91baea2ed68291f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/template_regex-8cb58f5e4438c11a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/template_version_3-cd8a0775b2f2e7cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/tmfapi639_datasource-bcae9474430ae5a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/trove-datasource-2aa7a88ff20aff8c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/notes/webhooks-139aeaaab7119302.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.091530 vitrage-9.0.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.091530 vitrage-9.0.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.091530 vitrage-9.0.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/_templates/.placeholder
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2661 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      893 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-08-02 10:17:31.000000 vitrage-9.0.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1355 2022-08-02 10:17:31.000000 vitrage-9.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2022-08-02 10:18:15.227531 vitrage-9.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-08-02 10:17:31.000000 vitrage-9.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2022-08-02 10:17:31.000000 vitrage-9.0.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.091530 vitrage-9.0.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.091530 vitrage-9.0.0/tools/datasource-scaffold/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/datasource-scaffold/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/datasource-scaffold/cookiecutter.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/datasource-scaffold/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.091530 vitrage-9.0.0/tools/datasource-scaffold/sample/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1820 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/datasource-scaffold/sample/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1855 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/datasource-scaffold/sample/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2558 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/datasource-scaffold/sample/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.091530 vitrage-9.0.0/tools/datasource-scaffold/{{cookiecutter.name}}/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2031 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/datasource-scaffold/{{cookiecutter.name}}/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1985 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/datasource-scaffold/{{cookiecutter.name}}/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2897 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/datasource-scaffold/{{cookiecutter.name}}/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.095530 vitrage-9.0.0/tools/load_generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/load_generator/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11806 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/load_generator/computes.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5389 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/load_generator/load_generator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8583 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/load_generator/notification_info.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.095530 vitrage-9.0.0/tools/load_generator/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2165 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/load_generator/templates/port_0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2165 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/load_generator/templates/port_1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2165 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/load_generator/templates/port_2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2164 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/load_generator/templates/port_3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2165 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/load_generator/templates/port_4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/load_generator/templates/vm_0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/load_generator/templates/vm_1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/load_generator/templates/vm_2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/load_generator/templates/vm_3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2022-08-02 10:17:31.000000 vitrage-9.0.0/tools/load_generator/templates/vm_4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2674 2022-08-02 10:17:31.000000 vitrage-9.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.095530 vitrage-9.0.0/vitrage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.099530 vitrage-9.0.0/vitrage/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4522 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      849 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/app.wsgi
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.099530 vitrage-9.0.0/vitrage/api/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1420 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/rest.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1103 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/root.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.103530 vitrage-9.0.0/vitrage/api/controllers/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2404 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/v1/alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3157 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/v1/alarm_base.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2999 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/v1/count.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2246 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/v1/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/v1/history.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2249 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/v1/rca.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4220 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/v1/resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/v1/root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1647 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/v1/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1381 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/v1/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9160 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/v1/template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5294 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/v1/topology.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4740 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/controllers/v1/webhook.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4039 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/hooks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api/policy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.103530 vitrage-9.0.0/vitrage/api_handler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api_handler/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.107530 vitrage-9.0.0/vitrage/api_handler/apis/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api_handler/apis/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5709 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api_handler/apis/alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4616 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api_handler/apis/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2758 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api_handler/apis/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api_handler/apis/operational.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3062 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api_handler/apis/rca.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api_handler/apis/resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4944 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api_handler/apis/template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8272 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api_handler/apis/topology.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5459 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/api_handler/apis/webhook.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.107530 vitrage-9.0.0/vitrage/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/cli/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/cli/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1371 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/cli/graph.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/cli/machine_learning.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/cli/notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/cli/persistor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      931 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/cli/snmp_parsing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1278 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/cli/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1892 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/cli/storage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.107530 vitrage-9.0.0/vitrage/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2318 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5961 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1186 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/exception.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.111530 vitrage-9.0.0/vitrage/common/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1274 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3030 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/policies/alarms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1023 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/policies/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1343 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/policies/rca.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2577 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/policies/resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/policies/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1031 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/policies/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2166 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/policies/template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/policies/topology.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2286 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/policies/webhook.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4719 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/common/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.111530 vitrage-9.0.0/vitrage/coordination/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/coordination/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3992 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/coordination/coordination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/coordination/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.115530 vitrage-9.0.0/vitrage/datasources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2358 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4899 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/alarm_driver_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/alarm_properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2410 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/alarm_transformer_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.115530 vitrage-9.0.0/vitrage/datasources/aodh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1683 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/aodh/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14147 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/aodh/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/aodh/properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6720 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/aodh/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.115530 vitrage-9.0.0/vitrage/datasources/ceilometer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1785 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/ceilometer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14986 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/ceilometer/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1690 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/ceilometer/properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6882 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/ceilometer/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.115530 vitrage-9.0.0/vitrage/datasources/cetus/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/cetus/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/cetus/cetus_driver_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.115530 vitrage-9.0.0/vitrage/datasources/cetus/cluster/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1609 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/cetus/cluster/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1722 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/cetus/cluster/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3863 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/cetus/cluster/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.119531 vitrage-9.0.0/vitrage/datasources/cetus/pod/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1577 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/cetus/pod/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1418 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/cetus/pod/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3777 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/cetus/pod/transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/cetus/properties.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.119531 vitrage-9.0.0/vitrage/datasources/cinder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/cinder/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.119531 vitrage-9.0.0/vitrage/datasources/cinder/volume/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1617 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/cinder/volume/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2381 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/cinder/volume/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/cinder/volume/properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7509 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/cinder/volume/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.119531 vitrage-9.0.0/vitrage/datasources/collectd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/collectd/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.119531 vitrage-9.0.0/vitrage/datasources/collectd/collectd_vitrage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/collectd/collectd_vitrage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/collectd/collectd_vitrage/getsigchld.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5179 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/collectd/collectd_vitrage/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1259 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/collectd/collectd_vitrage/readme
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4170 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/collectd/collectd_vitrage/vitrageplugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3887 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/collectd/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1947 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/collectd/mapper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      878 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/collectd/properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4587 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/collectd/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.119531 vitrage-9.0.0/vitrage/datasources/consistency/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      609 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/consistency/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2251 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/consistency/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.119531 vitrage-9.0.0/vitrage/datasources/doctor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/doctor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4625 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/doctor/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/doctor/properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4142 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/doctor/transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4459 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/driver_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.123530 vitrage-9.0.0/vitrage/datasources/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/heat/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.123530 vitrage-9.0.0/vitrage/datasources/heat/stack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1588 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/heat/stack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5719 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/heat/stack/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/heat/stack/properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5854 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/heat/stack/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.123530 vitrage-9.0.0/vitrage/datasources/kapacitor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1696 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/kapacitor/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.123530 vitrage-9.0.0/vitrage/datasources/kapacitor/auxiliary/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3448 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/kapacitor/auxiliary/kapacitor_vitrage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3242 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/kapacitor/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3396 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/kapacitor/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      943 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/kapacitor/properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4179 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/kapacitor/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.123530 vitrage-9.0.0/vitrage/datasources/kubernetes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1823 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/kubernetes/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2671 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/kubernetes/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/kubernetes/properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4313 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/kubernetes/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.123530 vitrage-9.0.0/vitrage/datasources/monasca/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1817 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/monasca/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2553 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/monasca/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      907 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/monasca/properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3487 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/monasca/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.127530 vitrage-9.0.0/vitrage/datasources/nagios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2078 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nagios/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3041 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nagios/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3738 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nagios/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4436 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nagios/parser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nagios/properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3910 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nagios/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.127530 vitrage-9.0.0/vitrage/datasources/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/neutron/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      949 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/neutron/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.127530 vitrage-9.0.0/vitrage/datasources/neutron/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1614 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/neutron/network/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1856 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/neutron/network/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4657 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/neutron/network/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.127530 vitrage-9.0.0/vitrage/datasources/neutron/port/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1564 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/neutron/port/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2199 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/neutron/port/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7103 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/neutron/port/transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1180 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/neutron/properties.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.127530 vitrage-9.0.0/vitrage/datasources/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nova/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.127530 vitrage-9.0.0/vitrage/datasources/nova/host/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1546 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nova/host/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1214 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nova/host/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3403 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nova/host/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.127530 vitrage-9.0.0/vitrage/datasources/nova/instance/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1604 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nova/instance/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4991 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nova/instance/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3184 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nova/instance/field_extractor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5708 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nova/instance/transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nova/nova_driver_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nova/properties.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.131531 vitrage-9.0.0/vitrage/datasources/nova/zone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1576 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nova/zone/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1400 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nova/zone/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5426 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/nova/zone/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.131531 vitrage-9.0.0/vitrage/datasources/prometheus/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2090 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/prometheus/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15542 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/prometheus/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1821 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/prometheus/properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4237 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/prometheus/transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/resource_transformer_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.131531 vitrage-9.0.0/vitrage/datasources/static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4524 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/static/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7444 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/static/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4634 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/static/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.131531 vitrage-9.0.0/vitrage/datasources/tmfapi639/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1974 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/tmfapi639/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1866 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/tmfapi639/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3293 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/tmfapi639/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3482 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/tmfapi639/transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12953 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/transformer_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.131531 vitrage-9.0.0/vitrage/datasources/trove/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/trove/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.131531 vitrage-9.0.0/vitrage/datasources/trove/cluster/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1847 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/trove/cluster/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1930 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/trove/cluster/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3436 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/trove/cluster/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.131531 vitrage-9.0.0/vitrage/datasources/trove/instance/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1854 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/trove/instance/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1814 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/trove/instance/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3265 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/trove/instance/transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      981 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/trove/properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3511 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/trove/trove_driver_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1624 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.135531 vitrage-9.0.0/vitrage/datasources/zabbix/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2064 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/zabbix/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.135531 vitrage-9.0.0/vitrage/datasources/zabbix/auxiliary/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/zabbix/auxiliary/readme
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3710 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/zabbix/auxiliary/zabbix_vitrage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7007 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/zabbix/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1678 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/zabbix/properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4973 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/datasources/zabbix/transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.135531 vitrage-9.0.0/vitrage/entity_graph/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1555 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.135531 vitrage-9.0.0/vitrage/entity_graph/consistency/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/consistency/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6054 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/consistency/consistency_enforcer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6877 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/driver_exec.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8349 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/graph_init.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4345 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/graph_persistency.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.135531 vitrage-9.0.0/vitrage/entity_graph/mappings/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/mappings/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1509 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/mappings/alarm_handler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10450 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/mappings/datasource_info_mapper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/mappings/handler_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/mappings/operational_alarm_severity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/mappings/operational_resource_state.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1574 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/mappings/resource_handler.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.139531 vitrage-9.0.0/vitrage/entity_graph/processor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/processor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1037 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/processor/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8954 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/processor/notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15733 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/processor/processor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3462 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/processor/processor_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3496 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/processor/transformer_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2977 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14393 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/entity_graph/workers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.139531 vitrage-9.0.0/vitrage/evaluator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      931 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.139531 vitrage-9.0.0/vitrage/evaluator/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      903 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/actions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6657 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/actions/action_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1059 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/actions/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7696 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/actions/evaluator_event_transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2741 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/actions/notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1972 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/actions/priority_tools.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.143531 vitrage-9.0.0/vitrage/evaluator/actions/recipes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/actions/recipes/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/actions/recipes/action_steps.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2260 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/actions/recipes/add_causal_relationship.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1673 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/actions/recipes/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/actions/recipes/execute_mistral.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2222 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/actions/recipes/mark_down.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2511 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/actions/recipes/raise_alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/actions/recipes/set_state.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1192 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6078 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/condition.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/equivalence_repository.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26439 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/scenario_evaluator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8342 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/scenario_repository.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3076 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_data.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.143531 vitrage-9.0.0/vitrage/evaluator/template_db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5292 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_db/template_repository.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1181 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_fields.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.143531 vitrage-9.0.0/vitrage/evaluator/template_functions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_functions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2644 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_functions/function_resolver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.143531 vitrage-9.0.0/vitrage/evaluator/template_functions/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1691 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_functions/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5471 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_functions/v2/functions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.143531 vitrage-9.0.0/vitrage/evaluator/template_loading/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_loading/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2269 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_loading/equivalence_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_loading/props_converter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7109 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_loading/scenario_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3245 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_loading/subgraph_builder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6308 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_loading/template_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5753 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_loading/template_loader_v3.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.143531 vitrage-9.0.0/vitrage/evaluator/template_loading/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_loading/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1327 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_loading/v1/action_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_loading/v1/execute_mistral_loader.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.143531 vitrage-9.0.0/vitrage/evaluator/template_loading/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_loading/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1514 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_loading/v3/action_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_loading/v3/raise_alarm_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1307 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_schema_factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6042 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_schemas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.147531 vitrage-9.0.0/vitrage/evaluator/template_validation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3102 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1772 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.147531 vitrage-9.0.0/vitrage/evaluator/template_validation/content/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2722 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4250 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/template_content_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5226 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/template_content_validator_v3.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.147531 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2785 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/add_causal_relationship_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8241 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/definitions_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1837 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/execute_mistral_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1563 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/get_param_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/mark_down_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1054 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/metadata_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2083 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/raise_alarm_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7286 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/scenario_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1902 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/set_state_validator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.147531 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2285 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v2/execute_mistral_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1505 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v2/get_param_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1565 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/content/v2/metadata_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5745 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/status_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11734 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/template_syntax_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4580 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/evaluator/template_validation/template_syntax_validator_v3.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.151531 vitrage-9.0.0/vitrage/graph/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/graph/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.151531 vitrage-9.0.0/vitrage/graph/algo_driver/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/graph/algo_driver/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3101 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/graph/algo_driver/algorithm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7507 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/graph/algo_driver/networkx_algorithm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12077 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/graph/algo_driver/sub_graph_matching.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.151531 vitrage-9.0.0/vitrage/graph/driver/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/graph/driver/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5063 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/graph/driver/elements.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12340 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/graph/driver/graph.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13096 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/graph/driver/networkx_graph.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2270 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/graph/driver/notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1641 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/graph/filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3502 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/graph/query.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4466 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/graph/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.151531 vitrage-9.0.0/vitrage/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5180 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3738 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/keystone_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.151531 vitrage-9.0.0/vitrage/machine_learning/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/machine_learning/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.151531 vitrage-9.0.0/vitrage/machine_learning/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/machine_learning/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      807 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/machine_learning/plugins/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.155531 vitrage-9.0.0/vitrage/machine_learning/plugins/jaccard_correlation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1430 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/machine_learning/plugins/jaccard_correlation/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1930 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/machine_learning/plugins/jaccard_correlation/accumulation_persistor_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2958 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/machine_learning/plugins/jaccard_correlation/alarm_data_accumulator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3756 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/machine_learning/plugins/jaccard_correlation/alarm_processor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3146 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/machine_learning/plugins/jaccard_correlation/correlation_collection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4510 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/machine_learning/plugins/jaccard_correlation/correlation_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3204 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/machine_learning/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2857 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/messaging.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.155531 vitrage-9.0.0/vitrage/middleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/middleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5361 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/middleware/basic_and_keystone_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7662 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/middleware/keycloak.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.155531 vitrage-9.0.0/vitrage/notifier/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      889 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.155531 vitrage-9.0.0/vitrage/notifier/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.155531 vitrage-9.0.0/vitrage/notifier/plugins/aodh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/aodh/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3734 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/aodh/aodh_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1039 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.155531 vitrage-9.0.0/vitrage/notifier/plugins/mistral/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/mistral/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2722 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/mistral/mistral_notifier.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.155531 vitrage-9.0.0/vitrage/notifier/plugins/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/nova/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2933 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/nova/nova_notifier.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.155531 vitrage-9.0.0/vitrage/notifier/plugins/snmp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1391 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/snmp/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/snmp/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2852 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/snmp/snmp_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6969 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/snmp/snmp_sender.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.155531 vitrage-9.0.0/vitrage/notifier/plugins/webhook/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      973 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/webhook/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/webhook/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6440 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/webhook/webhook.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.159531 vitrage-9.0.0/vitrage/notifier/plugins/zaqar/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/zaqar/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1373 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/plugins/zaqar/zaqar_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3795 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/notifier/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4214 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7714 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/os_clients.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.159531 vitrage-9.0.0/vitrage/persistency/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/persistency/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8015 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/persistency/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3164 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/rpc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.159531 vitrage-9.0.0/vitrage/snmp_parsing/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/snmp_parsing/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      689 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/snmp_parsing/properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6415 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/snmp_parsing/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.159531 vitrage-9.0.0/vitrage/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1932 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8354 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/storage/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18087 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/storage/history_facade.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17640 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/storage/impl_sqlalchemy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.159531 vitrage-9.0.0/vitrage/storage/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/storage/sqlalchemy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.159531 vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3021 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1084 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/alembic.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.159531 vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/alembic_migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/alembic_migrations/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/alembic_migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2369 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/alembic_migrations/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/alembic_migrations/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.159531 vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/alembic_migrations/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9428 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/alembic_migrations/versions/4e44c9414dff_initial_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/alembic_migrations/versions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10796 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/storage/sqlalchemy/models.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.159531 vitrage-9.0.0/vitrage/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4909 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.163531 vitrage-9.0.0/vitrage/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.163531 vitrage-9.0.0/vitrage/tests/functional/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6820 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api/test_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.163531 vitrage-9.0.0/vitrage/tests/functional/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2591 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api/v1/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6961 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api/v1/test_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1297 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api/v1/test_health.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4508 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api/v1/test_keycloak.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5877 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api/v1/test_noauth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3122 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api/v1/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2598 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api/v1/test_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1536 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api/v1/test_template_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.163531 vitrage-9.0.0/vitrage/tests/functional/api_handler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api_handler/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    29960 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api_handler/test_apis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12220 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api_handler/test_templates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2778 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api_handler/test_templates_v2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2485 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/api_handler/test_templates_v3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2389 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.163531 vitrage-9.0.0/vitrage/tests/functional/datasources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.163531 vitrage-9.0.0/vitrage/tests/functional/datasources/aodh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/aodh/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4063 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/aodh/test_aodh.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.163531 vitrage-9.0.0/vitrage/tests/functional/datasources/ceilometer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/ceilometer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4102 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/ceilometer/test_ceilometer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.167531 vitrage-9.0.0/vitrage/tests/functional/datasources/cinder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/cinder/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3922 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/cinder/test_cinder_volume.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.167531 vitrage-9.0.0/vitrage/tests/functional/datasources/collectd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/collectd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9277 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/collectd/test_collectd.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.167531 vitrage-9.0.0/vitrage/tests/functional/datasources/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/heat/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4189 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/heat/test_heat_stack.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.167531 vitrage-9.0.0/vitrage/tests/functional/datasources/listener_service/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/listener_service/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2416 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/listener_service/test_listener_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.167531 vitrage-9.0.0/vitrage/tests/functional/datasources/nagios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/nagios/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3734 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/nagios/test_nagios.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.167531 vitrage-9.0.0/vitrage/tests/functional/datasources/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/neutron/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/neutron/test_neutron_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/neutron/test_neutron_port.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.167531 vitrage-9.0.0/vitrage/tests/functional/datasources/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/nova/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/nova/test_nova_datasources.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.167531 vitrage-9.0.0/vitrage/tests/functional/datasources/trove/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/trove/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3645 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/datasources/trove/test_trove_instance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.167531 vitrage-9.0.0/vitrage/tests/functional/entity_graph/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/entity_graph/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.167531 vitrage-9.0.0/vitrage/tests/functional/entity_graph/consistency/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/entity_graph/consistency/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14775 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/entity_graph/consistency/test_consistency.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.167531 vitrage-9.0.0/vitrage/tests/functional/entity_graph/graph_persistor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/entity_graph/graph_persistor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4018 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/entity_graph/graph_persistor/test_graph_persistor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.167531 vitrage-9.0.0/vitrage/tests/functional/entity_graph/processor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/entity_graph/processor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1605 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/entity_graph/processor/test_processor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.171531 vitrage-9.0.0/vitrage/tests/functional/entity_graph/states/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/entity_graph/states/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2639 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/entity_graph/states/test_datasource_info_mapper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.171531 vitrage-9.0.0/vitrage/tests/functional/evaluator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/evaluator/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15003 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/evaluator/test_action_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    71082 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/evaluator/test_scenario_evaluator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2629 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/functional/test_configuration.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.171531 vitrage-9.0.0/vitrage/tests/mocks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/mocks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1416 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/mocks/entity_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8308 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/mocks/graph_generator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22849 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/mocks/mock_driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.171531 vitrage-9.0.0/vitrage/tests/mocks/mock_graph_datasource/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2079 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/mocks/mock_graph_datasource/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4320 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/mocks/mock_graph_datasource/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/mocks/mock_graph_datasource/transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8860 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/mocks/mock_transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29737 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/mocks/trace_generator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4597 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/mocks/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.027530 vitrage-9.0.0/vitrage/tests/resources/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.171531 vitrage-9.0.0/vitrage/tests/resources/datasources_values/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/datasources_values/default.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.175531 vitrage-9.0.0/vitrage/tests/resources/datasources_values/erroneous_values/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/datasources_values/erroneous_values/default.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/datasources_values/erroneous_values/nagios.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/datasources_values/erroneous_values/nova.host.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1552 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/datasources_values/erroneous_values/nova.instance.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/datasources_values/nagios.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/datasources_values/nova.host.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/datasources_values/nova.instance.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/datasources_values/nova.zone.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/datasources_values/vitrage.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.175531 vitrage-9.0.0/vitrage/tests/resources/kapacitor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/kapacitor/kapacitor_conf.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.175531 vitrage-9.0.0/vitrage/tests/resources/kubernetes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/kubernetes/kubernetes_config.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.027530 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.179531 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_aodh_update_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_collectd_update_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_consistency_update_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_doctor_update_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_host_snapshot_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4611 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_inst_snapshot_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_inst_snapshot_static.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_inst_update_legacy_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3829 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_inst_update_versioned_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_kapacitor_update_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_kubernetes_snapshot_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_nagios_snapshot_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       21 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_nagios_snapshot_static.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5366 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_prometheus_update_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_stack_snapshot_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1175 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_stack_update_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_static_snapshot_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_static_snapshot_static.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      453 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_trove_cluster_snapshot_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_trove_instance_snapshot_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_volume_snapshot_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_volume_update_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_zabbix_snapshot_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_zone_snapshot_dynamic.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.179531 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/edges/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/edges/attached.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/edges/contains.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/edges/on.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.179531 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1290 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_aodh_snapshot_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1289 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_aodh_update_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_collectd_update_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_doctor_update_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_host_snapshot_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_host_snapshot_static.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_inst_snapshot_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_inst_snapshot_static.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_kapacitor_update_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_prometheus_update_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_zone_snapshot_dynamic.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_zone_snapshot_static.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.183531 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      612 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/cinder.volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/neutron.network.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/neutron.port.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/nova.host.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/nova.instance.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      523 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/nova.zone.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/openstack-cluster.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/tripleo.controller.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/vitrage.alarm.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/zabbix.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.183531 vitrage-9.0.0/vitrage/tests/resources/nagios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26541 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/nagios/nagios-mock.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/nagios/nagios_conf.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.183531 vitrage-9.0.0/vitrage/tests/resources/prometheus/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/prometheus/prometheus_conf.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.183531 vitrage-9.0.0/vitrage/tests/resources/snmp_notifier/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/snmp_notifier/alarm_oid_mapping.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/snmp_notifier/dests.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/snmp_notifier/oid_tree_with_severity_mapping.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/snmp_notifier/oid_tree_without_severity_mapping.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.183531 vitrage-9.0.0/vitrage/tests/resources/snmp_parsing/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/snmp_parsing/snmp_parsing_conf.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.183531 vitrage-9.0.0/vitrage/tests/resources/static_datasources/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.183531 vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.183531 vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/added_resources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/added_resources/static.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.183531 vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/baseline/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/baseline/static.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.183531 vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/changed_resources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/changed_resources/static.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.183531 vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/deleted_resources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/deleted_resources/static.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.183531 vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/mixed_changes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/mixed_changes/static.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/switch_to_host_datasource.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/switch_to_switch_datasource.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1318 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/static_datasources/switch_to_host.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/static_datasources/switch_to_host_datasource.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/static_datasources/switch_to_switch_datasource.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.027530 vitrage-9.0.0/vitrage/tests/resources/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.187531 vitrage-9.0.0/vitrage/tests/resources/templates/consistency/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/consistency/deduced_alarm_on_instance.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.027530 vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.187531 vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/definition_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/definition_templates/basic_def_template.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1081 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/definition_templates/large_def_template.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/definition_templates/single_entity.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      518 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/definition_templates/with_include.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/definition_templates/with_scenarios.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.187531 vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/templates/basic_with_include.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/templates/basic_with_include_that_doesnt_exist.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      833 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/templates/basic_with_two_includes.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/templates/include_with_empty_name.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      399 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/templates/no_definitions_only_include.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      976 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/templates/only_using_def_template_definitions.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/templates/with_conflicting_include_entities.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.027530 vitrage-9.0.0/vitrage/tests/resources/templates/equivalences_dup/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.187531 vitrage-9.0.0/vitrage/tests/resources/templates/equivalences_dup/dup-in-multi-def/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      441 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/equivalences_dup/dup-in-multi-def/multi.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.187531 vitrage-9.0.0/vitrage/tests/resources/templates/equivalences_dup/dup-in-multi-file/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/equivalences_dup/dup-in-multi-file/first.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/equivalences_dup/dup-in-multi-file/second.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.187531 vitrage-9.0.0/vitrage/tests/resources/templates/equivalences_dup/dup-in-one-def/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/equivalences_dup/dup-in-one-def/one.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.187531 vitrage-9.0.0/vitrage/tests/resources/templates/equivalent_scenarios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/equivalent_scenarios/basic.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.187531 vitrage-9.0.0/vitrage/tests/resources/templates/equivalent_scenarios/equivalences/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/equivalent_scenarios/equivalences/basic.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.191531 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      850 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/causal_basic.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1167 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/complex_and_or_operator_deduced_alarm.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1571 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/complex_not_operator_deduced_alarm.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.191531 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1266 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/complex1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1205 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/complex2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1273 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/complex_not.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1289 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/complex_not_unsupported.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/not_edge_unsupported.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1025 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/not_or_unsupported.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/not_or_unsupported2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/one_edge.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/one_vertex.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      956 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/simple_and.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1191 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/simple_and2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/simple_or.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/simple_or2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/simple_or3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1259 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/simple_or_unsupported.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1486 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/deduced_alarm.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1117 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/deduced_state.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1250 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/deduced_state_2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/high_availability.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      728 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/simple_not_operator_deduced_alarm.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/simple_or_operator_deduced_alarm.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.191531 vitrage-9.0.0/vitrage/tests/resources/templates/general/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/general/bad_yaml.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/general/basic.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.191531 vitrage-9.0.0/vitrage/tests/resources/templates/general/equivalences/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/general/equivalences/basic.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1497 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/general/host_high_cpu_load_to_instance_cpu_suboptimal.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.195531 vitrage-9.0.0/vitrage/tests/resources/templates/not_operator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/not_operator/basic_correct_not_condition.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/not_operator/basic_incorrect_not_condition.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/not_operator/complicated_correct_not_condition.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/not_operator/complicated_incorrect_not_condition.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.195531 vitrage-9.0.0/vitrage/tests/resources/templates/parameters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1001 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/parameters/v2_with_extra_param_def.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/parameters/v2_with_missing_param_def.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      885 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/parameters/v2_with_params.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/parameters/v2_without_params.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      687 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/parameters/v3_with_extra_param_def.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      511 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/parameters/v3_with_missing_param_def.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/parameters/v3_with_params.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.195531 vitrage-9.0.0/vitrage/tests/resources/templates/regex/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/regex/basic_regex.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/regex/basic_regex_for_fail.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/regex/faulty_regex.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/regex/regex_for_exact_match.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.195531 vitrage-9.0.0/vitrage/tests/resources/templates/v3_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1567 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/v3_templates/valid_actions.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/v3_templates/valid_conditions.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.195531 vitrage-9.0.0/vitrage/tests/resources/templates/version/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/version/invalid_version.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/version/no_version.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.195531 vitrage-9.0.0/vitrage/tests/resources/templates/version/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/version/v1/v1_execute_mistral.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/version/v1/version1.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.195531 vitrage-9.0.0/vitrage/tests/resources/templates/version/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      667 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/version/v2/v2_execute_mistral.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/version/v2/v2_standard.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/templates/version/v2/v2_with_func.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.195531 vitrage-9.0.0/vitrage/tests/resources/zabbix/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/resources/zabbix/zabbix_conf.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.199531 vitrage-9.0.0/vitrage/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.199531 vitrage-9.0.0/vitrage/tests/unit/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/cli/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1186 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/cli/test_status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.199531 vitrage-9.0.0/vitrage/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2808 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/common/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.199531 vitrage-9.0.0/vitrage/tests/unit/datasources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.199531 vitrage-9.0.0/vitrage/tests/unit/datasources/aodh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/aodh/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5517 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/aodh/aodh_transformer_base_test.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/aodh/mock_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35245 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/aodh/test_aodh_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6231 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/aodh/test_aodh_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.199531 vitrage-9.0.0/vitrage/tests/unit/datasources/ceilometer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/ceilometer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5634 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/ceilometer/ceilometer_transformer_base_test.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/ceilometer/mock_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15691 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/ceilometer/test_ceilometer_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6500 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/ceilometer/test_ceilometer_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.199531 vitrage-9.0.0/vitrage/tests/unit/datasources/cetus/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/cetus/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7407 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/cetus/test_cetus_cluster_transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7199 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/cetus/test_cetus_pod_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.199531 vitrage-9.0.0/vitrage/tests/unit/datasources/cinder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/cinder/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9674 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/cinder/test_cinder_volume_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.207531 vitrage-9.0.0/vitrage/tests/unit/datasources/collectd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/collectd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3203 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/collectd/test_collectd_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4748 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/collectd/test_collectd_transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3118 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/collectd/test_mapper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.207531 vitrage-9.0.0/vitrage/tests/unit/datasources/consistency/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/consistency/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3911 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/consistency/test_consistency_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.207531 vitrage-9.0.0/vitrage/tests/unit/datasources/doctor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/doctor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5072 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/doctor/test_doctor_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4753 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/doctor/test_doctor_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.207531 vitrage-9.0.0/vitrage/tests/unit/datasources/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/heat/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9278 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/heat/test_heat_stack_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.207531 vitrage-9.0.0/vitrage/tests/unit/datasources/kapacitor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/kapacitor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3530 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/kapacitor/test_kapacitor_configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4533 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/kapacitor/test_kapacitor_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7182 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/kapacitor/test_kapacitor_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.207531 vitrage-9.0.0/vitrage/tests/unit/datasources/kubernetes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6600 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/kubernetes/test_kubernetes_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.207531 vitrage-9.0.0/vitrage/tests/unit/datasources/nagios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/nagios/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1563 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/nagios/mock_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1625 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/nagios/nagios_base_test.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8277 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/nagios/test_nagios_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23434 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/nagios/test_nagios_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3244 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/nagios/test_nagios_parser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8290 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/nagios/test_nagios_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.207531 vitrage-9.0.0/vitrage/tests/unit/datasources/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/neutron/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.211531 vitrage-9.0.0/vitrage/tests/unit/datasources/neutron/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/neutron/network/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/neutron/network/test_neutron_network_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.211531 vitrage-9.0.0/vitrage/tests/unit/datasources/neutron/port/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/neutron/port/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/neutron/port/test_neutron_port_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.211531 vitrage-9.0.0/vitrage/tests/unit/datasources/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/nova/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9942 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/nova/base_nova_instance_transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2050 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/nova/test_instance_transformer_legacy_notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5020 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/nova/test_instance_transformer_snapshot_events.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/nova/test_instance_transformer_versioned_notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9001 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/nova/test_nova_host_transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3120 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/nova/test_nova_instance_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10187 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/nova/test_nova_zone_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.211531 vitrage-9.0.0/vitrage/tests/unit/datasources/prometheus/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/prometheus/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8442 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/prometheus/test_prometheus_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6042 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/prometheus/test_prometheus_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.211531 vitrage-9.0.0/vitrage/tests/unit/datasources/static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/static/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8180 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/static/test_static_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5948 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/static/test_static_transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4500 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/test_alarm_transformer_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7859 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/test_datasource_update_method.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/test_transformer_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.211531 vitrage-9.0.0/vitrage/tests/unit/datasources/tmfapi639/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/tmfapi639/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4825 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/tmfapi639/test_tmfapi639_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.211531 vitrage-9.0.0/vitrage/tests/unit/datasources/trove/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/trove/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5734 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/trove/test_trove_cluster_transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5740 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/trove/test_trove_instance_transformer.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.215531 vitrage-9.0.0/vitrage/tests/unit/datasources/zabbix/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/zabbix/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1547 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/zabbix/mock_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3629 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/zabbix/test_zabbix_configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16899 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/zabbix/test_zabbix_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7777 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/zabbix/test_zabbix_transformer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1486 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/datasources/zabbix/zabbix_base_test.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.215531 vitrage-9.0.0/vitrage/tests/unit/entity_graph/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/entity_graph/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8324 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/entity_graph/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.215531 vitrage-9.0.0/vitrage/tests/unit/entity_graph/processor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/entity_graph/processor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2255 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/entity_graph/processor/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4998 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/entity_graph/processor/test_entity_graph.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18598 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/entity_graph/processor/test_processor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.215531 vitrage-9.0.0/vitrage/tests/unit/entity_graph/states/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/entity_graph/states/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11911 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/entity_graph/states/test_datasource_info_mapper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2582 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/entity_graph/test_processor_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2647 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/entity_graph/test_transformer_manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.215531 vitrage-9.0.0/vitrage/tests/unit/evaluator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.219531 vitrage-9.0.0/vitrage/tests/unit/evaluator/recipes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/recipes/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3399 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/recipes/test_add_causal_relationship_recipe.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2750 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/recipes/test_execute_mistral.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3117 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/recipes/test_mark_down.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4148 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/recipes/test_raise_alarm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3167 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/recipes/test_set_state_recipe.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.219531 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_functions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_functions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2243 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_functions/test_template_functions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.219531 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_loading/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_loading/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18579 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_loading/test_template_loading_v3.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.219531 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_loading/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_loading/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2088 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_loading/v2/test_template_loader.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.219531 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.219531 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3710 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4314 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/base_test_execute_mistral_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15528 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/test_template_content_validator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.223531 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4005 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/test_add_causal_relationship_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3666 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/test_execute_mistral_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2109 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/test_mark_down_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2799 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/test_metadata_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1656 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/test_parameters_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3279 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/test_raise_alarm_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2884 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/test_set_state_validator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.223531 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4374 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v2/test_execute_mistral_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2428 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v2/test_metadata_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8206 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v2/test_parameters_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3047 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/test_def_template_syntax_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12443 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/test_template_syntax_validator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12629 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/test_template_validator_v3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5316 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/test_condition.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2327 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/test_equivalence_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1599 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/test_equivalence_repository.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/test_scenario_evaluator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7568 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/test_scenario_repository.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16532 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/evaluator/test_template_loader.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.223531 vitrage-9.0.0/vitrage/tests/unit/graph/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/graph/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7891 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/graph/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25549 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/graph/test_graph.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    63886 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/graph/test_graph_algo.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.223531 vitrage-9.0.0/vitrage/tests/unit/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7585 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/hacking/test_hacking.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.223531 vitrage-9.0.0/vitrage/tests/unit/machine_learning/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/machine_learning/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.223531 vitrage-9.0.0/vitrage/tests/unit/machine_learning/jaccard_correlation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/machine_learning/jaccard_correlation/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14159 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/machine_learning/jaccard_correlation/test_jaccard_correlation.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.223531 vitrage-9.0.0/vitrage/tests/unit/notifier/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/notifier/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.223531 vitrage-9.0.0/vitrage/tests/unit/notifier/snmp_notifier/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/notifier/snmp_notifier/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/notifier/snmp_notifier/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2651 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/notifier/snmp_notifier/test_snmp_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4313 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/notifier/snmp_notifier/test_snmp_sender_with_severity_map.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3071 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/notifier/snmp_notifier/test_snmp_sender_without_severity_map.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8079 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/notifier/test_notifier.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.223531 vitrage-9.0.0/vitrage/tests/unit/snmp_parsing/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/snmp_parsing/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6059 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/snmp_parsing/test_snmp_parsing.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.227531 vitrage-9.0.0/vitrage/tests/unit/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4161 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/tests/unit/storage/test_migrations.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.227531 vitrage-9.0.0/vitrage/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1324 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2078 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/utils/datetime.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/utils/evaluator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2015 2022-08-02 10:17:31.000000 vitrage-9.0.0/vitrage/utils/file.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-02 10:18:15.099530 vitrage-9.0.0/vitrage.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2210 2022-08-02 10:18:14.000000 vitrage-9.0.0/vitrage.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52097 2022-08-02 10:18:15.000000 vitrage-9.0.0/vitrage.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-08-02 10:18:14.000000 vitrage-9.0.0/vitrage.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2022-08-02 10:18:14.000000 vitrage-9.0.0/vitrage.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-08-02 10:18:14.000000 vitrage-9.0.0/vitrage.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2022-08-02 10:18:14.000000 vitrage-9.0.0/vitrage.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2022-08-02 10:18:14.000000 vitrage-9.0.0/vitrage.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2022-08-02 10:18:14.000000 vitrage-9.0.0/vitrage.egg-info/top_level.txt
```

### Comparing `vitrage-8.0.1/.zuul.yaml` & `vitrage-9.0.0/.zuul.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
 - project:
+    queue: vitrage
     templates:
       - check-requirements
-      - openstack-python3-yoga-jobs
+      - openstack-python3-zed-jobs
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
     check:
       jobs:
         - vitrage-tempest-plugin-api
         - vitrage-tempest-plugin-api-ipv6-only
         - vitrage-tempest-plugin-datasources
         - vitrage-tempest-plugin-mock
         - vitrage-grenade
 
     gate:
-      queue: vitrage
       jobs:
         - vitrage-tempest-plugin-api
         - vitrage-tempest-plugin-api-ipv6-only
         - vitrage-tempest-plugin-datasources
         - vitrage-grenade
 
 - job:
```

### Comparing `vitrage-8.0.1/AUTHORS` & `vitrage-9.0.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 howardlee <lihongweibj@inspur.com>
 huang.zhiping <huang.zhiping@99cloud.net>
 idan kinory <idan.kinory@nokia.com>
 inspurericzhang <zhanglf01@inspur.com>
 iswarya_vakati <v.iswarya@nectechnologies.in>
 jiasirui <jiasirui@inspur.com>
 kangyufei <kangyf@inspur.com>
+leiyuehui <leiyuehui-s@inspur.com>
 liathartal <liat.har-tal@nokia.com>
 lingyongxu <lyxu@fiberhome.com>
 liushuobj <liushuobj@inspur.com>
 liuyuanfeng <liuyuanfeng@inspur.com>
 loooosy <syluo5695@fiberhome.com>
 maaoyu <maaoyu@inspur.com>
 marina.koushnir@nokia.com <marina.koushnir@nokia.com>
```

### Comparing `vitrage-8.0.1/CONTRIBUTING.rst` & `vitrage-9.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/ChangeLog` & `vitrage-9.0.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 CHANGES
 =======
 
-8.0.1
+9.0.0
 -----
 
-* fix yoga
+* Update python testing as per zed cycle teting runtime
+* move queue to project level
+* rename tenant to project\_id
+* Add Python3 zed unit tests
+* Update master for stable/yoga
 
 8.0.0
 -----
 
 * remove cielometer client, not used any more
 * Updating python testing classifier as per Yoga testing runtime
 * Add Python3 yoga unit tests
```

### Comparing `vitrage-8.0.1/HACKING.rst` & `vitrage-9.0.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/LICENSE` & `vitrage-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/PKG-INFO` & `vitrage-9.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitrage
-Version: 8.0.1
+Version: 9.0.0
 Summary: The OpenStack RCA Service
 Home-page: https://docs.openstack.org/vitrage/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =================
         OpenStack Vitrage
@@ -38,16 +38,14 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Monitoring
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: openstack
 Provides-Extra: test
 Provides-Extra: zabbix
```

### Comparing `vitrage-8.0.1/README.rst` & `vitrage-9.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/devstack/README.rst` & `vitrage-9.0.0/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/devstack/apache-vitrage.template` & `vitrage-9.0.0/devstack/apache-vitrage.template`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/devstack/plugin.sh` & `vitrage-9.0.0/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/devstack/settings` & `vitrage-9.0.0/devstack/settings`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/devstack/upgrade/settings` & `vitrage-9.0.0/devstack/upgrade/settings`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/devstack/upgrade/shutdhown.sh` & `vitrage-9.0.0/devstack/upgrade/shutdhown.sh`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/devstack/upgrade/upgrade.sh` & `vitrage-9.0.0/devstack/upgrade/upgrade.sh`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/cli/vitrage-purge-data.rst` & `vitrage-9.0.0/doc/source/cli/vitrage-purge-data.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/cli/vitrage-status.rst` & `vitrage-9.0.0/doc/source/cli/vitrage-status.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/conf.py` & `vitrage-9.0.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/configuration/index.rst` & `vitrage-9.0.0/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/add-new-datasource.rst` & `vitrage-9.0.0/doc/source/contributor/add-new-datasource.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/alarm-severity-config.rst` & `vitrage-9.0.0/doc/source/contributor/alarm-severity-config.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/cetus_datasource.rst` & `vitrage-9.0.0/doc/source/contributor/cetus_datasource.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/configuration.rst` & `vitrage-9.0.0/doc/source/contributor/configuration.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/contributing.rst` & `vitrage-9.0.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/datasource-snmp-parsing-support.rst` & `vitrage-9.0.0/doc/source/contributor/datasource-snmp-parsing-support.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/devstack-installation.rst` & `vitrage-9.0.0/doc/source/contributor/devstack-installation.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/entity_equivalence_use_cases.rst` & `vitrage-9.0.0/doc/source/contributor/entity_equivalence_use_cases.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/high-scale.rst` & `vitrage-9.0.0/doc/source/contributor/high-scale.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/host_high_memory_consumption.yaml` & `vitrage-9.0.0/doc/source/contributor/host_high_memory_consumption.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/images/add_aodh_alarm_flow.png` & `vitrage-9.0.0/doc/source/contributor/images/add_aodh_alarm_flow.png`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/images/add_aodh_alarm_graph.png` & `vitrage-9.0.0/doc/source/contributor/images/add_aodh_alarm_graph.png`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/images/add_nova_instance_flow.png` & `vitrage-9.0.0/doc/source/contributor/images/add_nova_instance_flow.png`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/images/add_nova_instance_graph.png` & `vitrage-9.0.0/doc/source/contributor/images/add_nova_instance_graph.png`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/images/complex_rca_graph.png` & `vitrage-9.0.0/doc/source/contributor/images/complex_rca_graph.png`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/images/low_level_design.png` & `vitrage-9.0.0/doc/source/contributor/images/low_level_design.png`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/images/nagios_causes_deduced_flow.png` & `vitrage-9.0.0/doc/source/contributor/images/nagios_causes_deduced_flow.png`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/images/nagios_causes_deduced_graph.png` & `vitrage-9.0.0/doc/source/contributor/images/nagios_causes_deduced_graph.png`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/images/osprofiler-html-output.png` & `vitrage-9.0.0/doc/source/contributor/images/osprofiler-html-output.png`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/images/rca_flow.png` & `vitrage-9.0.0/doc/source/contributor/images/rca_flow.png`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/images/rca_graph.png` & `vitrage-9.0.0/doc/source/contributor/images/rca_graph.png`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/images/vitrage-ha-vision.png` & `vitrage-9.0.0/doc/source/contributor/images/vitrage-ha-vision.png`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/images/vitrage_graph_architecture.png` & `vitrage-9.0.0/doc/source/contributor/images/vitrage_graph_architecture.png`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/k8s_datasource.rst` & `vitrage-9.0.0/doc/source/contributor/k8s_datasource.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/kapacitor-datasource.rst` & `vitrage-9.0.0/doc/source/contributor/kapacitor-datasource.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/keycloak-config.rst` & `vitrage-9.0.0/doc/source/contributor/keycloak-config.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/manual-tests.rst` & `vitrage-9.0.0/doc/source/contributor/manual-tests.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v1_template.yaml` & `vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v1_template.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v2_high_cpu_load.yaml` & `vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v2_high_cpu_load.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v2_host_down.yaml` & `vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v2_host_down.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v2_with_include.yaml` & `vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v2_with_include.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v2_with_invalid_include.yaml` & `vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v2_with_invalid_include.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v2_with_params.yaml` & `vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v2_with_params.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v2_wrong.yaml` & `vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v2_wrong.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/manual_tests/templates/v3_high_mem_consumption.yaml` & `vitrage-9.0.0/doc/source/contributor/manual_tests/templates/v3_high_mem_consumption.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/manual_tests/test_web_server.py` & `vitrage-9.0.0/doc/source/contributor/manual_tests/test_web_server.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/mistral-config.rst` & `vitrage-9.0.0/doc/source/contributor/mistral-config.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/ml-jaccard_correlation.rst` & `vitrage-9.0.0/doc/source/contributor/ml-jaccard_correlation.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/nagios-config.rst` & `vitrage-9.0.0/doc/source/contributor/nagios-config.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/nagios-devstack-installation.rst` & `vitrage-9.0.0/doc/source/contributor/nagios-devstack-installation.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/not_operator_support.rst` & `vitrage-9.0.0/doc/source/contributor/not_operator_support.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/not_operator_support_v2.rst` & `vitrage-9.0.0/doc/source/contributor/not_operator_support_v2.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/notifier-snmp-plugin.rst` & `vitrage-9.0.0/doc/source/contributor/notifier-snmp-plugin.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/notifier-webhook-plugin.rst` & `vitrage-9.0.0/doc/source/contributor/notifier-webhook-plugin.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/nova-config.rst` & `vitrage-9.0.0/doc/source/contributor/nova-config.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/nova-notifier.rst` & `vitrage-9.0.0/doc/source/contributor/nova-notifier.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/profiler-config.rst` & `vitrage-9.0.0/doc/source/contributor/profiler-config.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/prometheus-datasource.rst` & `vitrage-9.0.0/doc/source/contributor/prometheus-datasource.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/resource-state-config.rst` & `vitrage-9.0.0/doc/source/contributor/resource-state-config.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/scenario-evaluator.rst` & `vitrage-9.0.0/doc/source/contributor/scenario-evaluator.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/static-config.rst` & `vitrage-9.0.0/doc/source/contributor/static-config.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/template_validation_status_code.rst` & `vitrage-9.0.0/doc/source/contributor/template_validation_status_code.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/templates-loading-v2.rst` & `vitrage-9.0.0/doc/source/contributor/templates-loading-v2.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/templates-loading.rst` & `vitrage-9.0.0/doc/source/contributor/templates-loading.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/tmfapi639-datasource.rst` & `vitrage-9.0.0/doc/source/contributor/tmfapi639-datasource.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/vitrage-api.rst` & `vitrage-9.0.0/doc/source/contributor/vitrage-api.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/vitrage-first_steps.rst` & `vitrage-9.0.0/doc/source/contributor/vitrage-first_steps.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/vitrage-graph-design.rst` & `vitrage-9.0.0/doc/source/contributor/vitrage-graph-design.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/vitrage-ha-and-history-vision.rst` & `vitrage-9.0.0/doc/source/contributor/vitrage-ha-and-history-vision.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/vitrage-template-format-v2.rst` & `vitrage-9.0.0/doc/source/contributor/vitrage-template-format-v2.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/vitrage-templates.rst` & `vitrage-9.0.0/doc/source/contributor/vitrage-templates.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/vitrage-use-cases.rst` & `vitrage-9.0.0/doc/source/contributor/vitrage-use-cases.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/contributor/zabbix_vitrage.rst` & `vitrage-9.0.0/doc/source/contributor/zabbix_vitrage.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/index.rst` & `vitrage-9.0.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/install/get_started.rst` & `vitrage-9.0.0/doc/source/install/get_started.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/doc/source/install/install-rdo.rst` & `vitrage-9.0.0/doc/source/install/install-rdo.rst`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/api-paste.ini` & `vitrage-9.0.0/etc/vitrage/api-paste.ini`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/aodh.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/aodh.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/cetus.cluster.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/cetus.cluster.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/cetus.pod.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/cetus.pod.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/cinder.volume.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/cinder.volume.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/default.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/default.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/heat.stack.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/heat.stack.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/nagios.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/nagios.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/network.interface.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/network.interface.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/neutron.network.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/neutron.network.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/neutron.port.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/neutron.port.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/nova.host.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/nova.host.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/nova.instance.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/nova.instance.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/nova.zone.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/nova.zone.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/openstack.cluster.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/openstack.cluster.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/static.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/static.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/static_physical.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/static_physical.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/switch.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/switch.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/trove.cluster.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/trove.cluster.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/trove.instance.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/trove.instance.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/vitrage.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/vitrage.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/datasources_values/zabbix.yaml` & `vitrage-9.0.0/etc/vitrage/datasources_values/zabbix.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/templates.sample/database_cluster_capacity_autoscaling.yaml` & `vitrage-9.0.0/etc/vitrage/templates.sample/database_cluster_capacity_autoscaling.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/templates.sample/host_down_scenarios.yaml` & `vitrage-9.0.0/etc/vitrage/templates.sample/host_down_scenarios.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/etc/vitrage/templates.sample/host_high_cpu_load_scenarios.yaml` & `vitrage-9.0.0/etc/vitrage/templates.sample/host_high_cpu_load_scenarios.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/releasenotes/notes/cetus-datasource-0c8297005ac6ca92.yaml` & `vitrage-9.0.0/releasenotes/notes/cetus-datasource-0c8297005ac6ca92.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/releasenotes/notes/deprecate-json-formatted-policy-file-6a1e9b690fdbc132.yaml` & `vitrage-9.0.0/releasenotes/notes/deprecate-json-formatted-policy-file-6a1e9b690fdbc132.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/releasenotes/notes/monasca-datasource-9ca61922ef14c2a8.yaml` & `vitrage-9.0.0/releasenotes/notes/monasca-datasource-9ca61922ef14c2a8.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/releasenotes/notes/queens-prelude-a00e64274e8e64be.yaml` & `vitrage-9.0.0/releasenotes/notes/queens-prelude-a00e64274e8e64be.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/releasenotes/notes/static-datasource-refactoring-2cc7569fafbe65c6.yaml` & `vitrage-9.0.0/releasenotes/notes/static-datasource-refactoring-2cc7569fafbe65c6.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/releasenotes/notes/stein-prelude-5e6f583803807d84.yaml` & `vitrage-9.0.0/releasenotes/notes/stein-prelude-5e6f583803807d84.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/releasenotes/notes/trove-datasource-2aa7a88ff20aff8c.yaml` & `vitrage-9.0.0/releasenotes/notes/trove-datasource-2aa7a88ff20aff8c.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/releasenotes/source/conf.py` & `vitrage-9.0.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/releasenotes/source/index.rst` & `vitrage-9.0.0/releasenotes/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 Contents
 ========
 
 .. toctree::
    :maxdepth: 2
 
    unreleased
+   yoga
    xena
    wallaby
    victoria
    ussuri
    train
    stein
    rocky
```

### Comparing `vitrage-8.0.1/requirements.txt` & `vitrage-9.0.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/setup.cfg` & `vitrage-9.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 name = vitrage
 summary = The OpenStack RCA Service
 description_file = 
 	README.rst
 author = OpenStack
 author_email = openstack-discuss@lists.openstack.org
 home_page = https://docs.openstack.org/vitrage/latest/
-python_requires = >=3.6
+python_requires = >=3.8
 classifier = 
 	Environment :: OpenStack
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Topic :: System :: Monitoring
 
 [extras]
 openstack = 
 	aodhclient>=1.0.0
```

### Comparing `vitrage-8.0.1/setup.py` & `vitrage-9.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/test-requirements.txt` & `vitrage-9.0.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/datasource-scaffold/sample/__init__.py` & `vitrage-9.0.0/tools/datasource-scaffold/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/datasource-scaffold/sample/driver.py` & `vitrage-9.0.0/tools/datasource-scaffold/sample/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/datasource-scaffold/sample/transformer.py` & `vitrage-9.0.0/tools/datasource-scaffold/sample/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/datasource-scaffold/{{cookiecutter.name}}/__init__.py` & `vitrage-9.0.0/tools/datasource-scaffold/{{cookiecutter.name}}/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/datasource-scaffold/{{cookiecutter.name}}/driver.py` & `vitrage-9.0.0/tools/datasource-scaffold/{{cookiecutter.name}}/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/datasource-scaffold/{{cookiecutter.name}}/transformer.py` & `vitrage-9.0.0/tools/datasource-scaffold/{{cookiecutter.name}}/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/load_generator/computes.yaml` & `vitrage-9.0.0/tools/load_generator/computes.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/load_generator/load_generator.py` & `vitrage-9.0.0/tools/load_generator/load_generator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/load_generator/notification_info.py` & `vitrage-9.0.0/tools/load_generator/notification_info.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/load_generator/templates/port_0.yaml` & `vitrage-9.0.0/tools/load_generator/templates/port_0.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/load_generator/templates/port_1.yaml` & `vitrage-9.0.0/tools/load_generator/templates/port_1.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/load_generator/templates/port_2.yaml` & `vitrage-9.0.0/tools/load_generator/templates/port_2.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/load_generator/templates/port_3.yaml` & `vitrage-9.0.0/tools/load_generator/templates/port_3.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/load_generator/templates/port_4.yaml` & `vitrage-9.0.0/tools/load_generator/templates/port_4.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/load_generator/templates/vm_0.yaml` & `vitrage-9.0.0/tools/load_generator/templates/vm_0.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/load_generator/templates/vm_1.yaml` & `vitrage-9.0.0/tools/load_generator/templates/vm_1.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/load_generator/templates/vm_2.yaml` & `vitrage-9.0.0/tools/load_generator/templates/vm_2.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/load_generator/templates/vm_3.yaml` & `vitrage-9.0.0/tools/load_generator/templates/vm_3.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tools/load_generator/templates/vm_4.yaml` & `vitrage-9.0.0/tools/load_generator/templates/vm_4.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/tox.ini` & `vitrage-9.0.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [testenv]
 basepython = python3
 usedevelop = True
 allowlist_externals = find
 setenv =
    VIRTUAL_ENV={envdir}
 deps =
-   -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/yoga}
+   -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
    -r{toxinidir}/test-requirements.txt
    -r{toxinidir}/requirements.txt
 commands =
     stestr run --serial {posargs}
     stestr slowest
     oslo-config-generator --config-file=etc/vitrage/vitrage-config-generator.conf
     find . -type f -name "test-*.db" -delete
@@ -41,15 +41,15 @@
     coverage combine
     coverage html -d cover
     coverage xml -o cover/coverage.xml
     coverage report
 
 [testenv:docs]
 deps =
-    -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/yoga}
+    -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
     -r{toxinidir}/doc/requirements.txt
 commands = sphinx-build -W -b html doc/source doc/build/html
 
 [testenv:debug]
 commands = oslo_debug_helper {posargs}
 
 [flake8]
```

### Comparing `vitrage-8.0.1/vitrage/__init__.py` & `vitrage-9.0.0/vitrage/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/__init__.py` & `vitrage-9.0.0/vitrage/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/app.py` & `vitrage-9.0.0/vitrage/api/app.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/app.wsgi` & `vitrage-9.0.0/vitrage/api/app.wsgi`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/controllers/rest.py` & `vitrage-9.0.0/vitrage/api/controllers/rest.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/controllers/root.py` & `vitrage-9.0.0/vitrage/api/controllers/root.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/controllers/v1/alarm.py` & `vitrage-9.0.0/vitrage/api/controllers/v1/alarm.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/controllers/v1/alarm_base.py` & `vitrage-9.0.0/vitrage/api/controllers/v1/alarm_base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/controllers/v1/count.py` & `vitrage-9.0.0/vitrage/api/controllers/v1/count.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/controllers/v1/event.py` & `vitrage-9.0.0/vitrage/api/controllers/v1/event.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/controllers/v1/history.py` & `vitrage-9.0.0/vitrage/api/controllers/v1/history.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/controllers/v1/rca.py` & `vitrage-9.0.0/vitrage/api/controllers/v1/rca.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/controllers/v1/resource.py` & `vitrage-9.0.0/vitrage/api/controllers/v1/resource.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/controllers/v1/root.py` & `vitrage-9.0.0/vitrage/api/controllers/v1/root.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/controllers/v1/service.py` & `vitrage-9.0.0/vitrage/api/controllers/v1/service.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/controllers/v1/status.py` & `vitrage-9.0.0/vitrage/api/controllers/v1/status.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/controllers/v1/template.py` & `vitrage-9.0.0/vitrage/api/controllers/v1/template.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/controllers/v1/topology.py` & `vitrage-9.0.0/vitrage/api/controllers/v1/topology.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/controllers/v1/webhook.py` & `vitrage-9.0.0/vitrage/api/controllers/v1/webhook.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/hooks.py` & `vitrage-9.0.0/vitrage/api/hooks.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api/policy.py` & `vitrage-9.0.0/vitrage/api/policy.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api_handler/apis/alarm.py` & `vitrage-9.0.0/vitrage/api_handler/apis/alarm.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api_handler/apis/base.py` & `vitrage-9.0.0/vitrage/api_handler/apis/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api_handler/apis/event.py` & `vitrage-9.0.0/vitrage/api_handler/apis/event.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api_handler/apis/operational.py` & `vitrage-9.0.0/vitrage/api_handler/apis/operational.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api_handler/apis/rca.py` & `vitrage-9.0.0/vitrage/api_handler/apis/rca.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api_handler/apis/resource.py` & `vitrage-9.0.0/vitrage/api_handler/apis/resource.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api_handler/apis/template.py` & `vitrage-9.0.0/vitrage/api_handler/apis/template.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api_handler/apis/topology.py` & `vitrage-9.0.0/vitrage/api_handler/apis/topology.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/api_handler/apis/webhook.py` & `vitrage-9.0.0/vitrage/api_handler/apis/webhook.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/cli/__init__.py` & `vitrage-9.0.0/vitrage/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/cli/api.py` & `vitrage-9.0.0/vitrage/cli/api.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/cli/graph.py` & `vitrage-9.0.0/vitrage/cli/graph.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/cli/machine_learning.py` & `vitrage-9.0.0/vitrage/cli/machine_learning.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/cli/notifier.py` & `vitrage-9.0.0/vitrage/cli/notifier.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/cli/persistor.py` & `vitrage-9.0.0/vitrage/cli/persistor.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/cli/snmp_parsing.py` & `vitrage-9.0.0/vitrage/cli/snmp_parsing.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/cli/status.py` & `vitrage-9.0.0/vitrage/cli/status.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/cli/storage.py` & `vitrage-9.0.0/vitrage/cli/storage.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/common/config.py` & `vitrage-9.0.0/vitrage/common/config.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/common/constants.py` & `vitrage-9.0.0/vitrage/common/constants.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/common/exception.py` & `vitrage-9.0.0/vitrage/common/exception.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/common/policies/__init__.py` & `vitrage-9.0.0/vitrage/common/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/common/policies/alarms.py` & `vitrage-9.0.0/vitrage/common/policies/alarms.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/common/policies/base.py` & `vitrage-9.0.0/vitrage/common/policies/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/common/policies/event.py` & `vitrage-9.0.0/vitrage/common/policies/event.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/common/policies/rca.py` & `vitrage-9.0.0/vitrage/common/policies/rca.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/common/policies/resource.py` & `vitrage-9.0.0/vitrage/common/policies/resource.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/common/policies/service.py` & `vitrage-9.0.0/vitrage/common/policies/service.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/common/policies/status.py` & `vitrage-9.0.0/vitrage/common/policies/status.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/common/policies/template.py` & `vitrage-9.0.0/vitrage/common/policies/template.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/common/policies/topology.py` & `vitrage-9.0.0/vitrage/common/policies/topology.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/common/policies/webhook.py` & `vitrage-9.0.0/vitrage/common/policies/webhook.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/common/utils.py` & `vitrage-9.0.0/vitrage/common/utils.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/coordination/__init__.py` & `vitrage-9.0.0/vitrage/coordination/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/coordination/coordination.py` & `vitrage-9.0.0/vitrage/coordination/coordination.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/coordination/service.py` & `vitrage-9.0.0/vitrage/coordination/service.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/__init__.py` & `vitrage-9.0.0/vitrage/datasources/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/alarm_driver_base.py` & `vitrage-9.0.0/vitrage/datasources/alarm_driver_base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/alarm_properties.py` & `vitrage-9.0.0/vitrage/datasources/alarm_properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/alarm_transformer_base.py` & `vitrage-9.0.0/vitrage/datasources/alarm_transformer_base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/aodh/__init__.py` & `vitrage-9.0.0/vitrage/datasources/aodh/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/aodh/driver.py` & `vitrage-9.0.0/vitrage/datasources/aodh/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/aodh/properties.py` & `vitrage-9.0.0/vitrage/datasources/aodh/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/aodh/transformer.py` & `vitrage-9.0.0/vitrage/datasources/aodh/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/ceilometer/__init__.py` & `vitrage-9.0.0/vitrage/datasources/ceilometer/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/ceilometer/driver.py` & `vitrage-9.0.0/vitrage/datasources/ceilometer/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/ceilometer/properties.py` & `vitrage-9.0.0/vitrage/datasources/ceilometer/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/ceilometer/transformer.py` & `vitrage-9.0.0/vitrage/datasources/ceilometer/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/cetus/cetus_driver_base.py` & `vitrage-9.0.0/vitrage/datasources/cetus/cetus_driver_base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/cetus/cluster/__init__.py` & `vitrage-9.0.0/vitrage/datasources/cetus/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/cetus/cluster/driver.py` & `vitrage-9.0.0/vitrage/datasources/cetus/cluster/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/cetus/cluster/transformer.py` & `vitrage-9.0.0/vitrage/datasources/cetus/cluster/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/cetus/pod/__init__.py` & `vitrage-9.0.0/vitrage/datasources/cetus/pod/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/cetus/pod/driver.py` & `vitrage-9.0.0/vitrage/datasources/cetus/pod/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/cetus/pod/transformer.py` & `vitrage-9.0.0/vitrage/datasources/cetus/pod/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/cetus/properties.py` & `vitrage-9.0.0/vitrage/datasources/cetus/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/cinder/volume/__init__.py` & `vitrage-9.0.0/vitrage/datasources/cinder/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/cinder/volume/driver.py` & `vitrage-9.0.0/vitrage/datasources/cinder/volume/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/cinder/volume/properties.py` & `vitrage-9.0.0/vitrage/datasources/cinder/volume/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/cinder/volume/transformer.py` & `vitrage-9.0.0/vitrage/datasources/cinder/volume/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/collectd/__init__.py` & `vitrage-9.0.0/vitrage/datasources/collectd/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/collectd/collectd_vitrage/getsigchld.py` & `vitrage-9.0.0/vitrage/datasources/collectd/collectd_vitrage/getsigchld.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/collectd/collectd_vitrage/plugin.py` & `vitrage-9.0.0/vitrage/datasources/collectd/collectd_vitrage/plugin.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/collectd/collectd_vitrage/readme` & `vitrage-9.0.0/vitrage/datasources/collectd/collectd_vitrage/readme`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/collectd/collectd_vitrage/vitrageplugin.py` & `vitrage-9.0.0/vitrage/datasources/collectd/collectd_vitrage/vitrageplugin.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/collectd/driver.py` & `vitrage-9.0.0/vitrage/datasources/collectd/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/collectd/mapper.py` & `vitrage-9.0.0/vitrage/datasources/collectd/mapper.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/collectd/properties.py` & `vitrage-9.0.0/vitrage/datasources/collectd/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/collectd/transformer.py` & `vitrage-9.0.0/vitrage/datasources/collectd/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/consistency/__init__.py` & `vitrage-9.0.0/vitrage/datasources/consistency/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/consistency/transformer.py` & `vitrage-9.0.0/vitrage/datasources/consistency/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/doctor/__init__.py` & `vitrage-9.0.0/vitrage/datasources/doctor/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/doctor/driver.py` & `vitrage-9.0.0/vitrage/datasources/doctor/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/doctor/properties.py` & `vitrage-9.0.0/vitrage/datasources/doctor/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/doctor/transformer.py` & `vitrage-9.0.0/vitrage/datasources/doctor/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/driver_base.py` & `vitrage-9.0.0/vitrage/datasources/driver_base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/heat/stack/__init__.py` & `vitrage-9.0.0/vitrage/datasources/heat/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/heat/stack/driver.py` & `vitrage-9.0.0/vitrage/datasources/heat/stack/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/heat/stack/properties.py` & `vitrage-9.0.0/vitrage/datasources/heat/stack/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/heat/stack/transformer.py` & `vitrage-9.0.0/vitrage/datasources/heat/stack/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/kapacitor/__init__.py` & `vitrage-9.0.0/vitrage/datasources/kapacitor/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/kapacitor/auxiliary/kapacitor_vitrage.py` & `vitrage-9.0.0/vitrage/datasources/kapacitor/auxiliary/kapacitor_vitrage.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/kapacitor/config.py` & `vitrage-9.0.0/vitrage/datasources/kapacitor/config.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/kapacitor/driver.py` & `vitrage-9.0.0/vitrage/datasources/kapacitor/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/kapacitor/properties.py` & `vitrage-9.0.0/vitrage/datasources/kapacitor/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/kapacitor/transformer.py` & `vitrage-9.0.0/vitrage/datasources/kapacitor/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/kubernetes/__init__.py` & `vitrage-9.0.0/vitrage/datasources/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/kubernetes/driver.py` & `vitrage-9.0.0/vitrage/datasources/kubernetes/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/kubernetes/properties.py` & `vitrage-9.0.0/vitrage/datasources/kubernetes/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/kubernetes/transformer.py` & `vitrage-9.0.0/vitrage/datasources/kubernetes/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/monasca/__init__.py` & `vitrage-9.0.0/vitrage/datasources/monasca/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/monasca/driver.py` & `vitrage-9.0.0/vitrage/datasources/monasca/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/monasca/properties.py` & `vitrage-9.0.0/vitrage/datasources/monasca/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/monasca/transformer.py` & `vitrage-9.0.0/vitrage/datasources/monasca/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nagios/__init__.py` & `vitrage-9.0.0/vitrage/datasources/nagios/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nagios/config.py` & `vitrage-9.0.0/vitrage/datasources/nagios/config.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nagios/driver.py` & `vitrage-9.0.0/vitrage/datasources/nagios/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nagios/parser.py` & `vitrage-9.0.0/vitrage/datasources/nagios/parser.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nagios/properties.py` & `vitrage-9.0.0/vitrage/datasources/nagios/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nagios/transformer.py` & `vitrage-9.0.0/vitrage/datasources/nagios/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/neutron/base.py` & `vitrage-9.0.0/vitrage/datasources/neutron/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/neutron/network/__init__.py` & `vitrage-9.0.0/vitrage/datasources/neutron/network/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/neutron/network/driver.py` & `vitrage-9.0.0/vitrage/datasources/neutron/network/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/neutron/network/transformer.py` & `vitrage-9.0.0/vitrage/datasources/neutron/network/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/neutron/port/__init__.py` & `vitrage-9.0.0/vitrage/datasources/neutron/port/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/neutron/port/driver.py` & `vitrage-9.0.0/vitrage/datasources/neutron/port/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/neutron/port/transformer.py` & `vitrage-9.0.0/vitrage/datasources/neutron/port/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/neutron/properties.py` & `vitrage-9.0.0/vitrage/datasources/neutron/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nova/host/__init__.py` & `vitrage-9.0.0/vitrage/datasources/nova/host/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nova/host/driver.py` & `vitrage-9.0.0/vitrage/datasources/nova/host/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nova/host/transformer.py` & `vitrage-9.0.0/vitrage/datasources/nova/host/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nova/instance/__init__.py` & `vitrage-9.0.0/vitrage/datasources/nova/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nova/instance/driver.py` & `vitrage-9.0.0/vitrage/datasources/nova/instance/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nova/instance/field_extractor.py` & `vitrage-9.0.0/vitrage/datasources/nova/instance/field_extractor.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nova/instance/transformer.py` & `vitrage-9.0.0/vitrage/datasources/nova/instance/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nova/nova_driver_base.py` & `vitrage-9.0.0/vitrage/datasources/nova/nova_driver_base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nova/properties.py` & `vitrage-9.0.0/vitrage/datasources/nova/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nova/zone/__init__.py` & `vitrage-9.0.0/vitrage/datasources/nova/zone/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nova/zone/driver.py` & `vitrage-9.0.0/vitrage/datasources/nova/zone/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/nova/zone/transformer.py` & `vitrage-9.0.0/vitrage/datasources/nova/zone/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/prometheus/__init__.py` & `vitrage-9.0.0/vitrage/datasources/prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/prometheus/driver.py` & `vitrage-9.0.0/vitrage/datasources/prometheus/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/prometheus/properties.py` & `vitrage-9.0.0/vitrage/datasources/prometheus/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/prometheus/transformer.py` & `vitrage-9.0.0/vitrage/datasources/prometheus/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/resource_transformer_base.py` & `vitrage-9.0.0/vitrage/datasources/resource_transformer_base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/static/__init__.py` & `vitrage-9.0.0/vitrage/datasources/static/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/static/driver.py` & `vitrage-9.0.0/vitrage/datasources/static/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/static/transformer.py` & `vitrage-9.0.0/vitrage/datasources/static/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/tmfapi639/__init__.py` & `vitrage-9.0.0/vitrage/datasources/tmfapi639/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/tmfapi639/config.py` & `vitrage-9.0.0/vitrage/datasources/tmfapi639/config.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/tmfapi639/driver.py` & `vitrage-9.0.0/vitrage/datasources/tmfapi639/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/tmfapi639/transformer.py` & `vitrage-9.0.0/vitrage/datasources/tmfapi639/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/transformer_base.py` & `vitrage-9.0.0/vitrage/datasources/transformer_base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/trove/cluster/__init__.py` & `vitrage-9.0.0/vitrage/datasources/trove/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/trove/cluster/driver.py` & `vitrage-9.0.0/vitrage/datasources/trove/cluster/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/trove/cluster/transformer.py` & `vitrage-9.0.0/vitrage/datasources/trove/cluster/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/trove/instance/__init__.py` & `vitrage-9.0.0/vitrage/datasources/trove/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/trove/instance/driver.py` & `vitrage-9.0.0/vitrage/datasources/trove/instance/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/trove/instance/transformer.py` & `vitrage-9.0.0/vitrage/datasources/trove/instance/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/trove/properties.py` & `vitrage-9.0.0/vitrage/datasources/trove/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/trove/trove_driver_base.py` & `vitrage-9.0.0/vitrage/datasources/trove/trove_driver_base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/utils.py` & `vitrage-9.0.0/vitrage/datasources/utils.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/zabbix/__init__.py` & `vitrage-9.0.0/vitrage/datasources/zabbix/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/zabbix/auxiliary/readme` & `vitrage-9.0.0/vitrage/datasources/zabbix/auxiliary/readme`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/zabbix/auxiliary/zabbix_vitrage.py` & `vitrage-9.0.0/vitrage/datasources/zabbix/auxiliary/zabbix_vitrage.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/zabbix/driver.py` & `vitrage-9.0.0/vitrage/datasources/zabbix/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/zabbix/properties.py` & `vitrage-9.0.0/vitrage/datasources/zabbix/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/datasources/zabbix/transformer.py` & `vitrage-9.0.0/vitrage/datasources/zabbix/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/__init__.py` & `vitrage-9.0.0/vitrage/entity_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/consistency/__init__.py` & `vitrage-9.0.0/vitrage/entity_graph/consistency/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/consistency/consistency_enforcer.py` & `vitrage-9.0.0/vitrage/entity_graph/consistency/consistency_enforcer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/driver_exec.py` & `vitrage-9.0.0/vitrage/entity_graph/driver_exec.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/graph_init.py` & `vitrage-9.0.0/vitrage/entity_graph/graph_init.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/graph_persistency.py` & `vitrage-9.0.0/vitrage/entity_graph/graph_persistency.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/mappings/alarm_handler.py` & `vitrage-9.0.0/vitrage/entity_graph/mappings/alarm_handler.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/mappings/datasource_info_mapper.py` & `vitrage-9.0.0/vitrage/entity_graph/mappings/datasource_info_mapper.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/mappings/handler_base.py` & `vitrage-9.0.0/vitrage/entity_graph/mappings/handler_base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/mappings/operational_alarm_severity.py` & `vitrage-9.0.0/vitrage/entity_graph/mappings/operational_alarm_severity.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/mappings/operational_resource_state.py` & `vitrage-9.0.0/vitrage/entity_graph/mappings/operational_resource_state.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/mappings/resource_handler.py` & `vitrage-9.0.0/vitrage/entity_graph/mappings/resource_handler.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/processor/base.py` & `vitrage-9.0.0/vitrage/entity_graph/processor/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/processor/notifier.py` & `vitrage-9.0.0/vitrage/entity_graph/processor/notifier.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/processor/processor.py` & `vitrage-9.0.0/vitrage/entity_graph/processor/processor.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/processor/processor_utils.py` & `vitrage-9.0.0/vitrage/entity_graph/processor/processor_utils.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/processor/transformer_manager.py` & `vitrage-9.0.0/vitrage/entity_graph/processor/transformer_manager.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/scheduler.py` & `vitrage-9.0.0/vitrage/entity_graph/scheduler.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/entity_graph/workers.py` & `vitrage-9.0.0/vitrage/entity_graph/workers.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/__init__.py` & `vitrage-9.0.0/vitrage/evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/actions/__init__.py` & `vitrage-9.0.0/vitrage/evaluator/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/actions/action_executor.py` & `vitrage-9.0.0/vitrage/evaluator/actions/action_executor.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/actions/base.py` & `vitrage-9.0.0/vitrage/evaluator/actions/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/actions/evaluator_event_transformer.py` & `vitrage-9.0.0/vitrage/evaluator/actions/evaluator_event_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/actions/notifier.py` & `vitrage-9.0.0/vitrage/evaluator/actions/notifier.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/actions/priority_tools.py` & `vitrage-9.0.0/vitrage/evaluator/actions/priority_tools.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/actions/recipes/action_steps.py` & `vitrage-9.0.0/vitrage/evaluator/actions/recipes/action_steps.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/actions/recipes/add_causal_relationship.py` & `vitrage-9.0.0/vitrage/evaluator/actions/recipes/add_causal_relationship.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/actions/recipes/base.py` & `vitrage-9.0.0/vitrage/evaluator/actions/recipes/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/actions/recipes/execute_mistral.py` & `vitrage-9.0.0/vitrage/evaluator/actions/recipes/execute_mistral.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/actions/recipes/mark_down.py` & `vitrage-9.0.0/vitrage/evaluator/actions/recipes/mark_down.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/actions/recipes/raise_alarm.py` & `vitrage-9.0.0/vitrage/evaluator/actions/recipes/raise_alarm.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/actions/recipes/set_state.py` & `vitrage-9.0.0/vitrage/evaluator/actions/recipes/set_state.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/base.py` & `vitrage-9.0.0/vitrage/evaluator/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/condition.py` & `vitrage-9.0.0/vitrage/evaluator/condition.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/equivalence_repository.py` & `vitrage-9.0.0/vitrage/evaluator/equivalence_repository.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/scenario_evaluator.py` & `vitrage-9.0.0/vitrage/evaluator/scenario_evaluator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/scenario_repository.py` & `vitrage-9.0.0/vitrage/evaluator/scenario_repository.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_data.py` & `vitrage-9.0.0/vitrage/evaluator/template_data.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_db/template_repository.py` & `vitrage-9.0.0/vitrage/evaluator/template_db/template_repository.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_fields.py` & `vitrage-9.0.0/vitrage/evaluator/template_fields.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_functions/__init__.py` & `vitrage-9.0.0/vitrage/evaluator/template_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_functions/function_resolver.py` & `vitrage-9.0.0/vitrage/evaluator/template_functions/function_resolver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_functions/v2/__init__.py` & `vitrage-9.0.0/vitrage/evaluator/template_functions/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_functions/v2/functions.py` & `vitrage-9.0.0/vitrage/evaluator/template_functions/v2/functions.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_loading/equivalence_loader.py` & `vitrage-9.0.0/vitrage/evaluator/template_loading/equivalence_loader.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_loading/props_converter.py` & `vitrage-9.0.0/vitrage/evaluator/template_loading/props_converter.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_loading/scenario_loader.py` & `vitrage-9.0.0/vitrage/evaluator/template_loading/scenario_loader.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_loading/subgraph_builder.py` & `vitrage-9.0.0/vitrage/evaluator/template_loading/subgraph_builder.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_loading/template_loader.py` & `vitrage-9.0.0/vitrage/evaluator/template_loading/template_loader.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_loading/template_loader_v3.py` & `vitrage-9.0.0/vitrage/evaluator/template_loading/template_loader_v3.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_loading/v1/action_loader.py` & `vitrage-9.0.0/vitrage/evaluator/template_loading/v1/action_loader.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_loading/v1/execute_mistral_loader.py` & `vitrage-9.0.0/vitrage/evaluator/template_loading/v1/execute_mistral_loader.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_loading/v3/action_loader.py` & `vitrage-9.0.0/vitrage/evaluator/template_loading/v3/action_loader.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_loading/v3/raise_alarm_loader.py` & `vitrage-9.0.0/vitrage/evaluator/template_loading/v3/raise_alarm_loader.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_schema_factory.py` & `vitrage-9.0.0/vitrage/evaluator/template_schema_factory.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_schemas.py` & `vitrage-9.0.0/vitrage/evaluator/template_schemas.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/__init__.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/base.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/content/base.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/content/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/content/template_content_validator.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/content/template_content_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/content/template_content_validator_v3.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/content/template_content_validator_v3.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/add_causal_relationship_validator.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/add_causal_relationship_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/definitions_validator.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/definitions_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/execute_mistral_validator.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/execute_mistral_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/get_param_validator.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/get_param_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/mark_down_validator.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/mark_down_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/metadata_validator.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/metadata_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/raise_alarm_validator.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/raise_alarm_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/scenario_validator.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/scenario_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/content/v1/set_state_validator.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/content/v1/set_state_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/content/v2/execute_mistral_validator.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/content/v2/execute_mistral_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/content/v2/get_param_validator.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/content/v2/get_param_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/content/v2/metadata_validator.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/content/v2/metadata_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/status_messages.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/status_messages.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/template_syntax_validator.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/template_syntax_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/evaluator/template_validation/template_syntax_validator_v3.py` & `vitrage-9.0.0/vitrage/evaluator/template_validation/template_syntax_validator_v3.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/graph/__init__.py` & `vitrage-9.0.0/vitrage/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/graph/algo_driver/algorithm.py` & `vitrage-9.0.0/vitrage/graph/algo_driver/algorithm.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/graph/algo_driver/networkx_algorithm.py` & `vitrage-9.0.0/vitrage/graph/algo_driver/networkx_algorithm.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/graph/algo_driver/sub_graph_matching.py` & `vitrage-9.0.0/vitrage/graph/algo_driver/sub_graph_matching.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/graph/driver/__init__.py` & `vitrage-9.0.0/vitrage/graph/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/graph/driver/elements.py` & `vitrage-9.0.0/vitrage/graph/driver/elements.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/graph/driver/graph.py` & `vitrage-9.0.0/vitrage/graph/driver/graph.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/graph/driver/networkx_graph.py` & `vitrage-9.0.0/vitrage/graph/driver/networkx_graph.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/graph/driver/notifier.py` & `vitrage-9.0.0/vitrage/graph/driver/notifier.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/graph/filter.py` & `vitrage-9.0.0/vitrage/graph/filter.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/graph/query.py` & `vitrage-9.0.0/vitrage/graph/query.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/graph/utils.py` & `vitrage-9.0.0/vitrage/graph/utils.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/hacking/checks.py` & `vitrage-9.0.0/vitrage/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/i18n.py` & `vitrage-9.0.0/vitrage/i18n.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/keystone_client.py` & `vitrage-9.0.0/vitrage/keystone_client.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/machine_learning/__init__.py` & `vitrage-9.0.0/vitrage/machine_learning/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/machine_learning/plugins/base.py` & `vitrage-9.0.0/vitrage/machine_learning/plugins/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/machine_learning/plugins/jaccard_correlation/__init__.py` & `vitrage-9.0.0/vitrage/machine_learning/plugins/jaccard_correlation/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/machine_learning/plugins/jaccard_correlation/accumulation_persistor_utils.py` & `vitrage-9.0.0/vitrage/machine_learning/plugins/jaccard_correlation/accumulation_persistor_utils.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/machine_learning/plugins/jaccard_correlation/alarm_data_accumulator.py` & `vitrage-9.0.0/vitrage/machine_learning/plugins/jaccard_correlation/alarm_data_accumulator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/machine_learning/plugins/jaccard_correlation/alarm_processor.py` & `vitrage-9.0.0/vitrage/machine_learning/plugins/jaccard_correlation/alarm_processor.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/machine_learning/plugins/jaccard_correlation/correlation_collection.py` & `vitrage-9.0.0/vitrage/machine_learning/plugins/jaccard_correlation/correlation_collection.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/machine_learning/plugins/jaccard_correlation/correlation_manager.py` & `vitrage-9.0.0/vitrage/machine_learning/plugins/jaccard_correlation/correlation_manager.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/machine_learning/service.py` & `vitrage-9.0.0/vitrage/machine_learning/service.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/messaging.py` & `vitrage-9.0.0/vitrage/messaging.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/middleware/basic_and_keystone_auth.py` & `vitrage-9.0.0/vitrage/middleware/basic_and_keystone_auth.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/middleware/keycloak.py` & `vitrage-9.0.0/vitrage/middleware/keycloak.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/__init__.py` & `vitrage-9.0.0/vitrage/notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/aodh/__init__.py` & `vitrage-9.0.0/vitrage/notifier/plugins/aodh/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/aodh/aodh_notifier.py` & `vitrage-9.0.0/vitrage/notifier/plugins/aodh/aodh_notifier.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/base.py` & `vitrage-9.0.0/vitrage/notifier/plugins/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/mistral/__init__.py` & `vitrage-9.0.0/vitrage/notifier/plugins/mistral/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/mistral/mistral_notifier.py` & `vitrage-9.0.0/vitrage/notifier/plugins/mistral/mistral_notifier.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/nova/__init__.py` & `vitrage-9.0.0/vitrage/notifier/plugins/nova/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/nova/nova_notifier.py` & `vitrage-9.0.0/vitrage/notifier/plugins/nova/nova_notifier.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/snmp/__init__.py` & `vitrage-9.0.0/vitrage/notifier/plugins/snmp/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/snmp/base.py` & `vitrage-9.0.0/vitrage/notifier/plugins/snmp/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/snmp/snmp_notifier.py` & `vitrage-9.0.0/vitrage/notifier/plugins/snmp/snmp_notifier.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/snmp/snmp_sender.py` & `vitrage-9.0.0/vitrage/notifier/plugins/snmp/snmp_sender.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/webhook/__init__.py` & `vitrage-9.0.0/vitrage/notifier/plugins/webhook/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/webhook/utils.py` & `vitrage-9.0.0/vitrage/notifier/plugins/webhook/utils.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/webhook/webhook.py` & `vitrage-9.0.0/vitrage/notifier/plugins/webhook/webhook.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/zaqar/__init__.py` & `vitrage-9.0.0/vitrage/notifier/plugins/zaqar/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/plugins/zaqar/zaqar_notifier.py` & `vitrage-9.0.0/vitrage/notifier/plugins/zaqar/zaqar_notifier.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/notifier/service.py` & `vitrage-9.0.0/vitrage/notifier/service.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/opts.py` & `vitrage-9.0.0/vitrage/opts.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/os_clients.py` & `vitrage-9.0.0/vitrage/os_clients.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/persistency/__init__.py` & `vitrage-9.0.0/vitrage/persistency/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/persistency/service.py` & `vitrage-9.0.0/vitrage/persistency/service.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/rpc.py` & `vitrage-9.0.0/vitrage/rpc.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/snmp_parsing/__init__.py` & `vitrage-9.0.0/vitrage/snmp_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/snmp_parsing/properties.py` & `vitrage-9.0.0/vitrage/snmp_parsing/properties.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/snmp_parsing/service.py` & `vitrage-9.0.0/vitrage/snmp_parsing/service.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/storage/__init__.py` & `vitrage-9.0.0/vitrage/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/storage/base.py` & `vitrage-9.0.0/vitrage/storage/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/storage/history_facade.py` & `vitrage-9.0.0/vitrage/storage/history_facade.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/storage/impl_sqlalchemy.py` & `vitrage-9.0.0/vitrage/storage/impl_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/__init__.py` & `vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/alembic.ini` & `vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/alembic_migrations/README` & `vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/alembic_migrations/README`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/alembic_migrations/env.py` & `vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/alembic_migrations/env.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/alembic_migrations/script.py.mako` & `vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/alembic_migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/storage/sqlalchemy/migration/alembic_migrations/versions/4e44c9414dff_initial_migration.py` & `vitrage-9.0.0/vitrage/storage/sqlalchemy/migration/alembic_migrations/versions/4e44c9414dff_initial_migration.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/storage/sqlalchemy/models.py` & `vitrage-9.0.0/vitrage/storage/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/base.py` & `vitrage-9.0.0/vitrage/tests/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/api/__init__.py` & `vitrage-9.0.0/vitrage/tests/functional/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/api/test_versions.py` & `vitrage-9.0.0/vitrage/tests/functional/api/test_versions.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/api/v1/__init__.py` & `vitrage-9.0.0/vitrage/tests/functional/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/api/v1/test_auth.py` & `vitrage-9.0.0/vitrage/tests/functional/api/v1/test_auth.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/api/v1/test_basic.py` & `vitrage-9.0.0/vitrage/tests/functional/api/v1/test_basic.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/api/v1/test_health.py` & `vitrage-9.0.0/vitrage/tests/functional/api/v1/test_health.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/api/v1/test_keycloak.py` & `vitrage-9.0.0/vitrage/tests/functional/api/v1/test_keycloak.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/api/v1/test_noauth.py` & `vitrage-9.0.0/vitrage/tests/functional/api/v1/test_noauth.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/api/v1/test_service.py` & `vitrage-9.0.0/vitrage/tests/functional/api/v1/test_service.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/api/v1/test_status.py` & `vitrage-9.0.0/vitrage/tests/functional/api/v1/test_status.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/api/v1/test_template_versions.py` & `vitrage-9.0.0/vitrage/tests/functional/api/v1/test_template_versions.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/api_handler/test_apis.py` & `vitrage-9.0.0/vitrage/tests/functional/api_handler/test_apis.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/api_handler/test_templates.py` & `vitrage-9.0.0/vitrage/tests/functional/api_handler/test_templates.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/api_handler/test_templates_v2.py` & `vitrage-9.0.0/vitrage/tests/functional/api_handler/test_templates_v2.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/api_handler/test_templates_v3.py` & `vitrage-9.0.0/vitrage/tests/functional/api_handler/test_templates_v3.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/base.py` & `vitrage-9.0.0/vitrage/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/datasources/aodh/test_aodh.py` & `vitrage-9.0.0/vitrage/tests/functional/datasources/aodh/test_aodh.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/datasources/base.py` & `vitrage-9.0.0/vitrage/tests/functional/datasources/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/datasources/ceilometer/test_ceilometer.py` & `vitrage-9.0.0/vitrage/tests/functional/datasources/ceilometer/test_ceilometer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/datasources/cinder/test_cinder_volume.py` & `vitrage-9.0.0/vitrage/tests/functional/datasources/cinder/test_cinder_volume.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/datasources/collectd/test_collectd.py` & `vitrage-9.0.0/vitrage/tests/functional/datasources/collectd/test_collectd.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/datasources/heat/test_heat_stack.py` & `vitrage-9.0.0/vitrage/tests/functional/datasources/heat/test_heat_stack.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/datasources/listener_service/test_listener_service.py` & `vitrage-9.0.0/vitrage/tests/functional/datasources/listener_service/test_listener_service.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/datasources/nagios/test_nagios.py` & `vitrage-9.0.0/vitrage/tests/functional/datasources/nagios/test_nagios.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/datasources/nova/test_nova_datasources.py` & `vitrage-9.0.0/vitrage/tests/functional/datasources/nova/test_nova_datasources.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/datasources/trove/test_trove_instance.py` & `vitrage-9.0.0/vitrage/tests/functional/datasources/trove/test_trove_instance.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/entity_graph/consistency/test_consistency.py` & `vitrage-9.0.0/vitrage/tests/functional/entity_graph/consistency/test_consistency.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/entity_graph/graph_persistor/test_graph_persistor.py` & `vitrage-9.0.0/vitrage/tests/functional/entity_graph/graph_persistor/test_graph_persistor.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/entity_graph/processor/test_processor.py` & `vitrage-9.0.0/vitrage/tests/functional/entity_graph/processor/test_processor.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/entity_graph/states/test_datasource_info_mapper.py` & `vitrage-9.0.0/vitrage/tests/functional/entity_graph/states/test_datasource_info_mapper.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/evaluator/test_action_executor.py` & `vitrage-9.0.0/vitrage/tests/functional/evaluator/test_action_executor.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/evaluator/test_scenario_evaluator.py` & `vitrage-9.0.0/vitrage/tests/functional/evaluator/test_scenario_evaluator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/functional/test_configuration.py` & `vitrage-9.0.0/vitrage/tests/functional/test_configuration.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/mocks/entity_model.py` & `vitrage-9.0.0/vitrage/tests/mocks/entity_model.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/mocks/graph_generator.py` & `vitrage-9.0.0/vitrage/tests/mocks/graph_generator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/mocks/mock_driver.py` & `vitrage-9.0.0/vitrage/tests/mocks/mock_driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/mocks/mock_graph_datasource/__init__.py` & `vitrage-9.0.0/vitrage/tests/mocks/mock_graph_datasource/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/mocks/mock_graph_datasource/driver.py` & `vitrage-9.0.0/vitrage/tests/mocks/mock_graph_datasource/driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/mocks/mock_graph_datasource/transformer.py` & `vitrage-9.0.0/vitrage/tests/mocks/mock_graph_datasource/transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/mocks/mock_transformer.py` & `vitrage-9.0.0/vitrage/tests/mocks/mock_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/mocks/trace_generator.py` & `vitrage-9.0.0/vitrage/tests/mocks/trace_generator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/mocks/utils.py` & `vitrage-9.0.0/vitrage/tests/mocks/utils.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/datasources_values/default.yaml` & `vitrage-9.0.0/vitrage/tests/resources/datasources_values/default.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/datasources_values/erroneous_values/default.yaml` & `vitrage-9.0.0/vitrage/tests/resources/datasources_values/erroneous_values/default.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/datasources_values/erroneous_values/nagios.yaml` & `vitrage-9.0.0/vitrage/tests/resources/datasources_values/erroneous_values/nagios.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/datasources_values/erroneous_values/nova.host.yaml` & `vitrage-9.0.0/vitrage/tests/resources/datasources_values/erroneous_values/nova.host.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/datasources_values/erroneous_values/nova.instance.yaml` & `vitrage-9.0.0/vitrage/tests/resources/datasources_values/erroneous_values/nova.instance.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/datasources_values/nagios.yaml` & `vitrage-9.0.0/vitrage/tests/resources/datasources_values/nagios.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/datasources_values/nova.host.yaml` & `vitrage-9.0.0/vitrage/tests/resources/datasources_values/nova.host.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/datasources_values/nova.instance.yaml` & `vitrage-9.0.0/vitrage/tests/resources/datasources_values/nova.instance.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/datasources_values/nova.zone.yaml` & `vitrage-9.0.0/vitrage/tests/resources/datasources_values/nova.zone.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/datasources_values/vitrage.yaml` & `vitrage-9.0.0/vitrage/tests/resources/datasources_values/vitrage.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_inst_snapshot_dynamic.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_inst_snapshot_dynamic.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_inst_update_legacy_dynamic.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_inst_update_legacy_dynamic.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_inst_update_versioned_dynamic.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_inst_update_versioned_dynamic.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_prometheus_update_dynamic.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_prometheus_update_dynamic.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_stack_snapshot_dynamic.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_stack_snapshot_dynamic.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_stack_update_dynamic.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_stack_update_dynamic.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/driver/driver_zabbix_snapshot_dynamic.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/driver/driver_zabbix_snapshot_dynamic.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_aodh_snapshot_dynamic.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_aodh_snapshot_dynamic.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_aodh_update_dynamic.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_aodh_update_dynamic.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_kapacitor_update_dynamic.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_kapacitor_update_dynamic.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/transformer/transformer_prometheus_update_dynamic.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/transformer/transformer_prometheus_update_dynamic.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/cinder.volume.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/cinder.volume.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/neutron.network.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/neutron.network.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/neutron.port.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/neutron.port.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/nova.instance.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/nova.instance.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/nova.zone.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/nova.zone.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/tripleo.controller.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/tripleo.controller.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/vitrage.alarm.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/vitrage.alarm.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/mock_configurations/vertices/zabbix.json` & `vitrage-9.0.0/vitrage/tests/resources/mock_configurations/vertices/zabbix.json`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/nagios/nagios-mock.html` & `vitrage-9.0.0/vitrage/tests/resources/nagios/nagios-mock.html`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/snmp_notifier/oid_tree_with_severity_mapping.yaml` & `vitrage-9.0.0/vitrage/tests/resources/snmp_notifier/oid_tree_with_severity_mapping.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/added_resources/static.yaml` & `vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/added_resources/static.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/baseline/static.yaml` & `vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/baseline/static.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/changed_resources/static.yaml` & `vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/changed_resources/static.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/mixed_changes/static.yaml` & `vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/mixed_changes/static.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/static_datasources/changes_datasources/switch_to_host_datasource.yaml` & `vitrage-9.0.0/vitrage/tests/resources/static_datasources/changes_datasources/switch_to_host_datasource.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/static_datasources/switch_to_host.yaml` & `vitrage-9.0.0/vitrage/tests/resources/static_datasources/switch_to_host.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/static_datasources/switch_to_host_datasource.yaml` & `vitrage-9.0.0/vitrage/tests/resources/static_datasources/switch_to_host_datasource.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/consistency/deduced_alarm_on_instance.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/consistency/deduced_alarm_on_instance.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/definition_templates/large_def_template.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/definition_templates/large_def_template.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/definition_templates/with_include.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/definition_templates/with_include.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/definition_templates/with_scenarios.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/definition_templates/with_scenarios.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/templates/basic_with_include.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/templates/basic_with_include.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/templates/basic_with_include_that_doesnt_exist.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/templates/basic_with_include_that_doesnt_exist.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/templates/basic_with_two_includes.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/templates/basic_with_two_includes.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/templates/include_with_empty_name.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/templates/include_with_empty_name.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/def_template_tests/templates/only_using_def_template_definitions.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/def_template_tests/templates/only_using_def_template_definitions.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/equivalent_scenarios/basic.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/equivalent_scenarios/basic.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/causal_basic.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/causal_basic.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/complex_and_or_operator_deduced_alarm.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/complex_and_or_operator_deduced_alarm.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/complex_not_operator_deduced_alarm.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/complex_not_operator_deduced_alarm.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/complex1.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/complex1.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/complex2.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/complex2.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/complex_not.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/complex_not.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/complex_not_unsupported.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/complex_not_unsupported.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/not_edge_unsupported.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/not_edge_unsupported.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/not_or_unsupported.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/not_or_unsupported.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/not_or_unsupported2.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/not_or_unsupported2.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/one_edge.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/one_edge.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/simple_and.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/simple_and.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/simple_and2.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/simple_and2.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/simple_or.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/simple_or.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/simple_or2.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/simple_or2.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/simple_or3.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/simple_or3.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/conditions/simple_or_unsupported.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/conditions/simple_or_unsupported.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/deduced_alarm.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/deduced_alarm.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/deduced_state.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/deduced_state.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/deduced_state_2.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/deduced_state_2.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/high_availability.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/high_availability.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/simple_not_operator_deduced_alarm.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/simple_not_operator_deduced_alarm.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/evaluator/simple_or_operator_deduced_alarm.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/evaluator/simple_or_operator_deduced_alarm.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/general/basic.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/general/basic.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/general/equivalences/basic.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/general/equivalences/basic.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/general/host_high_cpu_load_to_instance_cpu_suboptimal.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/general/host_high_cpu_load_to_instance_cpu_suboptimal.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/not_operator/basic_correct_not_condition.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/not_operator/basic_correct_not_condition.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/not_operator/basic_incorrect_not_condition.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/not_operator/basic_incorrect_not_condition.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/not_operator/complicated_correct_not_condition.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/not_operator/complicated_correct_not_condition.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/not_operator/complicated_incorrect_not_condition.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/not_operator/complicated_incorrect_not_condition.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/parameters/v2_with_extra_param_def.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/parameters/v2_with_extra_param_def.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/parameters/v2_with_missing_param_def.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/parameters/v2_with_missing_param_def.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/parameters/v2_with_params.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/parameters/v2_with_params.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/parameters/v2_without_params.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/parameters/v2_without_params.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/parameters/v3_with_extra_param_def.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/parameters/v3_with_extra_param_def.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/parameters/v3_with_params.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/parameters/v3_with_params.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/regex/basic_regex.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/regex/basic_regex.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/regex/basic_regex_for_fail.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/regex/basic_regex_for_fail.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/regex/faulty_regex.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/regex/faulty_regex.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/regex/regex_for_exact_match.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/regex/regex_for_exact_match.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/v3_templates/valid_actions.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/v3_templates/valid_actions.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/v3_templates/valid_conditions.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/v3_templates/valid_conditions.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/version/invalid_version.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/version/invalid_version.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/version/no_version.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/version/no_version.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/version/v1/v1_execute_mistral.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/version/v1/v1_execute_mistral.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/version/v1/version1.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/version/v1/version1.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/version/v2/v2_execute_mistral.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/version/v2/v2_execute_mistral.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/version/v2/v2_standard.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/version/v2/v2_standard.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/resources/templates/version/v2/v2_with_func.yaml` & `vitrage-9.0.0/vitrage/tests/resources/templates/version/v2/v2_with_func.yaml`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/cli/test_status.py` & `vitrage-9.0.0/vitrage/tests/unit/cli/test_status.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/common/test_utils.py` & `vitrage-9.0.0/vitrage/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/aodh/aodh_transformer_base_test.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/aodh/aodh_transformer_base_test.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/aodh/mock_driver.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/aodh/mock_driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/aodh/test_aodh_driver.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/aodh/test_aodh_driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/aodh/test_aodh_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/aodh/test_aodh_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/ceilometer/ceilometer_transformer_base_test.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/ceilometer/ceilometer_transformer_base_test.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/ceilometer/mock_driver.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/ceilometer/mock_driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/ceilometer/test_ceilometer_driver.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/ceilometer/test_ceilometer_driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/ceilometer/test_ceilometer_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/ceilometer/test_ceilometer_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/cetus/test_cetus_cluster_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/cetus/test_cetus_cluster_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/cetus/test_cetus_pod_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/cetus/test_cetus_pod_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/cinder/test_cinder_volume_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/cinder/test_cinder_volume_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/collectd/test_collectd_driver.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/collectd/test_collectd_driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/collectd/test_collectd_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/collectd/test_collectd_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/collectd/test_mapper.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/collectd/test_mapper.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/consistency/test_consistency_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/consistency/test_consistency_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/doctor/test_doctor_driver.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/doctor/test_doctor_driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/doctor/test_doctor_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/doctor/test_doctor_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/heat/test_heat_stack_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/heat/test_heat_stack_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/kapacitor/test_kapacitor_configuration.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/kapacitor/test_kapacitor_configuration.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/kapacitor/test_kapacitor_driver.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/kapacitor/test_kapacitor_driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/kapacitor/test_kapacitor_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/kapacitor/test_kapacitor_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/kubernetes/test_kubernetes_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/kubernetes/test_kubernetes_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/nagios/mock_driver.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/nagios/mock_driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/nagios/nagios_base_test.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/nagios/nagios_base_test.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/nagios/test_nagios_config.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/nagios/test_nagios_config.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/nagios/test_nagios_driver.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/nagios/test_nagios_driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/nagios/test_nagios_parser.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/nagios/test_nagios_parser.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/nagios/test_nagios_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/nagios/test_nagios_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/nova/base_nova_instance_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/nova/base_nova_instance_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/nova/test_instance_transformer_legacy_notifications.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/nova/test_instance_transformer_legacy_notifications.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/nova/test_instance_transformer_snapshot_events.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/nova/test_instance_transformer_snapshot_events.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/nova/test_instance_transformer_versioned_notifications.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/nova/test_instance_transformer_versioned_notifications.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/nova/test_nova_host_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/nova/test_nova_host_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/nova/test_nova_instance_driver.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/nova/test_nova_instance_driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/nova/test_nova_zone_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/nova/test_nova_zone_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/prometheus/test_prometheus_driver.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/prometheus/test_prometheus_driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/prometheus/test_prometheus_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/prometheus/test_prometheus_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/static/test_static_driver.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/static/test_static_driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/static/test_static_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/static/test_static_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/test_alarm_transformer_base.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/test_alarm_transformer_base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/test_datasource_update_method.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/test_datasource_update_method.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/test_transformer_base.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/test_transformer_base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/tmfapi639/test_tmfapi639_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/tmfapi639/test_tmfapi639_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/trove/test_trove_cluster_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/trove/test_trove_cluster_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/trove/test_trove_instance_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/trove/test_trove_instance_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/zabbix/mock_driver.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/zabbix/mock_driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/zabbix/test_zabbix_configuration.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/zabbix/test_zabbix_configuration.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/zabbix/test_zabbix_driver.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/zabbix/test_zabbix_driver.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/zabbix/test_zabbix_transformer.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/zabbix/test_zabbix_transformer.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/datasources/zabbix/zabbix_base_test.py` & `vitrage-9.0.0/vitrage/tests/unit/datasources/zabbix/zabbix_base_test.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/entity_graph/base.py` & `vitrage-9.0.0/vitrage/tests/unit/entity_graph/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/entity_graph/processor/base.py` & `vitrage-9.0.0/vitrage/tests/unit/entity_graph/processor/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/entity_graph/processor/test_entity_graph.py` & `vitrage-9.0.0/vitrage/tests/unit/entity_graph/processor/test_entity_graph.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/entity_graph/processor/test_processor.py` & `vitrage-9.0.0/vitrage/tests/unit/entity_graph/processor/test_processor.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/entity_graph/states/test_datasource_info_mapper.py` & `vitrage-9.0.0/vitrage/tests/unit/entity_graph/states/test_datasource_info_mapper.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/entity_graph/test_processor_service.py` & `vitrage-9.0.0/vitrage/tests/unit/entity_graph/test_processor_service.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/entity_graph/test_transformer_manager.py` & `vitrage-9.0.0/vitrage/tests/unit/entity_graph/test_transformer_manager.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/__init__.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/recipes/test_add_causal_relationship_recipe.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/recipes/test_add_causal_relationship_recipe.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/recipes/test_execute_mistral.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/recipes/test_execute_mistral.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/recipes/test_mark_down.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/recipes/test_mark_down.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/recipes/test_raise_alarm.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/recipes/test_raise_alarm.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/recipes/test_set_state_recipe.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/recipes/test_set_state_recipe.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_functions/test_template_functions.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_functions/test_template_functions.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_loading/test_template_loading_v3.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_loading/test_template_loading_v3.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_loading/v2/test_template_loader.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_loading/v2/test_template_loader.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/base.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/base_test_execute_mistral_validator.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/base_test_execute_mistral_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/test_template_content_validator.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/test_template_content_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/test_add_causal_relationship_validator.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/test_add_causal_relationship_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/test_execute_mistral_validator.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/test_execute_mistral_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/test_mark_down_validator.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/test_mark_down_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/test_metadata_validator.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/test_metadata_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/test_parameters_validator.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/test_parameters_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/test_raise_alarm_validator.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/test_raise_alarm_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v1/test_set_state_validator.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v1/test_set_state_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v2/test_execute_mistral_validator.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v2/test_execute_mistral_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v2/test_metadata_validator.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v2/test_metadata_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/content/v2/test_parameters_validator.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/content/v2/test_parameters_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/test_def_template_syntax_validator.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/test_def_template_syntax_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/test_template_syntax_validator.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/test_template_syntax_validator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/template_validation/test_template_validator_v3.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/template_validation/test_template_validator_v3.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/test_condition.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/test_condition.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/test_equivalence_loader.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/test_equivalence_loader.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/test_equivalence_repository.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/test_equivalence_repository.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/test_scenario_evaluator.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/test_scenario_evaluator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/test_scenario_repository.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/test_scenario_repository.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/evaluator/test_template_loader.py` & `vitrage-9.0.0/vitrage/tests/unit/evaluator/test_template_loader.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/graph/base.py` & `vitrage-9.0.0/vitrage/tests/unit/graph/base.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/graph/test_graph.py` & `vitrage-9.0.0/vitrage/tests/unit/graph/test_graph.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/graph/test_graph_algo.py` & `vitrage-9.0.0/vitrage/tests/unit/graph/test_graph_algo.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/hacking/test_hacking.py` & `vitrage-9.0.0/vitrage/tests/unit/hacking/test_hacking.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/machine_learning/jaccard_correlation/test_jaccard_correlation.py` & `vitrage-9.0.0/vitrage/tests/unit/machine_learning/jaccard_correlation/test_jaccard_correlation.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/notifier/snmp_notifier/common.py` & `vitrage-9.0.0/vitrage/tests/unit/notifier/snmp_notifier/common.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/notifier/snmp_notifier/test_snmp_notifier.py` & `vitrage-9.0.0/vitrage/tests/unit/notifier/snmp_notifier/test_snmp_notifier.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/notifier/snmp_notifier/test_snmp_sender_with_severity_map.py` & `vitrage-9.0.0/vitrage/tests/unit/notifier/snmp_notifier/test_snmp_sender_with_severity_map.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/notifier/snmp_notifier/test_snmp_sender_without_severity_map.py` & `vitrage-9.0.0/vitrage/tests/unit/notifier/snmp_notifier/test_snmp_sender_without_severity_map.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/notifier/test_notifier.py` & `vitrage-9.0.0/vitrage/tests/unit/notifier/test_notifier.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/snmp_parsing/test_snmp_parsing.py` & `vitrage-9.0.0/vitrage/tests/unit/snmp_parsing/test_snmp_parsing.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/tests/unit/storage/test_migrations.py` & `vitrage-9.0.0/vitrage/tests/unit/storage/test_migrations.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/utils/__init__.py` & `vitrage-9.0.0/vitrage/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/utils/datetime.py` & `vitrage-9.0.0/vitrage/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/utils/evaluator.py` & `vitrage-9.0.0/vitrage/utils/evaluator.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage/utils/file.py` & `vitrage-9.0.0/vitrage/utils/file.py`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage.egg-info/PKG-INFO` & `vitrage-9.0.0/vitrage.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitrage
-Version: 8.0.1
+Version: 9.0.0
 Summary: The OpenStack RCA Service
 Home-page: https://docs.openstack.org/vitrage/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =================
         OpenStack Vitrage
@@ -38,16 +38,14 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Monitoring
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Provides-Extra: openstack
 Provides-Extra: test
 Provides-Extra: zabbix
```

### Comparing `vitrage-8.0.1/vitrage.egg-info/SOURCES.txt` & `vitrage-9.0.0/vitrage.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -161,14 +161,15 @@
 releasenotes/notes/datasource-scaffold-2f5ee6f0d9f83099.yaml
 releasenotes/notes/definition_templates-6c2c10bb3e6912a1.yaml
 releasenotes/notes/deprecate-json-formatted-policy-file-6a1e9b690fdbc132.yaml
 releasenotes/notes/deprecate-keystone_client-region-option-b3f30100370a5471.yaml
 releasenotes/notes/deprecate-static-physical-datasource-ab0094620c05d0ea.yaml
 releasenotes/notes/doctor-datasource-59ee5b2afb677ab4.yaml
 releasenotes/notes/drop-py-2-7-6add89c8aeb58399.yaml
+releasenotes/notes/drop-python-3-6-and-3-7-ca06b475787d017d.yaml
 releasenotes/notes/entity-equivalence-44c0da4cf3b5bc7e.yaml
 releasenotes/notes/event_persistor-1b0b4563cc219915.yaml
 releasenotes/notes/graph-fast-failover-e2d0a62f18ab27f7.yaml
 releasenotes/notes/health-check-api-19f180a104c7fa29.yaml
 releasenotes/notes/improve_tempest_tests-3e77197dfae4ad62.yaml
 releasenotes/notes/introduce-template-version-55bca9fc4e7d138f.yaml
 releasenotes/notes/kapacitor_datasource-c0c9563bb52ff1f1.yaml
@@ -230,14 +231,15 @@
 releasenotes/source/stein.rst
 releasenotes/source/train.rst
 releasenotes/source/unreleased.rst
 releasenotes/source/ussuri.rst
 releasenotes/source/victoria.rst
 releasenotes/source/wallaby.rst
 releasenotes/source/xena.rst
+releasenotes/source/yoga.rst
 releasenotes/source/_static/.placeholder
 releasenotes/source/_templates/.placeholder
 tools/__init__.py
 tools/datasource-scaffold/README
 tools/datasource-scaffold/cookiecutter.json
 tools/datasource-scaffold/requirements.txt
 tools/datasource-scaffold/sample/__init__.py
```

### Comparing `vitrage-8.0.1/vitrage.egg-info/entry_points.txt` & `vitrage-9.0.0/vitrage.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `vitrage-8.0.1/vitrage.egg-info/requires.txt` & `vitrage-9.0.0/vitrage.egg-info/requires.txt`

 * *Files identical despite different names*

