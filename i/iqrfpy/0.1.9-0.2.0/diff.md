# Comparing `tmp/iqrfpy-0.1.9.tar.gz` & `tmp/iqrfpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqrfpy-0.1.9.tar", last modified: Thu Apr 20 08:10:56 2023, max compression
+gzip compressed data, was "iqrfpy-0.2.0.tar", last modified: Tue Apr  2 15:26:37 2024, max compression
```

## Comparing `iqrfpy-0.1.9.tar` & `iqrfpy-0.2.0.tar`

### file list

```diff
@@ -1,219 +1,303 @@
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.155837 iqrfpy-0.1.9/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      309 2023-03-12 10:44:36.000000 iqrfpy-0.1.9/.editorconfig
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      113 2023-03-27 06:23:13.000000 iqrfpy-0.1.9/.gitignore
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      937 2023-03-22 19:16:00.000000 iqrfpy-0.1.9/.gitlab-ci.yml
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      203 2023-03-22 19:16:00.000000 iqrfpy-0.1.9/.pylintrc
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    11346 2023-03-24 07:47:59.000000 iqrfpy-0.1.9/LICENSE
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      699 2023-04-15 05:33:58.000000 iqrfpy-0.1.9/Makefile
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-20 08:10:56.155837 iqrfpy-0.1.9/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        9 2023-03-07 12:47:49.000000 iqrfpy-0.1.9/README.md
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.143837 iqrfpy-0.1.9/examples/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1007 2023-04-19 09:16:46.000000 iqrfpy-0.1.9/examples/mqtt_transport_async.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1200 2023-04-20 07:40:52.000000 iqrfpy-0.1.9/examples/mqtt_transport_sync.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2081 2023-04-19 10:00:28.000000 iqrfpy-0.1.9/examples/response_factories.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.143837 iqrfpy-0.1.9/iqrfpy/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      111 2023-04-20 08:10:35.000000 iqrfpy-0.1.9/iqrfpy/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.143837 iqrfpy-0.1.9/iqrfpy/enums/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       88 2023-04-18 07:35:52.000000 iqrfpy-0.1.9/iqrfpy/enums/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     6909 2023-04-18 07:34:49.000000 iqrfpy-0.1.9/iqrfpy/enums/commands.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5553 2023-04-18 08:53:31.000000 iqrfpy-0.1.9/iqrfpy/enums/message_types.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      692 2023-04-18 07:35:22.000000 iqrfpy-0.1.9/iqrfpy/enums/peripherals.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4687 2023-04-20 06:12:01.000000 iqrfpy-0.1.9/iqrfpy/exceptions.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.143837 iqrfpy-0.1.9/iqrfpy/messages/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       61 2023-03-24 07:14:54.000000 iqrfpy-0.1.9/iqrfpy/messages/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.143837 iqrfpy-0.1.9/iqrfpy/messages/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      184 2023-04-15 05:52:25.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.143837 iqrfpy-0.1.9/iqrfpy/messages/requests/binaryoutput/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:27.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/binaryoutput/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.143837 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      968 2023-04-18 07:04:34.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1024 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/addr_info.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2730 2023-04-18 07:12:41.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/authorize_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1595 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2400 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/bond_node.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1044 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/bonded_devices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1046 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/clear_all_bonds.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1060 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/discovered_devices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2044 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/discovery.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1677 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/remove_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1879 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1465 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/set_dpa_params.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2389 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/set_hops.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2135 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/set_mid.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5293 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/smart_connect.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.143837 iqrfpy-0.1.9/iqrfpy/messages/requests/dali/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:18.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/dali/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/requests/eeeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/eeeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/requests/eeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:21.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/eeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/requests/exploration/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/exploration/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/requests/frc/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:40.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/frc/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/requests/generic/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/generic/Raw.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/generic/RawHdp.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/generic/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/requests/io/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:21.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/io/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2516 2023-04-19 05:31:16.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/irequest.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/requests/ledg/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:15.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/ledg/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/requests/ledr/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:11.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/ledr/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      971 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/ledr/flashing.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      959 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/ledr/pulse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      965 2023-04-18 08:55:28.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/ledr/set_off.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      961 2023-04-18 08:55:31.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/ledr/set_on.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/requests/light/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:37.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/light/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/requests/node/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:41:43.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/node/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      957 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/node/read.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/requests/os/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:14.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/os/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      947 2023-04-19 06:17:42.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/os/read.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/requests/ram/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:31.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/ram/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/requests/sensor/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:31.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/sensor/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/requests/thermometer/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:27.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/thermometer/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/requests/uart/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:32.000000 iqrfpy-0.1.9/iqrfpy/messages/requests/uart/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    12590 2023-04-20 06:30:15.000000 iqrfpy-0.1.9/iqrfpy/messages/response_factory.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      215 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2735 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/async_response.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/responses/binaryoutput/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:04.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/binaryoutput/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2484 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/confirmation.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      996 2023-04-18 07:07:52.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2548 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/addr_info.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2659 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/authorize_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2468 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2582 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/bond_node.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/bonded_devices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2231 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/clear_all_bonds.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2627 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/discovered_devices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2475 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/discovery.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2480 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/remove_bond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2039 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2624 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/set_dpa_params.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2634 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/set_hops.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2033 2023-04-18 08:18:33.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/set_mid.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2650 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/smart_connect.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/responses/dali/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:58.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/dali/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/responses/eeeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:01.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/eeeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/responses/eeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:56.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/eeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/responses/exploration/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-04-15 05:56:54.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/exploration/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/responses/frc/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:43.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/frc/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/responses/generic/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-04-15 05:56:49.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/generic/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/responses/io/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:27.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/io/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3277 2023-04-15 08:09:43.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/iresponse.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/responses/ledg/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:23.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/ledg/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/responses/ledr/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      244 2023-04-18 08:29:27.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/ledr/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2108 2023-04-19 05:44:14.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/ledr/flashing.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2084 2023-04-18 08:13:48.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/ledr/pulse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2094 2023-04-18 08:55:48.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/ledr/set_off.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2086 2023-04-18 08:55:48.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/ledr/set_on.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/responses/light/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:14.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/light/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.147837 iqrfpy-0.1.9/iqrfpy/messages/responses/node/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:49.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/node/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2579 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/node/read.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.151837 iqrfpy-0.1.9/iqrfpy/messages/responses/os/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       65 2023-04-20 06:27:05.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/os/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4930 2023-04-20 06:46:39.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/os/read.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.151837 iqrfpy-0.1.9/iqrfpy/messages/responses/ram/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:05.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/ram/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.151837 iqrfpy-0.1.9/iqrfpy/messages/responses/sensor/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:09.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/sensor/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.151837 iqrfpy-0.1.9/iqrfpy/messages/responses/thermometer/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:32.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/thermometer/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.151837 iqrfpy-0.1.9/iqrfpy/messages/responses/uart/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:37.000000 iqrfpy-0.1.9/iqrfpy/messages/responses/uart/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.151837 iqrfpy-0.1.9/iqrfpy/transports/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      300 2023-03-22 19:16:00.000000 iqrfpy-0.1.9/iqrfpy/transports/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2414 2023-04-19 11:27:33.000000 iqrfpy-0.1.9/iqrfpy/transports/itransport.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5006 2023-04-20 07:40:03.000000 iqrfpy-0.1.9/iqrfpy/transports/mqtt_transport.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3788 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/iqrfpy/transports/udp_transport.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.151837 iqrfpy-0.1.9/iqrfpy/utils/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       50 2023-03-24 11:33:36.000000 iqrfpy-0.1.9/iqrfpy/utils/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    20492 2023-04-15 08:13:29.000000 iqrfpy-0.1.9/iqrfpy/utils/common.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1810 2023-04-15 07:47:59.000000 iqrfpy-0.1.9/iqrfpy/utils/dpa.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      343 2023-04-15 06:15:47.000000 iqrfpy-0.1.9/iqrfpy/utils/enums.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.143837 iqrfpy-0.1.9/iqrfpy.egg-info/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-20 08:10:56.000000 iqrfpy-0.1.9/iqrfpy.egg-info/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     7074 2023-04-20 08:10:56.000000 iqrfpy-0.1.9/iqrfpy.egg-info/SOURCES.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2023-04-20 08:10:56.000000 iqrfpy-0.1.9/iqrfpy.egg-info/dependency_links.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      159 2023-04-20 08:10:56.000000 iqrfpy-0.1.9/iqrfpy.egg-info/requires.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2023-04-20 08:10:56.000000 iqrfpy-0.1.9/iqrfpy.egg-info/top_level.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      138 2023-03-24 09:25:00.000000 iqrfpy-0.1.9/pyproject.toml
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       85 2023-03-24 07:40:43.000000 iqrfpy-0.1.9/requirements.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1162 2023-04-20 08:10:56.159837 iqrfpy-0.1.9/setup.cfg
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      102 2023-03-22 19:16:00.000000 iqrfpy-0.1.9/test_requirements.txt
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.151837 iqrfpy-0.1.9/tests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-07 12:49:34.000000 iqrfpy-0.1.9/tests/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.151837 iqrfpy-0.1.9/tests/enums/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1241 2023-03-24 10:31:41.000000 iqrfpy-0.1.9/tests/enums/peripherals_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.151837 iqrfpy-0.1.9/tests/messages/
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.151837 iqrfpy-0.1.9/tests/messages/requests/
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.151837 iqrfpy-0.1.9/tests/messages/requests/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      870 2023-04-18 07:02:34.000000 iqrfpy-0.1.9/tests/messages/requests/coordinator/addr_info_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3893 2023-04-18 07:14:42.000000 iqrfpy-0.1.9/tests/messages/requests/coordinator/authorize_bond_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2194 2023-04-18 07:02:34.000000 iqrfpy-0.1.9/tests/messages/requests/coordinator/backup_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3759 2023-04-18 07:02:54.000000 iqrfpy-0.1.9/tests/messages/requests/coordinator/bond_node_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      904 2023-04-18 07:02:54.000000 iqrfpy-0.1.9/tests/messages/requests/coordinator/bonded_devices_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      906 2023-04-18 07:02:54.000000 iqrfpy-0.1.9/tests/messages/requests/coordinator/clear_all_bonds_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      926 2023-04-18 07:04:34.000000 iqrfpy-0.1.9/tests/messages/requests/coordinator/discovered_devices_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3445 2023-04-18 07:04:34.000000 iqrfpy-0.1.9/tests/messages/requests/coordinator/discovery_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2323 2023-04-18 07:04:34.000000 iqrfpy-0.1.9/tests/messages/requests/coordinator/remove_bond_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4241 2023-04-18 07:04:34.000000 iqrfpy-0.1.9/tests/messages/requests/coordinator/restore_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2259 2023-04-18 07:04:34.000000 iqrfpy-0.1.9/tests/messages/requests/coordinator/set_dpa_params_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3673 2023-04-18 07:04:34.000000 iqrfpy-0.1.9/tests/messages/requests/coordinator/set_hops_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3512 2023-04-18 07:04:34.000000 iqrfpy-0.1.9/tests/messages/requests/coordinator/set_mid_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    11031 2023-04-18 07:04:34.000000 iqrfpy-0.1.9/tests/messages/requests/coordinator/smart_connect_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1293 2023-04-18 07:06:09.000000 iqrfpy-0.1.9/tests/messages/requests/irequest_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.155837 iqrfpy-0.1.9/tests/messages/requests/ledr/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      860 2023-04-19 05:58:57.000000 iqrfpy-0.1.9/tests/messages/requests/ledr/flashing_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      842 2023-04-19 05:57:37.000000 iqrfpy-0.1.9/tests/messages/requests/ledr/pulse_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      849 2023-04-19 05:56:05.000000 iqrfpy-0.1.9/tests/messages/requests/ledr/set_off_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      843 2023-04-19 05:29:51.000000 iqrfpy-0.1.9/tests/messages/requests/ledr/set_on_request_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.155837 iqrfpy-0.1.9/tests/messages/requests/os/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      835 2023-04-19 06:19:40.000000 iqrfpy-0.1.9/tests/messages/requests/os/read_request_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4828 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/tests/messages/response_factory_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.155837 iqrfpy-0.1.9/tests/messages/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2163 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/tests/messages/responses/async_response_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1280 2023-04-18 07:05:26.000000 iqrfpy-0.1.9/tests/messages/responses/confirmation_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.155837 iqrfpy-0.1.9/tests/messages/responses/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4326 2023-04-18 07:06:09.000000 iqrfpy-0.1.9/tests/messages/responses/coordinator/addr_info_response_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4515 2023-04-18 07:06:09.000000 iqrfpy-0.1.9/tests/messages/responses/coordinator/authorize_bond_response_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4765 2023-04-18 07:06:09.000000 iqrfpy-0.1.9/tests/messages/responses/coordinator/backup_response_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4392 2023-04-18 07:06:51.000000 iqrfpy-0.1.9/tests/messages/responses/coordinator/bond_node_response_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4213 2023-04-18 07:06:21.000000 iqrfpy-0.1.9/tests/messages/responses/coordinator/bonded_devices_response_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3157 2023-04-18 07:06:51.000000 iqrfpy-0.1.9/tests/messages/responses/coordinator/clear_all_bonds_response_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4345 2023-04-18 07:07:52.000000 iqrfpy-0.1.9/tests/messages/responses/coordinator/discovered_devices_response_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3785 2023-04-18 07:07:52.000000 iqrfpy-0.1.9/tests/messages/responses/coordinator/discovery_response_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3796 2023-04-18 07:07:52.000000 iqrfpy-0.1.9/tests/messages/responses/coordinator/remove_node_response_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3055 2023-04-18 07:07:52.000000 iqrfpy-0.1.9/tests/messages/responses/coordinator/restore_response_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3933 2023-04-18 07:07:52.000000 iqrfpy-0.1.9/tests/messages/responses/coordinator/set_dpa_params_response_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4492 2023-04-18 07:07:52.000000 iqrfpy-0.1.9/tests/messages/responses/coordinator/set_hops_response_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3054 2023-04-18 07:07:52.000000 iqrfpy-0.1.9/tests/messages/responses/coordinator/set_mid_response_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4488 2023-04-18 07:07:52.000000 iqrfpy-0.1.9/tests/messages/responses/coordinator/smart_connect_response_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.155837 iqrfpy-0.1.9/tests/messages/responses/os/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4173 2023-04-19 09:43:38.000000 iqrfpy-0.1.9/tests/messages/responses/os/read_response_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-20 08:10:56.155837 iqrfpy-0.1.9/tests/utils/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    16223 2023-04-15 05:36:55.000000 iqrfpy-0.1.9/tests/utils/common_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       78 2023-03-22 19:16:00.000000 iqrfpy-0.1.9/tox.ini
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.307729 iqrfpy-0.2.0/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    11351 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/LICENSE
+-rw-r--r--   0 khanak    (1000) khanak    (1000)     4862 2024-04-02 15:26:37.307729 iqrfpy-0.2.0/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3314 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/README.md
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.279728 iqrfpy-0.2.0/iqrfpy/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      235 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4377 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/async_response.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4162 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/confirmation.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/enums/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      285 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/enums/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     8125 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/enums/commands.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5591 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/enums/message_types.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      691 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/enums/peripherals.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/enums/py.typed
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     7981 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/exceptions.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/ext/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      281 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/ext/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/ext/py.typed
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    14585 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/irequest.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     6708 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/iresponse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3391 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/itransport.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    12857 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/messages.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/objects/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1421 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3119 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/binaryoutput_state.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2439 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/coordinator_authorize_bond_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      253 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/coordinator_dpa_param.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1316 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/exploration_per_enum_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      955 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/exploration_per_info_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1279 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/frc_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3135 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/io_triplet.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1249 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/node_read_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2327 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/node_validate_bonds_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5710 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_batch_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      224 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_indicate_param.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1295 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_load_code_flags.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1244 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_read_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      200 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_security_type_param.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3719 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_sleep_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4125 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_tr_conf_byte.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    29989 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/os_tr_conf_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1911 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/sensor_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2535 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/objects/sensor_written_data.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/peripherals/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      418 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      414 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      236 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2660 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/requests/enumerate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4543 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/requests/set_output.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      197 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3516 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/responses/enumerate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3616 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/binaryoutput/responses/set_output.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.283728 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1623 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.287728 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1338 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2612 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/addr_info.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4522 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/authorize_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3655 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5435 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/bond_node.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2647 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/bonded_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2650 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/clear_all_bonds.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2675 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/discovered_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5205 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/discovery.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3853 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/remove_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4203 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4036 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/set_dpa_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5298 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/set_hops.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5116 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/set_mid.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     9428 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/requests/smart_connect.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1046 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3677 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/addr_info.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3791 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/authorize_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3432 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3725 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/bond_node.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3563 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/bonded_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2941 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/clear_all_bonds.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3647 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/discovered_devices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3429 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/discovery.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3441 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/remove_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2857 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3588 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/set_dpa_params.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3783 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/set_hops.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2704 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/set_mid.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3776 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/smart_connect.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      299 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      160 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4978 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/requests/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5136 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/requests/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      165 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3330 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/responses/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2856 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/responses/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      298 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      159 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4934 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/requests/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5132 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/requests/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      164 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3351 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/responses/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2877 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/responses/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      733 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      376 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2870 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/requests/more_peripherals_information.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2730 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/requests/peripheral_enumeration.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3218 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/requests/peripheral_information.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      516 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4752 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/responses/more_peripherals_information.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4888 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/responses/peripheral_enumeration.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4183 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/exploration/responses/peripheral_information.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/frc/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      594 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      392 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2604 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/extra_result.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5101 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/send.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     6786 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/send_selective.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4064 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/requests/set_frc_params.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      336 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3483 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/extra_result.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3711 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/send.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3833 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/send_selective.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3485 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/frc/responses/set_frc_params.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/generic/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      370 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/generic/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/generic/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      106 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/generic/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3268 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/generic/requests/generic.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.291728 iqrfpy-0.2.0/iqrfpy/peripherals/generic/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      109 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/generic/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3182 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/generic/responses/generic.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/io/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      435 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/io/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      275 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4126 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/requests/direction.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2553 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/requests/get.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4084 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/requests/set.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/io/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      217 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2873 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/responses/direction.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3298 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/responses/get.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2795 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/io/responses/set.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      499 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      278 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2583 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/flashing.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2562 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/pulse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2574 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/set_off.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/requests/set_on.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      287 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2696 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/flashing.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2660 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/pulse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2677 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/set_off.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2665 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/set_on.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      499 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      278 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2583 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/flashing.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2562 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/pulse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2574 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/set_off.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/requests/set_on.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      287 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2696 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/flashing.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2660 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/pulse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2677 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/set_off.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2665 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/set_on.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/node/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      719 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.295729 iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      419 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3606 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2557 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2604 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/remove_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3938 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4425 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/requests/validate_bonds.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.299729 iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      448 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3430 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3858 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2756 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/remove_bond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2861 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2944 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/validate_bonds.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.299729 iqrfpy-0.2.0/iqrfpy/peripherals/os/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1860 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.299729 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1351 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3903 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/batch.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2625 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/factory_settings.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3203 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/indicate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     7831 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/load_code.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2543 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2615 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/read_tr_conf.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2550 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/reset.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2564 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/restart.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2550 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/rfpgm.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5689 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/selective_batch.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5437 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/set_security.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3209 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/sleep.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5979 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/test_rf_signal.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4243 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/write_tr_conf.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4128 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/write_tr_conf_byte.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1149 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2711 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/batch.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2846 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/factory_settings.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2750 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/indicate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4342 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/load_code.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4973 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4550 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/read_tr_conf.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2711 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/reset.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2737 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/restart.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2705 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/rfpgm.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2823 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/selective_batch.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2788 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/set_security.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2705 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/sleep.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4084 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/test_rf_signal.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2818 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/write_tr_conf.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2870 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/write_tr_conf_byte.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/py.typed
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/ram/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      396 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/ram/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      215 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4913 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/requests/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4878 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/requests/read_any.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5108 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/requests/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/ram/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      222 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3349 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/responses/read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3272 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/responses/read_any.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2856 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/ram/responses/write.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      587 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      381 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2592 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/requests/enumerate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5088 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/requests/read_sensors.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5631 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/requests/read_sensors_with_types.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      366 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3721 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/responses/enumerate.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3239 2024-03-26 15:40:45.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/responses/read_sensors.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3880 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/sensor/responses/read_sensors_with_types.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      229 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      112 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2606 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/requests/read.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      115 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3693 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/thermometer/responses/read.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/uart/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      515 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      303 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5734 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/clear_write_read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2564 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/close.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3778 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/open.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5684 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/requests/write_read.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.303729 iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      312 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3460 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/clear_write_read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2690 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/close.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2678 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/open.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3395 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/write_read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/py.typed
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    42518 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/response_factory.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.307729 iqrfpy-0.2.0/iqrfpy/utils/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      272 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    27163 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/common.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     8471 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/dpa.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      563 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/enums.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2175 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/frc_parser.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/utils/py.typed
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    14876 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/quantity_data.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2659 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/sensor_constants.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    26301 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/iqrfpy/utils/sensor_parser.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3397 2024-03-18 17:43:19.000000 iqrfpy-0.2.0/iqrfpy/utils/validators.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2024-04-02 15:26:37.307729 iqrfpy-0.2.0/iqrfpy.egg-info/
+-rw-r--r--   0 khanak    (1000) khanak    (1000)     4862 2024-04-02 15:26:37.000000 iqrfpy-0.2.0/iqrfpy.egg-info/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    10578 2024-04-02 15:26:37.000000 iqrfpy-0.2.0/iqrfpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2024-04-02 15:26:37.000000 iqrfpy-0.2.0/iqrfpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      114 2024-04-02 15:26:37.000000 iqrfpy-0.2.0/iqrfpy.egg-info/requires.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2024-04-02 15:26:37.000000 iqrfpy-0.2.0/iqrfpy.egg-info/top_level.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      116 2024-04-02 13:56:09.000000 iqrfpy-0.2.0/pyproject.toml
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1545 2024-04-02 15:26:37.307729 iqrfpy-0.2.0/setup.cfg
```

### Comparing `iqrfpy-0.1.9/LICENSE` & `iqrfpy-0.2.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2023 MICRORISC s.r.o
+   Copyright 2023-2024 MICRORISC s.r.o
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `iqrfpy-0.1.9/iqrfpy/enums/commands.py` & `iqrfpy-0.2.0/iqrfpy/enums/commands.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-"""
-Commands module.
+"""Commands module.
 
 This module contains embed peripherals and standards command enums.
 These enums are extended with has_value() method for member identification.
 """
 
-import enum
+from ..utils.enums import IntEnumMember
+from .peripherals import EmbedPeripherals
 
 __all__ = [
     'Command',
     'ExplorationRequestCommands',
+    'ExplorationRequestPeripheralCommand',
     'CoordinatorRequestCommands',
     'NodeRequestCommands',
     'OSRequestCommands',
     'EEPROMRequestCommands',
     'EEEPROMRequestCommands',
     'RAMRequestCommands',
     'LEDRequestCommands',
@@ -22,14 +23,15 @@
     'UartRequestCommands',
     'FrcRequestCommands',
     'DALIRequestCommands',
     'BinaryOutputRequestCommands',
     'SensorRequestCommands',
     'LightRequestCommands',
     'ExplorationResponseCommands',
+    'ExplorationResponsePeripheralCommand',
     'CoordinatorResponseCommands',
     'NodeResponseCommands',
     'OSResponseCommands',
     'EEPROMResponseCommands',
     'EEEPROMResponseCommands',
     'RAMResponseCommands',
     'LEDResponseCommands',
@@ -40,36 +42,41 @@
     'DALIResponseCommands',
     'BinaryOutputResponseCommands',
     'SensorResponseCommands',
     'LightResponseCommands'
 ]
 
 
-class Command(enum.IntEnum):
+class Command(IntEnumMember):
     """DPA commands base enum."""
 
-    pass
-
-    @classmethod
-    def has_value(cls, value):
-        """
-        Check if enum class has member value.
-
-        :param value: value to check
-        :return: True if value is a member of enum, False otherwise
-        """
-        return value in cls._value2member_map_
-
 
 class ExplorationRequestCommands(Command):
     """Exploration request commands enum."""
 
     PERIPHERALS_ENUMERATION_INFORMATION = 63
 
 
+class ExplorationRequestPeripheralCommand(Command):
+    """More peripherals information peripheral commands enum."""
+
+    PER_COORDINATOR = EmbedPeripherals.COORDINATOR
+    PER_NODE = EmbedPeripherals.NODE
+    PER_OS = EmbedPeripherals.OS
+    PER_EEPROM = EmbedPeripherals.EEPROM
+    PER_EEEPROM = EmbedPeripherals.EEEPROM
+    PER_RAM = EmbedPeripherals.RAM
+    PER_LEDR = EmbedPeripherals.LEDR
+    PER_LEDG = EmbedPeripherals.LEDG
+    PER_IO = EmbedPeripherals.IO
+    PER_THERMOMETER = EmbedPeripherals.THERMOMETER
+    PER_UART = EmbedPeripherals.UART
+    PER_FRC = EmbedPeripherals.FRC
+
+
 class CoordinatorRequestCommands(Command):
     """Coordinator request commands enum."""
 
     ADDR_INFO = 0
     DISCOVERED_DEVICES = 1
     BONDED_DEVICES = 2
     CLEAR_ALL_BONDS = 3
@@ -116,14 +123,15 @@
 
 
 class RAMRequestCommands(Command):
     """RAM request commands enum."""
 
     READ = 0
     WRITE = 1
+    READ_ANY = 15
 
 
 class EEPROMRequestCommands(Command):
     """EEPROM request commands enum."""
 
     READ = 0
     WRITE = 1
@@ -210,14 +218,32 @@
     ENUMERATE = 62
 
 
 class ExplorationResponseCommands(Command):
     """Exploration response commands enum."""
 
     PERIPHERALS_ENUMERATION_INFORMATION = 191
+    MORE_PERIPHERALS_INFORMATION = 255
+
+
+class ExplorationResponsePeripheralCommand(Command):
+    """More peripherals information peripheral commands enum."""
+
+    PER_COORDINATOR = EmbedPeripherals.COORDINATOR + 0x80
+    PER_NODE = EmbedPeripherals.NODE + 0x80
+    PER_OS = EmbedPeripherals.OS + 0x80
+    PER_EEPROM = EmbedPeripherals.EEPROM + 0x80
+    PER_EEEPROM = EmbedPeripherals.EEEPROM + 0x80
+    PER_RAM = EmbedPeripherals.RAM + 0x80
+    PER_LEDR = EmbedPeripherals.LEDR + 0x80
+    PER_LEDG = EmbedPeripherals.LEDG + 0x80
+    PER_IO = EmbedPeripherals.IO + 0x80
+    PER_THERMOMETER = EmbedPeripherals.THERMOMETER + 0x80
+    PER_UART = EmbedPeripherals.UART + 0x80
+    PER_FRC = EmbedPeripherals.FRC + 0x80
 
 
 class CoordinatorResponseCommands(Command):
     """Coordinator response commands enum."""
 
     ADDR_INFO = 128
     DISCOVERED_DEVICES = 129
@@ -258,22 +284,23 @@
     INDICATE = 135
     RESTART = 136
     WRITE_CFG_BYTE = 137
     LOAD_CODE = 138
     SELECTIVE_BATCH = 139
     TEST_RF_SIGNAL = 140
     FACTORY_SETTINGS = 141
-    WRITE_CFG = 142
+    WRITE_CFG = 143
 
 
 class RAMResponseCommands(Command):
     """RAM response commands enum."""
 
     READ = 128
     WRITE = 129
+    READ_ANY = 143
 
 
 class EEPROMResponseCommands(Command):
     """EEPROM response commands enum."""
 
     READ = 128
     WRITE = 129
```

### Comparing `iqrfpy-0.1.9/iqrfpy/enums/message_types.py` & `iqrfpy-0.2.0/iqrfpy/enums/message_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Message types module.
+"""Message types module.
 
 This module contains embed peripherals and standards message type enums.
 These enums are extended with has_value() method for member identification.
 """
 
 import enum
 
@@ -29,23 +28,22 @@
     'LightMessages'
 ]
 
 
 class MessageType(enum.Enum):
     """JSON API message type base enum."""
 
-    pass
-
     @classmethod
-    def has_value(cls, value):
-        """
-        Check if enum class has member value.
+    def has_value(cls, value: str):
+        """Check if enum class has member value.
 
-        :param value: value to check
-        :return: True if value is a member of enum, False otherwise
+        Args:
+            value (str): value to check
+        Returns:
+            :obj`bool`: True if value is a member of enum, False otherwise
         """
         return value in cls._value2member_map_
 
 
 class GenericMessages(MessageType):
     """Generic message types enum."""
 
@@ -139,16 +137,16 @@
     PULSE = 'iqrfEmbedLedr_Pulse'
     FLASHING = 'iqrfEmbedLedr_Flashing'
 
 
 class LEDGMessages(MessageType):
     """LEDG message types enum."""
 
-    SET = 'iqrfEmbedLedg_Set'
-    GET = 'iqrfEmbedLedg_Get'
+    SET_ON = 'iqrfEmbedLedg_SetOn'
+    SET_OFF = 'iqrfEmbedLedg_SetOff'
     PULSE = 'iqrfEmbedLedg_Pulse'
     FLASHING = 'iqrfEmbedLedg_Flashing'
 
 
 class IOMessages(MessageType):
     """IO message types enum."""
 
@@ -188,16 +186,16 @@
     SEND_COMMANDS_ASYNC = 'iqrfDali_SendCommandsAsync'
     FRC = 'iqrfDali_Frc'
 
 
 class BinaryOutputMessages(MessageType):
     """BinaryOutput message types enum."""
 
-    SET_OUTPUT = 'iqrfBinaryOutput_SetOutput'
-    ENUMERATE = 'iqrfBinaryOutput_Enumerate'
+    SET_OUTPUT = 'iqrfBinaryoutput_SetOutput'
+    ENUMERATE = 'iqrfBinaryoutput_Enumerate'
 
 
 class SensorMessages(MessageType):
     """Sensor message types enum."""
 
     READ_SENSORS_WITH_TYPES = 'iqrfSensor_ReadSensorsWithTypes'
     ENUMERATE = 'iqrfSensor_Enumerate'
```

### Comparing `iqrfpy-0.1.9/iqrfpy/enums/peripherals.py` & `iqrfpy-0.2.0/iqrfpy/enums/peripherals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Peripherals module.
+"""Peripherals module.
 
 This module contains embedded peripherals and standards enums.
 These enums are extended with has_value() method for member identification.
 """
 
 from ..utils.enums import IntEnumMember
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/requests/coordinator/__init__.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/os/requests/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,52 @@
-from .addr_info import AddrInfoRequest
-from .authorize_bond import AuthorizeBondRequest
-from .backup import BackupRequest
-from .bonded_devices import BondedDevicesRequest
-from .bond_node import BondNodeRequest
-from .clear_all_bonds import ClearAllBondsRequest
-from .discovered_devices import DiscoveredDevicesRequest
-from .discovery import DiscoveryRequest
-from .remove_bond import RemoveBondRequest
-from .restore import RestoreRequest
-from .set_dpa_params import SetDpaParamsRequest
-from .set_hops import SetHopsRequest
-from .set_mid import SetMIDRequest
-from .smart_connect import SmartConnectRequest
+"""OS peripheral request messages."""
 
-__all__ = [
-    'AddrInfoRequest',
-    'AuthorizeBondRequest',
-    'BackupRequest',
-    'BondedDevicesRequest',
-    'BondNodeRequest',
-    'ClearAllBondsRequest',
-    'DiscoveredDevicesRequest',
-    'DiscoveryRequest',
-    'RemoveBondRequest',
-    'RestoreRequest',
-    'SetDpaParamsRequest',
-    'SetHopsRequest',
-    'SetMIDRequest',
-    'SmartConnectRequest'
-]
+from .read import ReadRequest
+from .reset import ResetRequest
+from .restart import RestartRequest
+from .read_tr_conf import ReadTrConfRequest
+from .write_tr_conf import WriteTrConfRequest
+from .write_tr_conf_byte import WriteTrConfByteRequest
+from .rfpgm import RfpgmRequest
+from .sleep import SleepRequest
+from .set_security import SetSecurityRequest
+from .batch import BatchRequest
+from .selective_batch import SelectiveBatchRequest
+from .indicate import IndicateRequest
+from .factory_settings import FactorySettingsRequest
+from .test_rf_signal import TestRfSignalRequest
+from .load_code import LoadCodeRequest
+
+from iqrfpy.objects import (
+    OsBatchData,
+    OsTrConfData,
+    OsTrConfByte,
+    OsSleepParams,
+    OsSecurityTypeParam,
+    OsIndicateParam,
+    OsLoadCodeFlags,
+)
+
+__all__ = (
+    'BatchRequest',
+    'FactorySettingsRequest',
+    'IndicateRequest',
+    'LoadCodeRequest',
+    'ReadRequest',
+    'ReadTrConfRequest',
+    'ResetRequest',
+    'RestartRequest',
+    'RfpgmRequest',
+    'SelectiveBatchRequest',
+    'SetSecurityRequest',
+    'SleepRequest',
+    'TestRfSignalRequest',
+    'WriteTrConfRequest',
+    'WriteTrConfByteRequest',
+    'OsBatchData',
+    'OsIndicateParam',
+    'OsLoadCodeFlags',
+    'OsSecurityTypeParam',
+    'OsSleepParams',
+    'OsTrConfByte',
+    'OsTrConfData',
+)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/async_response.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/generic/responses/generic.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,79 @@
-from __future__ import annotations
-from typeguard import typechecked
-from typing import Optional
-from iqrfpy.enums.peripherals import Peripheral
+"""Generic response message."""
+
+from typing import List, Optional, Union
+from iqrfpy.iresponse import IResponseGetterMixin
 from iqrfpy.enums.commands import Command
 from iqrfpy.enums.message_types import GenericMessages
-from .iresponse import IResponse, IResponseGetterMixin
+from iqrfpy.enums.peripherals import Peripheral
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
+import iqrfpy.utils.dpa as dpa_constants
 from iqrfpy.utils.dpa import ResponsePacketMembers
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
 
-__all__ = ['AsyncResponse']
 
+class GenericResponse(IResponseGetterMixin):
+    """Generic response class."""
 
-@typechecked
-class AsyncResponse(IResponseGetterMixin):
-
-    def __init__(self, nadr: int, pnum: Peripheral, pcmd: Command, hwpid: int = DpaConstants.HWPID_MAX,
-                 rcode: int = 0x80, dpa_value: int = 0, pdata: Optional[bytes] = None, msgid: Optional[str] = None,
-                 result: Optional[dict] = None):
+    def __init__(self, nadr: int, pnum: Union[Peripheral, int], pcmd: Union[Command, int],
+                 hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+                 pdata: Optional[List[int]] = None, msgid: Optional[str] = None):
+        """Generic response constructor.
+
+        Args:
+            nadr (int): Device address.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            msgid (str, optional): Message ID. Defaults to None.
+        """
         super().__init__(
             nadr=nadr,
             pnum=pnum,
             pcmd=pcmd,
             m_type=GenericMessages.RAW,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
-            pdata=pdata,
             msgid=msgid,
-            result=result
+            pdata=pdata,
+            result=pdata,
         )
 
-    @staticmethod
-    def from_dpa(dpa: bytes) -> AsyncResponse:
-        IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        pnum = Common.pnum_from_dpa(dpa[ResponsePacketMembers.PNUM])
-        pcmd = Common.request_pcmd_from_dpa(pnum, dpa[ResponsePacketMembers.PCMD])
-        rcode = dpa[ResponsePacketMembers.RCODE]
-        result = None
-        if rcode == DpaConstants.ASYNC_RESPONSE_CODE:
-            if len(dpa) > 8:
-                result = {'rData': list(dpa)}
-        return AsyncResponse(nadr=dpa[ResponsePacketMembers.NADR], pnum=pnum, pcmd=pcmd, hwpid=hwpid, rcode=rcode,
-                             dpa_value=dpa[ResponsePacketMembers.DPA_VALUE], pdata=dpa, result=result)
-
-    @staticmethod
-    def from_json(json: dict) -> AsyncResponse:
-        msgid = Common.msgid_from_json(json)
-        result = json['data']['rsp']
-        packet = result['rData'].replace('.', '')
-        pdata = bytes.fromhex(packet)
-        ldata = Common.hex_string_to_list(packet)
-        hwpid = Common.hwpid_from_dpa(ldata[ResponsePacketMembers.HWPID_HI], ldata[ResponsePacketMembers.HWPID_LO])
-        pnum = Common.pnum_from_dpa(ldata[ResponsePacketMembers.PNUM])
-        pcmd = Common.request_pcmd_from_dpa(pnum, ldata[ResponsePacketMembers.PCMD])
-        return AsyncResponse(nadr=ldata[ResponsePacketMembers.NADR], pnum=pnum, pcmd=pcmd, hwpid=hwpid,
-                             rcode=ldata[ResponsePacketMembers.RCODE], dpa_value=ldata[ResponsePacketMembers.DPA_VALUE],
-                             pdata=pdata, msgid=msgid, result=result)
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'GenericResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs GenericResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            GenericResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        nadr, pnum, pcmd, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(nadr=nadr, pnum=pnum, pcmd=pcmd, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'GenericResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs GenericResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            GenericResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid = Common.msgid_from_json(json=json)
+        raw = [int(x, 16) for x in Common.generic_rdata_from_json(json=json).split('.')]
+        nadr = raw[ResponsePacketMembers.NADR]
+        pnum = raw[ResponsePacketMembers.PNUM]
+        pcmd = raw[ResponsePacketMembers.PCMD]
+        hwpid = Common.hwpid_from_dpa(raw[ResponsePacketMembers.HWPID_HI], raw[ResponsePacketMembers.HWPID_LO])
+        rcode = raw[ResponsePacketMembers.RCODE]
+        dpa_value = raw[ResponsePacketMembers.DPA_VALUE]
+        pdata = raw[8:] if len(raw) > 8 else None
+        return cls(nadr=nadr, pnum=pnum, pcmd=pcmd, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata,
+                   msgid=msgid)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/confirmation.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/clear_all_bonds.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,72 @@
-from __future__ import annotations
-from typing import Optional
-from iqrfpy.enums.commands import Command
-from iqrfpy.enums.peripherals import Peripheral
-from iqrfpy.exceptions import DpaConfirmationPacketError, DpaConfirmationPacketLengthError
+"""Coordinator Clear All Bonds response message."""
+
+from typing import List, Optional
+from iqrfpy.iresponse import IResponseGetterMixin
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
+from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
-from iqrfpy.messages.responses.iresponse import IResponseGetterMixin
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
 
-__all__ = ['Confirmation']
+__all__ = ['ClearAllBondsResponse']
 
 
-class Confirmation(IResponseGetterMixin):
-    __slots__ = '_request_hops', '_response_hops', '_timeslot'
+class ClearAllBondsResponse(IResponseGetterMixin):
+    """Coordinator ClearAllBonds response class."""
 
-    def __init__(self, nadr: int, pnum: Peripheral, pcmd: Command, hwpid: int, dpa_value: int, rcode: int,
-                 result: Optional[dict] = None):
+    def __init__(self, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+                 msgid: Optional[str] = None, pdata: Optional[List[int]] = None, result: Optional[dict] = None):
+        """ClearAllBonds response constructor.
+
+        Args:
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            pdata (List[int], optional): DPA response data. Defaults to None.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=nadr,
-            pcmd=pcmd,
-            pnum=pnum,
+            nadr=dpa_constants.COORDINATOR_NADR,
+            pnum=EmbedPeripherals.COORDINATOR,
+            pcmd=CoordinatorResponseCommands.CLEAR_ALL_BONDS,
+            m_type=CoordinatorMessages.CLEAR_ALL_BONDS,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
+            msgid=msgid,
+            pdata=pdata,
             result=result
         )
-        self._request_hops: int = result['requestHops']
-        self._response_hops: int = result['responseHops']
-        self._timeslot: int = result['timeslot']
-
-    def get_request_hops(self) -> int:
-        return self._request_hops
-
-    def get_response_hops(self) -> int:
-        return self._response_hops
-
-    def get_timeslot(self) -> int:
-        return self._timeslot
-
-    @staticmethod
-    def from_dpa(dpa: bytes) -> Confirmation:
-        if len(dpa) != DpaConstants.CONFIRMATION_PACKET_LEN:
-            raise DpaConfirmationPacketLengthError('Invalid DPA confirmation packet length.')
-        if dpa[ResponsePacketMembers.RCODE] != DpaConstants.CONFIRMATION_RCODE:
-            raise DpaConfirmationPacketError('Invalid DPA confirmation packet error code.')
-        pnum = Common.pnum_from_dpa(dpa[ResponsePacketMembers.PNUM])
-        pcmd = Common.request_pcmd_from_dpa(pnum, dpa[ResponsePacketMembers.PCMD])
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        result = {'requestHops': dpa[8], 'responseHops': dpa[10], 'timeslot': dpa[9]}
-        return Confirmation(nadr=dpa[ResponsePacketMembers.NADR], pnum=pnum, pcmd=pcmd, hwpid=hwpid,
-                            rcode=dpa[ResponsePacketMembers.RCODE], dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
-                            result=result)
-
-    @staticmethod
-    def from_json(json: dict) -> Confirmation:
-        raise NotImplementedError('from_json() method not implemented.')
+
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'ClearAllBondsResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs ClearAllBondsResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            ClearAllBondsResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        DpaValidator.response_length(dpa=dpa, expected_len=8)
+        _, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'ClearAllBondsResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs ClearAllBondsResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            ClearAllBondsResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, _, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
+        return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/__init__.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,33 @@
+"""Coordinator peripheral response messages."""
+
 from .addr_info import AddrInfoResponse
 from .authorize_bond import AuthorizeBondResponse
 from .backup import BackupResponse
-from .bonded_devices import BondedDevicesResponse
 from .bond_node import BondNodeResponse
+from .bonded_devices import BondedDevicesResponse
 from .clear_all_bonds import ClearAllBondsResponse
 from .discovered_devices import DiscoveredDevicesResponse
 from .discovery import DiscoveryResponse
 from .remove_bond import RemoveBondResponse
 from .restore import RestoreResponse
 from .set_dpa_params import SetDpaParamsResponse
 from .set_hops import SetHopsResponse
-from .set_mid import SetMIDResponse
+from .set_mid import SetMidResponse
 from .smart_connect import SmartConnectResponse
 
-__all__ = [
+__all__ = (
     'AddrInfoResponse',
     'AuthorizeBondResponse',
     'BackupResponse',
-    'BondedDevicesResponse',
     'BondNodeResponse',
+    'BondedDevicesResponse',
     'ClearAllBondsResponse',
     'DiscoveredDevicesResponse',
     'DiscoveryResponse',
     'RemoveBondResponse',
     'RestoreResponse',
     'SetDpaParamsResponse',
     'SetHopsResponse',
-    'SetMIDResponse',
-    'SmartConnectResponse'
-]
+    'SetMidResponse',
+    'SmartConnectResponse',
+)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/addr_info.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/eeeprom/responses/read.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,88 @@
-from __future__ import annotations
-from typeguard import typechecked
-from typing import Optional
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.commands import CoordinatorResponseCommands
-from iqrfpy.enums.message_types import CoordinatorMessages
+"""Eeeprom Read response message."""
+
+from typing import List, Optional
+from iqrfpy.iresponse import IResponseGetterMixin
+from iqrfpy.enums.commands import EEEPROMResponseCommands
+from iqrfpy.enums.message_types import EEEPROMMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
-
-__all__ = ['AddrInfoResponse']
-
-
-@typechecked
-class AddrInfoResponse(IResponseGetterMixin):
-    __slots__ = '_dev_nr', '_did'
-
-    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
-                 msgid: Optional[str] = None, result: Optional[dict] = None):
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.dpa import ResponseCodes
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
+
+__all__ = ['ReadResponse']
+
+
+class ReadResponse(IResponseGetterMixin):
+    """Eeeprom Read response class."""
+
+    __slots__ = ('_data',)
+
+    def __init__(self, nadr: int, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+                 msgid: Optional[str] = None, pdata: Optional[List[int]] = None, result: Optional[dict] = None):
+        """Read response constructor.
+
+        Args:
+            nadr (int): Device address.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            pdata (List[int], optional): DPA response data. Defaults to None.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=DpaConstants.COORDINATOR_NADR,
-            pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.ADDR_INFO,
-            m_type=CoordinatorMessages.ADDR_INFO,
+            nadr=nadr,
+            pnum=EmbedPeripherals.EEEPROM,
+            pcmd=EEEPROMResponseCommands.READ,
+            m_type=EEEPROMMessages.READ,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
+            pdata=pdata,
             result=result
         )
-        if rcode == ResponseCodes.OK:
-            self._dev_nr = result['devNr']
-            self._did = result['did']
-
-    def get_dev_nr(self) -> int:
-        return self._dev_nr
-
-    def get_did(self) -> int:
-        return self._did
+        self._data = result['pData'] if rcode == ResponseCodes.OK else None
 
-    @staticmethod
-    def from_dpa(dpa: bytes) -> AddrInfoResponse:
-        IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
+    @property
+    def data(self) -> Optional[List[int]]:
+        """:obj:`list` of :obj:`int` or :obj:`None`: Data read from memory.
+
+        Getter only.
+        """
+        return self._data
+
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'ReadResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs ReadResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            ReadResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
-            if len(dpa) != 10:
-                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'devNr': dpa[8], 'did': dpa[9]}
-        return AddrInfoResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE], result=result)
-
-    @staticmethod
-    def from_json(json: dict) -> AddrInfoResponse:
-        msgid = Common.msgid_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
-        return AddrInfoResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+            pdata = Common.pdata_from_dpa(dpa=dpa)
+            result = {'pData': list(dpa[8:])}
+        return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata, result=result)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'ReadResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs ReadResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            ReadResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
+        return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/authorize_bond.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/uart/responses/close.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,69 @@
-from __future__ import annotations
-from typeguard import typechecked
+"""UART Close response message."""
+
 from typing import Optional
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.commands import CoordinatorResponseCommands
-from iqrfpy.enums.message_types import CoordinatorMessages
+from iqrfpy.iresponse import IResponseGetterMixin
+from iqrfpy.enums.commands import UartResponseCommands
+from iqrfpy.enums.message_types import UartMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
-
-__all__ = ['AuthorizeBondResponse']
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
 
 
-@typechecked
-class AuthorizeBondResponse(IResponseGetterMixin):
-    __slots__ = '_bond_addr', '_dev_nr'
+class CloseResponse(IResponseGetterMixin):
+    """UART Close response class."""
 
-    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, nadr: int, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
+        """Close response constructor.
+
+        Args:
+            nadr (int): Device address.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=DpaConstants.COORDINATOR_NADR,
-            pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.AUTHORIZE_BOND,
-            m_type=CoordinatorMessages.AUTHORIZE_BOND,
+            nadr=nadr,
+            pnum=EmbedPeripherals.UART,
+            pcmd=UartResponseCommands.CLOSE,
+            m_type=UartMessages.CLOSE,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
-        if rcode == ResponseCodes.OK:
-            self._bond_addr = result['bondAddr']
-            self._dev_nr = result['devNr']
-
-    def get_bond_addr(self) -> int:
-        return self._bond_addr
-
-    def get_dev_nr(self) -> int:
-        return self._dev_nr
-
-    @staticmethod
-    def from_dpa(dpa: bytes) -> AuthorizeBondResponse:
-        IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
-        result = None
-        if rcode == ResponseCodes.OK:
-            if len(dpa) != 10:
-                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'bondAddr': dpa[8], 'devNr': dpa[9]}
-        return AuthorizeBondResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
-                                     result=result)
-
-    @staticmethod
-    def from_json(json: dict) -> AuthorizeBondResponse:
-        msgid = Common.msgid_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
-        return AuthorizeBondResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'CloseResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs :obj:`CloseResponse` object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            :obj:`CloseResponse`: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        DpaValidator.response_length(dpa=dpa, expected_len=8)
+        nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'CloseResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs :obj:`CloseResponse` object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            :obj:`CloseResponse`: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
+        return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/backup.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/validate_bonds.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,73 @@
-from __future__ import annotations
-from typeguard import typechecked
+"""Node Validate Bonds response message."""
+
 from typing import List, Optional
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.commands import CoordinatorResponseCommands
-from iqrfpy.enums.message_types import CoordinatorMessages
+from iqrfpy.iresponse import IResponseGetterMixin
+from iqrfpy.enums.commands import NodeResponseCommands
+from iqrfpy.enums.message_types import NodeMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
 
-__all__ = ['BackupResponse']
+__all__ = ['ValidateBondsResponse']
 
 
-@typechecked
-class BackupResponse(IResponseGetterMixin):
-    __slots__ = '_network_data'
+class ValidateBondsResponse(IResponseGetterMixin):
+    """Node Validate Bonds response class."""
 
-    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
-                 msgid: Optional[str] = None, result: Optional[dict] = None):
+    def __init__(self, nadr: int, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+                 msgid: Optional[str] = None, pdata: Optional[List[int]] = None, result: Optional[dict] = None):
+        """Validate Bonds response constructor.
+
+        Args:
+            nadr (int): Device address.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            pdata (List[int], optional): DPA response data. Defaults to None.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=DpaConstants.COORDINATOR_NADR,
-            pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.BACKUP,
-            m_type=CoordinatorMessages.BACKUP,
+            nadr=nadr,
+            pnum=EmbedPeripherals.NODE,
+            pcmd=NodeResponseCommands.VALIDATE_BONDS,
+            m_type=NodeMessages.VALIDATE_BONDS,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
+            pdata=pdata,
             result=result
         )
-        if rcode == ResponseCodes.OK:
-            self._network_data = result['networkData']
-
-    def get_network_data(self) -> List[int]:
-        return self._network_data
 
-    @staticmethod
-    def from_dpa(dpa: bytes) -> BackupResponse:
-        IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
-        result = None
-        if rcode == ResponseCodes.OK:
-            if len(dpa) != 57:
-                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'networkData': list(dpa[8:])}
-        return BackupResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE], result=result)
-
-    @staticmethod
-    def from_json(json: dict) -> BackupResponse:
-        msgid = Common.msgid_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
-        return BackupResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'ValidateBondsResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs ValidateBondsResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            ValidateBondsResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        DpaValidator.response_length(dpa=dpa, expected_len=8)
+        nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'ValidateBondsResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs ValidateBondsResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            ValidateBondsResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
+        return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/bond_node.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/pulse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,69 @@
-from __future__ import annotations
-from typeguard import typechecked
+"""LEDG Pulse response message."""
+
 from typing import Optional
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.commands import CoordinatorResponseCommands
-from iqrfpy.enums.message_types import CoordinatorMessages
+from iqrfpy.iresponse import IResponseGetterMixin
+from iqrfpy.enums.commands import LEDResponseCommands
+from iqrfpy.enums.message_types import LEDGMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
-
-__all__ = ['BondNodeResponse']
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
 
 
-@typechecked
-class BondNodeResponse(IResponseGetterMixin):
-    __slots__ = '_bond_addr', '_dev_nr'
+class PulseResponse(IResponseGetterMixin):
+    """LEDG Pulse response class."""
 
-    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, nadr: int, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
+        """Pulse response constructor.
+
+        Args:
+            nadr (int): Device address.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=DpaConstants.COORDINATOR_NADR,
-            pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.BOND_NODE,
-            m_type=CoordinatorMessages.BOND_NODE,
+            nadr=nadr,
+            pnum=EmbedPeripherals.LEDG,
+            pcmd=LEDResponseCommands.PULSE,
+            m_type=LEDGMessages.PULSE,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
-        if rcode == ResponseCodes.OK:
-            self._bond_addr = result['bondAddr']
-            self._dev_nr = result['devNr']
-
-    def get_bond_addr(self) -> int:
-        return self._bond_addr
-
-    def get_dev_nr(self) -> int:
-        return self._dev_nr
-
-    @staticmethod
-    def from_dpa(dpa: bytes) -> BondNodeResponse:
-        IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
-        result = None
-        if rcode == ResponseCodes.OK:
-            if len(dpa) != 10:
-                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'bondAddr': dpa[8], 'devNr': dpa[9]}
-        return BondNodeResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE], result=result)
-
-    @staticmethod
-    def from_json(json: dict) -> BondNodeResponse:
-        msgid = Common.msgid_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
-        return BondNodeResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'PulseResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs PulseResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            PulseResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        DpaValidator.response_length(dpa=dpa, expected_len=8)
+        nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'PulseResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs PulseResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            PulseResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
+        return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/bonded_devices.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/flashing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,69 @@
-from __future__ import annotations
-from typeguard import typechecked
-from typing import List, Optional
-from iqrfpy.enums.commands import CoordinatorResponseCommands
-from iqrfpy.enums.message_types import CoordinatorMessages
+"""LEDG Flashing response message."""
+
+from typing import Optional
+from iqrfpy.iresponse import IResponseGetterMixin
+from iqrfpy.enums.commands import LEDResponseCommands
+from iqrfpy.enums.message_types import LEDGMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
-
-__all__ = ['BondedDevicesResponse']
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
 
 
-@typechecked
-class BondedDevicesResponse(IResponseGetterMixin):
-    __slots__ = '_bonded'
+class FlashingResponse(IResponseGetterMixin):
+    """LEDG Flashing response class."""
 
-    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, nadr: int, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
+        """Flashing response constructor.
+
+        Args:
+            nadr (int): Device address.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=DpaConstants.COORDINATOR_NADR,
-            pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.BONDED_DEVICES,
-            m_type=CoordinatorMessages.BONDED_DEVICES,
+            nadr=nadr,
+            pnum=EmbedPeripherals.LEDG,
+            pcmd=LEDResponseCommands.FLASHING,
+            m_type=LEDGMessages.FLASHING,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
-        if rcode == ResponseCodes.OK:
-            self._bonded = result['bondedDevices']
-
-    def get_bonded(self) -> List[int]:
-        return self._bonded
 
-    @staticmethod
-    def from_dpa(dpa: bytes) -> BondedDevicesResponse:
-        IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
-        result = None
-        if rcode == ResponseCodes.OK:
-            if len(dpa) != 40:
-                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'bondedDevices': Common.bitmap_to_nodes(list(dpa[8:]))}
-        return BondedDevicesResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
-                                     result=result)
-
-    @staticmethod
-    def from_json(json: dict) -> BondedDevicesResponse:
-        msgid = Common.msgid_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
-        return BondedDevicesResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'FlashingResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs FlashingResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            FlashingResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        DpaValidator.response_length(dpa=dpa, expected_len=8)
+        nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'FlashingResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs FlashingResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            FlashingResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
+        return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/clear_all_bonds.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/set_off.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,69 @@
-from __future__ import annotations
-from typeguard import typechecked
+"""LEDG Set Off response message."""
+
 from typing import Optional
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.commands import CoordinatorResponseCommands
-from iqrfpy.enums.message_types import CoordinatorMessages
+from iqrfpy.iresponse import IResponseGetterMixin
+from iqrfpy.enums.commands import LEDResponseCommands
+from iqrfpy.enums.message_types import LEDGMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
-
-__all__ = ['ClearAllBondsResponse']
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
 
 
-@typechecked
-class ClearAllBondsResponse(IResponseGetterMixin):
+class SetOffResponse(IResponseGetterMixin):
+    """LEDG Set Off response class."""
 
-    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, nadr: int, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
+        """Set Off response constructor.
+
+        Args:
+            nadr (int): Device address.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=DpaConstants.COORDINATOR_NADR,
-            pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.CLEAR_ALL_BONDS,
-            m_type=CoordinatorMessages.CLEAR_ALL_BONDS,
+            nadr=nadr,
+            pnum=EmbedPeripherals.LEDG,
+            pcmd=LEDResponseCommands.SET_OFF,
+            m_type=LEDGMessages.SET_OFF,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
 
-    @staticmethod
-    def from_dpa(dpa: bytes) -> ClearAllBondsResponse:
-        IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
-        if len(dpa) != 8:
-            raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-        return ClearAllBondsResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
-                                     result=None)
-
-    @staticmethod
-    def from_json(json: dict) -> ClearAllBondsResponse:
-        msgid = Common.msgid_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
-        return ClearAllBondsResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'SetOffResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs SetOffResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            SetOffResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        DpaValidator.response_length(dpa=dpa, expected_len=8)
+        nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'SetOffResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs SetOffResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            SetOffResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
+        return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/discovered_devices.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/eeprom/responses/read.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,88 @@
-from __future__ import annotations
-from typeguard import typechecked
+"""Eeprom Read response message."""
+
 from typing import List, Optional
-from iqrfpy.enums.commands import CoordinatorResponseCommands
-from iqrfpy.enums.message_types import CoordinatorMessages
+from iqrfpy.iresponse import IResponseGetterMixin
+from iqrfpy.enums.commands import EEPROMResponseCommands
+from iqrfpy.enums.message_types import EEPROMMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
-
-__all__ = ['DiscoveredDevicesResponse']
-
-
-@typechecked
-class DiscoveredDevicesResponse(IResponseGetterMixin):
-    __slots__ = '_discovered'
-
-    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
-                 msgid: Optional[str] = None, result: Optional[dict] = None):
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.dpa import ResponseCodes
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
+
+__all__ = ['ReadResponse']
+
+
+class ReadResponse(IResponseGetterMixin):
+    """Eeprom Read response class."""
+
+    __slots__ = ('_data',)
+
+    def __init__(self, nadr: int, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+                 msgid: Optional[str] = None, pdata: Optional[List[int]] = None, result: Optional[dict] = None):
+        """Read response constructor.
+
+        Args:
+            nadr (int): Device address.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            pdata (List[int], optional): DPA response data. Defaults to None.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=DpaConstants.COORDINATOR_NADR,
-            pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.DISCOVERED_DEVICES,
-            m_type=CoordinatorMessages.DISCOVERED_DEVICES,
+            nadr=nadr,
+            pnum=EmbedPeripherals.EEPROM,
+            pcmd=EEPROMResponseCommands.READ,
+            m_type=EEPROMMessages.READ,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
+            pdata=pdata,
             result=result
         )
-        if rcode == ResponseCodes.OK:
-            self._discovered = result['discoveredDevices']
-
-    def get_discovered(self) -> List[int]:
-        return self._discovered
+        self._data = result['pData'] if rcode == ResponseCodes.OK else None
 
-    @staticmethod
-    def from_dpa(dpa: bytes) -> DiscoveredDevicesResponse:
-        IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
+    @property
+    def data(self) -> Optional[List[int]]:
+        """:obj:`list` of :obj:`int` or :obj:`None`: Data read from memory.
+
+        Getter only.
+        """
+        return self._data
+
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'ReadResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs :obj:`ReadResponse` object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            :obj:`ReadResponse`: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        nadr, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
-            if len(dpa) != 40:
-                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'discoveredDevices': Common.bitmap_to_nodes(list(dpa[8:]))}
-        return DiscoveredDevicesResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
-                                         result=result)
-
-    @staticmethod
-    def from_json(json: dict) -> DiscoveredDevicesResponse:
-        msgid = Common.msgid_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
-        return DiscoveredDevicesResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+            pdata = Common.pdata_from_dpa(dpa=dpa)
+            result = {'pData': list(dpa[8:])}
+        return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata, result=result)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'ReadResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs :obj:`ReadResponse` object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            :obj:`ReadResponse`: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, nadr, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
+        return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/discovery.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/remove_bond.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,88 @@
-from __future__ import annotations
-from typeguard import typechecked
-from typing import Optional
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
+"""Coordinator Remove Bond response message."""
+
+from typing import List, Optional
+from iqrfpy.iresponse import IResponseGetterMixin
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
-
-__all__ = ['DiscoveryResponse']
-
-
-@typechecked
-class DiscoveryResponse(IResponseGetterMixin):
-    __slots__ = '_disc_nr'
-
-    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
-                 msgid: Optional[str] = None, result: Optional[dict] = None):
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.dpa import ResponseCodes
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
+
+__all__ = ['RemoveBondResponse']
+
+
+class RemoveBondResponse(IResponseGetterMixin):
+    """Coordinator Remove Bond response class."""
+
+    __slots__ = ('_dev_nr',)
+
+    def __init__(self, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+                 msgid: Optional[str] = None, pdata: Optional[List[int]] = None, result: Optional[dict] = None):
+        """Remove Bond response constructor.
+
+        Args:
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            pdata (List[int], optional): DPA response data. Defaults to None.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=DpaConstants.COORDINATOR_NADR,
+            nadr=dpa_constants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.DISCOVERY,
-            m_type=CoordinatorMessages.DISCOVERY,
+            pcmd=CoordinatorResponseCommands.REMOVE_BOND,
+            m_type=CoordinatorMessages.REMOVE_BOND,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
+            pdata=pdata,
             result=result
         )
-        if rcode == ResponseCodes.OK:
-            self._disc_nr = result['discNr']
-
-    def get_disc_nr(self) -> int:
-        return self._disc_nr
+        self._dev_nr = result['devNr'] if rcode == ResponseCodes.OK else None
 
-    @staticmethod
-    def from_dpa(dpa: bytes) -> DiscoveryResponse:
-        IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
+    @property
+    def dev_nr(self) -> Optional[int]:
+        """:obj:`int` or :obj:`None`: Number of devices in network.
+
+        Getter only.
+        """
+        return self._dev_nr
+
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'RemoveBondResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs RemoveBondResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            RemoveBondResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        _, _, _, hwpid, rcode, dpa_value, pdata = Common.parse_dpa_into_members(dpa=dpa)
         result = None
         if rcode == ResponseCodes.OK:
-            if len(dpa) != 9:
-                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'discNr': dpa[8]}
-        return DiscoveryResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
-                                 result=result)
-
-    @staticmethod
-    def from_json(json: dict) -> DiscoveryResponse:
-        msgid = Common.msgid_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
-        return DiscoveryResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+            DpaValidator.response_length(dpa=dpa, expected_len=9)
+            pdata = Common.pdata_from_dpa(dpa=dpa)
+            result = {'devNr': dpa[8]}
+        return cls(hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, pdata=pdata, result=result)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'RemoveBondResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs RemoveBondResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            RemoveBondResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, _, hwpid, rcode, dpa_value, pdata, result = Common.parse_json_into_members(json=json)
+        return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, pdata=pdata, result=result)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/remove_bond.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/restore.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,72 @@
-from __future__ import annotations
-from typeguard import typechecked
-from typing import Optional
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
+"""Coordinator Restore response message."""
+
+from typing import List, Optional
+from iqrfpy.iresponse import IResponseGetterMixin
 from iqrfpy.enums.commands import CoordinatorResponseCommands
 from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
 
-__all__ = ['RemoveBondResponse']
+__all__ = ['RestoreResponse']
 
 
-@typechecked
-class RemoveBondResponse(IResponseGetterMixin):
-    __slots__ = '_dev_nr'
+class RestoreResponse(IResponseGetterMixin):
+    """Coordinator Restore response class."""
 
-    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
-                 msgid: Optional[str] = None, result: Optional[dict] = None):
+    def __init__(self, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+                 msgid: Optional[str] = None, pdata: Optional[List[int]] = None, result: Optional[dict] = None):
+        """Restore response constructor.
+
+        Args:
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            pdata (List[int], optional): DPA response data. Defaults to None.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=DpaConstants.COORDINATOR_NADR,
+            nadr=dpa_constants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.REMOVE_BOND,
-            m_type=CoordinatorMessages.REMOVE_BOND,
+            pcmd=CoordinatorResponseCommands.RESTORE,
+            m_type=CoordinatorMessages.RESTORE,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
+            pdata=pdata,
             result=result
         )
-        if rcode == ResponseCodes.OK:
-            self._dev_nr = result['devNr']
-
-    def get_dev_nr(self) -> int:
-        return self._dev_nr
 
-    @staticmethod
-    def from_dpa(dpa: bytes) -> RemoveBondResponse:
-        IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
-        result = None
-        if rcode == ResponseCodes.OK:
-            if len(dpa) != 9:
-                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'devNr': dpa[8]}
-        return RemoveBondResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
-                                  result=result)
-
-    @staticmethod
-    def from_json(json: dict) -> RemoveBondResponse:
-        msgid = Common.msgid_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
-        return RemoveBondResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'RestoreResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs RestoreResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            RestoreResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        DpaValidator.response_length(dpa=dpa, expected_len=8)
+        _, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'RestoreResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs RestoreResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            RestoreResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, _, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
+        return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/restore.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/remove_bond.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,71 @@
-from __future__ import annotations
-from typeguard import typechecked
+"""Node Remove Bond response message."""
+
 from typing import Optional
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.commands import CoordinatorResponseCommands
-from iqrfpy.enums.message_types import CoordinatorMessages
+from iqrfpy.iresponse import IResponseGetterMixin
+from iqrfpy.enums.commands import NodeResponseCommands
+from iqrfpy.enums.message_types import NodeMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponsePacketMembers
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
 
-__all__ = ['RestoreResponse']
+__all__ = ['RemoveBondResponse']
 
 
-@typechecked
-class RestoreResponse(IResponseGetterMixin):
+class RemoveBondResponse(IResponseGetterMixin):
+    """Node Remove response class."""
 
-    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, nadr: int, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
+        """Remove Bond response constructor.
+
+        Args:
+            nadr (int): Device address.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=DpaConstants.COORDINATOR_NADR,
-            pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.RESTORE,
-            m_type=CoordinatorMessages.RESTORE,
+            nadr=nadr,
+            pnum=EmbedPeripherals.NODE,
+            pcmd=NodeResponseCommands.REMOVE_BOND,
+            m_type=NodeMessages.REMOVE_BOND,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
 
-    @staticmethod
-    def from_dpa(dpa: bytes) -> RestoreResponse:
-        IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
-        if len(dpa) != 8:
-            raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-        return RestoreResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE], result=None)
-
-    @staticmethod
-    def from_json(json: dict) -> RestoreResponse:
-        msgid = Common.msgid_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        return RestoreResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=None)
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'RemoveBondResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs RemoveBondResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            RemoveBondResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        DpaValidator.response_length(dpa=dpa, expected_len=8)
+        nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'RemoveBondResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs RemoveBondResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            RemoveBondResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
+        return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/set_dpa_params.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/io/responses/direction.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,73 @@
-from __future__ import annotations
-from typeguard import typechecked
-from typing import Optional
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
-from iqrfpy.messages.requests.coordinator.set_dpa_params import DpaParam
-from iqrfpy.enums.commands import CoordinatorResponseCommands
-from iqrfpy.enums.message_types import CoordinatorMessages
+"""IO Direction response message."""
+
+from typing import List, Optional
+from iqrfpy.iresponse import IResponseGetterMixin
+from iqrfpy.enums.commands import IOResponseCommands
+from iqrfpy.enums.message_types import IOMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
 
-__all__ = ['SetDpaParamsResponse']
+__all__ = ['DirectionResponse']
 
 
-@typechecked
-class SetDpaParamsResponse(IResponseGetterMixin):
-    __slots__ = '_dpa_param'
+class DirectionResponse(IResponseGetterMixin):
+    """IO Direction response class."""
 
-    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
-                 msgid: Optional[str] = None, result: Optional[dict] = None):
+    def __init__(self, nadr: int, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+                 msgid: Optional[str] = None, pdata: Optional[List[int]] = None, result: Optional[dict] = None):
+        """Direction response constructor.
+
+        Args:
+            nadr (int): Device address.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            pdata (List[int], optional): DPA response data. Defaults to None.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=DpaConstants.COORDINATOR_NADR,
-            pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.SET_DPA_PARAMS,
-            m_type=CoordinatorMessages.SET_DPA_PARAMS,
+            nadr=nadr,
+            pnum=EmbedPeripherals.IO,
+            pcmd=IOResponseCommands.DIRECTION,
+            m_type=IOMessages.DIRECTION,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
+            pdata=pdata,
             result=result
         )
-        if rcode == ResponseCodes.OK:
-            self._dpa_param: DpaParam = DpaParam(result['prevDpaParam'])
-
-    def get_dpa_param(self) -> DpaParam:
-        return self._dpa_param
 
-    @staticmethod
-    def from_dpa(dpa: bytes) -> SetDpaParamsResponse:
-        IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
-        result = None
-        if rcode == ResponseCodes.OK:
-            if len(dpa) != 9:
-                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'prevDpaParam': dpa[8]}
-        return SetDpaParamsResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
-                                    result=result)
-
-    @staticmethod
-    def from_json(json: dict) -> SetDpaParamsResponse:
-        msgid = Common.msgid_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
-        return SetDpaParamsResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'DirectionResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs DirectionResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            DirectionResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        DpaValidator.response_length(dpa=dpa, expected_len=8)
+        nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'DirectionResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs DirectionResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            DirectionResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
+        return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/set_hops.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/node/responses/restore.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,73 @@
-from __future__ import annotations
-from typeguard import typechecked
-from typing import Optional
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.commands import CoordinatorResponseCommands
-from iqrfpy.enums.message_types import CoordinatorMessages
+"""Node Restore response message."""
+
+from typing import List, Optional
+from iqrfpy.iresponse import IResponseGetterMixin
+from iqrfpy.enums.commands import NodeResponseCommands
+from iqrfpy.enums.message_types import NodeMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
 
-__all__ = ['SetHopsResponse']
+__all__ = ['RestoreResponse']
 
 
-@typechecked
-class SetHopsResponse(IResponseGetterMixin):
-    __slots__ = '_request_hops', '_response_hops'
+class RestoreResponse(IResponseGetterMixin):
+    """Node Restore response class."""
 
-    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
-                 msgid: Optional[str] = None, result: Optional[dict] = None):
+    def __init__(self, nadr: int, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+                 msgid: Optional[str] = None, pdata: Optional[List[int]] = None, result: Optional[dict] = None):
+        """Restore response constructor.
+
+        Args:
+            nadr (int): Device address.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            pdata (List[int], optional): DPA response data. Defaults to None.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=DpaConstants.COORDINATOR_NADR,
-            pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.SET_HOPS,
-            m_type=CoordinatorMessages.SET_HOPS,
+            nadr=nadr,
+            pnum=EmbedPeripherals.NODE,
+            pcmd=NodeResponseCommands.RESTORE,
+            m_type=NodeMessages.RESTORE,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
+            pdata=pdata,
             result=result
         )
-        if rcode == ResponseCodes.OK:
-            self._request_hops = result['requestHops']
-            self._response_hops = result['responseHops']
-
-    def get_request_hops(self) -> int:
-        return self._request_hops
-
-    def get_response_hops(self) -> int:
-        return self._response_hops
-
-    @staticmethod
-    def from_dpa(dpa: bytes) -> SetHopsResponse:
-        IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
-        result = None
-        if rcode == ResponseCodes.OK:
-            if len(dpa) != 10:
-                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'requestHops': dpa[8], 'responseHops': dpa[9]}
-        return SetHopsResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE], result=result)
-
-    @staticmethod
-    def from_json(json: dict) -> SetHopsResponse:
-        msgid = Common.msgid_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
-        return SetHopsResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'RestoreResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs RestoreResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            RestoreResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        DpaValidator.response_length(dpa=dpa, expected_len=8)
+        nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'RestoreResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs RestoreResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            RestoreResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
+        return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/set_mid.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/ledg/responses/set_on.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,69 @@
-from __future__ import annotations
-from typeguard import typechecked
+"""LEDG Set On response message."""
+
 from typing import Optional
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.commands import CoordinatorResponseCommands
-from iqrfpy.enums.message_types import CoordinatorMessages
+from iqrfpy.iresponse import IResponseGetterMixin
+from iqrfpy.enums.commands import LEDResponseCommands
+from iqrfpy.enums.message_types import LEDGMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponsePacketMembers
-
-__all__ = ['SetMIDResponse']
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
 
 
-@typechecked
-class SetMIDResponse(IResponseGetterMixin):
+class SetOnResponse(IResponseGetterMixin):
+    """LEDG Set On response class."""
 
-    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, nadr: int, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
+        """Set On response constructor.
+
+        Args:
+            nadr (int): Device address.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=DpaConstants.COORDINATOR_NADR,
-            pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.SET_MID,
-            m_type=CoordinatorMessages.SET_MID,
+            nadr=nadr,
+            pnum=EmbedPeripherals.LEDG,
+            pcmd=LEDResponseCommands.SET_ON,
+            m_type=LEDGMessages.SET_ON,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
 
-    @staticmethod
-    def from_dpa(dpa: bytes) -> SetMIDResponse:
-        IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
-        if len(dpa) != 8:
-            raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-        return SetMIDResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE], result=None)
-
-    @staticmethod
-    def from_json(json: dict) -> SetMIDResponse:
-        msgid = Common.msgid_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        return SetMIDResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=None)
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'SetOnResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs SetOnResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            SetOnResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        DpaValidator.response_length(dpa=dpa, expected_len=8)
+        nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'SetOnResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs SetOnResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            SetOnResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
+        return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/coordinator/smart_connect.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/pulse.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,69 @@
-from __future__ import annotations
-from typeguard import typechecked
+"""LEDR Pulse response message."""
+
 from typing import Optional
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.commands import CoordinatorResponseCommands
-from iqrfpy.enums.message_types import CoordinatorMessages
+from iqrfpy.iresponse import IResponseGetterMixin
+from iqrfpy.enums.commands import LEDResponseCommands
+from iqrfpy.enums.message_types import LEDRMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
-
-__all__ = ['SmartConnectResponse']
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
 
 
-@typechecked
-class SmartConnectResponse(IResponseGetterMixin):
-    __slots__ = '_bond_addr', '_dev_nr'
+class PulseResponse(IResponseGetterMixin):
+    """LEDR Pulse response class."""
 
-    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, nadr: int, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
+        """Pulse response constructor.
+
+        Args:
+            nadr (int): Device address.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=DpaConstants.COORDINATOR_NADR,
-            pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.SMART_CONNECT,
-            m_type=CoordinatorMessages.SMART_CONNECT,
+            nadr=nadr,
+            pnum=EmbedPeripherals.LEDR,
+            pcmd=LEDResponseCommands.PULSE,
+            m_type=LEDRMessages.PULSE,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
-        if rcode == ResponseCodes.OK:
-            self._bond_addr = result['bondAddr']
-            self._dev_nr = result['devNr']
-
-    def get_bond_addr(self) -> int:
-        return self._bond_addr
-
-    def get_dev_nr(self) -> int:
-        return self._dev_nr
-
-    @staticmethod
-    def from_dpa(dpa: bytes) -> SmartConnectResponse:
-        IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
-        result = None
-        if rcode == ResponseCodes.OK:
-            if len(dpa) != 10:
-                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'bondAddr': dpa[8], 'devNr': dpa[9]}
-        return SmartConnectResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
-                                    result=result)
-
-    @staticmethod
-    def from_json(json: dict) -> SmartConnectResponse:
-        msgid = Common.msgid_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
-        return SmartConnectResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'PulseResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs PulseResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            PulseResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        DpaValidator.response_length(dpa=dpa, expected_len=8)
+        nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'PulseResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs PulseResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            PulseResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
+        return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/ledr/flashing.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/ledr/responses/flashing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,69 @@
-from __future__ import annotations
-from typeguard import typechecked
+"""LEDR Flashing response message."""
+
 from typing import Optional
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
+from iqrfpy.iresponse import IResponseGetterMixin
 from iqrfpy.enums.commands import LEDResponseCommands
 from iqrfpy.enums.message_types import LEDRMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponsePacketMembers
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
 
 
-@typechecked
 class FlashingResponse(IResponseGetterMixin):
+    """LEDR Flashing response class."""
 
-    def __init__(self, nadr: int, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, nadr: int, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
+        """Flashing response constructor.
+
+        Args:
+            nadr (int): Device address.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
             nadr=nadr,
             pnum=EmbedPeripherals.LEDR,
             pcmd=LEDResponseCommands.FLASHING,
             m_type=LEDRMessages.FLASHING,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
 
-    @staticmethod
-    def from_dpa(dpa: bytes) -> FlashingResponse:
-        IResponse.validate_dpa_response(dpa)
-        nadr = dpa[ResponsePacketMembers.NADR]
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
-        if len(dpa) != 8:
-            raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-        return FlashingResponse(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
-                                result=None)
-
-    @staticmethod
-    def from_json(json: dict) -> FlashingResponse:
-        msgid = Common.msgid_from_json(json)
-        nadr = Common.nadr_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        return FlashingResponse(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=None)
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'FlashingResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs FlashingResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            FlashingResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        DpaValidator.response_length(dpa=dpa, expected_len=8)
+        nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'FlashingResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs FlashingResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            FlashingResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
+        return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/ledr/pulse.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/os/responses/reset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,73 @@
-from __future__ import annotations
-from typeguard import typechecked
+"""OS Reset response message."""
+
 from typing import Optional
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.commands import LEDResponseCommands
-from iqrfpy.enums.message_types import LEDRMessages
+from iqrfpy.iresponse import IResponseGetterMixin
+from iqrfpy.enums.commands import OSResponseCommands
+from iqrfpy.enums.message_types import OSMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponsePacketMembers
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
+
+__all__ = [
+    'ResetResponse'
+]
 
 
-@typechecked
-class PulseResponse(IResponseGetterMixin):
+class ResetResponse(IResponseGetterMixin):
+    """OS Reset response class."""
 
-    def __init__(self, nadr: int, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, nadr: int, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
+        """Reset response constructor.
+
+        Args:
+            nadr (int): Device address.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
             nadr=nadr,
-            pnum=EmbedPeripherals.LEDR,
-            pcmd=LEDResponseCommands.PULSE,
-            m_type=LEDRMessages.PULSE,
+            pnum=EmbedPeripherals.OS,
+            pcmd=OSResponseCommands.RESET,
+            m_type=OSMessages.RESET,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
 
-    @staticmethod
-    def from_dpa(dpa: bytes) -> PulseResponse:
-        IResponse.validate_dpa_response(dpa)
-        nadr = dpa[ResponsePacketMembers.NADR]
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
-        if len(dpa) != 8:
-            raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-        return PulseResponse(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
-                             result=None)
-
-    @staticmethod
-    def from_json(json: dict) -> PulseResponse:
-        msgid = Common.msgid_from_json(json)
-        nadr = Common.nadr_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        return PulseResponse(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=None)
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'ResetResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs :obj:`ResetResponse` object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            :obj:`ResetResponse`: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        DpaValidator.response_length(dpa=dpa, expected_len=8)
+        nadr, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'ResetResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs :obj:`ResetResponse` object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            :obj:`ResetResponse`: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, nadr, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
+        return cls(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/messages/responses/ledr/set_on.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/coordinator/responses/set_mid.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,70 @@
-from __future__ import annotations
-from typeguard import typechecked
+"""Coordinator Set MID response message."""
+
 from typing import Optional
-from iqrfpy.messages.responses.iresponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.commands import LEDResponseCommands
-from iqrfpy.enums.message_types import LEDRMessages
+from iqrfpy.iresponse import IResponseGetterMixin
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-import iqrfpy.utils.dpa as DpaConstants
-from iqrfpy.utils.dpa import ResponsePacketMembers
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.validators import DpaValidator, JsonValidator
+
+__all__ = ['SetMidResponse']
 
 
-@typechecked
-class SetOnResponse(IResponseGetterMixin):
+class SetMidResponse(IResponseGetterMixin):
+    """Coordinator Set MID response class."""
 
-    def __init__(self, nadr: int, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, hwpid: int = dpa_constants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
+        """SetMID response constructor.
+
+        Args:
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535, this value ignores HWPID check.
+            rcode (int, optional): Response code. Defaults to 128.
+            dpa_value (int, optional): DPA value. Defaults to 0.
+            msgid (str, optional): Message ID. Defaults to None.
+            result (dict, optional): JSON response data. Defaults to None.
+        """
         super().__init__(
-            nadr=nadr,
-            pnum=EmbedPeripherals.LEDR,
-            pcmd=LEDResponseCommands.SET_ON,
-            m_type=LEDRMessages.SET_ON,
+            nadr=dpa_constants.COORDINATOR_NADR,
+            pnum=EmbedPeripherals.COORDINATOR,
+            pcmd=CoordinatorResponseCommands.SET_MID,
+            m_type=CoordinatorMessages.SET_MID,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
 
-    @staticmethod
-    def from_dpa(dpa: bytes) -> SetOnResponse:
-        IResponse.validate_dpa_response(dpa)
-        nadr = dpa[ResponsePacketMembers.NADR]
-        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
-        rcode = dpa[ResponsePacketMembers.RCODE]
-        if len(dpa) != 8:
-            raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-        return SetOnResponse(nadr=nadr, hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
-                             result=None)
-
-    @staticmethod
-    def from_json(json: dict) -> SetOnResponse:
-        msgid = Common.msgid_from_json(json)
-        nadr = Common.nadr_from_json(json)
-        hwpid = Common.hwpid_from_json(json)
-        dpa_value = Common.dpa_value_from_json(json)
-        rcode = Common.rcode_from_json(json)
-        return SetOnResponse(nadr=nadr, msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=None)
+    @classmethod
+    def from_dpa(cls, dpa: bytes) -> 'SetMidResponse':
+        """DPA response factory method.
+
+        Parses DPA data and constructs SetMidResponse object.
+
+        Args:
+            dpa (bytes): DPA response bytes.
+        Returns:
+            SetMidResponse: Response message object.
+        """
+        DpaValidator.base_response_length(dpa=dpa)
+        DpaValidator.response_length(dpa=dpa, expected_len=8)
+        _, _, _, hwpid, rcode, dpa_value, _ = Common.parse_dpa_into_members(dpa=dpa)
+        return cls(hwpid=hwpid, rcode=rcode, dpa_value=dpa_value)
+
+    @classmethod
+    def from_json(cls, json: dict) -> 'SetMidResponse':
+        """JSON response factory method.
+
+        Parses JSON API response and constructs SetMidResponse object.
+
+        Args:
+            json (dict): JSON API response.
+        Returns:
+            SetMidResponse: Response message object.
+        """
+        JsonValidator.response_received(json=json)
+        msgid, _, hwpid, rcode, dpa_value, _, _ = Common.parse_json_into_members(json=json, omit_result=True)
+        return cls(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode)
```

### Comparing `iqrfpy-0.1.9/iqrfpy/transports/mqtt_transport.py` & `iqrfpy-0.2.0/iqrfpy/peripherals/ram/requests/read.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,132 @@
-from dataclasses import dataclass
-import json
-import random
-import string
-import threading
-
-from typing import Callable, Optional
-from typeguard import typechecked
-from paho.mqtt.client import Client
-from iqrfpy.exceptions import TransportNotConnectedError, MessageNotReceivedError
-from iqrfpy.messages.requests.irequest import IRequest
-from iqrfpy.messages.responses.confirmation import Confirmation
-from iqrfpy.messages.responses.iresponse import IResponse
-from iqrfpy.messages.response_factory import ResponseFactory
-from iqrfpy.transports.itransport import ITransport
-
-__all__ = (
-    'MqttTransportParams'
-    'MqttTransport'
-)
-
-
-@dataclass
-@typechecked
-class MqttTransportParams:
-    host: str = 'localhost'
-    port: int = 1883
-    client_id: str = ''.join(random.choice(string.ascii_letters + string.digits) for i in range(16))
-    user: str = None
-    password: str = None
-    request_topic: str = None
-    response_topic: str = None
-    qos: int = 1
-    keepalive: int = 60
-
-    def __post_init__(self):
-        if not (1024 <= self.port <= 65535):
-            raise MqttParamsError('Port value should be between 1024 and 65535.')
-        if (self.user is not None and self.password is None) or (self.user is None and self.password is not None):
-            raise MqttParamsError('Both user and password parameters need to be specified, or neither of them.')
-        if not (0 <= self.qos <= 2):
-            raise MqttParamsError('QoS value should be between 0 and 2.')
-
-
-class MqttTransport(ITransport):
-
-    __slots__ = '_client', '_params', '_callback', '_sync', '_timeout', '_cv'
-
-    def __init__(self, params: MqttTransportParams, synchronous: bool = False, callback: Optional[Callable] = None,
-                 auto_init: bool = False, timeout: Optional[int] = 5):
-        self._client: Optional[Client] = None
-        self._params: MqttTransportParams = params
-        self._sync: bool = synchronous
-        self._callback: Optional[Callable] = callback
-        self._timeout: int = timeout
-        self._msg_id: Optional[str] = None
-        self._cv: threading.Condition = threading.Condition()
-        self._response: Optional[IResponse] = None
-        if auto_init:
-            self.initialize()
-
-    def initialize(self) -> None:
-        self._client = Client(self._params.client_id)
-        self._client.on_connect = self._connect_callback
-        self._client.on_message = self._message_callback
-        if self._params.user is not None and self._params.password is not None:
-            self._client.username_pw_set(self._params.user, self._params.password)
-        self._client.connect(self._params.host, self._params.port)
-        if self._sync:
-            self._client.loop_start()
-        else:
-            self._client.loop_forever()
-
-    def _connect_callback(self, client, userdata, flags, rc):
-        # pylint: disable=W0613
-        if rc == 0:
-            self._client.subscribe(self._params.response_topic, self._params.qos)
-
-    def _message_callback(self, client, userdata, message):
-        # pylint: disable=W0613
-        payload = json.loads(message.payload.decode('utf-8'))
-        response = ResponseFactory.get_response_from_json(payload)
-        if not self._sync:
-            if self._callback is not None:
-                self._callback(response)
-            return
-        if response.get_msgid() == self._msg_id:
-            self._response = response
-            with self._cv:
-                self._cv.notify()
-
-    def send(self, request: IRequest) -> None:
-        if self._client.is_connected():
-            self._client.publish(
-                topic=self._params.request_topic,
-                payload=json.dumps(request.to_json()),
-                qos=self._params.qos
-            )
-
-    def send_and_receive(self, request: IRequest, timeout: Optional[int] = None) -> IResponse:
-        self._response = None
-        self._msg_id = None
-        if not self._client.is_connected():
-            raise TransportNotConnectedError(f'MQTT client {self._params.client_id} not connected to broker.')
-        self._client.publish(
-            topic=self._params.request_topic,
-            payload=json.dumps(request.to_json()),
-            qos=self._params.qos
-        )
-        self._msg_id = request.get_msg_id()
-        timeout_to_use = timeout if timeout is not None else self._timeout
-        with self._cv:
-            self._cv.wait(timeout=timeout_to_use)
-        if self._response is None:
-            raise MessageNotReceivedError(f'Response message to request with ID {self._msg_id} not received within the'
-                                          f' specified time of {timeout_to_use} seconds.')
-        return self._response
-
-    def receive(self) -> IResponse:
-        pass
-
-    def confirmation(self) -> Confirmation:
-        raise NotImplementedError('Method not implemented.')
+"""RAM Read request message."""
 
-    def set_receive_callback(self, callback: Callable[[IResponse], None]) -> None:
-        self._callback = callback
+from typing import Optional, Union
+from iqrfpy.enums.commands import RAMRequestCommands
+from iqrfpy.enums.message_types import RAMMessages
+from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import RequestParameterInvalidValueError
+import iqrfpy.utils.dpa as dpa_constants
+from iqrfpy.utils.common import Common
+from iqrfpy.irequest import IRequest
+
+__all__ = ['ReadRequest']
+
+
+class ReadRequest(IRequest):
+    """RAM Read request class."""
+
+    __slots__ = '_address', '_length'
+
+    def __init__(self, nadr: int, address: int, length: int, hwpid: int = dpa_constants.HWPID_MAX,
+                 dpa_rsp_time: Optional[float] = None, dev_process_time: Optional[float] = None,
+                 msgid: Optional[str] = None):
+        """Read request constructor.
+
+        Args:
+            nadr (int): Device address.
+            address (int): Memory address to read from.
+            length (int): Number of bytes to read from memory.
+            hwpid (int, optional): Hardware profile ID. Defaults to 65535 (Ignore HWPID check).
+            dpa_rsp_time (float, optional): DPA request timeout in seconds. Defaults to None.
+            dev_process_time (float, optional): Device processing time. Defaults to None.
+            msgid (str, optional): JSON API message ID. Defaults to None. If the parameter is not specified, a random
+                UUIDv4 string is generated and used.
+        """
+        self._validate(address, length)
+        super().__init__(
+            nadr=nadr,
+            pnum=EmbedPeripherals.RAM,
+            pcmd=RAMRequestCommands.READ,
+            m_type=RAMMessages.READ,
+            hwpid=hwpid,
+            dpa_rsp_time=dpa_rsp_time,
+            dev_process_time=dev_process_time,
+            msgid=msgid
+        )
+        self._address = address
+        self._length = length
 
+    def _validate(self, address: int, length: int) -> None:
+        """Validate request parameters.
 
-class MqttParamsError(Exception):
-    pass
+        Args:
+            address (int): Memory address to read from.
+            length (int): Number of bytes to read from memory.
+        """
+        self._validate_address(address)
+        self._validate_length(length)
+
+    @staticmethod
+    def _validate_address(address: int):
+        """Validates memory address parameter.
+
+        Args:
+            address (int): Memory address to read from.
+        Raises:
+            RequestParameterInvalidValueError: If address is less than 0 or greater than 255.
+        """
+        if not dpa_constants.BYTE_MIN <= address <= dpa_constants.BYTE_MAX:
+            raise RequestParameterInvalidValueError('Address should be between 0 and 255')
+
+    @property
+    def address(self) -> int:
+        """:obj:`int`: Memory address to read from.
+
+        Getter and setter.
+        """
+        return self._address
+
+    @address.setter
+    def address(self, value: int) -> None:
+        self._validate_address(address=value)
+        self._address = value
+
+    @staticmethod
+    def _validate_length(length: int):
+        """Validates data length parameter.
+
+        Args:
+            length (int): Number of bytes to read from memory.
+        Raises:
+            RequestParameterInvalidValueError: If length is less than 0 or greater than 255.
+        """
+        if not dpa_constants.BYTE_MIN <= length <= dpa_constants.BYTE_MAX:
+            raise RequestParameterInvalidValueError('Length should be between 0 and 255.')
+
+    @property
+    def length(self) -> int:
+        """:obj:`int`: Number of bytes to read from memory.
+
+        Getter and setter.
+        """
+        return self._length
+
+    @length.setter
+    def length(self, value: int) -> None:
+        self._validate_length(length=value)
+        self._length = value
+
+    def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
+        """DPA request serialization method.
+
+        Args:
+            mutable (bool, optional): Serialize into mutable byte representation of DPA request packet.
+                Defaults to False.
+
+        Returns:
+            :obj:`bytes`: Immutable byte representation of DPA request packet.\n
+            :obj:`bytearray`: Mutable byte representation of DPA request packet (if argument mutable is True).
+        """
+        self._pdata = [self._address, self._length]
+        return Common.serialize_to_dpa(nadr=self._nadr, pnum=self._pnum, pcmd=self._pcmd, hwpid=self._hwpid,
+                                       pdata=self._pdata, mutable=mutable)
+
+    def to_json(self) -> dict:
+        """JSON API request serialization method.
+
+        Returns:
+            :obj:`dict`: JSON API request object.
+        """
+        self._params = {'address': self._address, 'len': self._length}
+        return Common.serialize_to_json(mtype=self._mtype, msgid=self._msgid, nadr=self._nadr, hwpid=self._hwpid,
+                                        params=self._params, dpa_rsp_time=self._dpa_rsp_time)
```

