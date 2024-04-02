# Comparing `tmp/cyclonedx_editor_validator-0.9.3.tar.gz` & `tmp/cyclonedx_editor_validator-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclonedx_editor_validator-0.9.3.tar", max compression
+gzip compressed data, was "cyclonedx_editor_validator-0.9.4.tar", max compression
```

## Comparing `cyclonedx_editor_validator-0.9.3.tar` & `cyclonedx_editor_validator-0.9.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    35114 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/LICENSE
--rw-r--r--   0        0        0     1302 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/README.md
--rw-r--r--   0        0        0       34 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/__init__.py
--rw-r--r--   0        0        0    20468 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/__main__.py
--rw-r--r--   0        0        0      390 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/amend/__init__.py
--rw-r--r--   0        0        0     1501 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/amend/command.py
--rw-r--r--   0        0        0    59830 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/amend/license_name_spdx_id_map.json
--rw-r--r--   0        0        0     7193 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/amend/operations.py
--rw-r--r--   0        0        0     7122 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/amend/process_license.py
--rw-r--r--   0        0        0        0 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/__init__.py
--rw-r--r--   0        0        0     5793 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/identity.py
--rw-r--r--   0        0        0     3854 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/output.py
--rw-r--r--   0        0        0    10454 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/sbomFunctions.py
--rw-r--r--   0        0        0        0 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/__init__.py
--rw-r--r--   0        0        0    13619 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.0.xsd
--rw-r--r--   0        0        0    39484 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.1.xsd
--rw-r--r--   0        0        0    37056 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.2-strict.schema.json
--rw-r--r--   0        0        0    36058 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.2.schema.json
--rw-r--r--   0        0        0    76147 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.2.xsd
--rw-r--r--   0        0        0    44063 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.3-custom.schema.json
--rw-r--r--   0        0        0    40239 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.3-strict.schema.json
--rw-r--r--   0        0        0    23176 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.3.proto
--rw-r--r--   0        0        0    39180 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.3.schema.json
--rw-r--r--   0        0        0    88384 2024-01-23 07:21:48.350190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.3.xsd
--rw-r--r--   0        0        0    77034 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.4-custom.schema.json
--rw-r--r--   0        0        0    34897 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.4.proto
--rw-r--r--   0        0        0    72249 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.4.schema.json
--rw-r--r--   0        0        0   133616 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.4.xsd
--rw-r--r--   0        0        0   167339 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.5-custom.schema.json
--rw-r--r--   0        0        0    77165 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.5.proto
--rw-r--r--   0        0        0   164769 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.5.schema.json
--rw-r--r--   0        0        0   311801 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.5.xsd
--rw-r--r--   0        0        0     9063 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/ext/bom-descriptor-0.9.xsd
--rw-r--r--   0        0        0     8233 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/ext/bom-descriptor-1.0.xsd
--rw-r--r--   0        0        0     3146 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/ext/dependency-graph-1.0.xsd
--rw-r--r--   0        0        0     6380 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/ext/vulnerability-1.0-SNAPSHOT.schema.json
--rw-r--r--   0        0        0    14195 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/ext/vulnerability-1.0.xsd
--rw-r--r--   0        0        0     8210 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/jsf-0.82.schema.json
--rw-r--r--   0        0        0    10482 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/spdx.schema.json
--rw-r--r--   0        0        0   125048 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/spdx.xsd
--rw-r--r--   0        0        0     5646 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/build_public_bom.py
--rw-r--r--   0        0        0     2642 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/error.py
--rw-r--r--   0        0        0     2763 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/log.py
--rw-r--r--   0        0        0    18104 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/merge.py
--rw-r--r--   0        0        0     2702 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/merge_vex.py
--rw-r--r--   0        0        0      135 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/pkg.py
--rw-r--r--   0        0        0     7573 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/set.py
--rw-r--r--   0        0        0       65 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/validator/__init__.py
--rw-r--r--   0        0        0     5570 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/validator/customreports.py
--rw-r--r--   0        0        0     4827 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/validator/helper.py
--rw-r--r--   0        0        0     7236 2024-01-23 07:21:48.354190 cyclonedx_editor_validator-0.9.3/cdxev/validator/validate.py
--rw-r--r--   0        0        0     1667 2024-01-23 07:21:58.598190 cyclonedx_editor_validator-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     2347 1970-01-01 00:00:00.000000 cyclonedx_editor_validator-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    35114 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/LICENSE
+-rw-r--r--   0        0        0     1302 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/README.md
+-rw-r--r--   0        0        0       34 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/__init__.py
+-rw-r--r--   0        0        0    20546 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/__main__.py
+-rw-r--r--   0        0        0      390 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/amend/__init__.py
+-rw-r--r--   0        0        0     1501 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/amend/command.py
+-rw-r--r--   0        0        0    59830 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/amend/license_name_spdx_id_map.json
+-rw-r--r--   0        0        0     7194 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/amend/operations.py
+-rw-r--r--   0        0        0     7122 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/amend/process_license.py
+-rw-r--r--   0        0        0        0 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/__init__.py
+-rw-r--r--   0        0        0     5793 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/identity.py
+-rw-r--r--   0        0        0     3854 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/output.py
+-rw-r--r--   0        0        0    10454 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/sbomFunctions.py
+-rw-r--r--   0        0        0        0 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/__init__.py
+-rw-r--r--   0        0        0    13619 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.0.xsd
+-rw-r--r--   0        0        0    39484 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.1.xsd
+-rw-r--r--   0        0        0    37056 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.2-strict.schema.json
+-rw-r--r--   0        0        0    36058 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.2.schema.json
+-rw-r--r--   0        0        0    76147 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.2.xsd
+-rw-r--r--   0        0        0    44063 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.3-custom.schema.json
+-rw-r--r--   0        0        0    40239 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.3-strict.schema.json
+-rw-r--r--   0        0        0    23176 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.3.proto
+-rw-r--r--   0        0        0    39180 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.3.schema.json
+-rw-r--r--   0        0        0    88384 2024-01-31 11:48:17.498865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.3.xsd
+-rw-r--r--   0        0        0    77034 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.4-custom.schema.json
+-rw-r--r--   0        0        0    34897 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.4.proto
+-rw-r--r--   0        0        0    72249 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.4.schema.json
+-rw-r--r--   0        0        0   133616 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.4.xsd
+-rw-r--r--   0        0        0   167339 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.5-custom.schema.json
+-rw-r--r--   0        0        0    77165 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.5.proto
+-rw-r--r--   0        0        0   164769 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.5.schema.json
+-rw-r--r--   0        0        0   311801 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.5.xsd
+-rw-r--r--   0        0        0     9063 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/ext/bom-descriptor-0.9.xsd
+-rw-r--r--   0        0        0     8233 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/ext/bom-descriptor-1.0.xsd
+-rw-r--r--   0        0        0     3146 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/ext/dependency-graph-1.0.xsd
+-rw-r--r--   0        0        0     6380 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/ext/vulnerability-1.0-SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    14195 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/ext/vulnerability-1.0.xsd
+-rw-r--r--   0        0        0     8210 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/jsf-0.82.schema.json
+-rw-r--r--   0        0        0    10482 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/spdx.schema.json
+-rw-r--r--   0        0        0   125048 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/spdx.xsd
+-rw-r--r--   0        0        0     5646 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/build_public_bom.py
+-rw-r--r--   0        0        0     2642 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/error.py
+-rw-r--r--   0        0        0     2763 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/log.py
+-rw-r--r--   0        0        0    18106 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/merge.py
+-rw-r--r--   0        0        0     2702 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/merge_vex.py
+-rw-r--r--   0        0        0      135 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/pkg.py
+-rw-r--r--   0        0        0     7573 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/set.py
+-rw-r--r--   0        0        0       65 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/validator/__init__.py
+-rw-r--r--   0        0        0     5570 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/validator/customreports.py
+-rw-r--r--   0        0        0     4827 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/validator/helper.py
+-rw-r--r--   0        0        0     7236 2024-01-31 11:48:17.502865 cyclonedx_editor_validator-0.9.4/cdxev/validator/validate.py
+-rw-r--r--   0        0        0     1666 2024-01-31 11:48:28.359007 cyclonedx_editor_validator-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     2347 1970-01-01 00:00:00.000000 cyclonedx_editor_validator-0.9.4/PKG-INFO
```

### Comparing `cyclonedx_editor_validator-0.9.3/LICENSE` & `cyclonedx_editor_validator-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/README.md` & `cyclonedx_editor_validator-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/__main__.py` & `cyclonedx_editor_validator-0.9.4/cdxev/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,17 +527,21 @@
         elif args.value is None:
             usage_error("--value is required, unless the --from-file option is used.")
 
         possible_targets = [
             args.swid,
             args.purl,
             args.cpe,
-            Key.from_coordinates(name=args.name, version=args.version, group=args.group)
-            if args.name is not None
-            else None,
+            (
+                Key.from_coordinates(
+                    name=args.name, version=args.version, group=args.group
+                )
+                if args.name is not None
+                else None
+            ),
         ]
         actual_targets = [x for x in possible_targets if x is not None]
         if len(actual_targets) > 1:
             usage_error("Cannot specify more than one <target>.")
 
         target: Key = actual_targets[0]
         try:
```

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/amend/command.py` & `cyclonedx_editor_validator-0.9.4/cdxev/amend/command.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/amend/license_name_spdx_id_map.json` & `cyclonedx_editor_validator-0.9.4/cdxev/amend/license_name_spdx_id_map.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/amend/operations.py` & `cyclonedx_editor_validator-0.9.4/cdxev/amend/operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module defines the amend operations which can be performed on an SBOM.
 It also declares a base class to inherit from when implementing new operations.
 """
+
 import importlib.resources
 import json
 import logging
 import uuid
 
 from cdxev.amend.process_license import process_license
```

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/amend/process_license.py` & `cyclonedx_editor_validator-0.9.4/cdxev/amend/process_license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/identity.py` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/identity.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/output.py` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/output.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/sbomFunctions.py` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/sbomFunctions.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.0.xsd` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.0.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.1.xsd` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.1.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.2-strict.schema.json` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.2-strict.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.2.schema.json` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.2.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.2.xsd` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.2.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.3-custom.schema.json` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.3-custom.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.3-strict.schema.json` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.3-strict.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.3.proto` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.3.proto`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.3.schema.json` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.3.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.3.xsd` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.3.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.4-custom.schema.json` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.4-custom.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.4.proto` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.4.proto`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.4.schema.json` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.4.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.4.xsd` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.4.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.5-custom.schema.json` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.5-custom.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.5.proto` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.5.proto`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.5.schema.json` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.5.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/bom-1.5.xsd` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/bom-1.5.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/ext/bom-descriptor-0.9.xsd` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/ext/bom-descriptor-0.9.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/ext/bom-descriptor-1.0.xsd` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/ext/bom-descriptor-1.0.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/ext/dependency-graph-1.0.xsd` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/ext/dependency-graph-1.0.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/ext/vulnerability-1.0-SNAPSHOT.schema.json` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/ext/vulnerability-1.0-SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/ext/vulnerability-1.0.xsd` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/ext/vulnerability-1.0.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/jsf-0.82.schema.json` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/jsf-0.82.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/spdx.schema.json` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/spdx.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/auxiliary/schema/spdx.xsd` & `cyclonedx_editor_validator-0.9.4/cdxev/auxiliary/schema/spdx.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/build_public_bom.py` & `cyclonedx_editor_validator-0.9.4/cdxev/build_public_bom.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/error.py` & `cyclonedx_editor_validator-0.9.4/cdxev/error.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/log.py` & `cyclonedx_editor_validator-0.9.4/cdxev/log.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/merge.py` & `cyclonedx_editor_validator-0.9.4/cdxev/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,17 +272,17 @@
                     merged_ratings = merge_ratings(
                         original_vulnerability.get("ratings", []),
                         vulnerability.get("ratings", 2),
                         time_flag,
                     )
                     entry_of_merged_vulnerability["ratings"] = merged_ratings
                 elif original_vulnerability.get("ratings", []):
-                    entry_of_merged_vulnerability[
-                        "ratings"
-                    ] = original_vulnerability.get("ratings", 2)
+                    entry_of_merged_vulnerability["ratings"] = (
+                        original_vulnerability.get("ratings", 2)
+                    )
                 elif vulnerability.get("ratings", []):
                     entry_of_merged_vulnerability["ratings"] = vulnerability.get(
                         "ratings", 2
                     )
                 list_of_merged_vulnerabilities.append(entry_of_merged_vulnerability)
         if not is_in:
             list_of_merged_vulnerabilities.append(vulnerability)
```

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/merge_vex.py` & `cyclonedx_editor_validator-0.9.4/cdxev/merge_vex.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/set.py` & `cyclonedx_editor_validator-0.9.4/cdxev/set.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/validator/customreports.py` & `cyclonedx_editor_validator-0.9.4/cdxev/validator/customreports.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/validator/helper.py` & `cyclonedx_editor_validator-0.9.4/cdxev/validator/helper.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_editor_validator-0.9.3/cdxev/validator/validate.py` & `cyclonedx_editor_validator-0.9.4/cdxev/validator/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                             dependencies[int(index_ref)]["ref"]
                             + " has the mistake: the dependencies in dependsOn are non-unique"
                         )
                     else:
                         errors.append(
                             "SBOM has the mistake: Could not find reference for dependencies"
                         )
-                elif "too short" in error.message:
+                elif "non-empty" in error.message:
                     errors.append(
                         error_path
                         + "'"
                         + error.absolute_path[-1]
                         + "' should be non-empty"
                     )
                 elif error.validator == "pattern":
```

### Comparing `cyclonedx_editor_validator-0.9.3/pyproject.toml` & `cyclonedx_editor_validator-0.9.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cyclonedx-editor-validator"
-version = "v0.9.3"
+version = "v0.9.4"
 description = "Tool for creating, modifying and validating CycloneDX SBOMs."
 authors = [
     "Aleg Vilinski <aleg.vilinski@festo.com>",
     "Christian Beck <christian.beck@festo.com>",
     "Moritz Marseu <moritz.marseu@festo.com>"
 ]
 license = "GPL-3.0-only"
@@ -23,24 +23,24 @@
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dateutil = "2.8.2"
 jsonschema = {version = "4.21.1", extras = ["format"]}
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "7.0.0"
-black = "23.12.1"
+black = "24.1.1"
 pep8-naming = "0.13.3"
 mypy = "1.8.0"
 types-python-dateutil = "2.8.19.20240106"
 types-jsonschema = "4.21.0.20240118"
-pytest = "7.4.4"
-coverage = "7.4.0"
+pytest = "8.0.0"
+coverage = "7.4.1"
 toml = "0.10.2"
 typing-extensions = "4.9.0"
-bandit = "1.7.6"
+bandit = "1.7.7"
 isort = "5.13.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
```

### Comparing `cyclonedx_editor_validator-0.9.3/PKG-INFO` & `cyclonedx_editor_validator-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclonedx-editor-validator
-Version: 0.9.3
+Version: 0.9.4
 Summary: Tool for creating, modifying and validating CycloneDX SBOMs.
 License: GPL-3.0-only
 Author: Aleg Vilinski
 Author-email: aleg.vilinski@festo.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

