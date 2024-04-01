# Comparing `tmp/traffic_taffy-0.8.1.tar.gz` & `tmp/traffic_taffy-0.8.5.tar.gz`

## Comparing `traffic_taffy-0.8.1.tar` & `traffic_taffy-0.8.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/__init__.py
--rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/compare.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/comparison.py
--rw-r--r--   0        0        0    17390 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/dissection.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/dissectmany.py
--rw-r--r--   0        0        0    11685 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/dissector.py
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/graph.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/graphdata.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/report.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/algorithms/__init__.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/algorithms/statistical.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/dissector_engine/__init__.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/dissector_engine/dnstap.py
--rw-r--r--   0        0        0    10949 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/dissector_engine/dpkt.py
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/dissector_engine/scapy.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/hooks/__init__.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/hooks/ip2asn.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/hooks/psl.py
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/output/__init__.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/output/console.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/output/fsdb.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/output/memory.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tests/test_compare_results.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tests/test_dict_merge.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tests/test_dpkt_engine.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tests/test_hooks.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tests/test_normalize.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tests/test_pcap_dissector.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tests/test_pcap_splitter.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tests/test_splitter.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tests/test_value_printing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tools/__init__.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tools/cache_info.py
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tools/compare.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tools/dissect.py
--rw-r--r--   0        0        0    24180 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tools/explore.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tools/export.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/traffic_taffy/tools/graph.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/.gitignore
--rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/LICENSE.txt
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/README.md
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 traffic_taffy-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/__init__.py
+-rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/compare.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/comparison.py
+-rw-r--r--   0        0        0    21567 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/dissection.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/dissectmany.py
+-rw-r--r--   0        0        0    11685 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/dissector.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/graph.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/graphdata.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/report.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/algorithms/__init__.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/algorithms/statistical.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/dissector_engine/__init__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/dissector_engine/dnstap.py
+-rw-r--r--   0        0        0    10949 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/dissector_engine/dpkt.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/dissector_engine/scapy.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/hooks/__init__.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/hooks/ip2asn.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/hooks/psl.py
+-rw-r--r--   0        0        0   172825 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/iana/tables.msgpak
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/output/__init__.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/output/console.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/output/fsdb.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/output/memory.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/tests/test_compare_results.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/tests/test_dict_merge.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/tests/test_hooks.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/tests/test_normalize.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/tests/test_pcap_dissector.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/tests/test_pcap_splitter.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/tests/test_splitter.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/tests/test_value_printing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/tools/__init__.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/tools/cache_info.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/tools/compare.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/tools/dissect.py
+-rw-r--r--   0        0        0    24180 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/tools/explore.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/tools/export.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/traffic_taffy/tools/graph.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/.gitignore
+-rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/LICENSE.txt
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/README.md
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 traffic_taffy-0.8.5/PKG-INFO
```

### Comparing `traffic_taffy-0.8.1/traffic_taffy/compare.py` & `traffic_taffy-0.8.5/traffic_taffy/compare.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/comparison.py` & `traffic_taffy-0.8.5/traffic_taffy/comparison.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/dissection.py` & `traffic_taffy-0.8.5/traffic_taffy/dissection.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,31 @@
 from enum import Enum
 import msgpack
 import ipaddress
 from typing import List
 from copy import deepcopy
 from pathlib import Path
 from traffic_taffy import __VERSION__ as VERSION
+from io import BytesIO
+import pkgutil
+
+# TODO(hardaker): fix to not use a global
+# note that this is designed to load only once before forking
+iana_data = None
+if not iana_data:
+    # try a local copy first
+    if Path("traffic_taffy/iana/tables.msgpakx").exists():
+        iana_data = msgpack.load(Path.open("traffic_taffy/iana/tables.msgpak", "rb"))
+    else:
+        content = pkgutil.get_data("traffic_taffy", "iana/tables.msgpak")
+        if content:
+            content = BytesIO(content)
+            iana_data = msgpack.load(content)
+        else:
+            warning("failed to load IANA data tables -- no enum expansion available")
 
 
 class PCAPDissectorLevel(Enum):
     """Enumeration of supported dissection levels."""
 
     COUNT_ONLY = 1
     THROUGH_IP = 2
@@ -53,14 +70,15 @@
         self.cache_file_suffix = cache_file_suffix
         self._data = defaultdict(Dissection.subdict_producer)
         self._timestamp = 0
         self.dissector_level = dissector_level
         self.maximum_count = maximum_count
         self.pcap_filter = pcap_filter
         self.ignore_list = ignore_list or []
+        self.iana_data = defaultdict(dict)
 
         self.parameters = [
             "pcap_file",
             "bin_size",
             "dissector_level",
             "pcap_filter",
             "maximum_count",
@@ -417,14 +435,16 @@
             if isinstance(value, bytes):
                 if value_type in Dissection.DISPLAY_TRANSFORMERS:
                     value = str(
                         Dissection.DISPLAY_TRANSFORMERS[value_type](value_type, value)
                     )
                 else:
                     value = "0x" + value.hex()
+            elif value_type in Dissection.ENUM_TRANSLATORS:
+                value = str(Dissection.ENUM_TRANSLATORS[value_type](value_type, value))
             else:
                 value = str(value)
         except Exception:
             if isinstance(value, bytes):
                 value = "0x" + value.hex()
             else:
                 value = "[unprintable]"
@@ -444,14 +464,87 @@
         return ":".join(map(two_hex, value))
 
     @staticmethod
     def print_ip_address(value_type: str, value: bytes) -> str:
         """Convert binary bytes to IP addresses (v4 and v6)."""
         return ipaddress.ip_address(value)
 
+    UDP_PORTS: ClassVar[Dict[str, str]] = {
+        "53": "DNS",
+    }
+
+    IANA_TRANSLATORS: ClassVar[Dict[str, str]] = {
+        "Ethernet_IP_proto": "protocols",
+        "Ethernet_IPv6_proto": "protocols",
+        "Ethernet_IP_UDP_sport": "udp_ports",
+        "Ethernet_IP_UDP_dport": "udp_ports",
+        "Ethernet_IP_TCP_sport": "tcp_ports",
+        "Ethernet_IP_TCP_dport": "tcp_ports",
+        "Ethernet_IPv6_UDP_sport": "udp_ports",
+        "Ethernet_IPv6_UDP_dport": "udp_ports",
+        "Ethernet_IPv6_TCP_sport": "tcp_ports",
+        "Ethernet_IPv6_TCP_dport": "tcp_ports",
+        "Ethernet_IP_ICMP_code": "icmp_codes",
+        "Ethernet_IP_ICMP_type": "icmp_types",
+        "Ethernet_IP_ICMP_IP in ICMP_UDP in ICMP_dport": "udp_ports",
+        "Ethernet_IP_ICMP_IP in ICMP_UDP in ICMP_sport": "udp_ports",
+        "Ethernet_IP_ICMP_IP in ICMP_TCP in ICMP_dport": "tcp_ports",
+        "Ethernet_IP_ICMP_IP in ICMP_TCP in ICMP_sport": "tcp_ports",
+        "Ethernet_IP_ICMP_IP in ICMP_protoc": "protocols",
+        "Ethernet_IP_UDP_DNS_qd_qclass": "dns_classes",
+        "Ethernet_IP_UDP_DNS_ns_rclass": "dns_classes",
+        "Ethernet_IP_UDP_DNS_an_rclass": "dns_classes",
+        "Ethernet_IP_UDP_DNS_qd_qtype": "dns_rrtypes",
+        "Ethernet_IP_UDP_DNS_ns_type": "dns_rrtypes",
+        "Ethernet_IP_UDP_DNS_an_type": "dns_rrtypes",
+        "Ethernet_IP_UDP_DNS_opcode": "dns_opcodes",
+    }
+
+    @staticmethod
+    def print_iana_values(value_type: str, value: bytes) -> str:
+        """Use IANA lookup tables for converting protocol enumerations to human readable types."""
+        table_name = Dissection.IANA_TRANSLATORS.get(value_type)
+
+        if not table_name:
+            return value
+
+        table = iana_data[table_name]
+        value = str(value)
+        if value not in table:
+            return value
+
+        return f"{value} ({table[value]})"
+
+    ENUM_TRANSLATORS: ClassVar[Dict[str, callable]] = {
+        "Ethernet_IP_proto": print_iana_values,
+        "Ethernet_IPv6_proto": print_iana_values,
+        "Ethernet_IP_UDP_sport": print_iana_values,
+        "Ethernet_IP_UDP_dport": print_iana_values,
+        "Ethernet_IP_TCP_sport": print_iana_values,
+        "Ethernet_IP_TCP_dport": print_iana_values,
+        "Ethernet_IP_ICMP_IP in ICMP_UDP in ICMP_dport": print_iana_values,
+        "Ethernet_IP_ICMP_IP in ICMP_UDP in ICMP_sport": print_iana_values,
+        "Ethernet_IP_ICMP_IP in ICMP_TCP in ICMP_dport": print_iana_values,
+        "Ethernet_IP_ICMP_IP in ICMP_TCP in ICMP_sport": print_iana_values,
+        "Ethernet_IP_ICMP_IP in ICMP_proto": print_iana_values,
+        "Ethernet_IPv6_UDP_sport": print_iana_values,
+        "Ethernet_IPv6_UDP_dport": print_iana_values,
+        "Ethernet_IPv6_TCP_sport": print_iana_values,
+        "Ethernet_IPv6_TCP_dport": print_iana_values,
+        "Ethernet_IP_ICMP_code": print_iana_values,
+        "Ethernet_IP_ICMP_type": print_iana_values,
+        "Ethernet_IP_UDP_DNS_qd_qclass": print_iana_values,
+        "Ethernet_IP_UDP_DNS_ns_rclass": print_iana_values,
+        "Ethernet_IP_UDP_DNS_an_rclass": print_iana_values,
+        "Ethernet_IP_UDP_DNS_qd_qtype": print_iana_values,
+        "Ethernet_IP_UDP_DNS_ns_type": print_iana_values,
+        "Ethernet_IP_UDP_DNS_an_type": print_iana_values,
+        "Ethernet_IP_UDP_DNS_opcode": print_iana_values,
+    }
+
     # has to go at the end to pick up the above function names
     DISPLAY_TRANSFORMERS: ClassVar[Dict[str, callable]] = {
         "Ethernet_IP_src": print_ip_address,
         "Ethernet_IP_dst": print_ip_address,
         "Ethernet_IP6_src": print_ip_address,
         "Ethernet_IP6_dst": print_ip_address,
         "Ethernet_src": print_mac_address,
```

### Comparing `traffic_taffy-0.8.1/traffic_taffy/dissectmany.py` & `traffic_taffy-0.8.5/traffic_taffy/dissectmany.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/dissector.py` & `traffic_taffy-0.8.5/traffic_taffy/dissector.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/graph.py` & `traffic_taffy-0.8.5/traffic_taffy/graph.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/graphdata.py` & `traffic_taffy-0.8.5/traffic_taffy/graphdata.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/algorithms/statistical.py` & `traffic_taffy-0.8.5/traffic_taffy/algorithms/statistical.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/dissector_engine/__init__.py` & `traffic_taffy-0.8.5/traffic_taffy/dissector_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/dissector_engine/dnstap.py` & `traffic_taffy-0.8.5/traffic_taffy/dissector_engine/dnstap.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/dissector_engine/dpkt.py` & `traffic_taffy-0.8.5/traffic_taffy/dissector_engine/dpkt.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/dissector_engine/scapy.py` & `traffic_taffy-0.8.5/traffic_taffy/dissector_engine/scapy.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/hooks/__init__.py` & `traffic_taffy-0.8.5/traffic_taffy/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/hooks/ip2asn.py` & `traffic_taffy-0.8.5/traffic_taffy/hooks/ip2asn.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/hooks/psl.py` & `traffic_taffy-0.8.5/traffic_taffy/hooks/psl.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/output/__init__.py` & `traffic_taffy-0.8.5/traffic_taffy/output/__init__.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/output/console.py` & `traffic_taffy-0.8.5/traffic_taffy/output/console.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/output/fsdb.py` & `traffic_taffy-0.8.5/traffic_taffy/output/fsdb.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/output/memory.py` & `traffic_taffy-0.8.5/traffic_taffy/output/memory.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/tests/test_compare_results.py` & `traffic_taffy-0.8.5/traffic_taffy/tests/test_compare_results.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/tests/test_dict_merge.py` & `traffic_taffy-0.8.5/traffic_taffy/tests/test_dict_merge.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/tests/test_hooks.py` & `traffic_taffy-0.8.5/traffic_taffy/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/tests/test_normalize.py` & `traffic_taffy-0.8.5/traffic_taffy/tests/test_normalize.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/tests/test_pcap_dissector.py` & `traffic_taffy-0.8.5/traffic_taffy/tests/test_pcap_dissector.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/tests/test_pcap_splitter.py` & `traffic_taffy-0.8.5/traffic_taffy/tests/test_pcap_splitter.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/tests/test_splitter.py` & `traffic_taffy-0.8.5/traffic_taffy/tests/test_splitter.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/tools/cache_info.py` & `traffic_taffy-0.8.5/traffic_taffy/tools/cache_info.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/tools/compare.py` & `traffic_taffy-0.8.5/traffic_taffy/tools/compare.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/tools/dissect.py` & `traffic_taffy-0.8.5/traffic_taffy/tools/dissect.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/tools/explore.py` & `traffic_taffy-0.8.5/traffic_taffy/tools/explore.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/tools/export.py` & `traffic_taffy-0.8.5/traffic_taffy/tools/export.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/traffic_taffy/tools/graph.py` & `traffic_taffy-0.8.5/traffic_taffy/tools/graph.py`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/LICENSE.txt` & `traffic_taffy-0.8.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/README.md` & `traffic_taffy-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `traffic_taffy-0.8.1/pyproject.toml` & `traffic_taffy-0.8.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,17 @@
     "seaborn",
     "cryptography",
     "pyOpenSSL==22.1.0",
     "dnssplitter",
     "ip2asn",
 ]
 
+[project.package_data]
+"traffic_taffy.iana" = ['tables.msgpak']
+
 [project.scripts]
 taffy-cache-info = "traffic_taffy.tools.cache_info:main"
 taffy-compare = "traffic_taffy.tools.compare:main"
 taffy-dissect = "traffic_taffy.tools.dissect:main"
 taffy-explorer = "traffic_taffy.tools.explorer:main"
 taffy-graph = "traffic_taffy.tools.graph:main"
 taffy-export = "traffic_taffy.tools.export:main"
```

### Comparing `traffic_taffy-0.8.1/PKG-INFO` & `traffic_taffy-0.8.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traffic-taffy
-Version: 0.8.1
+Version: 0.8.5
 Summary: A tool for doing differential analysis of pcap files
 Project-URL: Homepage, https://traffic-taffy.github.io/
 Author-email: Wes Hardaker <opensource@hardakers.net>
 License-File: LICENSE.txt
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

