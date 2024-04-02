# Comparing `tmp/idds-server-2.1.8.tar.gz` & `tmp/idds-server-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-server-2.1.8.tar", last modified: Wed Jan 31 16:35:23 2024, max compression
+gzip compressed data, was "idds-server-2.1.9.tar", last modified: Wed Jan 31 17:27:20 2024, max compression
```

## Comparing `idds-server-2.1.8.tar` & `idds-server-2.1.9.tar`

### file list

```diff
@@ -1,299 +1,299 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.123234 idds-server-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-31 16:35:12.000000 idds-server-2.1.8/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-01-31 16:35:23.123234 idds-server-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-31 16:35:12.000000 idds-server-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.075234 idds-server-2.1.8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1687 2024-01-31 16:35:12.000000 idds-server-2.1.8/bin/idds-daemon
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-31 16:35:22.000000 idds-server-2.1.8/bin/idds.wsgi
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-31 16:35:12.000000 idds-server-2.1.8/bin/idds.wsgi.template
--rwxr-xr-x   0 runner    (1001) docker     (127)      584 2024-01-31 16:35:12.000000 idds-server-2.1.8/bin/run-idds
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-31 16:35:12.000000 idds-server-2.1.8/bin/run-idds-fake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.075234 idds-server-2.1.8/config_default/
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-01-31 16:35:12.000000 idds-server-2.1.8/config_default/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-01-31 16:35:12.000000 idds-server-2.1.8/config_default/auth.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-31 16:35:12.000000 idds-server-2.1.8/config_default/gacl
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-01-31 16:35:12.000000 idds-server-2.1.8/config_default/httpd-idds-443-py39-cc7.conf
--rwxr-xr-x   0 runner    (1001) docker     (127)     3727 2024-01-31 16:35:12.000000 idds-server-2.1.8/config_default/idds.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3724 2024-01-31 16:35:12.000000 idds-server-2.1.8/config_default/idds.cfg.orig
--rwxr-xr-x   0 runner    (1001) docker     (127)      273 2024-01-31 16:35:12.000000 idds-server-2.1.8/config_default/logrotate_daemon
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-01-31 16:35:12.000000 idds-server-2.1.8/config_default/logrotate_idds
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-31 16:35:12.000000 idds-server-2.1.8/config_default/panda.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-31 16:35:12.000000 idds-server-2.1.8/config_default/rucio.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-01-31 16:35:12.000000 idds-server-2.1.8/config_default/supervisord_httpd.ini
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-01-31 16:35:12.000000 idds-server-2.1.8/config_default/supervisord_idds.ini
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-31 16:35:12.000000 idds-server-2.1.8/config_default/supervisord_iddsfake.ini
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-31 16:35:12.000000 idds-server-2.1.8/config_default/supervisord_logrotate.ini
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-01-31 16:35:12.000000 idds-server-2.1.8/config_default/supervisord_syslog-ng.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.071234 idds-server-2.1.8/etc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.075234 idds-server-2.1.8/etc/idds/
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/idds/alembic.ini.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.079234 idds-server-2.1.8/etc/idds/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/idds/auth/auth.cfg.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.067234 idds-server-2.1.8/etc/idds/condor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.079234 idds-server-2.1.8/etc/idds/condor/client/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/idds/condor/client/00personal_condor.config
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.079234 idds-server-2.1.8/etc/idds/condor/server/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/idds/condor/server/00personal_condor.config
--rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/idds/idds.cfg.client.template
--rwxr-xr-x   0 runner    (1001) docker     (127)     4069 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/idds/idds.cfg.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.079234 idds-server-2.1.8/etc/idds/rest/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/idds/rest/gacl.template
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-01-31 16:35:22.000000 idds-server-2.1.8/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/idds/rest/httpd-idds-443-py39-cc7.conf.template
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/idds/rest/ssl.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.079234 idds-server-2.1.8/etc/idds/supervisord.d/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/idds/supervisord.d/idds.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.079234 idds-server-2.1.8/etc/idds/website/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/idds/website/25-port443.conf
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/idds/website/25-port80.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.079234 idds-server-2.1.8/etc/sql/
--rw-r--r--   0 runner    (1001) docker     (127)    25596 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/sql/oracle_11.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/sql/oracle_11_test.sql
--rw-r--r--   0 runner    (1001) docker     (127)    22610 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/sql/oracle_19.sql
--rw-r--r--   0 runner    (1001) docker     (127)    19542 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/sql/oracle_update.sql
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/sql/postgres_partition.sql
--rw-r--r--   0 runner    (1001) docker     (127)    19376 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/sql/postgresql.sql
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/sql/postgresql_init.sql
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-31 16:35:12.000000 idds-server-2.1.8/etc/sql/postgresql_update.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.071234 idds-server-2.1.8/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.079234 idds-server-2.1.8/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.079234 idds-server-2.1.8/lib/idds/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.083234 idds-server-2.1.8/lib/idds/agents/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/archive/archiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/archive/run_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.083234 idds-server-2.1.8/lib/idds/agents/carrier/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/carrier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18470 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/carrier/finisher.py
--rw-r--r--   0 runner    (1001) docker     (127)    26043 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/carrier/poller.py
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/carrier/receiver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10975 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/carrier/submitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15702 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/carrier/trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)   111580 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/carrier/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.083234 idds-server-2.1.8/lib/idds/agents/clerk/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/clerk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72929 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/clerk/clerk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.083234 idds-server-2.1.8/lib/idds/agents/common/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15319 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/common/baseagent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.083234 idds-server-2.1.8/lib/idds/agents/common/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/common/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/common/cache/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.087234 idds-server-2.1.8/lib/idds/agents/common/eventbus/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/common/eventbus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/common/eventbus/baseeventbusbackend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/common/eventbus/baseeventbusbackendopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/common/eventbus/dbeventbusbackend.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/common/eventbus/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/common/eventbus/eventbus.py
--rw-r--r--   0 runner    (1001) docker     (127)    25237 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/common/eventbus/msgeventbusbackend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.087234 idds-server-2.1.8/lib/idds/agents/common/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/common/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/common/plugins/messaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/common/timerscheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/common/timertask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.087234 idds-server-2.1.8/lib/idds/agents/conductor/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/conductor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/conductor/conductor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/conductor/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.087234 idds-server-2.1.8/lib/idds/agents/coordinator/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/coordinator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/coordinator/coordinator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5863 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.087234 idds-server-2.1.8/lib/idds/agents/marshaller/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/marshaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/marshaller/marshaller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.087234 idds-server-2.1.8/lib/idds/agents/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41651 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/transformer/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.087234 idds-server-2.1.8/lib/idds/agents/transporter/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/transporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22626 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/agents/transporter/transporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.087234 idds-server-2.1.8/lib/idds/api/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/api/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/api/contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/api/processings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/api/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/api/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.091234 idds-server-2.1.8/lib/idds/core/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31707 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/core/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/core/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/core/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/core/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/core/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    20758 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/core/processings.py
--rw-r--r--   0 runner    (1001) docker     (127)    22323 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/core/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/core/throttlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    34741 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/core/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/core/workprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.095234 idds-server-2.1.8/lib/idds/orm/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.095234 idds-server-2.1.8/lib/idds/orm/base/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.095234 idds-server-2.1.8/lib/idds/orm/base/alembic/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/alembic/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.095234 idds-server-2.1.8/lib/idds/orm/base/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/alembic/versions/0204f391c32d_add_poll_period_in_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/alembic/versions/1bc6e82e8514_using_hash_on_contents_long_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/alembic/versions/354f8e5a5879_add_meta_info_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/alembic/versions/53d0af715dab_add_site_throttler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/alembic/versions/5e0aa2aa1fa3_add_fetch_status_in_contents_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/alembic/versions/6ca0e5e466eb_update_message_null_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/alembic/versions/b0ec813021d6_add_sub_map_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/alembic/versions/f79663a7e94e_add_external_content_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    54894 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13488 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16744 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    43595 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/contents.py
--rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    18268 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/processings.py
--rw-r--r--   0 runner    (1001) docker     (127)    50940 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/throttlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    21690 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/orm/workprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.099234 idds-server-2.1.8/lib/idds/rest/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.099234 idds-server-2.1.8/lib/idds/rest/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/rest/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/rest/v1/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/rest/v1/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/rest/v1/cacher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/rest/v1/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/rest/v1/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/rest/v1/hyperparameteropt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/rest/v1/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/rest/v1/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)    28102 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/rest/v1/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/rest/v1/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)    21409 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/rest/v1/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/rest/v1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.115234 idds-server-2.1.8/lib/idds/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/activelearning_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/auth_test_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/cacher_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/catalog_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12118 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    23008 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/core_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/core_tests_dep_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/core_tests_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/datacarousel_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/doma_build_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/doma_build_test_pandaclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/find_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/fix_content_dep_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/fix_trasnform_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/hyperparameteropt_bayesian_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/hyperparameteropt_client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/hyperparameteropt_docker_local_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/hyperparameteropt_docker_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/hyperparameteropt_nevergrad_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/jsonload_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/kill_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/logs_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/match_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/message_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/message_test1.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/migrating_requests_v1_to_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/os_boto3_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/panda_client_submit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/panda_client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/panda_iam_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/panda_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/performance_test_with_cx_oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/performance_test_with_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/relation_map_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/rest_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/retry_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/run_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/scaling_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/set_throttlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/split_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/subprocess_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_activelearning.py
--rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_atlaspandawork.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_big_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    34114 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_catalog_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_class_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_core_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_datacarousel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_domapanda.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_domapanda_big.py
--rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_domapanda_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_domapanda_build_pandaclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    13018 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_domapanda_es.py
--rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_domapanda_long_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_domapanda_lsst_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_domapanda_pandaclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    11619 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_domapanda_small_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_domapanda_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_get_dn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_get_request_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_get_request_info_panda.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_hyperparameteropt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_merge_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_migrate_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_request_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_running_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     9544 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_transform_collection_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_transform_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    28166 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_workflow_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    69660 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_workflow_condition_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/test_workflow_condition_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-01-31 16:35:12.000000 idds-server-2.1.8/lib/idds/tests/trigger_release.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 16:35:22.000000 idds-server-2.1.8/lib/idds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.119234 idds-server-2.1.8/lib/idds_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-01-31 16:35:23.000000 idds-server-2.1.8/lib/idds_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-01-31 16:35:23.000000 idds-server-2.1.8/lib/idds_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 16:35:23.000000 idds-server-2.1.8/lib/idds_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-31 16:35:23.000000 idds-server-2.1.8/lib/idds_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 16:35:23.000000 idds-server-2.1.8/lib/idds_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 16:35:23.123234 idds-server-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-01-31 16:35:12.000000 idds-server-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.071234 idds-server-2.1.8/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 16:35:23.119234 idds-server-2.1.8/tools/env/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/clean_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/config_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/config_server
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/create_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/create_postgres_db.sh
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/destroy_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/dump_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-01-31 16:35:22.000000 idds-server-2.1.8/tools/env/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/install_env_conda.sh
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/install_idds.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/install_idds_example.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/install_idds_full.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      152 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/install_packages.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/merge_configmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/merge_idds_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/setup_idds.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-01-31 16:35:12.000000 idds-server-2.1.8/tools/env/setup_panda.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.441875 idds-server-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-31 17:27:09.000000 idds-server-2.1.9/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-01-31 17:27:20.441875 idds-server-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-31 17:27:09.000000 idds-server-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.393875 idds-server-2.1.9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1687 2024-01-31 17:27:09.000000 idds-server-2.1.9/bin/idds-daemon
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-31 17:27:20.000000 idds-server-2.1.9/bin/idds.wsgi
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-31 17:27:09.000000 idds-server-2.1.9/bin/idds.wsgi.template
+-rwxr-xr-x   0 runner    (1001) docker     (127)      584 2024-01-31 17:27:09.000000 idds-server-2.1.9/bin/run-idds
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-31 17:27:09.000000 idds-server-2.1.9/bin/run-idds-fake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.397875 idds-server-2.1.9/config_default/
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-01-31 17:27:09.000000 idds-server-2.1.9/config_default/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-01-31 17:27:09.000000 idds-server-2.1.9/config_default/auth.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-31 17:27:09.000000 idds-server-2.1.9/config_default/gacl
+-rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-01-31 17:27:09.000000 idds-server-2.1.9/config_default/httpd-idds-443-py39-cc7.conf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3727 2024-01-31 17:27:09.000000 idds-server-2.1.9/config_default/idds.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3724 2024-01-31 17:27:09.000000 idds-server-2.1.9/config_default/idds.cfg.orig
+-rwxr-xr-x   0 runner    (1001) docker     (127)      273 2024-01-31 17:27:09.000000 idds-server-2.1.9/config_default/logrotate_daemon
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-01-31 17:27:09.000000 idds-server-2.1.9/config_default/logrotate_idds
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-31 17:27:09.000000 idds-server-2.1.9/config_default/panda.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-31 17:27:09.000000 idds-server-2.1.9/config_default/rucio.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-01-31 17:27:09.000000 idds-server-2.1.9/config_default/supervisord_httpd.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-01-31 17:27:09.000000 idds-server-2.1.9/config_default/supervisord_idds.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-31 17:27:09.000000 idds-server-2.1.9/config_default/supervisord_iddsfake.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-01-31 17:27:09.000000 idds-server-2.1.9/config_default/supervisord_logrotate.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-01-31 17:27:09.000000 idds-server-2.1.9/config_default/supervisord_syslog-ng.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.389875 idds-server-2.1.9/etc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.397875 idds-server-2.1.9/etc/idds/
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/idds/alembic.ini.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.397875 idds-server-2.1.9/etc/idds/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/idds/auth/auth.cfg.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.389875 idds-server-2.1.9/etc/idds/condor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.397875 idds-server-2.1.9/etc/idds/condor/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/idds/condor/client/00personal_condor.config
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.397875 idds-server-2.1.9/etc/idds/condor/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/idds/condor/server/00personal_condor.config
+-rwxr-xr-x   0 runner    (1001) docker     (127)      811 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/idds/idds.cfg.client.template
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4069 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/idds/idds.cfg.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.401875 idds-server-2.1.9/etc/idds/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/idds/rest/gacl.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-01-31 17:27:20.000000 idds-server-2.1.9/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/idds/rest/httpd-idds-443-py39-cc7.conf.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/idds/rest/ssl.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.401875 idds-server-2.1.9/etc/idds/supervisord.d/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/idds/supervisord.d/idds.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.401875 idds-server-2.1.9/etc/idds/website/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/idds/website/25-port443.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/idds/website/25-port80.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.401875 idds-server-2.1.9/etc/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)    25596 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/sql/oracle_11.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/sql/oracle_11_test.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    22610 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/sql/oracle_19.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    19542 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/sql/oracle_update.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/sql/postgres_partition.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    19376 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/sql/postgresql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/sql/postgresql_init.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-01-31 17:27:09.000000 idds-server-2.1.9/etc/sql/postgresql_update.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.393875 idds-server-2.1.9/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.401875 idds-server-2.1.9/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.401875 idds-server-2.1.9/lib/idds/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.401875 idds-server-2.1.9/lib/idds/agents/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/archive/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/archive/run_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.405875 idds-server-2.1.9/lib/idds/agents/carrier/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/carrier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18470 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/carrier/finisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26043 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/carrier/poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/carrier/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10975 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/carrier/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15702 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/carrier/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111580 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/carrier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.405875 idds-server-2.1.9/lib/idds/agents/clerk/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/clerk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72929 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/clerk/clerk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.405875 idds-server-2.1.9/lib/idds/agents/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15319 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/common/baseagent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.405875 idds-server-2.1.9/lib/idds/agents/common/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/common/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/common/cache/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.409875 idds-server-2.1.9/lib/idds/agents/common/eventbus/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/common/eventbus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/common/eventbus/baseeventbusbackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/common/eventbus/baseeventbusbackendopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/common/eventbus/dbeventbusbackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/common/eventbus/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/common/eventbus/eventbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25237 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/common/eventbus/msgeventbusbackend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.409875 idds-server-2.1.9/lib/idds/agents/common/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/common/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/common/plugins/messaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/common/timerscheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/common/timertask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.409875 idds-server-2.1.9/lib/idds/agents/conductor/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/conductor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/conductor/conductor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/conductor/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.409875 idds-server-2.1.9/lib/idds/agents/coordinator/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/coordinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/coordinator/coordinator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5863 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.409875 idds-server-2.1.9/lib/idds/agents/marshaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/marshaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13740 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/marshaller/marshaller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.409875 idds-server-2.1.9/lib/idds/agents/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41651 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/transformer/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.409875 idds-server-2.1.9/lib/idds/agents/transporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/transporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22626 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/agents/transporter/transporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.413875 idds-server-2.1.9/lib/idds/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/api/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/api/contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/api/processings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/api/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/api/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.413875 idds-server-2.1.9/lib/idds/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31707 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/core/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/core/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/core/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/core/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20758 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/core/processings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22323 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/core/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/core/throttlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34741 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/core/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/core/workprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.417875 idds-server-2.1.9/lib/idds/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.417875 idds-server-2.1.9/lib/idds/orm/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.421875 idds-server-2.1.9/lib/idds/orm/base/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/alembic/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.421875 idds-server-2.1.9/lib/idds/orm/base/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/alembic/versions/0204f391c32d_add_poll_period_in_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/alembic/versions/1bc6e82e8514_using_hash_on_contents_long_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/alembic/versions/354f8e5a5879_add_meta_info_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/alembic/versions/53d0af715dab_add_site_throttler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/alembic/versions/5e0aa2aa1fa3_add_fetch_status_in_contents_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/alembic/versions/6ca0e5e466eb_update_message_null_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/alembic/versions/b0ec813021d6_add_sub_map_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/alembic/versions/f79663a7e94e_add_external_content_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54894 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13488 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5887 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16744 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43595 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11839 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18268 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/processings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50940 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/throttlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21690 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/orm/workprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.421875 idds-server-2.1.9/lib/idds/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.425875 idds-server-2.1.9/lib/idds/rest/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/rest/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/rest/v1/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/rest/v1/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/rest/v1/cacher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/rest/v1/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/rest/v1/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/rest/v1/hyperparameteropt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/rest/v1/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/rest/v1/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28102 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/rest/v1/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/rest/v1/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21409 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/rest/v1/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/rest/v1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.437875 idds-server-2.1.9/lib/idds/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/activelearning_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/auth_test_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/cacher_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/catalog_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12118 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23008 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/core_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/core_tests_dep_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/core_tests_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/datacarousel_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/doma_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/doma_build_test_pandaclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/find_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/fix_content_dep_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/fix_trasnform_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/hyperparameteropt_bayesian_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/hyperparameteropt_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/hyperparameteropt_docker_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/hyperparameteropt_docker_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/hyperparameteropt_nevergrad_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/jsonload_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/kill_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/logs_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/match_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/message_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/message_test1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/migrating_requests_v1_to_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/os_boto3_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/panda_client_submit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/panda_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/panda_iam_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/panda_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/performance_test_with_cx_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/performance_test_with_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/relation_map_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/rest_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/retry_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/run_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/scaling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/set_throttlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/split_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/subprocess_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_activelearning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_atlaspandawork.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_big_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34114 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_catalog_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_class_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_core_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_datacarousel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_domapanda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_domapanda_big.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_domapanda_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_domapanda_build_pandaclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13018 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_domapanda_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_domapanda_long_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11404 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_domapanda_lsst_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_domapanda_pandaclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11619 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_domapanda_small_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_domapanda_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_get_dn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_get_request_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_get_request_info_panda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_hyperparameteropt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_merge_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_migrate_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_request_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_running_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9544 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_transform_collection_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_transform_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28166 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_workflow_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69660 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_workflow_condition_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/test_workflow_condition_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-01-31 17:27:09.000000 idds-server-2.1.9/lib/idds/tests/trigger_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-31 17:27:19.000000 idds-server-2.1.9/lib/idds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.441875 idds-server-2.1.9/lib/idds_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-01-31 17:27:20.000000 idds-server-2.1.9/lib/idds_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-01-31 17:27:20.000000 idds-server-2.1.9/lib/idds_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 17:27:20.000000 idds-server-2.1.9/lib/idds_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-31 17:27:20.000000 idds-server-2.1.9/lib/idds_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-31 17:27:20.000000 idds-server-2.1.9/lib/idds_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-31 17:27:20.441875 idds-server-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-01-31 17:27:09.000000 idds-server-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.393875 idds-server-2.1.9/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 17:27:20.441875 idds-server-2.1.9/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/clean_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/config_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/config_server
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/create_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/create_postgres_db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/destroy_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/dump_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-01-31 17:27:19.000000 idds-server-2.1.9/tools/env/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/install_env_conda.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/install_idds.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/install_idds_example.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/install_idds_full.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      152 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/install_packages.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/merge_configmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/merge_idds_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/setup_idds.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-01-31 17:27:09.000000 idds-server-2.1.9/tools/env/setup_panda.sh
```

### Comparing `idds-server-2.1.8/LICENSE.rst` & `idds-server-2.1.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/PKG-INFO` & `idds-server-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-server
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-server-2.1.8/bin/idds-daemon` & `idds-server-2.1.9/bin/idds-daemon`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/bin/idds.wsgi` & `idds-server-2.1.9/bin/idds.wsgi`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/bin/idds.wsgi.template` & `idds-server-2.1.9/bin/idds.wsgi.template`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/bin/run-idds` & `idds-server-2.1.9/bin/run-idds`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/config_default/alembic.ini` & `idds-server-2.1.9/config_default/alembic.ini`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/config_default/gacl` & `idds-server-2.1.9/config_default/gacl`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/config_default/httpd-idds-443-py39-cc7.conf` & `idds-server-2.1.9/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template`

 * *Files 19% similar despite different names*

```diff
@@ -4,64 +4,63 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Authors:
 # - Wen Guan, <wen.guan@cern.ch>, 2019
 
 TimeOut 600
 KeepAliveTimeout 600
+SSLSessionCacheTimeout 600
 
 # Built-in modules
 LoadModule ssl_module /usr/lib64/httpd/modules/mod_ssl.so
 
 # # LoadModule log_config_module    /usr/lib64/httpd/modules/mod_log_config.so
 # # LoadModule ssl_module           /usr/lib64/httpd/modules/mod_ssl.so
 # # LoadModule gridsite_module      /usr/lib64/httpd/modules/mod_gridsite.so
 # # LoadModule mime_module          /usr/lib64/httpd/modules/mod_mime.so
 # # LoadModule dir_module           /usr/lib64/httpd/modules/mod_dir.so
 # # LoadModule alias_module         /usr/lib64/httpd/modules/mod_alias.so
 # # LoadModule cgi_module           /usr/lib64/httpd/modules/mod_cgi.so
 
 # External modules
 LoadModule gridsite_module /usr/lib64/httpd/modules/mod_gridsite.so
-# #LoadModule wsgi_module /usr/lib64/httpd/modules/mod_wsgi.so
-LoadModule wsgi_module /opt/idds/lib/python3.9/site-packages/mod_wsgi/server/mod_wsgi-py39.cpython-39-x86_64-linux-gnu.so
+#LoadModule wsgi_module /usr/lib64/httpd/modules/mod_wsgi.so
+LoadModule wsgi_module {python_site_packages_path}/mod_wsgi/server/mod_wsgi-py36.cpython-36m-x86_64-linux-gnu.so
 
-WSGIPythonHome /opt/idds
-WSGIPythonPath /opt/idds/lib/python3.9/site-packages
+WSGIPythonHome {python_site_home_path}
+WSGIPythonPath {python_site_packages_path}
 
 <IfModule mod_wsgi.c>
-    WSGIDaemonProcess idds_daemon processes=25 threads=2 request-timeout=600 queue-timeout=600 python-home=/opt/idds python-path=/opt/idds/lib/python3.9/site-packages python-path=/opt/idds python-path=/opt/idds/lib/python3.9/site-packages
+    WSGIDaemonProcess idds_daemon processes=25 threads=2 request-timeout=600 queue-timeout=600 python-home={python_site_home_path} python-path={python_site_packages_path}
     WSGIProcessGroup idds_daemon
-    WSGIApplicationGroup %GLOBAL
-    WSGIScriptAlias /idds /opt/idds/bin/idds.wsgi
+    WSGIApplicationGroup %{GLOBAL}
+    WSGIScriptAlias /idds {python_site_bin_path}/idds.wsgi
     # WSGIScriptAliasMatch ^/idds/(.+)$ /opt/idds/etc/idds/rest/test.wsgi
-    WSGISocketPrefix /var/idds/wsgisocks/wsgi
+    WSGISocketPrefix /var/log/idds/wsgisocks/wsgi
     WSGIPassAuthorization On
 </IfModule>
 
-Listen 8443
-Listen 8080
+Listen 443
 
 RewriteEngine on
-RewriteCond %REQUEST_METHOD ^(TRACE|TRACK)
+RewriteCond %{REQUEST_METHOD} ^(TRACE|TRACK)
 RewriteRule .* - [F]
 RedirectMatch 403 /\..*$
 TraceEnable off
 
 Alias "/website"     "/opt/idds/website/data"
 Alias "/monitor"     "/opt/idds/monitor/data"
 
-<VirtualHost *:8443>
-    # ServerName aipanda182.cern.ch:8443
+<VirtualHost *:443>
+    # ServerName aipanda182.cern.ch:443
     ServerAdmin wguan@cern.ch
 
     SSLEngine on
     SSLCertificateFile /etc/grid-security/hostcert.pem
     SSLCertificateKeyFile /etc/grid-security/hostkey.pem
-    SSLCertificateChainFile /etc/grid-security/chain.pem
     SSLCACertificatePath /etc/grid-security/certificates
     SSLCARevocationPath /etc/grid-security/certificates
     SSLVerifyClient optional
     SSLVerifyDepth 16
     SSLOptions +StdEnvVars +ExportCertData
 
     # CERN security recommendation to only allow the seven strongest ssl ciphers
@@ -81,84 +80,29 @@
         GridSiteGSIProxyLimit 16
         GridSiteEnvs on
         GridSiteACLPath /opt/idds/etc/idds/rest/gacl
     </LocationMatch>
 
     <LocationMatch "^/idds">
         GridSiteIndexes on
-        # GridSiteAuth on
+        GridSiteAuth on
         GridSiteDNlists /etc/grid-security/dn-lists/
         GridSiteGSIProxyLimit 16
         GridSiteEnvs on
         GridSiteACLPath /opt/idds/etc/idds/rest/gacl
         # GridSiteMethods GET
     </LocationMatch>
 
-    <Directory /opt/idds/lib/python3.9/site-packages>
-        # Order deny,allow
-        # Allow from all
-        # Require all granted
-    </Directory>
-
-    <Directory /opt/idds/bin>
+    <Directory {python_site_packages_path}>
         Order deny,allow
         Allow from all
         Require all granted
     </Directory>
 
-    <Directory /opt/idds/website/data>
-        Order deny,allow
-        Allow from all
-        Require all granted
-    </Directory>
-
-    <Directory /opt/idds/monitor/data>
-        Order deny,allow
-        Allow from all
-        Require all granted
-        DirectoryIndex dashboard.html
-        DirectoryIndex index.html
-    </Directory>
-</VirtualHost>
-
-<VirtualHost *:8080>
-    # ServerName aipanda182.cern.ch:8080
-    ServerAdmin wguan@cern.ch
-
-    LogLevel debug
-    ErrorLog /var/log/idds/httpd_error_log
-    TransferLog /var/log/idds/httpd_access_log
-
-    # Proxy authentication via mod_gridsite
-    <LocationMatch /auth/x509_proxy>
-        GridSiteIndexes on
-        GridSiteAuth on
-        GridSiteDNlists /etc/grid-security/dn-lists/
-        GridSiteGSIProxyLimit 16
-        GridSiteEnvs on
-        GridSiteACLPath /opt/idds/etc/idds/rest/gacl
-    </LocationMatch>
-
-    <LocationMatch "^/idds">
-        GridSiteIndexes on
-        # GridSiteAuth on
-        GridSiteDNlists /etc/grid-security/dn-lists/
-        GridSiteGSIProxyLimit 16
-        GridSiteEnvs on
-        GridSiteACLPath /opt/idds/etc/idds/rest/gacl
-        # GridSiteMethods GET
-    </LocationMatch>
-
-    <Directory /opt/idds/lib/python3.9/site-packages>
-        # Order deny,allow
-        # Allow from all
-        # Require all granted
-    </Directory>
-
-    <Directory /opt/idds/bin>
+    <Directory {python_site_bin_path}>
         Order deny,allow
         Allow from all
         Require all granted
     </Directory>
 
     <Directory /opt/idds/website/data>
         Order deny,allow
```

### Comparing `idds-server-2.1.8/config_default/idds.cfg` & `idds-server-2.1.9/config_default/idds.cfg`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/config_default/idds.cfg.orig` & `idds-server-2.1.9/config_default/idds.cfg.orig`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/config_default/rucio.cfg` & `idds-server-2.1.9/config_default/rucio.cfg`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/config_default/supervisord_httpd.ini` & `idds-server-2.1.9/config_default/supervisord_httpd.ini`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/config_default/supervisord_idds.ini` & `idds-server-2.1.9/config_default/supervisord_idds.ini`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/config_default/supervisord_iddsfake.ini` & `idds-server-2.1.9/config_default/supervisord_iddsfake.ini`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/config_default/supervisord_logrotate.ini` & `idds-server-2.1.9/config_default/supervisord_logrotate.ini`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/config_default/supervisord_syslog-ng.ini` & `idds-server-2.1.9/config_default/supervisord_syslog-ng.ini`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/idds/alembic.ini.template` & `idds-server-2.1.9/etc/idds/alembic.ini.template`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/idds/auth/auth.cfg.template` & `idds-server-2.1.9/etc/idds/auth/auth.cfg.template`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/idds/condor/client/00personal_condor.config` & `idds-server-2.1.9/etc/idds/condor/client/00personal_condor.config`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/idds/condor/server/00personal_condor.config` & `idds-server-2.1.9/etc/idds/condor/server/00personal_condor.config`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/idds/idds.cfg.client.template` & `idds-server-2.1.9/etc/idds/idds.cfg.client.template`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/idds/idds.cfg.template` & `idds-server-2.1.9/etc/idds/idds.cfg.template`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/idds/rest/gacl.template` & `idds-server-2.1.9/etc/idds/rest/gacl.template`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template` & `idds-server-2.1.9/etc/idds/rest/httpd-idds-443-py39-cc7.conf.template`

 * *Files 22% similar despite different names*

```diff
@@ -20,30 +20,32 @@
 # # LoadModule dir_module           /usr/lib64/httpd/modules/mod_dir.so
 # # LoadModule alias_module         /usr/lib64/httpd/modules/mod_alias.so
 # # LoadModule cgi_module           /usr/lib64/httpd/modules/mod_cgi.so
 
 # External modules
 LoadModule gridsite_module /usr/lib64/httpd/modules/mod_gridsite.so
 #LoadModule wsgi_module /usr/lib64/httpd/modules/mod_wsgi.so
-LoadModule wsgi_module {python_site_packages_path}/mod_wsgi/server/mod_wsgi-py36.cpython-36m-x86_64-linux-gnu.so
+LoadModule wsgi_module {python_site_packages_path}/mod_wsgi/server/mod_wsgi-py39.cpython-39-x86_64-linux-gnu.so
 
 WSGIPythonHome {python_site_home_path}
 WSGIPythonPath {python_site_packages_path}
 
 <IfModule mod_wsgi.c>
     WSGIDaemonProcess idds_daemon processes=25 threads=2 request-timeout=600 queue-timeout=600 python-home={python_site_home_path} python-path={python_site_packages_path}
     WSGIProcessGroup idds_daemon
     WSGIApplicationGroup %{GLOBAL}
     WSGIScriptAlias /idds {python_site_bin_path}/idds.wsgi
     # WSGIScriptAliasMatch ^/idds/(.+)$ /opt/idds/etc/idds/rest/test.wsgi
     WSGISocketPrefix /var/log/idds/wsgisocks/wsgi
+    # WSGISocketPrefix /tmp/idds/wsgisocks/wsgi
     WSGIPassAuthorization On
 </IfModule>
 
 Listen 443
+Listen 8443
 
 RewriteEngine on
 RewriteCond %{REQUEST_METHOD} ^(TRACE|TRACK)
 RewriteRule .* - [F]
 RedirectMatch 403 /\..*$
 TraceEnable off
 
@@ -68,14 +70,25 @@
     SSLCipherSuite HIGH:!CAMELLIA:!ADH:!aNULL:!eNULL:!EXPORT:!DES:!RC4:!MD5:!PSK:!3DES
     SSLHonorCipherOrder on
 
     LogLevel debug
     ErrorLog /var/log/idds/httpd_error_log
     TransferLog /var/log/idds/httpd_access_log
 
+    <IfModule mod_wsgi.c>
+        WSGIDaemonProcess idds_daemon processes=25 threads=2 request-timeout=600 queue-timeout=600 python-home={python_site_home_path} python-path={python_site_packages_path}
+        WSGIProcessGroup idds_daemon
+        WSGIApplicationGroup %{GLOBAL}
+        WSGIScriptAlias /idds {python_site_bin_path}/idds.wsgi
+        # WSGIScriptAliasMatch ^/idds/(.+)$ /opt/idds/etc/idds/rest/test.wsgi
+        # WSGISocketPrefix /var/log/idds/wsgisocks/wsgi
+        WSGISocketPrefix /tmp/idds/wsgisocks/wsgi
+        WSGIPassAuthorization On
+    </IfModule>
+
     # Proxy authentication via mod_gridsite
     <LocationMatch /auth/x509_proxy>
         GridSiteIndexes on
         GridSiteAuth on
         GridSiteDNlists /etc/grid-security/dn-lists/
         GridSiteGSIProxyLimit 16
         GridSiteEnvs on
@@ -89,17 +102,17 @@
         GridSiteGSIProxyLimit 16
         GridSiteEnvs on
         GridSiteACLPath /opt/idds/etc/idds/rest/gacl
         # GridSiteMethods GET
     </LocationMatch>
 
     <Directory {python_site_packages_path}>
-        Order deny,allow
-        Allow from all
-        Require all granted
+        # Order deny,allow
+        # Allow from all
+        # Require all granted
     </Directory>
 
     <Directory {python_site_bin_path}>
         Order deny,allow
         Allow from all
         Require all granted
     </Directory>
```

### Comparing `idds-server-2.1.8/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template` & `idds-server-2.1.9/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template` & `idds-server-2.1.9/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/idds/rest/ssl.conf` & `idds-server-2.1.9/etc/idds/rest/ssl.conf`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/idds/supervisord.d/idds.ini` & `idds-server-2.1.9/etc/idds/supervisord.d/idds.ini`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/idds/website/25-port443.conf` & `idds-server-2.1.9/etc/idds/website/25-port443.conf`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/sql/oracle_11.sql` & `idds-server-2.1.9/etc/sql/oracle_11.sql`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/sql/oracle_11_test.sql` & `idds-server-2.1.9/etc/sql/oracle_11_test.sql`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/sql/oracle_19.sql` & `idds-server-2.1.9/etc/sql/oracle_19.sql`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/sql/oracle_update.sql` & `idds-server-2.1.9/etc/sql/oracle_update.sql`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/sql/postgresql.sql` & `idds-server-2.1.9/etc/sql/postgresql.sql`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/sql/postgresql_init.sql` & `idds-server-2.1.9/etc/sql/postgresql_init.sql`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/etc/sql/postgresql_update.sql` & `idds-server-2.1.9/etc/sql/postgresql_update.sql`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/archive/archiver.py` & `idds-server-2.1.9/lib/idds/agents/archive/archiver.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/archive/run_archive.py` & `idds-server-2.1.9/lib/idds/agents/archive/run_archive.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/carrier/finisher.py` & `idds-server-2.1.9/lib/idds/agents/carrier/finisher.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/carrier/poller.py` & `idds-server-2.1.9/lib/idds/agents/carrier/poller.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/carrier/receiver.py` & `idds-server-2.1.9/lib/idds/agents/carrier/receiver.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/carrier/submitter.py` & `idds-server-2.1.9/lib/idds/agents/carrier/submitter.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/carrier/trigger.py` & `idds-server-2.1.9/lib/idds/agents/carrier/trigger.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/carrier/utils.py` & `idds-server-2.1.9/lib/idds/agents/carrier/utils.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/clerk/clerk.py` & `idds-server-2.1.9/lib/idds/agents/clerk/clerk.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/common/baseagent.py` & `idds-server-2.1.9/lib/idds/agents/common/baseagent.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/common/cache/redis.py` & `idds-server-2.1.9/lib/idds/agents/common/cache/redis.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/common/eventbus/baseeventbusbackend.py` & `idds-server-2.1.9/lib/idds/agents/common/eventbus/baseeventbusbackend.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/common/eventbus/baseeventbusbackendopt.py` & `idds-server-2.1.9/lib/idds/agents/common/eventbus/baseeventbusbackendopt.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/common/eventbus/dbeventbusbackend.py` & `idds-server-2.1.9/lib/idds/agents/common/eventbus/dbeventbusbackend.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/common/eventbus/eventbus.py` & `idds-server-2.1.9/lib/idds/agents/common/eventbus/eventbus.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/common/eventbus/msgeventbusbackend.py` & `idds-server-2.1.9/lib/idds/agents/common/eventbus/msgeventbusbackend.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/common/plugins/messaging.py` & `idds-server-2.1.9/lib/idds/agents/common/plugins/messaging.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/common/timerscheduler.py` & `idds-server-2.1.9/lib/idds/agents/common/timerscheduler.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/common/timertask.py` & `idds-server-2.1.9/lib/idds/agents/common/timertask.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/conductor/conductor.py` & `idds-server-2.1.9/lib/idds/agents/conductor/conductor.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/conductor/consumer.py` & `idds-server-2.1.9/lib/idds/agents/conductor/consumer.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/coordinator/coordinator.py` & `idds-server-2.1.9/lib/idds/agents/coordinator/coordinator.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/main.py` & `idds-server-2.1.9/lib/idds/agents/main.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/marshaller/marshaller.py` & `idds-server-2.1.9/lib/idds/agents/marshaller/marshaller.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/transformer/transformer.py` & `idds-server-2.1.9/lib/idds/agents/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/agents/transporter/transporter.py` & `idds-server-2.1.9/lib/idds/agents/transporter/transporter.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/api/catalog.py` & `idds-server-2.1.9/lib/idds/api/catalog.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/api/collections.py` & `idds-server-2.1.9/lib/idds/api/collections.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/api/contents.py` & `idds-server-2.1.9/lib/idds/api/contents.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/api/processings.py` & `idds-server-2.1.9/lib/idds/api/processings.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/api/requests.py` & `idds-server-2.1.9/lib/idds/api/requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/api/transforms.py` & `idds-server-2.1.9/lib/idds/api/transforms.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/core/catalog.py` & `idds-server-2.1.9/lib/idds/core/catalog.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/core/commands.py` & `idds-server-2.1.9/lib/idds/core/commands.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/core/events.py` & `idds-server-2.1.9/lib/idds/core/events.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/core/health.py` & `idds-server-2.1.9/lib/idds/core/health.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/core/messages.py` & `idds-server-2.1.9/lib/idds/core/messages.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/core/meta.py` & `idds-server-2.1.9/lib/idds/core/meta.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/core/processings.py` & `idds-server-2.1.9/lib/idds/core/processings.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/core/requests.py` & `idds-server-2.1.9/lib/idds/core/requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/core/throttlers.py` & `idds-server-2.1.9/lib/idds/core/throttlers.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/core/transforms.py` & `idds-server-2.1.9/lib/idds/core/transforms.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/core/workprogress.py` & `idds-server-2.1.9/lib/idds/core/workprogress.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/base/alembic/env.py` & `idds-server-2.1.9/lib/idds/orm/base/alembic/env.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/base/alembic/versions/0204f391c32d_add_poll_period_in_message.py` & `idds-server-2.1.9/lib/idds/orm/base/alembic/versions/0204f391c32d_add_poll_period_in_message.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/base/alembic/versions/1bc6e82e8514_using_hash_on_contents_long_name.py` & `idds-server-2.1.9/lib/idds/orm/base/alembic/versions/1bc6e82e8514_using_hash_on_contents_long_name.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/base/alembic/versions/354f8e5a5879_add_meta_info_table.py` & `idds-server-2.1.9/lib/idds/orm/base/alembic/versions/354f8e5a5879_add_meta_info_table.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/base/alembic/versions/53d0af715dab_add_site_throttler.py` & `idds-server-2.1.9/lib/idds/orm/base/alembic/versions/53d0af715dab_add_site_throttler.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/base/alembic/versions/5e0aa2aa1fa3_add_fetch_status_in_contents_update.py` & `idds-server-2.1.9/lib/idds/orm/base/alembic/versions/5e0aa2aa1fa3_add_fetch_status_in_contents_update.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/base/alembic/versions/6ca0e5e466eb_update_message_null_constraints.py` & `idds-server-2.1.9/lib/idds/orm/base/alembic/versions/6ca0e5e466eb_update_message_null_constraints.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/base/alembic/versions/b0ec813021d6_add_sub_map_id.py` & `idds-server-2.1.9/lib/idds/orm/base/alembic/versions/b0ec813021d6_add_sub_map_id.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/base/alembic/versions/f79663a7e94e_add_external_content_id.py` & `idds-server-2.1.9/lib/idds/orm/base/alembic/versions/f79663a7e94e_add_external_content_id.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/base/enum.py` & `idds-server-2.1.9/lib/idds/orm/base/enum.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/base/models.py` & `idds-server-2.1.9/lib/idds/orm/base/models.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/base/session.py` & `idds-server-2.1.9/lib/idds/orm/base/session.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/base/types.py` & `idds-server-2.1.9/lib/idds/orm/base/types.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/base/utils.py` & `idds-server-2.1.9/lib/idds/orm/base/utils.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/collections.py` & `idds-server-2.1.9/lib/idds/orm/collections.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/commands.py` & `idds-server-2.1.9/lib/idds/orm/commands.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/contents.py` & `idds-server-2.1.9/lib/idds/orm/contents.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/events.py` & `idds-server-2.1.9/lib/idds/orm/events.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/health.py` & `idds-server-2.1.9/lib/idds/orm/health.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/messages.py` & `idds-server-2.1.9/lib/idds/orm/messages.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/meta.py` & `idds-server-2.1.9/lib/idds/orm/meta.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/processings.py` & `idds-server-2.1.9/lib/idds/orm/processings.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/requests.py` & `idds-server-2.1.9/lib/idds/orm/requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/throttlers.py` & `idds-server-2.1.9/lib/idds/orm/throttlers.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/transforms.py` & `idds-server-2.1.9/lib/idds/orm/transforms.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/orm/workprogress.py` & `idds-server-2.1.9/lib/idds/orm/workprogress.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/rest/v1/app.py` & `idds-server-2.1.9/lib/idds/rest/v1/app.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/rest/v1/auth.py` & `idds-server-2.1.9/lib/idds/rest/v1/auth.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/rest/v1/cacher.py` & `idds-server-2.1.9/lib/idds/rest/v1/cacher.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/rest/v1/catalog.py` & `idds-server-2.1.9/lib/idds/rest/v1/catalog.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/rest/v1/controller.py` & `idds-server-2.1.9/lib/idds/rest/v1/controller.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/rest/v1/hyperparameteropt.py` & `idds-server-2.1.9/lib/idds/rest/v1/hyperparameteropt.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/rest/v1/logs.py` & `idds-server-2.1.9/lib/idds/rest/v1/logs.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/rest/v1/messages.py` & `idds-server-2.1.9/lib/idds/rest/v1/messages.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/rest/v1/monitor.py` & `idds-server-2.1.9/lib/idds/rest/v1/monitor.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/rest/v1/ping.py` & `idds-server-2.1.9/lib/idds/rest/v1/ping.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/rest/v1/requests.py` & `idds-server-2.1.9/lib/idds/rest/v1/requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/rest/v1/utils.py` & `idds-server-2.1.9/lib/idds/rest/v1/utils.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/activelearning_test.py` & `idds-server-2.1.9/lib/idds/tests/activelearning_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/auth_test_script.py` & `idds-server-2.1.9/lib/idds/tests/auth_test_script.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/cacher_test.py` & `idds-server-2.1.9/lib/idds/tests/cacher_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/catalog_test.py` & `idds-server-2.1.9/lib/idds/tests/catalog_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/client_test.py` & `idds-server-2.1.9/lib/idds/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/common.py` & `idds-server-2.1.9/lib/idds/tests/common.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/core_tests.py` & `idds-server-2.1.9/lib/idds/tests/core_tests.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/core_tests_dep_id.py` & `idds-server-2.1.9/lib/idds/tests/core_tests_dep_id.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/core_tests_stat.py` & `idds-server-2.1.9/lib/idds/tests/core_tests_stat.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/datacarousel_test.py` & `idds-server-2.1.9/lib/idds/tests/datacarousel_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/doma_build_test.py` & `idds-server-2.1.9/lib/idds/tests/doma_build_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/doma_build_test_pandaclient.py` & `idds-server-2.1.9/lib/idds/tests/doma_build_test_pandaclient.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/find_dependencies.py` & `idds-server-2.1.9/lib/idds/tests/find_dependencies.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/fix_content_dep_id.py` & `idds-server-2.1.9/lib/idds/tests/fix_content_dep_id.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/fix_trasnform_name.py` & `idds-server-2.1.9/lib/idds/tests/fix_trasnform_name.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/hyperparameteropt_bayesian_test.py` & `idds-server-2.1.9/lib/idds/tests/hyperparameteropt_bayesian_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/hyperparameteropt_client_test.py` & `idds-server-2.1.9/lib/idds/tests/hyperparameteropt_client_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/hyperparameteropt_docker_local_test.py` & `idds-server-2.1.9/lib/idds/tests/hyperparameteropt_docker_local_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/hyperparameteropt_docker_test.py` & `idds-server-2.1.9/lib/idds/tests/hyperparameteropt_docker_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/hyperparameteropt_nevergrad_test.py` & `idds-server-2.1.9/lib/idds/tests/hyperparameteropt_nevergrad_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/jsonload_test.py` & `idds-server-2.1.9/lib/idds/tests/jsonload_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/kill_workflow_task.py` & `idds-server-2.1.9/lib/idds/tests/kill_workflow_task.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/logs_test.py` & `idds-server-2.1.9/lib/idds/tests/logs_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/match_test.py` & `idds-server-2.1.9/lib/idds/tests/match_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/message_test.py` & `idds-server-2.1.9/lib/idds/tests/message_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/message_test1.py` & `idds-server-2.1.9/lib/idds/tests/message_test1.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/migrating_requests_v1_to_v2.py` & `idds-server-2.1.9/lib/idds/tests/migrating_requests_v1_to_v2.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/os_boto3_test.py` & `idds-server-2.1.9/lib/idds/tests/os_boto3_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/panda_client_submit_test.py` & `idds-server-2.1.9/lib/idds/tests/panda_client_submit_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/panda_client_test.py` & `idds-server-2.1.9/lib/idds/tests/panda_client_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/panda_iam_test.py` & `idds-server-2.1.9/lib/idds/tests/panda_iam_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/panda_test.py` & `idds-server-2.1.9/lib/idds/tests/panda_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/performance_test_with_cx_oracle.py` & `idds-server-2.1.9/lib/idds/tests/performance_test_with_cx_oracle.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/performance_test_with_sqlalchemy.py` & `idds-server-2.1.9/lib/idds/tests/performance_test_with_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/relation_map_test.py` & `idds-server-2.1.9/lib/idds/tests/relation_map_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/rest_test.py` & `idds-server-2.1.9/lib/idds/tests/rest_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/run_sql.py` & `idds-server-2.1.9/lib/idds/tests/run_sql.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/scaling_checks.py` & `idds-server-2.1.9/lib/idds/tests/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/split_messages.py` & `idds-server-2.1.9/lib/idds/tests/split_messages.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/subprocess_test.py` & `idds-server-2.1.9/lib/idds/tests/subprocess_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_activelearning.py` & `idds-server-2.1.9/lib/idds/tests/test_activelearning.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_atlaspandawork.py` & `idds-server-2.1.9/lib/idds/tests/test_atlaspandawork.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_auth.py` & `idds-server-2.1.9/lib/idds/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_big_request.py` & `idds-server-2.1.9/lib/idds/tests/test_big_request.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_catalog.py` & `idds-server-2.1.9/lib/idds/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_catalog_core.py` & `idds-server-2.1.9/lib/idds/tests/test_catalog_core.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_class_attr.py` & `idds-server-2.1.9/lib/idds/tests/test_class_attr.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_client.py` & `idds-server-2.1.9/lib/idds/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_core_debug.py` & `idds-server-2.1.9/lib/idds/tests/test_core_debug.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_datacarousel.py` & `idds-server-2.1.9/lib/idds/tests/test_datacarousel.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_domapanda.py` & `idds-server-2.1.9/lib/idds/tests/test_domapanda.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_domapanda_big.py` & `idds-server-2.1.9/lib/idds/tests/test_domapanda_big.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_domapanda_build.py` & `idds-server-2.1.9/lib/idds/tests/test_domapanda_build.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_domapanda_build_pandaclient.py` & `idds-server-2.1.9/lib/idds/tests/test_domapanda_build_pandaclient.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_domapanda_es.py` & `idds-server-2.1.9/lib/idds/tests/test_domapanda_es.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_domapanda_long_name.py` & `idds-server-2.1.9/lib/idds/tests/test_domapanda_long_name.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_domapanda_lsst_workflow.py` & `idds-server-2.1.9/lib/idds/tests/test_domapanda_lsst_workflow.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_domapanda_pandaclient.py` & `idds-server-2.1.9/lib/idds/tests/test_domapanda_pandaclient.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_domapanda_small_mem.py` & `idds-server-2.1.9/lib/idds/tests/test_domapanda_small_mem.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_domapanda_workflow.py` & `idds-server-2.1.9/lib/idds/tests/test_domapanda_workflow.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_get_dn.py` & `idds-server-2.1.9/lib/idds/tests/test_get_dn.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_get_request_info.py` & `idds-server-2.1.9/lib/idds/tests/test_get_request_info.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_get_request_info_panda.py` & `idds-server-2.1.9/lib/idds/tests/test_get_request_info_panda.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_hyperparameteropt.py` & `idds-server-2.1.9/lib/idds/tests/test_hyperparameteropt.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_logger.py` & `idds-server-2.1.9/lib/idds/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_merge_dict.py` & `idds-server-2.1.9/lib/idds/tests/test_merge_dict.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_migrate_requests.py` & `idds-server-2.1.9/lib/idds/tests/test_migrate_requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_request_transform.py` & `idds-server-2.1.9/lib/idds/tests/test_request_transform.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_requests.py` & `idds-server-2.1.9/lib/idds/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_running_data.py` & `idds-server-2.1.9/lib/idds/tests/test_running_data.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_scaling.py` & `idds-server-2.1.9/lib/idds/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_transform_collection_content.py` & `idds-server-2.1.9/lib/idds/tests/test_transform_collection_content.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_transform_processing.py` & `idds-server-2.1.9/lib/idds/tests/test_transform_processing.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_workflow.py` & `idds-server-2.1.9/lib/idds/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_workflow_condition.py` & `idds-server-2.1.9/lib/idds/tests/test_workflow_condition.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_workflow_condition_v2.py` & `idds-server-2.1.9/lib/idds/tests/test_workflow_condition_v2.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/test_workflow_condition_v2_1.py` & `idds-server-2.1.9/lib/idds/tests/test_workflow_condition_v2_1.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds/tests/trigger_release.py` & `idds-server-2.1.9/lib/idds/tests/trigger_release.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/lib/idds_server.egg-info/PKG-INFO` & `idds-server-2.1.9/lib/idds_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-server
-Version: 2.1.8
+Version: 2.1.9
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-server-2.1.8/lib/idds_server.egg-info/SOURCES.txt` & `idds-server-2.1.9/lib/idds_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/setup.py` & `idds-server-2.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/tools/env/clean_heartbeat.py` & `idds-server-2.1.9/tools/env/clean_heartbeat.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/tools/env/config_monitor.py` & `idds-server-2.1.9/tools/env/config_monitor.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/tools/env/create_database.py` & `idds-server-2.1.9/tools/env/create_database.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/tools/env/destroy_database.py` & `idds-server-2.1.9/tools/env/destroy_database.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/tools/env/dump_database.py` & `idds-server-2.1.9/tools/env/dump_database.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/tools/env/environment.yml` & `idds-server-2.1.9/tools/env/environment.yml`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/tools/env/install_env_conda.sh` & `idds-server-2.1.9/tools/env/install_env_conda.sh`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/tools/env/install_idds_example.sh` & `idds-server-2.1.9/tools/env/install_idds_example.sh`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/tools/env/install_idds_full.sh` & `idds-server-2.1.9/tools/env/install_idds_full.sh`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/tools/env/merge_configmap.py` & `idds-server-2.1.9/tools/env/merge_configmap.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/tools/env/merge_idds_configs.py` & `idds-server-2.1.9/tools/env/merge_idds_configs.py`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/tools/env/setup_dev.sh` & `idds-server-2.1.9/tools/env/setup_dev.sh`

 * *Files identical despite different names*

### Comparing `idds-server-2.1.8/tools/env/setup_panda.sh` & `idds-server-2.1.9/tools/env/setup_panda.sh`

 * *Files identical despite different names*

