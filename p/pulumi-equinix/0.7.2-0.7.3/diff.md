# Comparing `tmp/pulumi_equinix-0.7.2.tar.gz` & `tmp/pulumi_equinix-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_equinix-0.7.2.tar", last modified: Wed Mar  6 21:20:33 2024, max compression
+gzip compressed data, was "pulumi_equinix-0.7.3.tar", last modified: Tue Apr  2 21:30:08 2024, max compression
```

## Comparing `pulumi_equinix-0.7.2.tar` & `pulumi_equinix-0.7.3.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:20:33.168075 pulumi_equinix-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-03-06 21:20:33.168075 pulumi_equinix-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:20:33.152075 pulumi_equinix-0.7.2/pulumi_equinix/
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:20:33.152075 pulumi_equinix-0.7.2/pulumi_equinix/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:20:33.156075 pulumi_equinix-0.7.2/pulumi_equinix/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)   234933 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    41365 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/cloud_router.py
--rw-r--r--   0 runner    (1001) docker     (127)    41755 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_cloud_router.py
--rw-r--r--   0 runner    (1001) docker     (127)    11922 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_routing_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    12844 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_service_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_service_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    25175 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/network.py
--rw-r--r--   0 runner    (1001) docker     (127)   448415 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    37312 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/routing_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    49242 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/fabric/service_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:20:33.168075 pulumi_equinix-0.7.2/pulumi_equinix/metal/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    43853 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/bgp_session.py
--rw-r--r--   0 runner    (1001) docker     (127)   116196 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/device_network_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    17219 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_device_bgp_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_facility.py
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_hardware_reservation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_interconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_ip_block_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_metro.py
--rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_operating_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)    10395 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_port.py
--rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_precreated_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     7580 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_project_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_reserved_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_spot_market_price.py
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_spot_market_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8710 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/get_vrf.py
--rw-r--r--   0 runner    (1001) docker     (127)    46971 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/interconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20819 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/ip_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    17973 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    22562 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/organization_member.py
--rw-r--r--   0 runner    (1001) docker     (127)    74180 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27669 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/port.py
--rw-r--r--   0 runner    (1001) docker     (127)    20188 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/port_vlan_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    22739 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/project_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/project_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    48263 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/reserved_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    29655 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/spot_market_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/user_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    42418 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    17551 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)    18196 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/metal/vrf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:20:33.168075 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    68241 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25570 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/acl_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    23204 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)   104590 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    22431 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/device_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/get_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    26748 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/get_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/get_device_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/get_device_software.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/get_device_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    23223 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/network_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    97627 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14424 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/networkedge/ssh_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/pulumi_equinix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:20:33.152075 pulumi_equinix-0.7.2/pulumi_equinix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-03-06 21:20:33.000000 pulumi_equinix-0.7.2/pulumi_equinix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-03-06 21:20:33.000000 pulumi_equinix-0.7.2/pulumi_equinix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 21:20:33.000000 pulumi_equinix-0.7.2/pulumi_equinix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 21:20:33.000000 pulumi_equinix-0.7.2/pulumi_equinix.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-06 21:20:33.000000 pulumi_equinix-0.7.2/pulumi_equinix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-06 21:20:33.000000 pulumi_equinix-0.7.2/pulumi_equinix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 21:20:33.168075 pulumi_equinix-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-03-06 21:20:32.000000 pulumi_equinix-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:30:08.036569 pulumi_equinix-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-02 21:30:08.036569 pulumi_equinix-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:30:08.024569 pulumi_equinix-0.7.3/pulumi_equinix/
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:30:08.024569 pulumi_equinix-0.7.3/pulumi_equinix/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:30:08.028570 pulumi_equinix-0.7.3/pulumi_equinix/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)   234701 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41365 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/cloud_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41755 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_cloud_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12062 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_routing_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_service_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_service_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25331 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)   448327 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37312 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/routing_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49242 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/fabric/service_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:30:08.036569 pulumi_equinix-0.7.3/pulumi_equinix/metal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43853 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/bgp_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116162 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/device_network_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17499 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_device_bgp_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_facility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_hardware_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_interconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_ip_block_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_metro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_precreated_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_project_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_reserved_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_spot_market_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8899 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/get_vrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51542 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/interconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20819 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/ip_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17879 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22528 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/organization_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74121 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27669 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20188 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/port_vlan_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22695 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/project_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/project_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48229 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/reserved_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29621 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/user_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42384 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17497 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18162 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/metal/vrf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:30:08.036569 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68241 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25536 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/acl_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23170 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104546 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22397 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/device_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26888 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/get_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/get_device_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/get_device_software.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/get_device_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23179 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/network_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97627 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/networkedge/ssh_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/pulumi_equinix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:30:08.024569 pulumi_equinix-0.7.3/pulumi_equinix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-02 21:30:08.000000 pulumi_equinix-0.7.3/pulumi_equinix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-02 21:30:08.000000 pulumi_equinix-0.7.3/pulumi_equinix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:30:08.000000 pulumi_equinix-0.7.3/pulumi_equinix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:30:08.000000 pulumi_equinix-0.7.3/pulumi_equinix.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 21:30:08.000000 pulumi_equinix-0.7.3/pulumi_equinix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 21:30:08.000000 pulumi_equinix-0.7.3/pulumi_equinix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 21:30:08.036569 pulumi_equinix-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-02 21:30:07.000000 pulumi_equinix-0.7.3/setup.py
```

### Comparing `pulumi_equinix-0.7.2/PKG-INFO` & `pulumi_equinix-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_equinix
-Version: 0.7.2
+Version: 0.7.3
 Summary: A Pulumi package for creating and managing equinix cloud resources.
 Home-page: https://deploy.equinix.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/equinix/pulumi-equinix
 Keywords: pulumi equinix category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_equinix-0.7.2/README.md` & `pulumi_equinix-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/__init__.py` & `pulumi_equinix-0.7.3/pulumi_equinix/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/_enums.py` & `pulumi_equinix-0.7.3/pulumi_equinix/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/_utilities.py` & `pulumi_equinix-0.7.3/pulumi_equinix/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/config/vars.py` & `pulumi_equinix-0.7.3/pulumi_equinix/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/__init__.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/_enums.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/_inputs.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1294,28 +1294,28 @@
 
 
 @pulumi.input_type
 class ConnectionASideAccessPointPortArgs:
     def __init__(__self__, *,
                  href: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 redundancies: Optional[pulumi.Input[Sequence[pulumi.Input['ConnectionASideAccessPointPortRedundancyArgs']]]] = None,
+                 redundancy: Optional[pulumi.Input['ConnectionASideAccessPointPortRedundancyArgs']] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] href: Unique Resource Identifier
         :param pulumi.Input[str] name: Port name
-        :param pulumi.Input[Sequence[pulumi.Input['ConnectionASideAccessPointPortRedundancyArgs']]] redundancies: Redundancy Information
+        :param pulumi.Input['ConnectionASideAccessPointPortRedundancyArgs'] redundancy: Redundancy Information
         :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if redundancies is not None:
-            pulumi.set(__self__, "redundancies", redundancies)
+        if redundancy is not None:
+            pulumi.set(__self__, "redundancy", redundancy)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def href(self) -> Optional[pulumi.Input[str]]:
         """
@@ -1337,23 +1337,23 @@
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def redundancies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ConnectionASideAccessPointPortRedundancyArgs']]]]:
+    def redundancy(self) -> Optional[pulumi.Input['ConnectionASideAccessPointPortRedundancyArgs']]:
         """
         Redundancy Information
         """
-        return pulumi.get(self, "redundancies")
+        return pulumi.get(self, "redundancy")
 
-    @redundancies.setter
-    def redundancies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ConnectionASideAccessPointPortRedundancyArgs']]]]):
-        pulumi.set(self, "redundancies", value)
+    @redundancy.setter
+    def redundancy(self, value: Optional[pulumi.Input['ConnectionASideAccessPointPortRedundancyArgs']]):
+        pulumi.set(self, "redundancy", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
         Equinix-assigned virtual gateway identifier
         """
@@ -3231,28 +3231,28 @@
 
 
 @pulumi.input_type
 class ConnectionZSideAccessPointPortArgs:
     def __init__(__self__, *,
                  href: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 redundancies: Optional[pulumi.Input[Sequence[pulumi.Input['ConnectionZSideAccessPointPortRedundancyArgs']]]] = None,
+                 redundancy: Optional[pulumi.Input['ConnectionZSideAccessPointPortRedundancyArgs']] = None,
                  uuid: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] href: Unique Resource Identifier
         :param pulumi.Input[str] name: Port name
-        :param pulumi.Input[Sequence[pulumi.Input['ConnectionZSideAccessPointPortRedundancyArgs']]] redundancies: Redundancy Information
+        :param pulumi.Input['ConnectionZSideAccessPointPortRedundancyArgs'] redundancy: Redundancy Information
         :param pulumi.Input[str] uuid: Equinix-assigned virtual gateway identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if redundancies is not None:
-            pulumi.set(__self__, "redundancies", redundancies)
+        if redundancy is not None:
+            pulumi.set(__self__, "redundancy", redundancy)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def href(self) -> Optional[pulumi.Input[str]]:
         """
@@ -3274,23 +3274,23 @@
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
-    def redundancies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ConnectionZSideAccessPointPortRedundancyArgs']]]]:
+    def redundancy(self) -> Optional[pulumi.Input['ConnectionZSideAccessPointPortRedundancyArgs']]:
         """
         Redundancy Information
         """
-        return pulumi.get(self, "redundancies")
+        return pulumi.get(self, "redundancy")
 
-    @redundancies.setter
-    def redundancies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ConnectionZSideAccessPointPortRedundancyArgs']]]]):
-        pulumi.set(self, "redundancies", value)
+    @redundancy.setter
+    def redundancy(self, value: Optional[pulumi.Input['ConnectionZSideAccessPointPortRedundancyArgs']]):
+        pulumi.set(self, "redundancy", value)
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[pulumi.Input[str]]:
         """
         Equinix-assigned virtual gateway identifier
         """
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/cloud_router.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/cloud_router.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/connection.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_cloud_router.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_cloud_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,20 +278,22 @@
     """
     Fabric V4 API compatible data resource that allow user to fetch Fabric Cloud Router for a given UUID
 
     API documentation can be found here - https://developer.equinix.com/dev-docs/fabric/api-reference/fabric-v4-apis#fabric-cloud-routers
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     cloud_router_data_name = equinix.fabric.get_cloud_router(uuid="<uuid_of_cloud_router>")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str uuid: Equinix-assigned Fabric Cloud Router identifier
     """
     __args__ = dict()
     __args__['uuid'] = uuid
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -326,18 +328,20 @@
     """
     Fabric V4 API compatible data resource that allow user to fetch Fabric Cloud Router for a given UUID
 
     API documentation can be found here - https://developer.equinix.com/dev-docs/fabric/api-reference/fabric-v4-apis#fabric-cloud-routers
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     cloud_router_data_name = equinix.fabric.get_cloud_router(uuid="<uuid_of_cloud_router>")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str uuid: Equinix-assigned Fabric Cloud Router identifier
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_connection.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,20 +276,22 @@
 def get_connection(uuid: Optional[str] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetConnectionResult:
     """
     Fabric V4 API compatible data resource that allow user to fetch connection for a given UUID
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     connection_data_name = equinix.fabric.get_connection(uuid="<uuid_of_connection>")
     ```
+    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     __args__['uuid'] = uuid
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('equinix:fabric/getConnection:getConnection', __args__, opts=opts, typ=GetConnectionResult).value
 
     return AwaitableGetConnectionResult(
@@ -319,15 +321,17 @@
 def get_connection_output(uuid: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetConnectionResult]:
     """
     Fabric V4 API compatible data resource that allow user to fetch connection for a given UUID
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     connection_data_name = equinix.fabric.get_connection(uuid="<uuid_of_connection>")
     ```
+    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_network.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,20 +204,22 @@
 def get_network(uuid: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetNetworkResult:
     """
     Fabric V4 API compatible data resource that allow user to fetch Fabric Network for a given UUID
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     network_data_name = equinix.fabric.get_network(uuid="<uuid_of_network>")
     ```
+    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     __args__['uuid'] = uuid
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('equinix:fabric/getNetwork:getNetwork', __args__, opts=opts, typ=GetNetworkResult).value
 
     return AwaitableGetNetworkResult(
@@ -241,15 +243,17 @@
 def get_network_output(uuid: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNetworkResult]:
     """
     Fabric V4 API compatible data resource that allow user to fetch Fabric Network for a given UUID
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     network_data_name = equinix.fabric.get_network(uuid="<uuid_of_network>")
     ```
+    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_port.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_port.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,20 +264,22 @@
 def get_port(uuid: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPortResult:
     """
     Fabric V4 API compatible data resource that allow user to fetch port by uuid
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     port_data_name = equinix.fabric.get_port(uuid="<uuid_of_port>")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str uuid: Equinix-assigned port identifier
     """
     __args__ = dict()
     __args__['uuid'] = uuid
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -309,18 +311,20 @@
 def get_port_output(uuid: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPortResult]:
     """
     Fabric V4 API compatible data resource that allow user to fetch port by uuid
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     port_data_name = equinix.fabric.get_port(uuid="<uuid_of_port>")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str uuid: Equinix-assigned port identifier
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_ports.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_ports.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,22 +73,24 @@
 def get_ports(filter: Optional[pulumi.InputType['GetPortsFilterArgs']] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPortsResult:
     """
     Fabric V4 API compatible data resource that allow user to fetch port by name
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     ports_data_name = equinix.fabric.get_ports(filter=equinix.fabric.GetPortsFilterArgs(
         name="<name_of_port||port_prefix>",
     ))
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param pulumi.InputType['GetPortsFilterArgs'] filter: name
     """
     __args__ = dict()
     __args__['filter'] = filter
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -104,20 +106,22 @@
 def get_ports_output(filter: Optional[pulumi.Input[pulumi.InputType['GetPortsFilterArgs']]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPortsResult]:
     """
     Fabric V4 API compatible data resource that allow user to fetch port by name
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     ports_data_name = equinix.fabric.get_ports(filter=equinix.fabric.GetPortsFilterArgs(
         name="<name_of_port||port_prefix>",
     ))
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param pulumi.InputType['GetPortsFilterArgs'] filter: name
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_routing_protocol.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_routing_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,21 +267,23 @@
     """
     Fabric V4 API compatible data resource that allow user to fetch routing protocol for a given UUID
 
     API documentation can be found here - https://developer.equinix.com/dev-docs/fabric/api-reference/fabric-v4-apis#routing-protocols
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     routing_protocol_data_name = equinix.fabric.get_routing_protocol(connection_uuid="<uuid_of_connection_routing_protocol_is_applied_to>",
         uuid="<uuid_of_routing_protocol>")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str connection_uuid: Connection URI associated with Routing Protocol
     """
     __args__ = dict()
     __args__['connectionUuid'] = connection_uuid
     __args__['uuid'] = uuid
@@ -317,19 +319,21 @@
     """
     Fabric V4 API compatible data resource that allow user to fetch routing protocol for a given UUID
 
     API documentation can be found here - https://developer.equinix.com/dev-docs/fabric/api-reference/fabric-v4-apis#routing-protocols
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     routing_protocol_data_name = equinix.fabric.get_routing_protocol(connection_uuid="<uuid_of_connection_routing_protocol_is_applied_to>",
         uuid="<uuid_of_routing_protocol>")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str connection_uuid: Connection URI associated with Routing Protocol
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_service_profile.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_service_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,20 +288,22 @@
 def get_service_profile(uuid: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServiceProfileResult:
     """
     Fabric V4 API compatible data resource that allow user to fetch Service Profile by UUID filter criteria
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     service_profile_data_name = equinix.fabric.get_service_profile(uuid="<uuid_of_service_profile>")
     ```
+    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     __args__['uuid'] = uuid
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('equinix:fabric/getServiceProfile:getServiceProfile', __args__, opts=opts, typ=GetServiceProfileResult).value
 
     return AwaitableGetServiceProfileResult(
@@ -332,15 +334,17 @@
 def get_service_profile_output(uuid: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServiceProfileResult]:
     """
     Fabric V4 API compatible data resource that allow user to fetch Service Profile by UUID filter criteria
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     service_profile_data_name = equinix.fabric.get_service_profile(uuid="<uuid_of_service_profile>")
     ```
+    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/get_service_profiles.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/get_service_profiles.py`

 * *Files 10% similar despite different names*

```diff
@@ -99,24 +99,26 @@
                          view_point: Optional[str] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServiceProfilesResult:
     """
     Fabric V4 API compatible data resource that allow user to fetch Service Profile by name filter criteria
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     service_profiles_data_name = equinix.fabric.get_service_profiles(filter=equinix.fabric.GetServiceProfilesFilterArgs(
         operator="=",
         property="/name",
         values=["<list_of_profiles_to_return>"],
     ))
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param pulumi.InputType['GetServiceProfilesFilterArgs'] filter: Service Profile Search Filter
     :param Sequence[pulumi.InputType['GetServiceProfilesSortArgs']] sort: Service Profile Sort criteria for Search Request response payload
     :param str view_point: flips view between buyer and seller representation. Available values : aSide, zSide. Default value : aSide
     """
     __args__ = dict()
@@ -140,24 +142,26 @@
                                 view_point: Optional[pulumi.Input[Optional[str]]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServiceProfilesResult]:
     """
     Fabric V4 API compatible data resource that allow user to fetch Service Profile by name filter criteria
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     service_profiles_data_name = equinix.fabric.get_service_profiles(filter=equinix.fabric.GetServiceProfilesFilterArgs(
         operator="=",
         property="/name",
         values=["<list_of_profiles_to_return>"],
     ))
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param pulumi.InputType['GetServiceProfilesFilterArgs'] filter: Service Profile Search Filter
     :param Sequence[pulumi.InputType['GetServiceProfilesSortArgs']] sort: Service Profile Sort criteria for Search Request response payload
     :param str view_point: flips view between buyer and seller representation. Available values : aSide, zSide. Default value : aSide
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/network.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,14 +342,15 @@
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Fabric V4 API compatible resource allows creation and management of Equinix Fabric Network
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         new_network = equinix.fabric.Network("newNetwork",
             notifications=[equinix.fabric.NetworkNotificationArgs(
                 emails=[
@@ -360,14 +361,15 @@
             )],
             project=equinix.fabric.NetworkProjectArgs(
                 project_id="776847000642406",
             ),
             scope="GLOBAL",
             type="EVPLAN")
         ```
+        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['NetworkLocationArgs']] location: Fabric Network location
         :param pulumi.Input[str] name: Fabric Network name. An alpha-numeric 24 characters string which can include only hyphens and underscores
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NetworkNotificationArgs']]]] notifications: Preferences for notifications on Fabric Network configuration or status changes
         :param pulumi.Input[pulumi.InputType['NetworkProjectArgs']] project: Fabric Network project
@@ -381,14 +383,15 @@
                  args: NetworkArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Fabric V4 API compatible resource allows creation and management of Equinix Fabric Network
 
         ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_equinix as equinix
 
         new_network = equinix.fabric.Network("newNetwork",
             notifications=[equinix.fabric.NetworkNotificationArgs(
                 emails=[
@@ -399,14 +402,15 @@
             )],
             project=equinix.fabric.NetworkProjectArgs(
                 project_id="776847000642406",
             ),
             scope="GLOBAL",
             type="EVPLAN")
         ```
+        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param NetworkArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/outputs.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1385,28 +1385,28 @@
 
 
 @pulumi.output_type
 class ConnectionASideAccessPointPort(dict):
     def __init__(__self__, *,
                  href: Optional[str] = None,
                  name: Optional[str] = None,
-                 redundancies: Optional[Sequence['outputs.ConnectionASideAccessPointPortRedundancy']] = None,
+                 redundancy: Optional['outputs.ConnectionASideAccessPointPortRedundancy'] = None,
                  uuid: Optional[str] = None):
         """
         :param str href: Unique Resource Identifier
         :param str name: Port name
-        :param Sequence['ConnectionASideAccessPointPortRedundancyArgs'] redundancies: Redundancy Information
+        :param 'ConnectionASideAccessPointPortRedundancyArgs' redundancy: Redundancy Information
         :param str uuid: Equinix-assigned virtual gateway identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if redundancies is not None:
-            pulumi.set(__self__, "redundancies", redundancies)
+        if redundancy is not None:
+            pulumi.set(__self__, "redundancy", redundancy)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def href(self) -> Optional[str]:
         """
@@ -1420,19 +1420,19 @@
         """
         Port name
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def redundancies(self) -> Optional[Sequence['outputs.ConnectionASideAccessPointPortRedundancy']]:
+    def redundancy(self) -> Optional['outputs.ConnectionASideAccessPointPortRedundancy']:
         """
         Redundancy Information
         """
-        return pulumi.get(self, "redundancies")
+        return pulumi.get(self, "redundancy")
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[str]:
         """
         Equinix-assigned virtual gateway identifier
         """
@@ -3184,28 +3184,28 @@
 
 
 @pulumi.output_type
 class ConnectionZSideAccessPointPort(dict):
     def __init__(__self__, *,
                  href: Optional[str] = None,
                  name: Optional[str] = None,
-                 redundancies: Optional[Sequence['outputs.ConnectionZSideAccessPointPortRedundancy']] = None,
+                 redundancy: Optional['outputs.ConnectionZSideAccessPointPortRedundancy'] = None,
                  uuid: Optional[str] = None):
         """
         :param str href: Unique Resource Identifier
         :param str name: Port name
-        :param Sequence['ConnectionZSideAccessPointPortRedundancyArgs'] redundancies: Redundancy Information
+        :param 'ConnectionZSideAccessPointPortRedundancyArgs' redundancy: Redundancy Information
         :param str uuid: Equinix-assigned virtual gateway identifier
         """
         if href is not None:
             pulumi.set(__self__, "href", href)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if redundancies is not None:
-            pulumi.set(__self__, "redundancies", redundancies)
+        if redundancy is not None:
+            pulumi.set(__self__, "redundancy", redundancy)
         if uuid is not None:
             pulumi.set(__self__, "uuid", uuid)
 
     @property
     @pulumi.getter
     def href(self) -> Optional[str]:
         """
@@ -3219,19 +3219,19 @@
         """
         Port name
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def redundancies(self) -> Optional[Sequence['outputs.ConnectionZSideAccessPointPortRedundancy']]:
+    def redundancy(self) -> Optional['outputs.ConnectionZSideAccessPointPortRedundancy']:
         """
         Redundancy Information
         """
-        return pulumi.get(self, "redundancies")
+        return pulumi.get(self, "redundancy")
 
     @property
     @pulumi.getter
     def uuid(self) -> Optional[str]:
         """
         Equinix-assigned virtual gateway identifier
         """
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/routing_protocol.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/routing_protocol.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/fabric/service_profile.py` & `pulumi_equinix-0.7.3/pulumi_equinix/fabric/service_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/__init__.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/_enums.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/_inputs.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/bgp_session.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/bgp_session.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/device.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1246,15 +1246,19 @@
             billing_cycle="hourly",
             project_id=project_id)
         pulumi.export("webPublicIp", web.access_public_ipv4.apply(lambda access_public_ipv4: f"http://{access_public_ipv4}"))
         ```
 
         ## Import
 
-        This resource can be imported using an existing device ID:<break><break> ```sh<break> $ pulumi import equinix:metal/device:Device equinix_metal_device {existing_device_id} <break>```<break><break>
+        This resource can be imported using an existing device ID:
+
+        ```sh
+        $ pulumi import equinix:metal/device:Device equinix_metal_device {existing_device_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] always_pxe: If true, a device with OS `custom_ipxe` will continue to boot via iPXE
                on reboots.
         :param pulumi.Input[pulumi.InputType['DeviceBehaviorArgs']] behavior: Behavioral overrides that change how the resource handles certain attribute updates. See Behavior below for more details.
         :param pulumi.Input[Union[str, 'BillingCycle']] billing_cycle: monthly or hourly
@@ -1341,15 +1345,19 @@
             billing_cycle="hourly",
             project_id=project_id)
         pulumi.export("webPublicIp", web.access_public_ipv4.apply(lambda access_public_ipv4: f"http://{access_public_ipv4}"))
         ```
 
         ## Import
 
-        This resource can be imported using an existing device ID:<break><break> ```sh<break> $ pulumi import equinix:metal/device:Device equinix_metal_device {existing_device_id} <break>```<break><break>
+        This resource can be imported using an existing device ID:
+
+        ```sh
+        $ pulumi import equinix:metal/device:Device equinix_metal_device {existing_device_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param DeviceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/device_network_type.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/device_network_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,15 +116,19 @@
             device_id=device_id,
             type=network_type)
         pulumi.export("deviceNetworkId", device_network.id)
         ```
 
         ## Import
 
-        This resource can also be imported using existing device ID:<break><break> ```sh<break> $ pulumi import equinix:metal/deviceNetworkType:DeviceNetworkType equinix_metal_device_network_type {existing device_id} <break>```<break><break>
+        This resource can also be imported using existing device ID:
+
+        ```sh
+        $ pulumi import equinix:metal/deviceNetworkType:DeviceNetworkType equinix_metal_device_network_type {existing device_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] device_id: The ID of the device on which the network type should be set.
         :param pulumi.Input[str] type: Network type to set. Must be one of `layer3`, `hybrid`, `hybrid-bonded`, `layer2-individual`
                and `layer2-bonded`.
         """
@@ -149,15 +153,19 @@
             device_id=device_id,
             type=network_type)
         pulumi.export("deviceNetworkId", device_network.id)
         ```
 
         ## Import
 
-        This resource can also be imported using existing device ID:<break><break> ```sh<break> $ pulumi import equinix:metal/deviceNetworkType:DeviceNetworkType equinix_metal_device_network_type {existing device_id} <break>```<break><break>
+        This resource can also be imported using existing device ID:
+
+        ```sh
+        $ pulumi import equinix:metal/deviceNetworkType:DeviceNetworkType equinix_metal_device_network_type {existing device_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param DeviceNetworkTypeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/gateway.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_device.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -332,30 +332,34 @@
 
     > **Note:** All arguments including the `root_password` and `user_data` will be stored in
      the raw state as plain-text.
     Read more about sensitive data in state.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_device(project_id=local["project_id"],
         hostname="mydevice")
     pulumi.export("id", test.id)
     ```
+    <!--End PulumiCodeChooser -->
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_device(device_id="4c641195-25e5-4c3c-b2b7-4cd7a42c7b40")
     pulumi.export("ipv4", test.access_public_ipv4)
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: Device ID.
            
            > **NOTE:** You should pass either `device_id`, or both `project_id` and `hostname`.
     :param str hostname: The device name.
     :param str project_id: The id of the project in which the devices exists.
@@ -407,30 +411,34 @@
 
     > **Note:** All arguments including the `root_password` and `user_data` will be stored in
      the raw state as plain-text.
     Read more about sensitive data in state.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_device(project_id=local["project_id"],
         hostname="mydevice")
     pulumi.export("id", test.id)
     ```
+    <!--End PulumiCodeChooser -->
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_device(device_id="4c641195-25e5-4c3c-b2b7-4cd7a42c7b40")
     pulumi.export("ipv4", test.access_public_ipv4)
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: Device ID.
            
            > **NOTE:** You should pass either `device_id`, or both `project_id` and `hostname`.
     :param str hostname: The device name.
     :param str project_id: The id of the project in which the devices exists.
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_device_bgp_neighbors.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_device_bgp_neighbors.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,21 +75,23 @@
     and have a BGP session assigned.
 
     To learn more about using BGP in Equinix Metal, see the
     metal.BgpSession resource documentation.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_device_bgp_neighbors(device_id="4c641195-25e5-4c3c-b2b7-4cd7a42c7b40")
     pulumi.export("bgpNeighborsListing", test.bgp_neighbors)
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: UUID of BGP-enabled device whose neighbors to list.
     """
     __args__ = dict()
     __args__['deviceId'] = device_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -111,19 +113,21 @@
     and have a BGP session assigned.
 
     To learn more about using BGP in Equinix Metal, see the
     metal.BgpSession resource documentation.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_device_bgp_neighbors(device_id="4c641195-25e5-4c3c-b2b7-4cd7a42c7b40")
     pulumi.export("bgpNeighborsListing", test.bgp_neighbors)
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: UUID of BGP-enabled device whose neighbors to list.
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_devices.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_devices.py`

 * *Files 13% similar despite different names*

```diff
@@ -112,14 +112,15 @@
     """
     The datasource can be used to find a list of devices which meet filter criteria.
 
     If you need to fetch a single device by ID or by project ID and hostname, use the metal.Device datasource.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_devices(project_id=local["project_id"],
         filters=[
             equinix.metal.GetDevicesFilterArgs(
@@ -132,22 +133,26 @@
                     "da",
                     "sv",
                 ],
             ),
         ])
     pulumi.export("devices", example.devices)
     ```
+    <!--End PulumiCodeChooser -->
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_devices(search="database")
     pulumi.export("devices", example.devices)
     ```
+    <!--End PulumiCodeChooser -->
+
     ## search vs filter
 
     The difference between `search` and `filter` is that `search` is an API parameter, interpreted by the Equinix Metal service. The "filter" arguments will reduce the API list (or search) results by applying client-side filtering, within this provider.
 
 
     :param Sequence[pulumi.InputType['GetDevicesFilterArgs']] filters: One or more attribute/values pairs to filter. List of atributes to filter can be found in the attribute reference of the `metal.Device` datasource.
     :param str organization_id: ID of organization containing the devices.
@@ -183,14 +188,15 @@
     """
     The datasource can be used to find a list of devices which meet filter criteria.
 
     If you need to fetch a single device by ID or by project ID and hostname, use the metal.Device datasource.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_devices(project_id=local["project_id"],
         filters=[
             equinix.metal.GetDevicesFilterArgs(
@@ -203,22 +209,26 @@
                     "da",
                     "sv",
                 ],
             ),
         ])
     pulumi.export("devices", example.devices)
     ```
+    <!--End PulumiCodeChooser -->
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_devices(search="database")
     pulumi.export("devices", example.devices)
     ```
+    <!--End PulumiCodeChooser -->
+
     ## search vs filter
 
     The difference between `search` and `filter` is that `search` is an API parameter, interpreted by the Equinix Metal service. The "filter" arguments will reduce the API list (or search) results by applying client-side filtering, within this provider.
 
 
     :param Sequence[pulumi.InputType['GetDevicesFilterArgs']] filters: One or more attribute/values pairs to filter. List of atributes to filter can be found in the attribute reference of the `metal.Device` datasource.
     :param str organization_id: ID of organization containing the devices.
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_facility.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_facility.py`

 * *Files 11% similar despite different names*

```diff
@@ -114,14 +114,26 @@
                  features_requireds: Optional[Sequence[str]] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetFacilityResult:
     """
     > **Deprecated** Use `metal_get_metro` instead.  For more information, refer to the facility to metro migration guide.
 
     Provides an Equinix Metal facility datasource.
 
+    ## Example Usage
+
+    <!--Start PulumiCodeChooser -->
+    ```python
+    import pulumi
+    import pulumi_equinix as equinix
+
+    ny5 = equinix.metal.get_facility(code="ny5")
+    pulumi.export("id", ny5.id)
+    ```
+    <!--End PulumiCodeChooser -->
+
 
     :param Sequence[pulumi.InputType['GetFacilityCapacityArgs']] capacities: One or more device plans for which the facility must have capacity.
     :param str code: The facility code to search for facilities.
     :param Sequence[str] features_requireds: Set of feature strings that the facility must have. Some
            possible values are `baremetal`, `ibx`, `storage`, `global_ipv4`, `backend_transfer`, `layer_2`.
     """
     __args__ = dict()
@@ -147,14 +159,26 @@
                         features_requireds: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFacilityResult]:
     """
     > **Deprecated** Use `metal_get_metro` instead.  For more information, refer to the facility to metro migration guide.
 
     Provides an Equinix Metal facility datasource.
 
+    ## Example Usage
+
+    <!--Start PulumiCodeChooser -->
+    ```python
+    import pulumi
+    import pulumi_equinix as equinix
+
+    ny5 = equinix.metal.get_facility(code="ny5")
+    pulumi.export("id", ny5.id)
+    ```
+    <!--End PulumiCodeChooser -->
+
 
     :param Sequence[pulumi.InputType['GetFacilityCapacityArgs']] capacities: One or more device plans for which the facility must have capacity.
     :param str code: The facility code to search for facilities.
     :param Sequence[str] features_requireds: Set of feature strings that the facility must have. Some
            possible values are `baremetal`, `ibx`, `storage`, `global_ipv4`, `backend_transfer`, `layer_2`.
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_gateway.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,25 +128,27 @@
     """
     Use this datasource to retrieve Metal Gateway resources in Equinix Metal.
 
     > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     # Create Metal Gateway for a VLAN with a private IPv4 block with 8 IP addresses
     test_vlan = equinix.metal.Vlan("testVlan",
         description="test VLAN in SV",
         metro="sv",
         project_id=local["project_id"])
     test_gateway = equinix.metal.get_gateway(gateway_id=local["gateway_id"])
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str gateway_id: UUID of the metal gateway resource to retrieve.
     """
     __args__ = dict()
     __args__['gatewayId'] = gateway_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -169,23 +171,25 @@
     """
     Use this datasource to retrieve Metal Gateway resources in Equinix Metal.
 
     > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     # Create Metal Gateway for a VLAN with a private IPv4 block with 8 IP addresses
     test_vlan = equinix.metal.Vlan("testVlan",
         description="test VLAN in SV",
         metro="sv",
         project_id=local["project_id"])
     test_gateway = equinix.metal.get_gateway(gateway_id=local["gateway_id"])
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str gateway_id: UUID of the metal gateway resource to retrieve.
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_hardware_reservation.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_hardware_reservation.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,21 +152,23 @@
     """
     Use this data source to retrieve a [hardware reservation resource from Equinix Metal](https://metal.equinix.com/developers/docs/deploy/reserved/).
 
     You can look up hardware reservation by its ID or by ID of device which occupies it.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_hardware_reservation(id="4347e805-eb46-4699-9eb9-5c116e6a0172")
     example_by_device_id = equinix.metal.get_hardware_reservation(device_id="ff85aa58-c106-4624-8f1c-7c64554047ea")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: UUID of device occupying the reservation.
     :param str id: ID of the hardware reservation.
     """
     __args__ = dict()
     __args__['deviceId'] = device_id
@@ -193,20 +195,22 @@
     """
     Use this data source to retrieve a [hardware reservation resource from Equinix Metal](https://metal.equinix.com/developers/docs/deploy/reserved/).
 
     You can look up hardware reservation by its ID or by ID of device which occupies it.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_hardware_reservation(id="4347e805-eb46-4699-9eb9-5c116e6a0172")
     example_by_device_id = equinix.metal.get_hardware_reservation(device_id="ff85aa58-c106-4624-8f1c-7c64554047ea")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: UUID of device occupying the reservation.
     :param str id: ID of the hardware reservation.
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_interconnection.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_interconnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,18 @@
 ]
 
 @pulumi.output_type
 class GetInterconnectionResult:
     """
     A collection of values returned by getInterconnection.
     """
-    def __init__(__self__, connection_id=None, contact_email=None, description=None, facility=None, id=None, metro=None, mode=None, name=None, organization_id=None, ports=None, project_id=None, redundancy=None, service_token_type=None, service_tokens=None, speed=None, status=None, tags=None, token=None, type=None, vlans=None):
+    def __init__(__self__, authorization_code=None, connection_id=None, contact_email=None, description=None, facility=None, id=None, metro=None, mode=None, name=None, organization_id=None, ports=None, project_id=None, redundancy=None, service_token_type=None, service_tokens=None, speed=None, status=None, tags=None, token=None, type=None, vlans=None, vrfs=None):
+        if authorization_code and not isinstance(authorization_code, str):
+            raise TypeError("Expected argument 'authorization_code' to be a str")
+        pulumi.set(__self__, "authorization_code", authorization_code)
         if connection_id and not isinstance(connection_id, str):
             raise TypeError("Expected argument 'connection_id' to be a str")
         pulumi.set(__self__, "connection_id", connection_id)
         if contact_email and not isinstance(contact_email, str):
             raise TypeError("Expected argument 'contact_email' to be a str")
         pulumi.set(__self__, "contact_email", contact_email)
         if description and not isinstance(description, str):
@@ -79,14 +82,22 @@
         pulumi.set(__self__, "token", token)
         if type and not isinstance(type, str):
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
         if vlans and not isinstance(vlans, list):
             raise TypeError("Expected argument 'vlans' to be a list")
         pulumi.set(__self__, "vlans", vlans)
+        if vrfs and not isinstance(vrfs, list):
+            raise TypeError("Expected argument 'vrfs' to be a list")
+        pulumi.set(__self__, "vrfs", vrfs)
+
+    @property
+    @pulumi.getter(name="authorizationCode")
+    def authorization_code(self) -> str:
+        return pulumi.get(self, "authorization_code")
 
     @property
     @pulumi.getter(name="connectionId")
     def connection_id(self) -> str:
         return pulumi.get(self, "connection_id")
 
     @property
@@ -243,21 +254,27 @@
     @pulumi.getter
     def vlans(self) -> Sequence[int]:
         """
         Attached VLANs. Only available in shared connection. One vlan for Primary/Single connection and two vlans for Redundant connection.
         """
         return pulumi.get(self, "vlans")
 
+    @property
+    @pulumi.getter
+    def vrfs(self) -> Sequence[str]:
+        return pulumi.get(self, "vrfs")
+
 
 class AwaitableGetInterconnectionResult(GetInterconnectionResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetInterconnectionResult(
+            authorization_code=self.authorization_code,
             connection_id=self.connection_id,
             contact_email=self.contact_email,
             description=self.description,
             facility=self.facility,
             id=self.id,
             metro=self.metro,
             mode=self.mode,
@@ -269,42 +286,46 @@
             service_token_type=self.service_token_type,
             service_tokens=self.service_tokens,
             speed=self.speed,
             status=self.status,
             tags=self.tags,
             token=self.token,
             type=self.type,
-            vlans=self.vlans)
+            vlans=self.vlans,
+            vrfs=self.vrfs)
 
 
 def get_interconnection(connection_id: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetInterconnectionResult:
     """
     Use this data source to retrieve a [connection resource](https://metal.equinix.com/developers/docs/networking/fabric/)
 
     > Equinix Metal connection with with Service Token A-side / Z-side (service_token_type) is not generally available and may not be enabled yet for your organization.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_interconnection(connection_id="4347e805-eb46-4699-9eb9-5c116e6a017d")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str connection_id: ID of the connection resource.
     """
     __args__ = dict()
     __args__['connectionId'] = connection_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('equinix:metal/getInterconnection:getInterconnection', __args__, opts=opts, typ=GetInterconnectionResult).value
 
     return AwaitableGetInterconnectionResult(
+        authorization_code=pulumi.get(__ret__, 'authorization_code'),
         connection_id=pulumi.get(__ret__, 'connection_id'),
         contact_email=pulumi.get(__ret__, 'contact_email'),
         description=pulumi.get(__ret__, 'description'),
         facility=pulumi.get(__ret__, 'facility'),
         id=pulumi.get(__ret__, 'id'),
         metro=pulumi.get(__ret__, 'metro'),
         mode=pulumi.get(__ret__, 'mode'),
@@ -316,31 +337,34 @@
         service_token_type=pulumi.get(__ret__, 'service_token_type'),
         service_tokens=pulumi.get(__ret__, 'service_tokens'),
         speed=pulumi.get(__ret__, 'speed'),
         status=pulumi.get(__ret__, 'status'),
         tags=pulumi.get(__ret__, 'tags'),
         token=pulumi.get(__ret__, 'token'),
         type=pulumi.get(__ret__, 'type'),
-        vlans=pulumi.get(__ret__, 'vlans'))
+        vlans=pulumi.get(__ret__, 'vlans'),
+        vrfs=pulumi.get(__ret__, 'vrfs'))
 
 
 @_utilities.lift_output_func(get_interconnection)
 def get_interconnection_output(connection_id: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInterconnectionResult]:
     """
     Use this data source to retrieve a [connection resource](https://metal.equinix.com/developers/docs/networking/fabric/)
 
     > Equinix Metal connection with with Service Token A-side / Z-side (service_token_type) is not generally available and may not be enabled yet for your organization.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_interconnection(connection_id="4347e805-eb46-4699-9eb9-5c116e6a017d")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str connection_id: ID of the connection resource.
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_ip_block_ranges.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_ip_block_ranges.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,22 +131,24 @@
 
     There are four types of IP blocks in Equinix: equinix_metal_global IPv4, public IPv4, private IPv4 and IPv6. Both global and public IPv4 are routable from the Internet. Public IPv4 blocks are allocated in a facility or metro, and addresses from it can only be assigned to devices in that location. Addresses from Global IPv4 block can be assigned to a device in any metro.
 
     The datasource has 4 list attributes: `global_ipv4`, `public_ipv4`, `private_ipv4` and `ipv6`, each listing CIDR notation (`<network>/<mask>`) of respective blocks from the project.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     project_id = "<UUID_of_your_project>"
     test = equinix.metal.get_ip_block_ranges(project_id=project_id)
     pulumi.export("out", test)
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str facility: Facility code filtering the IP blocks. Global IPv4 blocks will be listed
            anyway. If you omit this and metro, all the block from the project will be listed.   Use metro instead; read the facility to metro migration guide
     :param str metro: Metro code filtering the IP blocks. Global IPv4 blocks will be listed
            anyway. If you omit this and facility, all the block from the project will be listed.
     :param str project_id: ID of the project from which to list the blocks.
@@ -179,22 +181,24 @@
 
     There are four types of IP blocks in Equinix: equinix_metal_global IPv4, public IPv4, private IPv4 and IPv6. Both global and public IPv4 are routable from the Internet. Public IPv4 blocks are allocated in a facility or metro, and addresses from it can only be assigned to devices in that location. Addresses from Global IPv4 block can be assigned to a device in any metro.
 
     The datasource has 4 list attributes: `global_ipv4`, `public_ipv4`, `private_ipv4` and `ipv6`, each listing CIDR notation (`<network>/<mask>`) of respective blocks from the project.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     project_id = "<UUID_of_your_project>"
     test = equinix.metal.get_ip_block_ranges(project_id=project_id)
     pulumi.export("out", test)
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str facility: Facility code filtering the IP blocks. Global IPv4 blocks will be listed
            anyway. If you omit this and metro, all the block from the project will be listed.   Use metro instead; read the facility to metro migration guide
     :param str metro: Metro code filtering the IP blocks. Global IPv4 blocks will be listed
            anyway. If you omit this and facility, all the block from the project will be listed.
     :param str project_id: ID of the project from which to list the blocks.
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_metro.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_metro.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,14 +90,26 @@
 
 def get_metro(capacities: Optional[Sequence[pulumi.InputType['GetMetroCapacityArgs']]] = None,
               code: Optional[str] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMetroResult:
     """
     Provides an Equinix Metal metro datasource.
 
+    ## Example Usage
+
+    <!--Start PulumiCodeChooser -->
+    ```python
+    import pulumi
+    import pulumi_equinix as equinix
+
+    sv = equinix.metal.get_metro(code="sv")
+    pulumi.export("id", sv.id)
+    ```
+    <!--End PulumiCodeChooser -->
+
 
     :param Sequence[pulumi.InputType['GetMetroCapacityArgs']] capacities: One or more device plans for which the metro must have capacity.
     :param str code: The metro code to search for.
     """
     __args__ = dict()
     __args__['capacities'] = capacities
     __args__['code'] = code
@@ -115,12 +127,24 @@
 @_utilities.lift_output_func(get_metro)
 def get_metro_output(capacities: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetMetroCapacityArgs']]]]] = None,
                      code: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMetroResult]:
     """
     Provides an Equinix Metal metro datasource.
 
+    ## Example Usage
+
+    <!--Start PulumiCodeChooser -->
+    ```python
+    import pulumi
+    import pulumi_equinix as equinix
+
+    sv = equinix.metal.get_metro(code="sv")
+    pulumi.export("id", sv.id)
+    ```
+    <!--End PulumiCodeChooser -->
+
 
     :param Sequence[pulumi.InputType['GetMetroCapacityArgs']] capacities: One or more device plans for which the metro must have capacity.
     :param str code: The metro code to search for.
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_operating_system.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_operating_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,29 +98,31 @@
                          version: Optional[str] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOperatingSystemResult:
     """
     Use this data source to get Equinix Metal Operating System image.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_operating_system(distro="ubuntu",
         version="20.04",
         provisionable_on="c3.medium.x86")
     server = equinix.metal.Device("server",
         hostname="tf.ubuntu",
-        plan="c3.medium.x86",
+        plan=equinix.metal.Plan.C3_MEDIUM_X86,
         metro="ny",
-        operating_system=example.id.apply(lambda x: equinix.metal/operatingsystem.OperatingSystem(x)),
-        billing_cycle="hourly",
+        operating_system=example.id.apply(lambda x: equinix.metal.OperatingSystem(x)),
+        billing_cycle=equinix.metal.BillingCycle.HOURLY,
         project_id=local["project_id"])
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str distro: Name of the OS distribution.
     :param str name: Name or part of the name of the distribution. Case insensitive.
     :param str provisionable_on: Plan name.
     :param str version: Version of the distribution.
     """
@@ -148,29 +150,31 @@
                                 version: Optional[pulumi.Input[Optional[str]]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOperatingSystemResult]:
     """
     Use this data source to get Equinix Metal Operating System image.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_operating_system(distro="ubuntu",
         version="20.04",
         provisionable_on="c3.medium.x86")
     server = equinix.metal.Device("server",
         hostname="tf.ubuntu",
-        plan="c3.medium.x86",
+        plan=equinix.metal.Plan.C3_MEDIUM_X86,
         metro="ny",
-        operating_system=example.id.apply(lambda x: equinix.metal/operatingsystem.OperatingSystem(x)),
-        billing_cycle="hourly",
+        operating_system=example.id.apply(lambda x: equinix.metal.OperatingSystem(x)),
+        billing_cycle=equinix.metal.BillingCycle.HOURLY,
         project_id=local["project_id"])
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str distro: Name of the OS distribution.
     :param str name: Name or part of the name of the distribution. Case insensitive.
     :param str provisionable_on: Plan name.
     :param str version: Version of the distribution.
     """
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_organization.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_organization.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,26 +57,23 @@
         """
         Postal address.
         """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter
-    def description(self) -> str:
+    def description(self) -> Optional[str]:
         """
         Description string.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def logo(self) -> str:
         """
         Logo URL.
@@ -131,37 +128,42 @@
             name=self.name,
             organization_id=self.organization_id,
             project_ids=self.project_ids,
             twitter=self.twitter,
             website=self.website)
 
 
-def get_organization(name: Optional[str] = None,
+def get_organization(description: Optional[str] = None,
+                     name: Optional[str] = None,
                      organization_id: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetOrganizationResult:
     """
     Provides an Equinix Metal organization datasource.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_organization(organization_id=local["org_id"])
     pulumi.export("projectsInTheOrg", test.project_ids)
     ```
+    <!--End PulumiCodeChooser -->
 
 
+    :param str description: Description string.
     :param str name: The organization name.
     :param str organization_id: The UUID of the organization resource.
            
            Exactly one of `name` or `organization_id` must be given.
     """
     __args__ = dict()
+    __args__['description'] = description
     __args__['name'] = name
     __args__['organizationId'] = organization_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('equinix:metal/getOrganization:getOrganization', __args__, opts=opts, typ=GetOrganizationResult).value
 
     return AwaitableGetOrganizationResult(
         address=pulumi.get(__ret__, 'address'),
@@ -172,30 +174,34 @@
         organization_id=pulumi.get(__ret__, 'organization_id'),
         project_ids=pulumi.get(__ret__, 'project_ids'),
         twitter=pulumi.get(__ret__, 'twitter'),
         website=pulumi.get(__ret__, 'website'))
 
 
 @_utilities.lift_output_func(get_organization)
-def get_organization_output(name: Optional[pulumi.Input[Optional[str]]] = None,
+def get_organization_output(description: Optional[pulumi.Input[Optional[str]]] = None,
+                            name: Optional[pulumi.Input[Optional[str]]] = None,
                             organization_id: Optional[pulumi.Input[Optional[str]]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOrganizationResult]:
     """
     Provides an Equinix Metal organization datasource.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     test = equinix.metal.get_organization(organization_id=local["org_id"])
     pulumi.export("projectsInTheOrg", test.project_ids)
     ```
+    <!--End PulumiCodeChooser -->
 
 
+    :param str description: Description string.
     :param str name: The organization name.
     :param str organization_id: The UUID of the organization resource.
            
            Exactly one of `name` or `organization_id` must be given.
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_plans.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_plans.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,14 +77,15 @@
               sorts: Optional[Sequence[pulumi.InputType['GetPlansSortArgs']]] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetPlansResult:
     """
     Provides an Equinix Metal plans datasource. This can be used to find plans that meet a filter criteria.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_plans(sorts=[equinix.metal.GetPlansSortArgs(
             attribute="pricing_hour",
             direction="asc",
@@ -101,15 +102,17 @@
                     "da",
                     "sv",
                 ],
             ),
         ])
     pulumi.export("plans", example.plans)
     ```
+    <!--End PulumiCodeChooser -->
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_plans(filters=[
         equinix.metal.GetPlansFilterArgs(
             attribute="class",
@@ -127,20 +130,23 @@
                 "sv",
             ],
             all=True,
         ),
     ])
     pulumi.export("plans", example.plans)
     ```
+    <!--End PulumiCodeChooser -->
+
     ### Ignoring Changes to Plans/Metro
 
     Preserve deployed device plan, facility and metro when creating a new execution plan.
 
     As described in the `data-resource-behavior` feature as shown in the example below.
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example_plans = equinix.metal.get_plans(sorts=[equinix.metal.GetPlansSortArgs(
             attribute="pricing_hour",
             direction="asc",
@@ -159,35 +165,38 @@
                 values=["sv"],
             ),
         ])
     # This equinix_metal_device will use the first returned plan and the first metro in which that plan is available
     # It will ignore future changes on plan and metro
     example_device = equinix.metal.Device("exampleDevice",
         hostname="example",
-        plan=example_plans.plans[0].name.apply(lambda x: equinix.metal/plan.Plan(x)),
+        plan=example_plans.plans[0].name.apply(lambda x: equinix.metal.Plan(x)),
         metro=example_plans.plans[0].available_in_metros[0],
-        operating_system="ubuntu_20_04",
-        billing_cycle="hourly",
+        operating_system=equinix.metal.OperatingSystem.UBUNTU20_04,
+        billing_cycle=equinix.metal.BillingCycle.HOURLY,
         project_id=var["project_id"])
     ```
+    <!--End PulumiCodeChooser -->
 
     If your use case requires dynamic changes of a device plan or metro you can define the lifecycle with a condition.
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     config = pulumi.Config()
     ignore_plans_metros_changes = config.get_bool("ignorePlansMetrosChanges")
     if ignore_plans_metros_changes is None:
         ignore_plans_metros_changes = False
     example_plans = equinix.metal.get_plans()
     # required device arguments
     example_device = equinix.metal.Device("exampleDevice")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetPlansFilterArgs']] filters: One or more attribute/values pairs to filter off of
     :param Sequence[pulumi.InputType['GetPlansSortArgs']] sorts: One or more attribute/direction pairs on which to sort results. If multiple
            sorts are provided, they will be applied in order
     """
     __args__ = dict()
@@ -208,14 +217,15 @@
                      sorts: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetPlansSortArgs']]]]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPlansResult]:
     """
     Provides an Equinix Metal plans datasource. This can be used to find plans that meet a filter criteria.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_plans(sorts=[equinix.metal.GetPlansSortArgs(
             attribute="pricing_hour",
             direction="asc",
@@ -232,15 +242,17 @@
                     "da",
                     "sv",
                 ],
             ),
         ])
     pulumi.export("plans", example.plans)
     ```
+    <!--End PulumiCodeChooser -->
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_plans(filters=[
         equinix.metal.GetPlansFilterArgs(
             attribute="class",
@@ -258,20 +270,23 @@
                 "sv",
             ],
             all=True,
         ),
     ])
     pulumi.export("plans", example.plans)
     ```
+    <!--End PulumiCodeChooser -->
+
     ### Ignoring Changes to Plans/Metro
 
     Preserve deployed device plan, facility and metro when creating a new execution plan.
 
     As described in the `data-resource-behavior` feature as shown in the example below.
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example_plans = equinix.metal.get_plans(sorts=[equinix.metal.GetPlansSortArgs(
             attribute="pricing_hour",
             direction="asc",
@@ -290,35 +305,38 @@
                 values=["sv"],
             ),
         ])
     # This equinix_metal_device will use the first returned plan and the first metro in which that plan is available
     # It will ignore future changes on plan and metro
     example_device = equinix.metal.Device("exampleDevice",
         hostname="example",
-        plan=example_plans.plans[0].name.apply(lambda x: equinix.metal/plan.Plan(x)),
+        plan=example_plans.plans[0].name.apply(lambda x: equinix.metal.Plan(x)),
         metro=example_plans.plans[0].available_in_metros[0],
-        operating_system="ubuntu_20_04",
-        billing_cycle="hourly",
+        operating_system=equinix.metal.OperatingSystem.UBUNTU20_04,
+        billing_cycle=equinix.metal.BillingCycle.HOURLY,
         project_id=var["project_id"])
     ```
+    <!--End PulumiCodeChooser -->
 
     If your use case requires dynamic changes of a device plan or metro you can define the lifecycle with a condition.
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     config = pulumi.Config()
     ignore_plans_metros_changes = config.get_bool("ignorePlansMetrosChanges")
     if ignore_plans_metros_changes is None:
         ignore_plans_metros_changes = False
     example_plans = equinix.metal.get_plans()
     # required device arguments
     example_device = equinix.metal.Device("exampleDevice")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetPlansFilterArgs']] filters: One or more attribute/values pairs to filter off of
     :param Sequence[pulumi.InputType['GetPlansSortArgs']] sorts: One or more attribute/direction pairs on which to sort results. If multiple
            sorts are provided, they will be applied in order
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_port.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_port.py`

 * *Files 5% similar despite different names*

```diff
@@ -208,29 +208,31 @@
     Use this data source to read ports of existing devices. You can read port by either its UUID,
     or by a device UUID and port name.
 
     ## Example Usage
 
     Create a device and read it's eth0 port to the datasource.
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     project_id = "<UUID_of_your_project>"
     test_device = equinix.metal.Device("testDevice",
         hostname="tfacc-test-device-port",
-        plan="c3.medium.x86",
+        plan=equinix.metal.Plan.C3_MEDIUM_X86,
         metro="sv",
-        operating_system="ubuntu_20_04",
-        billing_cycle="hourly",
+        operating_system=equinix.metal.OperatingSystem.UBUNTU20_04,
+        billing_cycle=equinix.metal.BillingCycle.HOURLY,
         project_id=project_id)
     test_port = equinix.metal.get_port_output(device_id=test_device.id,
         name="eth0")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: Device UUID where to lookup the port.
     :param str name: Name of the port to look up, i.e. `bond0`, `eth1`.
     :param str port_id: ID of the port to read, conflicts with `device_id`.
     """
     __args__ = dict()
@@ -267,29 +269,31 @@
     Use this data source to read ports of existing devices. You can read port by either its UUID,
     or by a device UUID and port name.
 
     ## Example Usage
 
     Create a device and read it's eth0 port to the datasource.
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     project_id = "<UUID_of_your_project>"
     test_device = equinix.metal.Device("testDevice",
         hostname="tfacc-test-device-port",
-        plan="c3.medium.x86",
+        plan=equinix.metal.Plan.C3_MEDIUM_X86,
         metro="sv",
-        operating_system="ubuntu_20_04",
-        billing_cycle="hourly",
+        operating_system=equinix.metal.OperatingSystem.UBUNTU20_04,
+        billing_cycle=equinix.metal.BillingCycle.HOURLY,
         project_id=project_id)
     test_port = equinix.metal.get_port_output(device_id=test_device.id,
         name="eth0")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str device_id: Device UUID where to lookup the port.
     :param str name: Name of the port to look up, i.e. `bond0`, `eth1`.
     :param str port_id: ID of the port to read, conflicts with `device_id`.
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_precreated_ip_block.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_precreated_ip_block.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_project.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,17 +77,14 @@
         The timestamp for when the project was created.
         """
         return pulumi.get(self, "created")
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> str:
         return pulumi.get(self, "name")
 
@@ -151,21 +148,23 @@
                 project_id: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetProjectResult:
     """
     Use this datasource to retrieve attributes of the Project API resource.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     tf_project1 = equinix.metal.get_project(name="Terraform Fun")
     pulumi.export("usersOfTerraformFun", tf_project1.user_ids)
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name which is used to look up the project.
     :param str project_id: The UUID by which to look up the project.
     """
     __args__ = dict()
     __args__['name'] = name
@@ -191,20 +190,22 @@
                        project_id: Optional[pulumi.Input[Optional[str]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectResult]:
     """
     Use this datasource to retrieve attributes of the Project API resource.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     tf_project1 = equinix.metal.get_project(name="Terraform Fun")
     pulumi.export("usersOfTerraformFun", tf_project1.user_ids)
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name which is used to look up the project.
     :param str project_id: The UUID by which to look up the project.
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_project_ssh_key.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_project_ssh_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,21 +142,23 @@
                         search: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetProjectSshKeyResult:
     """
     Use this datasource to retrieve attributes of a Project SSH Key API resource.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     my_key = equinix.metal.get_project_ssh_key(search="username@hostname",
         project_id=local["project_id"])
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str id: The id of the SSH Key to search for in the Equinix Metal project.
     :param str project_id: The Equinix Metal project id of the Equinix Metal SSH Key.
            
            > **NOTE:** One of either `search` or `id` must be provided along with `project_id`.
     :param str search: The name, fingerprint, or public_key of the SSH Key to search for
@@ -187,21 +189,23 @@
                                search: Optional[pulumi.Input[Optional[str]]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectSshKeyResult]:
     """
     Use this datasource to retrieve attributes of a Project SSH Key API resource.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     my_key = equinix.metal.get_project_ssh_key(search="username@hostname",
         project_id=local["project_id"])
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str id: The id of the SSH Key to search for in the Equinix Metal project.
     :param str project_id: The Equinix Metal project id of the Equinix Metal SSH Key.
            
            > **NOTE:** One of either `search` or `id` must be provided along with `project_id`.
     :param str search: The name, fingerprint, or public_key of the SSH Key to search for
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_reserved_ip_block.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_reserved_ip_block.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_spot_market_price.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_spot_market_price.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,21 +93,23 @@
     """
     Use this data source to get Equinix Metal Spot Market Price for a plan.
 
     ## Example Usage
 
     Lookup by metro:
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_spot_market_price(metro="sv",
         plan="c3.small.x86")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str facility: Name of the facility. Use metro instead; read the facility to metro migration guide
     :param str metro: Name of the metro.
     :param str plan: Name of the plan.
     """
     __args__ = dict()
@@ -133,21 +135,23 @@
     """
     Use this data source to get Equinix Metal Spot Market Price for a plan.
 
     ## Example Usage
 
     Lookup by metro:
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example = equinix.metal.get_spot_market_price(metro="sv",
         plan="c3.small.x86")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str facility: Name of the facility. Use metro instead; read the facility to metro migration guide
     :param str metro: Name of the metro.
     :param str plan: Name of the plan.
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_spot_market_request.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_spot_market_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_virtual_circuit.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_virtual_circuit.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_vlan.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_vlan.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,17 +70,14 @@
         pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
 
         return pulumi.get(self, "facility")
 
     @property
     @pulumi.getter
     def id(self) -> str:
-        """
-        The provider-assigned unique ID for this managed resource.
-        """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def metro(self) -> str:
         return pulumi.get(self, "metro")
 
@@ -126,35 +123,39 @@
     Provides an Equinix Metal Virtual Network datasource. VLANs data sources can be
     searched by VLAN UUID, or project UUID and vxlan number.
 
     ## Example Usage
 
     Fetch a vlan by ID:
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     foovlan = equinix.metal.Vlan("foovlan",
         project_id=local["project_id"],
         metro="sv",
         vxlan=5)
     dsvlan = equinix.metal.get_vlan_output(vlan_id=foovlan.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Fetch a vlan by project ID, vxlan and metro
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     dsvlan = equinix.metal.get_vlan(project_id=local["project_id"],
         vxlan=5,
         metro="sv")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str facility: Facility where the VLAN is deployed. Deprecated, see https://feedback.equinixmetal.com/changelog/bye-facilities-hello-again-metros
     :param str metro: Metro where the VLAN is deployed.
            
            > **NOTE:** You must set either `vlan_id` or a combination of `vxlan`, `project_id`, and, `metro` or `facility`.
     :param str project_id: UUID of parent project of the VLAN. Use together with the vxlan number and metro or facility.
@@ -192,35 +193,39 @@
     Provides an Equinix Metal Virtual Network datasource. VLANs data sources can be
     searched by VLAN UUID, or project UUID and vxlan number.
 
     ## Example Usage
 
     Fetch a vlan by ID:
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     foovlan = equinix.metal.Vlan("foovlan",
         project_id=local["project_id"],
         metro="sv",
         vxlan=5)
     dsvlan = equinix.metal.get_vlan_output(vlan_id=foovlan.id)
     ```
+    <!--End PulumiCodeChooser -->
 
     Fetch a vlan by project ID, vxlan and metro
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     dsvlan = equinix.metal.get_vlan(project_id=local["project_id"],
         vxlan=5,
         metro="sv")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str facility: Facility where the VLAN is deployed. Deprecated, see https://feedback.equinixmetal.com/changelog/bye-facilities-hello-again-metros
     :param str metro: Metro where the VLAN is deployed.
            
            > **NOTE:** You must set either `vlan_id` or a combination of `vxlan`, `project_id`, and, `metro` or `facility`.
     :param str project_id: UUID of parent project of the VLAN. Use together with the vxlan number and metro or facility.
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/get_vrf.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/get_vrf.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,20 +130,22 @@
     """
     Use this data source to retrieve a VRF resource.
 
     > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example_vrf = equinix.metal.get_vrf(vrf_id="48630899-9ff2-4ce6-a93f-50ff4ebcdf6e")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str vrf_id: ID of the VRF resource
     """
     __args__ = dict()
     __args__['vrfId'] = vrf_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -166,18 +168,20 @@
     """
     Use this data source to retrieve a VRF resource.
 
     > VRF features are not generally available. The interfaces related to VRF resources may change ahead of general availability.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     example_vrf = equinix.metal.get_vrf(vrf_id="48630899-9ff2-4ce6-a93f-50ff4ebcdf6e")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str vrf_id: ID of the VRF resource
     """
     ...
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/interconnection.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/interconnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
                  mode: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  organization_id: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  service_token_type: Optional[pulumi.Input[str]] = None,
                  speed: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 vlans: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None):
+                 vlans: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
+                 vrfs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a Interconnection resource.
         :param pulumi.Input[str] redundancy: Connection redundancy - redundant or primary.
         :param pulumi.Input[str] type: Connection type - dedicated or shared.
         :param pulumi.Input[str] contact_email: The preferred email used for communication and notifications about the Equinix Fabric interconnection. Required when using a Project API key. Optional and defaults to the primary user email address when using a User API key.
         :param pulumi.Input[str] description: Description for the connection resource.
         :param pulumi.Input[str] facility: Facility where the connection will be created.   Use metro instead; read the facility to metro migration guide
@@ -42,14 +43,16 @@
         :param pulumi.Input[str] name: Name of the connection resource
         :param pulumi.Input[str] organization_id: ID of the organization where the connection is scoped to.
         :param pulumi.Input[str] project_id: ID of the project where the connection is scoped to, must be set for.
         :param pulumi.Input[str] service_token_type: Only used with shared connection. Type of service token to use for the connection, a_side or z_side
         :param pulumi.Input[str] speed: Connection speed -  Values must be in the format '<number>Mbps' or '<number>Gpbs', for example '100Mbps' or '50Gbps'.  Actual supported values will depend on the connection type and whether the connection uses VLANs or VRF.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: String list of tags.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] vlans: Only used with shared connection. Vlans to attach. Pass one vlan for Primary/Single connection and two vlans for Redundant connection.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] vrfs: Only used with shared connection. VRFs to attach. Pass one VRF for Primary/Single connection and two VRFs for Redundant
+               connection
         """
         pulumi.set(__self__, "redundancy", redundancy)
         pulumi.set(__self__, "type", type)
         if contact_email is not None:
             pulumi.set(__self__, "contact_email", contact_email)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -72,14 +75,16 @@
             pulumi.set(__self__, "service_token_type", service_token_type)
         if speed is not None:
             pulumi.set(__self__, "speed", speed)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if vlans is not None:
             pulumi.set(__self__, "vlans", vlans)
+        if vrfs is not None:
+            pulumi.set(__self__, "vrfs", vrfs)
 
     @property
     @pulumi.getter
     def redundancy(self) -> pulumi.Input[str]:
         """
         Connection redundancy - redundant or primary.
         """
@@ -244,18 +249,32 @@
         """
         return pulumi.get(self, "vlans")
 
     @vlans.setter
     def vlans(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]):
         pulumi.set(self, "vlans", value)
 
+    @property
+    @pulumi.getter
+    def vrfs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Only used with shared connection. VRFs to attach. Pass one VRF for Primary/Single connection and two VRFs for Redundant
+        connection
+        """
+        return pulumi.get(self, "vrfs")
+
+    @vrfs.setter
+    def vrfs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "vrfs", value)
+
 
 @pulumi.input_type
 class _InterconnectionState:
     def __init__(__self__, *,
+                 authorization_code: Optional[pulumi.Input[str]] = None,
                  contact_email: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  facility: Optional[pulumi.Input[str]] = None,
                  metro: Optional[pulumi.Input[str]] = None,
                  mode: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  organization_id: Optional[pulumi.Input[str]] = None,
@@ -265,17 +284,20 @@
                  service_token_type: Optional[pulumi.Input[str]] = None,
                  service_tokens: Optional[pulumi.Input[Sequence[pulumi.Input['InterconnectionServiceTokenArgs']]]] = None,
                  speed: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  token: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 vlans: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None):
+                 vlans: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
+                 vrfs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering Interconnection resources.
+        :param pulumi.Input[str] authorization_code: Only used with Fabric Shared connection. Fabric uses this token to be able to give more detailed information about the
+               Metal end of the network, when viewing resources from within Fabric.
         :param pulumi.Input[str] contact_email: The preferred email used for communication and notifications about the Equinix Fabric interconnection. Required when using a Project API key. Optional and defaults to the primary user email address when using a User API key.
         :param pulumi.Input[str] description: Description for the connection resource.
         :param pulumi.Input[str] facility: Facility where the connection will be created.   Use metro instead; read the facility to metro migration guide
         :param pulumi.Input[str] metro: Metro where the connection will be created.
         :param pulumi.Input[str] mode: Mode for connections in IBX facilities with the dedicated type - standard or tunnel. Default is standard.
         :param pulumi.Input[str] name: Name of the connection resource
         :param pulumi.Input[str] organization_id: ID of the organization where the connection is scoped to.
@@ -288,15 +310,19 @@
         :param pulumi.Input[Sequence[pulumi.Input['InterconnectionServiceTokenArgs']]] service_tokens: List of connection service tokens with attributes required to configure the connection in Equinix Fabric with the equinix_ecx_l2_connection resource or from the [Equinix Fabric Portal](https://ecxfabric.equinix.com/dashboard). Scehma of service_token is described in documentation of the metal.Interconnection datasource.
         :param pulumi.Input[str] speed: Connection speed -  Values must be in the format '<number>Mbps' or '<number>Gpbs', for example '100Mbps' or '50Gbps'.  Actual supported values will depend on the connection type and whether the connection uses VLANs or VRF.
         :param pulumi.Input[str] status: Status of the connection resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: String list of tags.
         :param pulumi.Input[str] token: (Deprecated) Fabric Token required to configure the connection in Equinix Fabric with the equinix_ecx_l2_connection resource or from the [Equinix Fabric Portal](https://ecxfabric.equinix.com/dashboard). If your organization already has connection service tokens enabled, use `service_tokens` instead.
         :param pulumi.Input[str] type: Connection type - dedicated or shared.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] vlans: Only used with shared connection. Vlans to attach. Pass one vlan for Primary/Single connection and two vlans for Redundant connection.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] vrfs: Only used with shared connection. VRFs to attach. Pass one VRF for Primary/Single connection and two VRFs for Redundant
+               connection
         """
+        if authorization_code is not None:
+            pulumi.set(__self__, "authorization_code", authorization_code)
         if contact_email is not None:
             pulumi.set(__self__, "contact_email", contact_email)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if facility is not None:
             warnings.warn("""Use metro instead of facility. For more information, read the migration guide.""", DeprecationWarning)
             pulumi.log.warn("""facility is deprecated: Use metro instead of facility. For more information, read the migration guide.""")
@@ -331,14 +357,29 @@
             pulumi.log.warn("""token is deprecated: If your organization already has connection service tokens enabled, use `service_tokens` instead""")
         if token is not None:
             pulumi.set(__self__, "token", token)
         if type is not None:
             pulumi.set(__self__, "type", type)
         if vlans is not None:
             pulumi.set(__self__, "vlans", vlans)
+        if vrfs is not None:
+            pulumi.set(__self__, "vrfs", vrfs)
+
+    @property
+    @pulumi.getter(name="authorizationCode")
+    def authorization_code(self) -> Optional[pulumi.Input[str]]:
+        """
+        Only used with Fabric Shared connection. Fabric uses this token to be able to give more detailed information about the
+        Metal end of the network, when viewing resources from within Fabric.
+        """
+        return pulumi.get(self, "authorization_code")
+
+    @authorization_code.setter
+    def authorization_code(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "authorization_code", value)
 
     @property
     @pulumi.getter(name="contactEmail")
     def contact_email(self) -> Optional[pulumi.Input[str]]:
         """
         The preferred email used for communication and notifications about the Equinix Fabric interconnection. Required when using a Project API key. Optional and defaults to the primary user email address when using a User API key.
         """
@@ -556,14 +597,27 @@
         """
         return pulumi.get(self, "vlans")
 
     @vlans.setter
     def vlans(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]]):
         pulumi.set(self, "vlans", value)
 
+    @property
+    @pulumi.getter
+    def vrfs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        """
+        Only used with shared connection. VRFs to attach. Pass one VRF for Primary/Single connection and two VRFs for Redundant
+        connection
+        """
+        return pulumi.get(self, "vrfs")
+
+    @vrfs.setter
+    def vrfs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "vrfs", value)
+
 
 class Interconnection(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  contact_email: Optional[pulumi.Input[str]] = None,
@@ -576,14 +630,15 @@
                  project_id: Optional[pulumi.Input[str]] = None,
                  redundancy: Optional[pulumi.Input[str]] = None,
                  service_token_type: Optional[pulumi.Input[str]] = None,
                  speed: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  vlans: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
+                 vrfs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Use this resource to request the creation an Interconnection asset to connect with other parties using [Equinix Fabric - software-defined interconnections](https://metal.equinix.com/developers/docs/networking/fabric/).
 
         > Equinix Metal connection with with Service Token A-side / Z-side (service_token_type) is not generally available and may not be enabled yet for your organization.
 
         ## Example Usage
@@ -623,14 +678,16 @@
         :param pulumi.Input[str] project_id: ID of the project where the connection is scoped to, must be set for.
         :param pulumi.Input[str] redundancy: Connection redundancy - redundant or primary.
         :param pulumi.Input[str] service_token_type: Only used with shared connection. Type of service token to use for the connection, a_side or z_side
         :param pulumi.Input[str] speed: Connection speed -  Values must be in the format '<number>Mbps' or '<number>Gpbs', for example '100Mbps' or '50Gbps'.  Actual supported values will depend on the connection type and whether the connection uses VLANs or VRF.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: String list of tags.
         :param pulumi.Input[str] type: Connection type - dedicated or shared.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] vlans: Only used with shared connection. Vlans to attach. Pass one vlan for Primary/Single connection and two vlans for Redundant connection.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] vrfs: Only used with shared connection. VRFs to attach. Pass one VRF for Primary/Single connection and two VRFs for Redundant
+               connection
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: InterconnectionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -689,14 +746,15 @@
                  project_id: Optional[pulumi.Input[str]] = None,
                  redundancy: Optional[pulumi.Input[str]] = None,
                  service_token_type: Optional[pulumi.Input[str]] = None,
                  speed: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  vlans: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
+                 vrfs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -716,28 +774,31 @@
             __props__.__dict__["service_token_type"] = service_token_type
             __props__.__dict__["speed"] = speed
             __props__.__dict__["tags"] = tags
             if type is None and not opts.urn:
                 raise TypeError("Missing required property 'type'")
             __props__.__dict__["type"] = type
             __props__.__dict__["vlans"] = vlans
+            __props__.__dict__["vrfs"] = vrfs
+            __props__.__dict__["authorization_code"] = None
             __props__.__dict__["ports"] = None
             __props__.__dict__["service_tokens"] = None
             __props__.__dict__["status"] = None
             __props__.__dict__["token"] = None
         super(Interconnection, __self__).__init__(
             'equinix:metal/interconnection:Interconnection',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            authorization_code: Optional[pulumi.Input[str]] = None,
             contact_email: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             facility: Optional[pulumi.Input[str]] = None,
             metro: Optional[pulumi.Input[str]] = None,
             mode: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             organization_id: Optional[pulumi.Input[str]] = None,
@@ -747,22 +808,25 @@
             service_token_type: Optional[pulumi.Input[str]] = None,
             service_tokens: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InterconnectionServiceTokenArgs']]]]] = None,
             speed: Optional[pulumi.Input[str]] = None,
             status: Optional[pulumi.Input[str]] = None,
             tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             token: Optional[pulumi.Input[str]] = None,
             type: Optional[pulumi.Input[str]] = None,
-            vlans: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None) -> 'Interconnection':
+            vlans: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
+            vrfs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None) -> 'Interconnection':
         """
         Get an existing Interconnection resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] authorization_code: Only used with Fabric Shared connection. Fabric uses this token to be able to give more detailed information about the
+               Metal end of the network, when viewing resources from within Fabric.
         :param pulumi.Input[str] contact_email: The preferred email used for communication and notifications about the Equinix Fabric interconnection. Required when using a Project API key. Optional and defaults to the primary user email address when using a User API key.
         :param pulumi.Input[str] description: Description for the connection resource.
         :param pulumi.Input[str] facility: Facility where the connection will be created.   Use metro instead; read the facility to metro migration guide
         :param pulumi.Input[str] metro: Metro where the connection will be created.
         :param pulumi.Input[str] mode: Mode for connections in IBX facilities with the dedicated type - standard or tunnel. Default is standard.
         :param pulumi.Input[str] name: Name of the connection resource
         :param pulumi.Input[str] organization_id: ID of the organization where the connection is scoped to.
@@ -775,19 +839,22 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['InterconnectionServiceTokenArgs']]]] service_tokens: List of connection service tokens with attributes required to configure the connection in Equinix Fabric with the equinix_ecx_l2_connection resource or from the [Equinix Fabric Portal](https://ecxfabric.equinix.com/dashboard). Scehma of service_token is described in documentation of the metal.Interconnection datasource.
         :param pulumi.Input[str] speed: Connection speed -  Values must be in the format '<number>Mbps' or '<number>Gpbs', for example '100Mbps' or '50Gbps'.  Actual supported values will depend on the connection type and whether the connection uses VLANs or VRF.
         :param pulumi.Input[str] status: Status of the connection resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: String list of tags.
         :param pulumi.Input[str] token: (Deprecated) Fabric Token required to configure the connection in Equinix Fabric with the equinix_ecx_l2_connection resource or from the [Equinix Fabric Portal](https://ecxfabric.equinix.com/dashboard). If your organization already has connection service tokens enabled, use `service_tokens` instead.
         :param pulumi.Input[str] type: Connection type - dedicated or shared.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] vlans: Only used with shared connection. Vlans to attach. Pass one vlan for Primary/Single connection and two vlans for Redundant connection.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] vrfs: Only used with shared connection. VRFs to attach. Pass one VRF for Primary/Single connection and two VRFs for Redundant
+               connection
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _InterconnectionState.__new__(_InterconnectionState)
 
+        __props__.__dict__["authorization_code"] = authorization_code
         __props__.__dict__["contact_email"] = contact_email
         __props__.__dict__["description"] = description
         __props__.__dict__["facility"] = facility
         __props__.__dict__["metro"] = metro
         __props__.__dict__["mode"] = mode
         __props__.__dict__["name"] = name
         __props__.__dict__["organization_id"] = organization_id
@@ -798,17 +865,27 @@
         __props__.__dict__["service_tokens"] = service_tokens
         __props__.__dict__["speed"] = speed
         __props__.__dict__["status"] = status
         __props__.__dict__["tags"] = tags
         __props__.__dict__["token"] = token
         __props__.__dict__["type"] = type
         __props__.__dict__["vlans"] = vlans
+        __props__.__dict__["vrfs"] = vrfs
         return Interconnection(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter(name="authorizationCode")
+    def authorization_code(self) -> pulumi.Output[str]:
+        """
+        Only used with Fabric Shared connection. Fabric uses this token to be able to give more detailed information about the
+        Metal end of the network, when viewing resources from within Fabric.
+        """
+        return pulumi.get(self, "authorization_code")
+
+    @property
     @pulumi.getter(name="contactEmail")
     def contact_email(self) -> pulumi.Output[str]:
         """
         The preferred email used for communication and notifications about the Equinix Fabric interconnection. Required when using a Project API key. Optional and defaults to the primary user email address when using a User API key.
         """
         return pulumi.get(self, "contact_email")
 
@@ -952,7 +1029,16 @@
     @pulumi.getter
     def vlans(self) -> pulumi.Output[Optional[Sequence[int]]]:
         """
         Only used with shared connection. Vlans to attach. Pass one vlan for Primary/Single connection and two vlans for Redundant connection.
         """
         return pulumi.get(self, "vlans")
 
+    @property
+    @pulumi.getter
+    def vrfs(self) -> pulumi.Output[Optional[Sequence[str]]]:
+        """
+        Only used with shared connection. VRFs to attach. Pass one VRF for Primary/Single connection and two VRFs for Redundant
+        connection
+        """
+        return pulumi.get(self, "vrfs")
+
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/ip_attachment.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/ip_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/organization.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ._inputs import *
 
 __all__ = ['OrganizationArgs', 'Organization']
 
 @pulumi.input_type
 class OrganizationArgs:
     def __init__(__self__, *,
-                 address: pulumi.Input['OrganizationAddressArgs'],
+                 address: Optional[pulumi.Input['OrganizationAddressArgs']] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  logo: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  twitter: Optional[pulumi.Input[str]] = None,
                  website: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Organization resource.
@@ -28,37 +28,38 @@
                below for more details.
         :param pulumi.Input[str] description: Description string.
         :param pulumi.Input[str] logo: Logo URL.
         :param pulumi.Input[str] name: The name of the Organization.
         :param pulumi.Input[str] twitter: Twitter handle.
         :param pulumi.Input[str] website: Website link.
         """
-        pulumi.set(__self__, "address", address)
+        if address is not None:
+            pulumi.set(__self__, "address", address)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if logo is not None:
             pulumi.set(__self__, "logo", logo)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if twitter is not None:
             pulumi.set(__self__, "twitter", twitter)
         if website is not None:
             pulumi.set(__self__, "website", website)
 
     @property
     @pulumi.getter
-    def address(self) -> pulumi.Input['OrganizationAddressArgs']:
+    def address(self) -> Optional[pulumi.Input['OrganizationAddressArgs']]:
         """
         An object that has the address information. See Address
         below for more details.
         """
         return pulumi.get(self, "address")
 
     @address.setter
-    def address(self, value: pulumi.Input['OrganizationAddressArgs']):
+    def address(self, value: Optional[pulumi.Input['OrganizationAddressArgs']]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
         Description string.
@@ -286,15 +287,19 @@
             ),
             description="An organization")
         pulumi.export("org", org_resource.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing organization ID:<break><break> ```sh<break> $ pulumi import equinix:metal/organization:Organization equinix_metal_organization {existing_organization_id} <break>```<break><break>
+        This resource can be imported using an existing organization ID:
+
+        ```sh
+        $ pulumi import equinix:metal/organization:Organization equinix_metal_organization {existing_organization_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['OrganizationAddressArgs']] address: An object that has the address information. See Address
                below for more details.
         :param pulumi.Input[str] description: Description string.
         :param pulumi.Input[str] logo: Logo URL.
@@ -302,15 +307,15 @@
         :param pulumi.Input[str] twitter: Twitter handle.
         :param pulumi.Input[str] website: Website link.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: OrganizationArgs,
+                 args: Optional[OrganizationArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a resource to manage organization resource in Equinix Metal.
 
         ## Example Usage
         ```python
         import pulumi
@@ -326,15 +331,19 @@
             ),
             description="An organization")
         pulumi.export("org", org_resource.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing organization ID:<break><break> ```sh<break> $ pulumi import equinix:metal/organization:Organization equinix_metal_organization {existing_organization_id} <break>```<break><break>
+        This resource can be imported using an existing organization ID:
+
+        ```sh
+        $ pulumi import equinix:metal/organization:Organization equinix_metal_organization {existing_organization_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param OrganizationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -358,16 +367,14 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = OrganizationArgs.__new__(OrganizationArgs)
 
-            if address is None and not opts.urn:
-                raise TypeError("Missing required property 'address'")
             __props__.__dict__["address"] = address
             __props__.__dict__["description"] = description
             __props__.__dict__["logo"] = logo
             __props__.__dict__["name"] = name
             __props__.__dict__["twitter"] = twitter
             __props__.__dict__["website"] = website
             __props__.__dict__["created"] = None
@@ -419,15 +426,15 @@
         __props__.__dict__["twitter"] = twitter
         __props__.__dict__["updated"] = updated
         __props__.__dict__["website"] = website
         return Organization(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def address(self) -> pulumi.Output['outputs.OrganizationAddress']:
+    def address(self) -> pulumi.Output[Optional['outputs.OrganizationAddress']]:
         """
         An object that has the address information. See Address
         below for more details.
         """
         return pulumi.get(self, "address")
 
     @property
@@ -436,23 +443,23 @@
         """
         The timestamp for when the organization was created.
         """
         return pulumi.get(self, "created")
 
     @property
     @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
+    def description(self) -> pulumi.Output[str]:
         """
         Description string.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
-    def logo(self) -> pulumi.Output[Optional[str]]:
+    def logo(self) -> pulumi.Output[str]:
         """
         Logo URL.
         """
         return pulumi.get(self, "logo")
 
     @property
     @pulumi.getter
@@ -460,15 +467,15 @@
         """
         The name of the Organization.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def twitter(self) -> pulumi.Output[Optional[str]]:
+    def twitter(self) -> pulumi.Output[str]:
         """
         Twitter handle.
         """
         return pulumi.get(self, "twitter")
 
     @property
     @pulumi.getter
@@ -476,13 +483,13 @@
         """
         The timestamp for the last time the organization was updated.
         """
         return pulumi.get(self, "updated")
 
     @property
     @pulumi.getter
-    def website(self) -> pulumi.Output[Optional[str]]:
+    def website(self) -> pulumi.Output[str]:
         """
         Website link.
         """
         return pulumi.get(self, "website")
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/organization_member.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/organization_member.py`

 * *Files 2% similar despite different names*

```diff
@@ -293,15 +293,19 @@
             organization_id=organization_id)
         pulumi.export("memberId", member.id)
         pulumi.export("memberState", member.state)
         ```
 
         ## Import
 
-        This resource can be imported using the `invitee` and `organization_id` as colon separated arguments:<break><break> ```sh<break> $ pulumi import equinix:metal/organizationMember:OrganizationMember resource_name {invitee}:{organization_id} <break>```<break><break>
+        This resource can be imported using the `invitee` and `organization_id` as colon separated arguments:
+
+        ```sh
+        $ pulumi import equinix:metal/organizationMember:OrganizationMember resource_name {invitee}:{organization_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] invitee: The email address of the user to invite
         :param pulumi.Input[str] message: A message to include in the emailed invitation.
         :param pulumi.Input[str] organization_id: The organization to invite the user to
         :param pulumi.Input[Sequence[pulumi.Input[str]]] projects_ids: Project IDs the member has access to within the organization. If the member is an 'admin', the projects list should be empty.
@@ -332,15 +336,19 @@
             organization_id=organization_id)
         pulumi.export("memberId", member.id)
         pulumi.export("memberState", member.state)
         ```
 
         ## Import
 
-        This resource can be imported using the `invitee` and `organization_id` as colon separated arguments:<break><break> ```sh<break> $ pulumi import equinix:metal/organizationMember:OrganizationMember resource_name {invitee}:{organization_id} <break>```<break><break>
+        This resource can be imported using the `invitee` and `organization_id` as colon separated arguments:
+
+        ```sh
+        $ pulumi import equinix:metal/organizationMember:OrganizationMember resource_name {invitee}:{organization_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param OrganizationMemberArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/outputs.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2151,29 +2151,28 @@
 
 @pulumi.output_type
 class GetProjectBgpConfigResult(dict):
     def __init__(__self__, *,
                  asn: int,
                  deployment_type: str,
                  max_prefix: int,
-                 status: str,
-                 md5: Optional[str] = None):
+                 md5: str,
+                 status: str):
         """
         :param int asn: Autonomous System Number for local BGP deployment.
         :param str deployment_type: One of `private`, `public`.
         :param int max_prefix: The maximum number of route filters allowed per server.
-        :param str status: Status of BGP configuration in the project.
         :param str md5: Password for BGP session in plaintext (not a checksum).
+        :param str status: Status of BGP configuration in the project.
         """
         pulumi.set(__self__, "asn", asn)
         pulumi.set(__self__, "deployment_type", deployment_type)
         pulumi.set(__self__, "max_prefix", max_prefix)
+        pulumi.set(__self__, "md5", md5)
         pulumi.set(__self__, "status", status)
-        if md5 is not None:
-            pulumi.set(__self__, "md5", md5)
 
     @property
     @pulumi.getter
     def asn(self) -> int:
         """
         Autonomous System Number for local BGP deployment.
         """
@@ -2193,22 +2192,22 @@
         """
         The maximum number of route filters allowed per server.
         """
         return pulumi.get(self, "max_prefix")
 
     @property
     @pulumi.getter
-    def status(self) -> str:
+    def md5(self) -> str:
         """
-        Status of BGP configuration in the project.
+        Password for BGP session in plaintext (not a checksum).
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "md5")
 
     @property
     @pulumi.getter
-    def md5(self) -> Optional[str]:
+    def status(self) -> str:
         """
-        Password for BGP session in plaintext (not a checksum).
+        Status of BGP configuration in the project.
         """
-        return pulumi.get(self, "md5")
+        return pulumi.get(self, "status")
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/port.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/port.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/port_vlan_attachment.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/port_vlan_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/project.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,19 @@
             name=name,
             organization_id=organization_id)
         pulumi.export("projectId", project_resource.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing project ID:<break><break> ```sh<break> $ pulumi import equinix:metal/project:Project equinix_metal_project {existing_project_id} <break>```<break><break>
+        This resource can be imported using an existing project ID:
+
+        ```sh
+        $ pulumi import equinix:metal/project:Project equinix_metal_project {existing_project_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] backend_transfer: Enable or disable [Backend Transfer](https://metal.equinix.com/developers/docs/networking/backend-transfer/), default is `false`.
         :param pulumi.Input[pulumi.InputType['ProjectBgpConfigArgs']] bgp_config: Optional BGP settings. Refer to [Equinix Metal guide for BGP](https://metal.equinix.com/developers/docs/networking/local-global-bgp/).
                
                > **NOTE:** Once you set the BGP config in a project, it can't be removed (due to a limitation in
@@ -321,15 +325,19 @@
             name=name,
             organization_id=organization_id)
         pulumi.export("projectId", project_resource.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing project ID:<break><break> ```sh<break> $ pulumi import equinix:metal/project:Project equinix_metal_project {existing_project_id} <break>```<break><break>
+        This resource can be imported using an existing project ID:
+
+        ```sh
+        $ pulumi import equinix:metal/project:Project equinix_metal_project {existing_project_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param ProjectArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -411,15 +419,15 @@
         __props__.__dict__["organization_id"] = organization_id
         __props__.__dict__["payment_method_id"] = payment_method_id
         __props__.__dict__["updated"] = updated
         return Project(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="backendTransfer")
-    def backend_transfer(self) -> pulumi.Output[Optional[bool]]:
+    def backend_transfer(self) -> pulumi.Output[bool]:
         """
         Enable or disable [Backend Transfer](https://metal.equinix.com/developers/docs/networking/backend-transfer/), default is `false`.
         """
         return pulumi.get(self, "backend_transfer")
 
     @property
     @pulumi.getter(name="bgpConfig")
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/project_api_key.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/project_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/project_ssh_key.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/project_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/reserved_ip_block.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/reserved_ip_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -614,15 +614,19 @@
             metro=metro)
         pulumi.export("ipBlockId", ip_block.id)
         pulumi.export("ipBlockSubent", ip_block.cidr_notation)
         ```
 
         ## Import
 
-        This resource can be imported using an existing IP reservation ID:<break><break> ```sh<break> $ pulumi import equinix:metal/reservedIpBlock:ReservedIpBlock equinix_metal_reserved_ip_block {existing_ip_reservation_id} <break>```<break><break>
+        This resource can be imported using an existing IP reservation ID:
+
+        ```sh
+        $ pulumi import equinix:metal/reservedIpBlock:ReservedIpBlock equinix_metal_reserved_ip_block {existing_ip_reservation_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] cidr: Only valid as an argument and required when `type` is `vrf`. The size of the network to reserve from an existing VRF ip_range. `cidr` can only be specified with `vrf_id`. Range is 22-31. Virtual Circuits require 30-31. Other VRF resources must use a CIDR in the 22-29 range.
         :param pulumi.Input[str] custom_data: Custom Data is an arbitrary object (submitted in Terraform as serialized JSON) to assign to the IP Reservation. This may
                be helpful for self-managed IPAM. The object must be valid JSON.
         :param pulumi.Input[str] description: Arbitrary description.
@@ -684,15 +688,19 @@
             metro=metro)
         pulumi.export("ipBlockId", ip_block.id)
         pulumi.export("ipBlockSubent", ip_block.cidr_notation)
         ```
 
         ## Import
 
-        This resource can be imported using an existing IP reservation ID:<break><break> ```sh<break> $ pulumi import equinix:metal/reservedIpBlock:ReservedIpBlock equinix_metal_reserved_ip_block {existing_ip_reservation_id} <break>```<break><break>
+        This resource can be imported using an existing IP reservation ID:
+
+        ```sh
+        $ pulumi import equinix:metal/reservedIpBlock:ReservedIpBlock equinix_metal_reserved_ip_block {existing_ip_reservation_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param ReservedIpBlockArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/spot_market_request.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/spot_market_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,15 +354,19 @@
                 plan="c3.small.x86",
             ))
         pulumi.export("requestId", request.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing spot market request ID:<break><break> ```sh<break> $ pulumi import equinix:metal/spotMarketRequest:SpotMarketRequest equinix_metal_spot_market_request {existing_spot_market_request_id} <break>```<break><break>
+        This resource can be imported using an existing spot market request ID:
+
+        ```sh
+        $ pulumi import equinix:metal/spotMarketRequest:SpotMarketRequest equinix_metal_spot_market_request {existing_spot_market_request_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] devices_max: Maximum number devices to be created.
         :param pulumi.Input[int] devices_min: Miniumum number devices to be created.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] facilities: Facility IDs where devices should be created. Use metro instead; read the facility to metro migration guide
         :param pulumi.Input[pulumi.InputType['SpotMarketRequestInstanceParametersArgs']] instance_parameters: Key/Value pairs of parameters for devices provisioned from
@@ -410,15 +414,19 @@
                 plan="c3.small.x86",
             ))
         pulumi.export("requestId", request.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing spot market request ID:<break><break> ```sh<break> $ pulumi import equinix:metal/spotMarketRequest:SpotMarketRequest equinix_metal_spot_market_request {existing_spot_market_request_id} <break>```<break><break>
+        This resource can be imported using an existing spot market request ID:
+
+        ```sh
+        $ pulumi import equinix:metal/spotMarketRequest:SpotMarketRequest equinix_metal_spot_market_request {existing_spot_market_request_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param SpotMarketRequestArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/ssh_key.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/ssh_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -180,15 +180,19 @@
             name="johnKent",
             public_key=(lambda path: open(path).read())("/Users/John/.ssh/metal_rsa.pub"))
         pulumi.export("sshKeyId", ssh_key.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing SSH Key ID:<break><break> ```sh<break> $ pulumi import equinix:metal/sshKey:SshKey equinix_metal_ssh_key {existing_sshkey_id} <break>```<break><break>
+        This resource can be imported using an existing SSH Key ID:
+
+        ```sh
+        $ pulumi import equinix:metal/sshKey:SshKey equinix_metal_ssh_key {existing_sshkey_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: The name of the SSH key for identification
         :param pulumi.Input[str] public_key: The public key. If this is a file, it
                can be read using the file interpolation function
         """
@@ -212,15 +216,19 @@
             name="johnKent",
             public_key=(lambda path: open(path).read())("/Users/John/.ssh/metal_rsa.pub"))
         pulumi.export("sshKeyId", ssh_key.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing SSH Key ID:<break><break> ```sh<break> $ pulumi import equinix:metal/sshKey:SshKey equinix_metal_ssh_key {existing_sshkey_id} <break>```<break><break>
+        This resource can be imported using an existing SSH Key ID:
+
+        ```sh
+        $ pulumi import equinix:metal/sshKey:SshKey equinix_metal_ssh_key {existing_sshkey_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param SshKeyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/user_api_key.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/user_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/virtual_circuit.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/virtual_circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -613,15 +613,19 @@
             nni_vlan=1056)
         pulumi.export("vcStatus", vc.status)
         pulumi.export("vcVnid", vc.vnid)
         ```
 
         ## Import
 
-        This resource can be imported using an existing Virtual Circuit ID:<break><break> ```sh<break> $ pulumi import equinix:metal/virtualCircuit:VirtualCircuit equinix_metal_virtual_circuit {existing_id} <break>```<break><break>
+        This resource can be imported using an existing Virtual Circuit ID:
+
+        ```sh
+        $ pulumi import equinix:metal/virtualCircuit:VirtualCircuit equinix_metal_virtual_circuit {existing_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] connection_id: UUID of Connection where the VC is scoped to.
         :param pulumi.Input[str] customer_ip: The Customer IP address which the CSR switch will peer with. Will default to the other usable IP in the subnet.
         :param pulumi.Input[str] description: Description for the Virtual Circuit resource.
         :param pulumi.Input[str] md5: The password that can be set for the VRF BGP peer
@@ -671,15 +675,19 @@
             nni_vlan=1056)
         pulumi.export("vcStatus", vc.status)
         pulumi.export("vcVnid", vc.vnid)
         ```
 
         ## Import
 
-        This resource can be imported using an existing Virtual Circuit ID:<break><break> ```sh<break> $ pulumi import equinix:metal/virtualCircuit:VirtualCircuit equinix_metal_virtual_circuit {existing_id} <break>```<break><break>
+        This resource can be imported using an existing Virtual Circuit ID:
+
+        ```sh
+        $ pulumi import equinix:metal/virtualCircuit:VirtualCircuit equinix_metal_virtual_circuit {existing_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param VirtualCircuitArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/vlan.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/vlan.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,19 @@
             metro=metro,
             vxlan=vxlan)
         pulumi.export("vlanId", vlan.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing VLAN ID (UUID):<break><break> ```sh<break> $ pulumi import equinix:metal/vlan:Vlan equinix_metal_vlan {existing_vlan_id} <break>```<break><break>
+        This resource can be imported using an existing VLAN ID (UUID):
+
+        ```sh
+        $ pulumi import equinix:metal/vlan:Vlan equinix_metal_vlan {existing_vlan_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description string.
         :param pulumi.Input[Union[str, 'Facility']] facility: Facility where to create the VLAN. Use metro instead; read the facility to metro migration guide
         :param pulumi.Input[str] metro: Metro in which to create the VLAN
         :param pulumi.Input[str] project_id: ID of parent project.
@@ -280,15 +284,19 @@
             metro=metro,
             vxlan=vxlan)
         pulumi.export("vlanId", vlan.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing VLAN ID (UUID):<break><break> ```sh<break> $ pulumi import equinix:metal/vlan:Vlan equinix_metal_vlan {existing_vlan_id} <break>```<break><break>
+        This resource can be imported using an existing VLAN ID (UUID):
+
+        ```sh
+        $ pulumi import equinix:metal/vlan:Vlan equinix_metal_vlan {existing_vlan_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param VlanArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -367,26 +375,26 @@
         """
         Description string.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
-    def facility(self) -> pulumi.Output[Optional[str]]:
+    def facility(self) -> pulumi.Output[str]:
         """
         Facility where to create the VLAN. Use metro instead; read the facility to metro migration guide
         """
         warnings.warn("""Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""", DeprecationWarning)
         pulumi.log.warn("""facility is deprecated: Use metro instead of facility.  For more information, read the migration guide: https://registry.terraform.io/providers/equinix/equinix/latest/docs/guides/migration_guide_facilities_to_metros_devices""")
 
         return pulumi.get(self, "facility")
 
     @property
     @pulumi.getter
-    def metro(self) -> pulumi.Output[Optional[str]]:
+    def metro(self) -> pulumi.Output[str]:
         """
         Metro in which to create the VLAN
         """
         return pulumi.get(self, "metro")
 
     @property
     @pulumi.getter(name="projectId")
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/metal/vrf.py` & `pulumi_equinix-0.7.3/pulumi_equinix/metal/vrf.py`

 * *Files 3% similar despite different names*

```diff
@@ -255,15 +255,19 @@
             ],
             project_id=project_id)
         pulumi.export("vrfId", vrf.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing VRF ID:<break><break> ```sh<break> $ pulumi import equinix:metal/vrf:Vrf equinix_metal_vrf {existing_id} <break>```<break><break>
+        This resource can be imported using an existing VRF ID:
+
+        ```sh
+        $ pulumi import equinix:metal/vrf:Vrf equinix_metal_vrf {existing_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Description of the VRF.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_ranges: All IPv4 and IPv6 Ranges that will be available to BGP Peers. IPv4 addresses must be /8 or smaller with a minimum size of /29. IPv6 must be /56 or smaller with a minimum size of /64. Ranges must not overlap other ranges within the VRF.
         :param pulumi.Input[int] local_asn: The 4-byte ASN set on the VRF.
         :param pulumi.Input[str] metro: Metro ID or Code where the VRF will be deployed.
@@ -302,15 +306,19 @@
             ],
             project_id=project_id)
         pulumi.export("vrfId", vrf.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing VRF ID:<break><break> ```sh<break> $ pulumi import equinix:metal/vrf:Vrf equinix_metal_vrf {existing_id} <break>```<break><break>
+        This resource can be imported using an existing VRF ID:
+
+        ```sh
+        $ pulumi import equinix:metal/vrf:Vrf equinix_metal_vrf {existing_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param VrfArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/__init__.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/_enums.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/_inputs.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/acl_template.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/acl_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,15 +332,19 @@
                 ),
             ])
         pulumi.export("templateId", acl_template.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing ID:<break><break> ```sh<break> $ pulumi import equinix:networkedge/aclTemplate:AclTemplate example {existing_id} <break>```<break><break>
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/aclTemplate:AclTemplate example {existing_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Inbound rule description, up to 200 characters.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AclTemplateInboundRuleArgs']]]] inbound_rules: One or more rules to specify allowed inbound traffic.
                Rules are ordered, matching traffic rule stops processing subsequent ones.
                
@@ -388,15 +392,19 @@
                 ),
             ])
         pulumi.export("templateId", acl_template.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing ID:<break><break> ```sh<break> $ pulumi import equinix:networkedge/aclTemplate:AclTemplate example {existing_id} <break>```<break><break>
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/aclTemplate:AclTemplate example {existing_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param AclTemplateArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/bgp.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/bgp.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,15 +318,19 @@
             authentication_key="secret")
         pulumi.export("state", bgp.state)
         pulumi.export("provisioningStatus", bgp.provisioning_status)
         ```
 
         ## Import
 
-        This resource can be imported using an existing ID:<break><break> ```sh<break> $ pulumi import equinix:networkedge/bgp:Bgp example {existing_id} <break>```<break><break>
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/bgp:Bgp example {existing_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] authentication_key: shared key used for BGP peer authentication.
         :param pulumi.Input[str] connection_id: identifier of a connection established between.
                network device and remote service provider that will be used for peering.
         :param pulumi.Input[int] local_asn: Local ASN number.
@@ -358,15 +362,19 @@
             authentication_key="secret")
         pulumi.export("state", bgp.state)
         pulumi.export("provisioningStatus", bgp.provisioning_status)
         ```
 
         ## Import
 
-        This resource can be imported using an existing ID:<break><break> ```sh<break> $ pulumi import equinix:networkedge/bgp:Bgp example {existing_id} <break>```<break><break>
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/bgp:Bgp example {existing_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param BgpArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/device.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1442,15 +1442,21 @@
         pulumi.export("provisionStatus", c8_k_router.status)
         pulumi.export("licenseStatus", c8_k_router.license_status)
         pulumi.export("sshIpAddress", c8_k_router.ssh_ip_address)
         ```
 
         ## Import
 
-        This resource can be imported using an existing ID:<break><break> ```sh<break> $ pulumi import equinix:networkedge/device:Device example {existing_id} <break>```<break><break> The `license_token`, `mgmt_acl_template_uuid` and `cloud_init_file_id` fields can not be imported.<break><break>
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/device:Device example {existing_id}
+        ```
+
+        The `license_token`, `mgmt_acl_template_uuid` and `cloud_init_file_id` fields can not be imported.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] account_number: Billing account number for a device.
         :param pulumi.Input[str] acl_template_id: Identifier of a WAN interface ACL template that will be applied on the device.
         :param pulumi.Input[int] additional_bandwidth: Additional Internet bandwidth, in Mbps, that will be
                allocated to the device (in addition to default 15Mbps).
@@ -1580,15 +1586,21 @@
         pulumi.export("provisionStatus", c8_k_router.status)
         pulumi.export("licenseStatus", c8_k_router.license_status)
         pulumi.export("sshIpAddress", c8_k_router.ssh_ip_address)
         ```
 
         ## Import
 
-        This resource can be imported using an existing ID:<break><break> ```sh<break> $ pulumi import equinix:networkedge/device:Device example {existing_id} <break>```<break><break> The `license_token`, `mgmt_acl_template_uuid` and `cloud_init_file_id` fields can not be imported.<break><break>
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/device:Device example {existing_id}
+        ```
+
+        The `license_token`, `mgmt_acl_template_uuid` and `cloud_init_file_id` fields can not be imported.
 
         :param str resource_name: The name of the resource.
         :param DeviceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/device_link.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/device_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,15 +291,19 @@
             )])
         pulumi.export("status", device_link.status)
         pulumi.export("devices", device_link.devices)
         ```
 
         ## Import
 
-        This resource can be imported using an existing ID:<break><break> ```sh<break> $ pulumi import equinix:networkedge/deviceLink:DeviceLink example {existing_id} <break>```<break><break>
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/deviceLink:DeviceLink example {existing_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkDeviceArgs']]]] devices: definition of one or more devices belonging to the
                device link. See Device section below for more details.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['DeviceLinkLinkArgs']]]] links: definition of one or more, inter metro, connections belonging
                to the device link. See Link section below for more details.
@@ -357,15 +361,19 @@
             )])
         pulumi.export("status", device_link.status)
         pulumi.export("devices", device_link.devices)
         ```
 
         ## Import
 
-        This resource can be imported using an existing ID:<break><break> ```sh<break> $ pulumi import equinix:networkedge/deviceLink:DeviceLink example {existing_id} <break>```<break><break>
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/deviceLink:DeviceLink example {existing_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param DeviceLinkArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/get_account.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/get_account.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,23 +114,25 @@
     billing account in a given metro location.
 
     Billing account reference is required to create Network Edge virtual device
     in corresponding metro location.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     dc = equinix.networkedge.get_account(metro_code="DC",
         status="Active",
         project_id="a86d7112-d740-4758-9c9c-31e66373746b")
     pulumi.export("number", dc.number)
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str metro_code: Account location metro code.
     :param str name: Account name for filtering.
     :param str project_id: Unique Identifier for the project resource where the account is scoped to.If you
            leave it out, all the billing accounts under all projects in your organization will be returned and it may return more than one account.
     :param str status: Account status for filtering. Possible values are: `Active`, `Processing`,
@@ -165,23 +167,25 @@
     billing account in a given metro location.
 
     Billing account reference is required to create Network Edge virtual device
     in corresponding metro location.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     dc = equinix.networkedge.get_account(metro_code="DC",
         status="Active",
         project_id="a86d7112-d740-4758-9c9c-31e66373746b")
     pulumi.export("number", dc.number)
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str metro_code: Account location metro code.
     :param str name: Account name for filtering.
     :param str project_id: Unique Identifier for the project resource where the account is scoped to.If you
            leave it out, all the billing accounts under all projects in your organization will be returned and it may return more than one account.
     :param str status: Account status for filtering. Possible values are: `Active`, `Processing`,
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/get_device.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/get_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -536,21 +536,23 @@
                valid_status_list: Optional[str] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDeviceResult:
     """
     Use this data source to get Equinix Network Edge device details.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     by_uuid = equinix.networkedge.get_device(uuid="f0b5c553-cdeb-4bc3-95b8-23db9ccfd5ee")
     by_name = equinix.networkedge.get_device(name="Arcus-Gateway-A1")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str name: Name of an existing Equinix Network Edge device
     :param str uuid: UUID of an existing Equinix Network Edge device
     :param str valid_status_list: Device states to be considered valid when searching for a device by name
            
            NOTE: Exactly one of either `uuid` or `name` must be specified.
@@ -617,21 +619,23 @@
                       valid_status_list: Optional[pulumi.Input[Optional[str]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDeviceResult]:
     """
     Use this data source to get Equinix Network Edge device details.
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     by_uuid = equinix.networkedge.get_device(uuid="f0b5c553-cdeb-4bc3-95b8-23db9ccfd5ee")
     by_name = equinix.networkedge.get_device(name="Arcus-Gateway-A1")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str name: Name of an existing Equinix Network Edge device
     :param str uuid: UUID of an existing Equinix Network Edge device
     :param str valid_status_list: Device states to be considered valid when searching for a device by name
            
            NOTE: Exactly one of either `uuid` or `name` must be specified.
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/get_device_platform.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/get_device_platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,22 +132,24 @@
     """
     Use this data source to get Equinix Network Edge device platform configuration details
     for a given device type. For further details, check supported
     [Network Edge Vendors and Devices](https://docs.equinix.com/en-us/Content/Interconnection/NE/user-guide/NE-vendors-devices.htm).
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     csr_large = equinix.networkedge.get_device_platform(device_type="CSR1000V",
         flavor="large",
         packages=["IPBASE"])
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param int core_count: Number of CPU cores used to limit platform search results.
     :param str device_type: Device type code
     :param str flavor: Device platform flavor that determines number of CPU cores and memory.
            Supported values are: `small`, `medium`, `large`, `xlarge`.
     :param Sequence[str] license_options: List of device licensing options to limit platform search result.
@@ -189,22 +191,24 @@
     """
     Use this data source to get Equinix Network Edge device platform configuration details
     for a given device type. For further details, check supported
     [Network Edge Vendors and Devices](https://docs.equinix.com/en-us/Content/Interconnection/NE/user-guide/NE-vendors-devices.htm).
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     csr_large = equinix.networkedge.get_device_platform(device_type="CSR1000V",
         flavor="large",
         packages=["IPBASE"])
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param int core_count: Number of CPU cores used to limit platform search results.
     :param str device_type: Device type code
     :param str flavor: Device platform flavor that determines number of CPU cores and memory.
            Supported values are: `small`, `medium`, `large`, `xlarge`.
     :param Sequence[str] license_options: List of device licensing options to limit platform search result.
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/get_device_software.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/get_device_software.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,23 +158,25 @@
     """
     Use this data source to get Equinix Network Edge device software details for a given
     device type. For further details, check supported
     [Network Edge Vendors and Devices](https://docs.equinix.com/en-us/Content/Interconnection/NE/user-guide/NE-vendors-devices.htm).
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     csr_latest1609 = equinix.networkedge.get_device_software(device_type="CSR1000V",
         most_recent=True,
         packages=["IPBASE"],
         version_regex="^16.09.+")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str device_type: Code of a device type.
     :param bool most_recent: Boolean value to indicate that most recent version should be used *(in
            case when more than one result is returned)*.
     :param Sequence[str] packages: Limits returned versions to those that are supported by given software
            package codes.
@@ -215,23 +217,25 @@
     """
     Use this data source to get Equinix Network Edge device software details for a given
     device type. For further details, check supported
     [Network Edge Vendors and Devices](https://docs.equinix.com/en-us/Content/Interconnection/NE/user-guide/NE-vendors-devices.htm).
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     csr_latest1609 = equinix.networkedge.get_device_software(device_type="CSR1000V",
         most_recent=True,
         packages=["IPBASE"],
         version_regex="^16.09.+")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str device_type: Code of a device type.
     :param bool most_recent: Boolean value to indicate that most recent version should be used *(in
            case when more than one result is returned)*.
     :param Sequence[str] packages: Limits returned versions to those that are supported by given software
            package codes.
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/get_device_type.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/get_device_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,25 +111,27 @@
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDeviceTypeResult:
     """
     Use this data source to get Equinix Network Edge device type details. For further details, check supported
     [Network Edge Vendors and Devices](https://docs.equinix.com/en-us/Content/Interconnection/NE/user-guide/NE-vendors-devices.htm).
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     cisco_router = equinix.networkedge.get_device_type(category="Router",
         metro_codes=[
             "DC",
             "SV",
         ],
         vendor="Cisco")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str category: Device type category. One of: `Router`, `Firewall`, `SDWAN`.
     :param Sequence[str] metro_codes: List of metro codes where device type has to be available
     :param str name: Device type name.
     :param str vendor: Device type vendor i.e. `Cisco`, `Juniper Networks`, `VERSA Networks`.
     """
@@ -159,25 +161,27 @@
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDeviceTypeResult]:
     """
     Use this data source to get Equinix Network Edge device type details. For further details, check supported
     [Network Edge Vendors and Devices](https://docs.equinix.com/en-us/Content/Interconnection/NE/user-guide/NE-vendors-devices.htm).
 
     ## Example Usage
 
+    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_equinix as equinix
 
     cisco_router = equinix.networkedge.get_device_type(category="Router",
         metro_codes=[
             "DC",
             "SV",
         ],
         vendor="Cisco")
     ```
+    <!--End PulumiCodeChooser -->
 
 
     :param str category: Device type category. One of: `Router`, `Firewall`, `SDWAN`.
     :param Sequence[str] metro_codes: List of metro codes where device type has to be available
     :param str name: Device type name.
     :param str vendor: Device type vendor i.e. `Cisco`, `Juniper Networks`, `VERSA Networks`.
     """
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/network_file.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/network_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,15 +321,21 @@
             byol=True)
         pulumi.export("networkFileId", network_file.id)
         pulumi.export("networkFileStatus", network_file.status)
         ```
 
         ## Import
 
-        This resource can be imported using an existing ID:<break><break> ```sh<break> $ pulumi import equinix:networkedge/networkFile:NetworkFile example {existing_id} <break>```<break><break> The `content`, `self_managed` and `byol` fields can not be imported.<break><break>
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/networkFile:NetworkFile example {existing_id}
+        ```
+
+        The `content`, `self_managed` and `byol` fields can not be imported.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] byol: Boolean value that determines device licensing mode, i.e.,
                `bring your own license` or `subscription`.
         :param pulumi.Input[str] content: Uploaded file content, expected to be a UTF-8 encoded string.
         :param pulumi.Input[str] device_type_code: Device type code
@@ -367,15 +373,21 @@
             byol=True)
         pulumi.export("networkFileId", network_file.id)
         pulumi.export("networkFileStatus", network_file.status)
         ```
 
         ## Import
 
-        This resource can be imported using an existing ID:<break><break> ```sh<break> $ pulumi import equinix:networkedge/networkFile:NetworkFile example {existing_id} <break>```<break><break> The `content`, `self_managed` and `byol` fields can not be imported.<break><break>
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/networkFile:NetworkFile example {existing_id}
+        ```
+
+        The `content`, `self_managed` and `byol` fields can not be imported.
 
         :param str resource_name: The name of the resource.
         :param NetworkFileArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/outputs.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/ssh_key.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/ssh_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -200,15 +200,19 @@
             name="johnKent",
             public_key=(lambda path: open(path).read())("/Users/John/.ssh/ne_rsa.pub"))
         pulumi.export("sshKeyId", ssh_key.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing ID:<break><break> ```sh<break> $ pulumi import equinix:networkedge/sshKey:SshKey example {existing_id} <break>```<break><break>
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/sshKey:SshKey example {existing_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: The name of SSH key used for identification.
         :param pulumi.Input[str] project_id: Unique Identifier for the project resource where the SSH key is scoped to.If you
                leave it out, the ssh key will be created under the default project id of your organization.
         :param pulumi.Input[str] public_key: The SSH public key. If this is a file, it can be read using the file
@@ -233,15 +237,19 @@
             name="johnKent",
             public_key=(lambda path: open(path).read())("/Users/John/.ssh/ne_rsa.pub"))
         pulumi.export("sshKeyId", ssh_key.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing ID:<break><break> ```sh<break> $ pulumi import equinix:networkedge/sshKey:SshKey example {existing_id} <break>```<break><break>
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/sshKey:SshKey example {existing_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param SshKeyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/networkedge/ssh_user.py` & `pulumi_equinix-0.7.3/pulumi_equinix/networkedge/ssh_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,15 +164,19 @@
                 device2_id,
             ])
         pulumi.export("sshUserId", ssh_user.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing ID:<break><break> ```sh<break> $ pulumi import equinix:networkedge/sshUser:SshUser example {existing_id} <break>```<break><break>
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/sshUser:SshUser example {existing_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] device_ids: list of device identifiers to which user will have access.
         :param pulumi.Input[str] password: SSH user password.
         :param pulumi.Input[str] username: SSH user login name.
         """
@@ -201,15 +205,19 @@
                 device2_id,
             ])
         pulumi.export("sshUserId", ssh_user.id)
         ```
 
         ## Import
 
-        This resource can be imported using an existing ID:<break><break> ```sh<break> $ pulumi import equinix:networkedge/sshUser:SshUser example {existing_id} <break>```<break><break>
+        This resource can be imported using an existing ID:
+
+        ```sh
+        $ pulumi import equinix:networkedge/sshUser:SshUser example {existing_id}
+        ```
 
         :param str resource_name: The name of the resource.
         :param SshUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix/provider.py` & `pulumi_equinix-0.7.3/pulumi_equinix/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix.egg-info/PKG-INFO` & `pulumi_equinix-0.7.3/pulumi_equinix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-equinix
-Version: 0.7.2
+Version: 0.7.3
 Summary: A Pulumi package for creating and managing equinix cloud resources.
 Home-page: https://deploy.equinix.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/equinix/pulumi-equinix
 Keywords: pulumi equinix category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_equinix-0.7.2/pulumi_equinix.egg-info/SOURCES.txt` & `pulumi_equinix-0.7.3/pulumi_equinix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.7.2/setup.py` & `pulumi_equinix-0.7.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import errno
-import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.7.2"
+VERSION = "0.7.3"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "equinix Pulumi Package - Development Version"
```

