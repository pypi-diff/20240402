# Comparing `tmp/onnxscript-0.1.0.dev20240401.tar.gz` & `tmp/onnxscript-0.1.0.dev20240402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240401.tar", last modified: Mon Apr  1 00:01:19 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240402.tar", last modified: Tue Apr  2 00:02:42 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240401.tar` & `onnxscript-0.1.0.dev20240402.tar`

### file list

```diff
@@ -1,198 +1,211 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.371909 onnxscript-0.1.0.dev20240401/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-01 00:01:19.371909 onnxscript-0.1.0.dev20240401/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.335909 onnxscript-0.1.0.dev20240401/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2124 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.339909 onnxscript-0.1.0.dev20240401/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5284 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.339909 onnxscript-0.1.0.dev20240401/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.327909 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.339909 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.351909 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.327909 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.327909 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.351909 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.351909 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1285 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/_flags.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43396 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/graph_building.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.355908 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   288377 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/tensor_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19636 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.355908 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4509 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.359909 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   152497 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53435 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   156522 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    42746 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   139640 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19297 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50619 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20956 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    69354 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    74270 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58408 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39028 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13834 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/onnx_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/py.typed
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tensor.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11925 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/testing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.359909 onnxscript-0.1.0.dev20240401/onnxscript/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.359909 onnxscript-0.1.0.dev20240401/onnxscript/tests/common/
--rw-r--r--   0 vsts      (1001) docker     (127)       37 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/common/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10707 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/common/onnx_script_test_case.py
--rw-r--r--   0 vsts      (1001) docker     (127)      497 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/common/testutils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.327909 onnxscript-0.1.0.dev20240401/onnxscript/tests/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.363909 onnxscript-0.1.0.dev20240401/onnxscript/tests/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)     6115 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/function_libs/torch_lib/error_reproduction.py
--rw-r--r--   0 vsts      (1001) docker     (127)    79029 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23392 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/function_libs/torch_lib/ops_test_common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   102066 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/function_libs/torch_lib/ops_test_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.363909 onnxscript-0.1.0.dev20240401/onnxscript/tests/functions/
--rw-r--r--   0 vsts      (1001) docker     (127)      945 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/functions/gemmgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      993 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/functions/ort_custom_ops.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.371909 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      515 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/attrref.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2349 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/cast_like.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1380 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/different_opset.py
--rw-r--r--   0 vsts      (1001) docker     (127)      640 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/dropout.py
--rw-r--r--   0 vsts      (1001) docker     (127)      538 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/eager_op.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1140 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/eg1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4713 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/getitem.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2025 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/graph_attr.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1569 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/identity.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3093 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/if_statement.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/loops_break.py
--rw-r--r--   0 vsts      (1001) docker     (127)      863 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/loops_while.py
--rw-r--r--   0 vsts      (1001) docker     (127)      431 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/m1.py
--rw-r--r--   0 vsts      (1001) docker     (127)      441 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/multi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2907 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/onnxfns1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1965 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/onnxfns1A.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4969 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/onnxfns2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2564 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/opt_input.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2549 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/opt_output.py
--rw-r--r--   0 vsts      (1001) docker     (127)      642 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/renaming.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/sequences.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13534 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/signal_dft.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1432 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/subfunction.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2202 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/tests/models/type_double.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/type_annotation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24781 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-01 00:01:19.371909 onnxscript-0.1.0.dev20240401/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-01 00:01:19.000000 onnxscript-0.1.0.dev20240401/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     7536 2024-04-01 00:01:19.000000 onnxscript-0.1.0.dev20240401/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-01 00:01:19.000000 onnxscript-0.1.0.dev20240401/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-01 00:01:19.000000 onnxscript-0.1.0.dev20240401/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-01 00:01:19.000000 onnxscript-0.1.0.dev20240401/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     5273 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-01 00:01:19.371909 onnxscript-0.1.0.dev20240401/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-01 00:01:01.000000 onnxscript-0.1.0.dev20240401/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.420872 onnxscript-0.1.0.dev20240402/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-02 00:02:42.420872 onnxscript-0.1.0.dev20240402/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.384872 onnxscript-0.1.0.dev20240402/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2124 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.388872 onnxscript-0.1.0.dev20240402/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1081 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5284 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.388872 onnxscript-0.1.0.dev20240402/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10580 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.388872 onnxscript-0.1.0.dev20240402/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.380871 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.388872 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.400872 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.380871 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.380871 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.400872 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.400872 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1285 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/_flags.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43657 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/graph_building.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.404872 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   288377 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.404872 onnxscript-0.1.0.dev20240402/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1997 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50865 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1528 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2449 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      653 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1606 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2278 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10861 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1242 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/ir/convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43700 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19636 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.404872 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4509 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.412872 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   152497 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53435 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   156522 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    42746 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   139640 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19297 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50619 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20956 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    69354 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    74270 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58408 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39028 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13834 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/onnx_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tensor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11925 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/testing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.412872 onnxscript-0.1.0.dev20240402/onnxscript/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.412872 onnxscript-0.1.0.dev20240402/onnxscript/tests/common/
+-rw-r--r--   0 vsts      (1001) docker     (127)       37 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/common/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10707 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/common/onnx_script_test_case.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      497 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/common/testutils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.380871 onnxscript-0.1.0.dev20240402/onnxscript/tests/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.412872 onnxscript-0.1.0.dev20240402/onnxscript/tests/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6115 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/function_libs/torch_lib/error_reproduction.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    79029 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23392 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/function_libs/torch_lib/ops_test_common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   102066 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/function_libs/torch_lib/ops_test_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.412872 onnxscript-0.1.0.dev20240402/onnxscript/tests/functions/
+-rw-r--r--   0 vsts      (1001) docker     (127)      945 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/functions/gemmgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      993 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/functions/ort_custom_ops.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.420872 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      515 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/attrref.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2349 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/cast_like.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1380 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/different_opset.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      640 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/dropout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      538 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/eager_op.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1140 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/eg1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4713 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/getitem.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2025 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/graph_attr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1569 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/identity.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3093 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/if_statement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/loops_break.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      863 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/loops_while.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      431 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/m1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      441 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/multi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2907 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/onnxfns1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1965 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/onnxfns1A.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4969 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/onnxfns2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2564 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/opt_input.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2549 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/opt_output.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      642 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/renaming.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/sequences.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13534 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/signal_dft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1432 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/subfunction.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2202 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/tests/models/type_double.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/type_annotation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24781 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-02 00:02:42.420872 onnxscript-0.1.0.dev20240402/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10846 2024-04-02 00:02:42.000000 onnxscript-0.1.0.dev20240402/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     7845 2024-04-02 00:02:42.000000 onnxscript-0.1.0.dev20240402/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-02 00:02:42.000000 onnxscript-0.1.0.dev20240402/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-02 00:02:42.000000 onnxscript-0.1.0.dev20240402/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-02 00:02:42.000000 onnxscript-0.1.0.dev20240402/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     5163 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-02 00:02:42.420872 onnxscript-0.1.0.dev20240402/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-02 00:01:08.000000 onnxscript-0.1.0.dev20240402/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240401/LICENSE` & `onnxscript-0.1.0.dev20240402/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/PKG-INFO` & `onnxscript-0.1.0.dev20240402/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240401
+Version: 0.1.0.dev20240402
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240401/README.md` & `onnxscript-0.1.0.dev20240402/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240402/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240402/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240402/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240402/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240402/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240402/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240402/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240402/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240402/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240402/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240402/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240402/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240402/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240402/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/graph_building.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/graph_building.py`

 * *Files 0% similar despite different names*

```diff
@@ -818,17 +818,23 @@
         # Insert value info for nodes within nested function calls.
         # NOTE: This is an experimental feature, will be replaced by ValueInfo inside FunctionProto
         # in ONNX 1.16. https://github.com/microsoft/onnxscript/issues/1268
         # The naming strategy is subject to change. Since all local functions representing
         # nn.Modules exported by dynamo exporter have unique call sites, their function
         # op_type name can serve to form the unique identifier for value info.
         # Store inside top level GraphProto.
-        existing_value_info.update(self.generate_subgraphs_value_info_proto())
-        # Insert value info for nodes in top level graph.
-        existing_value_info.update(self.generate_maingraph_value_info_proto())
+        new_value_info = self.generate_maingraph_value_info_proto()
+        # Do not store input, output or initializer into value_info
+        for input in onnx_model.graph.input:
+            new_value_info.pop(input.name, None)
+        for output in onnx_model.graph.output:
+            new_value_info.pop(output.name, None)
+        for tensor in onnx_model.graph.initializer:
+            new_value_info.pop(tensor.name, None)
+        existing_value_info.update(new_value_info)
         onnx_model.graph.value_info.extend(existing_value_info.values())
 
         return onnx_model
 
     @runtime_typing.checked
     def add_op_call(
         self,
@@ -914,15 +920,15 @@
         """
         named_value_info: Dict[str, onnx.ValueInfoProto] = {}
         for name, sub_graph in self._sub_torch_script_graphs.items():
             named_value_info.update(sub_graph.generate_function_value_info_proto(name))
         return named_value_info
 
     @runtime_typing.checked
-    def generate_maingraph_value_info_proto(self) -> Mapping[str, onnx.ValueInfoProto]:
+    def generate_maingraph_value_info_proto(self) -> Dict[str, onnx.ValueInfoProto]:
         """Returns value info proto for values in the main graph."""
         named_value_info: Dict[str, onnx.ValueInfoProto] = {}
         for torch_value, tensor in self._value_to_tensor.items():
             if (value_info := tensor.value_info()) is None:
                 continue
             # NOTE: _C.Value re-naming.
             # _C.Value's debugName is unstable.
```

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240402/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240402/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/main.py` & `onnxscript-0.1.0.dev20240402/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240402/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240402/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/testing.py` & `onnxscript-0.1.0.dev20240402/onnxscript/testing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/common/onnx_script_test_case.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/common/onnx_script_test_case.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/function_libs/torch_lib/error_reproduction.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/function_libs/torch_lib/error_reproduction.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/function_libs/torch_lib/extra_opinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/function_libs/torch_lib/ops_test_common.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/function_libs/torch_lib/ops_test_common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/function_libs/torch_lib/ops_test_data.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/function_libs/torch_lib/ops_test_data.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/functions/gemmgelu.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/functions/gemmgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/functions/ort_custom_ops.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/functions/ort_custom_ops.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/attrref.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/attrref.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/cast_like.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/cast_like.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/different_opset.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/different_opset.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/dropout.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/dropout.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/eager_op.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/eager_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/eg1.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/eg1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/getitem.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/getitem.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/graph_attr.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/graph_attr.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/identity.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/identity.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/if_statement.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/if_statement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/loops_break.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/loops_break.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/loops_while.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/loops_while.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/onnxfns1.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/onnxfns1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/onnxfns1A.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/onnxfns1A.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/onnxfns2.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/onnxfns2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/opt_input.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/opt_input.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/opt_output.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/opt_output.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/renaming.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/renaming.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/sequences.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/sequences.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/signal_dft.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/signal_dft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/subfunction.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/subfunction.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/tests/models/type_double.py` & `onnxscript-0.1.0.dev20240402/onnxscript/tests/models/type_double.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240402/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript/values.py` & `onnxscript-0.1.0.dev20240402/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240402/onnxscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240401
+Version: 0.1.0.dev20240402
 Summary: Naturally author ONNX functions and models using a subset of Python
 Home-page: https://onnxscript.ai/
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
```

### Comparing `onnxscript-0.1.0.dev20240401/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240402/onnxscript.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 onnxscript/_internal/ast_utils.py
 onnxscript/_internal/autocast.py
 onnxscript/_internal/deprecation.py
 onnxscript/_internal/param_manipulation.py
 onnxscript/_internal/runtime_typing.py
 onnxscript/_internal/utils.py
 onnxscript/_internal/version_utils.py
+onnxscript/_thirdparty/asciichartpy.py
 onnxscript/backend/__init__.py
 onnxscript/backend/onnx_backend.py
 onnxscript/backend/onnx_export.py
 onnxscript/diagnostics/infra/__init__.py
 onnxscript/diagnostics/infra/_infra.py
 onnxscript/diagnostics/infra/context.py
 onnxscript/diagnostics/infra/decorator.py
@@ -110,14 +111,24 @@
 onnxscript/function_libs/torch_lib/ops/linalg.py
 onnxscript/function_libs/torch_lib/ops/nested.py
 onnxscript/function_libs/torch_lib/ops/nn.py
 onnxscript/function_libs/torch_lib/ops/prims.py
 onnxscript/function_libs/torch_lib/ops/sparse.py
 onnxscript/function_libs/torch_lib/ops/special.py
 onnxscript/function_libs/torch_lib/ops/vision.py
+onnxscript/ir/__init__.py
+onnxscript/ir/_core.py
+onnxscript/ir/_display.py
+onnxscript/ir/_enums.py
+onnxscript/ir/_graph_comparison.py
+onnxscript/ir/_invariants.py
+onnxscript/ir/_metadata.py
+onnxscript/ir/_protocols.py
+onnxscript/ir/convenience.py
+onnxscript/ir/serde.py
 onnxscript/onnx_opset/__init__.py
 onnxscript/onnx_opset/_impl/opset1.py
 onnxscript/onnx_opset/_impl/opset10.py
 onnxscript/onnx_opset/_impl/opset11.py
 onnxscript/onnx_opset/_impl/opset12.py
 onnxscript/onnx_opset/_impl/opset13.py
 onnxscript/onnx_opset/_impl/opset14.py
```

### Comparing `onnxscript-0.1.0.dev20240401/pyproject.toml` & `onnxscript-0.1.0.dev20240402/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -34,28 +34,26 @@
 onnx = ["py.typed"]
 
 [tool.pytest.ini_options]
 filterwarnings = ["ignore::UserWarning", "ignore::DeprecationWarning"]
 addopts = "-rsfEX --tb=short --color=yes"
 
 [tool.mypy]
-follow_imports = "silent"   # TODO: Remove when we fix all the mypy errors
-strict_optional = true
-warn_no_return = true
-warn_unused_ignores = false # TODO: CI and local are inconsistent when this is true. Investigate.
-warn_redundant_casts = true
-warn_incomplete_stub = true
-# TODO disallow_untyped_calls = true
+# TODO disallow_incomplete_defs = true
 check_untyped_defs = true
+disable_error_code = 'override,import-untyped'
 disallow_any_generics = false
-# TODO disallow_incomplete_defs = true
-# TODO disallow_subclassing_any = true
 disallow_untyped_decorators = true
-warn_unused_configs = true
 show_column_numbers = true
+strict_optional = true
+warn_incomplete_stub = true
+warn_no_return = true
+warn_redundant_casts = true
+warn_unused_configs = true
+warn_unused_ignores = false
 
 [[tool.mypy.overrides]]
 module = [
   "onnx.*",
   "onnxruntime.*",
   "parameterized.*",
   "torchgen.*",
@@ -84,22 +82,24 @@
 [tool.isort]
 profile = "black"
 extend_skip_glob = [
   "onnxscript/tests/onnx_backend_test_code/*.py",
 ]
 
 [tool.pylint.messages_control]
-# This list is for vscode. Add new disables in pyproject_pylint.toml for lintrunner
+# NOTE: This list is for vscode. Add new disables in pyproject_pylint.toml for lintrunner
 # Exclude patterns should be modified in .lintrunner.toml
 disable = [
+  "consider-using-from-import",
   "format",
   "import-error",
   "invalid-name",      # TODO: Add naming guidance and enable this check.
   "line-too-long",
   "no-name-in-module",
+  "unnecessary-ellipsis",
   "use-dict-literal",  # Sometime it is preferable when we construct kwargs
 ]
 
 [tool.pydocstyle]
 convention = "google"
 
 [tool.ruff]
```

### Comparing `onnxscript-0.1.0.dev20240401/setup.py` & `onnxscript-0.1.0.dev20240402/setup.py`

 * *Files identical despite different names*

