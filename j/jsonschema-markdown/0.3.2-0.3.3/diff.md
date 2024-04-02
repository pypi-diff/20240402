# Comparing `tmp/jsonschema_markdown-0.3.2-py3-none-any.whl.zip` & `tmp/jsonschema_markdown-0.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8732 bytes, number of entries: 10
+Zip file size: 8967 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       81 b- defN 80-Jan-01 00:00 jsonschema_markdown/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 jsonschema_markdown/converter/__init__.py
--rw-r--r--  2.0 unx    12993 b- defN 80-Jan-01 00:00 jsonschema_markdown/converter/markdown.py
--rw-r--r--  2.0 unx     1311 b- defN 80-Jan-01 00:00 jsonschema_markdown/main.py
+-rw-r--r--  2.0 unx    13589 b- defN 80-Jan-01 00:00 jsonschema_markdown/converter/markdown.py
+-rw-r--r--  2.0 unx     1321 b- defN 80-Jan-01 00:00 jsonschema_markdown/main.py
 -rw-r--r--  2.0 unx     1103 b- defN 80-Jan-01 00:00 jsonschema_markdown/utils.py
--rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.3.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4097 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       68 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.3.2.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      898 b- defN 16-Jan-01 00:00 jsonschema_markdown-0.3.2.dist-info/RECORD
-10 files, 21712 bytes uncompressed, 7170 bytes compressed:  67.0%
+-rw-r--r--  2.0 unx     1073 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.3.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4097 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.3.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.3.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       68 b- defN 80-Jan-01 00:00 jsonschema_markdown-0.3.3.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      898 b- defN 16-Jan-01 00:00 jsonschema_markdown-0.3.3.dist-info/RECORD
+10 files, 22318 bytes uncompressed, 7405 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: jsonschema_markdown/main.py
 Comment: 
 
 Filename: jsonschema_markdown/utils.py
 Comment: 
 
-Filename: jsonschema_markdown-0.3.2.dist-info/LICENSE
+Filename: jsonschema_markdown-0.3.3.dist-info/LICENSE
 Comment: 
 
-Filename: jsonschema_markdown-0.3.2.dist-info/METADATA
+Filename: jsonschema_markdown-0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: jsonschema_markdown-0.3.2.dist-info/WHEEL
+Filename: jsonschema_markdown-0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: jsonschema_markdown-0.3.2.dist-info/entry_points.txt
+Filename: jsonschema_markdown-0.3.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: jsonschema_markdown-0.3.2.dist-info/RECORD
+Filename: jsonschema_markdown-0.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jsonschema_markdown/converter/markdown.py

```diff
@@ -105,18 +105,22 @@
     - Deprecated
     - Default value
     - Description
 
     Search for deprecated string in the description or a deprecated key set to true in the property
     """
 
+    logger.debug(f"Creating definition table for schema: {schema}")
+
     if schema.get("enum"):
+        logger.debug("Creating enum markdown")
         return create_enum_markdown(schema)
 
     if schema.get("const"):
+        logger.debug("Creating const markdown")
         return create_const_markdown(schema)
 
     if schema.get("properties"):
         schema["properties"] = sort_properties(schema)
 
     markdown = ""
 
@@ -195,130 +199,138 @@
     )
     if ref_from_additional_properties:
         return _get_property_ref(ref_from_additional_properties, defs)
 
     return None, None
 
 
-def _get_property_details(property_type: str, property_details: dict, defs: dict):
+def _handle_array_like_property(property_type: str, property_details: dict, defs: dict):
     """
-    Get the possible values for a property.
+    Handle properties that are array-like.
     """
 
-    # Check if the property is a reference
-    ref_type, ref_details = get_property_if_ref(property_details, defs)
-    if ref_type or ref_details:
-        return ref_type, ref_details
-
-    if "enum" in property_details:
-        return (
-            property_type,
-            " ".join([f"`{str(value)}`" for value in property_details["enum"]]),
-        )
-
-    array_like = (
+    array_type = (
         "oneOf"
         if "oneOf" in property_details
         else (
             "anyOf"
             if "anyOf" in property_details
             else "allOf" if "allOf" in property_details else None
         )
     )
 
+    if array_type is None:
+        logger.warning(
+            f"Array-like property without oneOf, anyOf or allOf: {property_type} {property_details}"
+        )
+        return property_type, {}
+
     array_separator = {"oneOf": " or ", "anyOf": " and/or ", "allOf": " and "}
 
-    # TODO: Check why are we removing null from array_like
-    if array_like:
-        with contextlib.suppress(Exception):
-            property_details[array_like].remove({"type": "null"})
-            if len(property_details[array_like]) == 1:
-                return _get_property_details(
-                    property_details[array_like][0].get("type"),
-                    property_details[array_like][0],
-                    defs,
-                )
-
-    if array_like:
-        types = []
-        details = []
-        for value in property_details[array_like]:
-            ref_type, ref_details = get_property_if_ref(value, defs)
-            if ref_type or ref_details:
-                types.append(ref_type)
-                details.append(ref_details)
-            else:
-                ref_type, ref_details = _get_property_details(
-                    value.get("type"), value, defs
-                )
-                types.append(ref_type)
-                details.append(ref_details)
-        types_set = set(types)
-        if len(types_set) > 1:
-            logger.warning(f"Multiple types in {array_like} property: {types_set}")
+    # TODO: We are removing the null type from the this property, some libraries add this
+    # for nullable properties, we should find a better way to handle this
+    removed_null = False
+    with contextlib.suppress(Exception):
+        property_details[array_type].remove({"type": "null"})
+        removed_null = True
+        if len(property_details[array_type]) == 1:
+            return _get_property_details(
+                property_details[array_type][0].get("type"),
+                property_details[array_type][0],
+                defs,
+            )
 
-        return (
-            types[0],
-            array_separator[array_like].join(details),
+    types = []
+    details = []
+    for value in property_details[array_type]:
+        ref_type, ref_details = get_property_if_ref(value, defs)
+        if ref_type or ref_details:
+            types.append(ref_type)
+            details.append(ref_details)
+        else:
+            ref_type, ref_details = _get_property_details(
+                value.get("type"), value, defs
+            )
+            types.append(ref_type)
+            details.append(ref_details)
+    types_set = set(types)
+    if len(types_set) > 1 and removed_null:
+        logger.warning(
+            f"Multiple types in items,{array_type} property: {types_set}. Selecting the first one.",
         )
 
-    elif "items" in property_details:
-        array_like = (
-            "oneOf"
-            if "oneOf" in property_details["items"]
-            else (
-                "anyOf"
-                if "anyOf" in property_details["items"]
-                else "allOf" if "allOf" in property_details["items"] else None
-            )
+    if removed_null:
+        logger.debug(
+            f"Removed null type from {property_type} property, got {types_set} as types, selecting the first one {types[0]}"
+        )
+        return types[0], array_separator[array_type].join(details)
+    elif property_type is None:
+        logger.warning(
+            f"Array-like property without type, selecting first type of subschema: {types[0]}"
         )
+        return types[0], array_separator[array_type].join(details)
+    else:
+        logger.debug(
+            f"Array-like property without null type, selecting original type {property_type}"
+        )
+        return property_type, array_separator[array_type].join(details)
+
+
+def _get_property_details(property_type: str, property_details: dict, defs: dict):
+    """
+    Get the possible values for a property.
+    """
+
+    # Check if the property is a reference
+    ref_type, ref_details = get_property_if_ref(property_details, defs)
+    if ref_type or ref_details:
+        return ref_type, ref_details
 
-        if array_like:
-            types = []
-            details = []
-            for value in property_details["items"][array_like]:
-                ref_type, ref_details = get_property_if_ref(value, defs)
-                if ref_type or ref_details:
-                    types.append(ref_type)
-                    details.append(ref_details)
-                else:
-                    ref_type, ref_details = _get_property_details(
-                        value.get("type"), value, defs
-                    )
-                    types.append(ref_type)
-                    details.append(ref_details)
-            types_set = set(types)
-            if len(types_set) > 1:
-                logger.warning(
-                    f"Multiple types in items,{array_like} property: {types_set}"
-                )
-
-            return (
-                types[0],
-                array_separator[array_like].join(details),
+    if "additionalProperties" in property_details and not isinstance(
+        property_details["additionalProperties"], bool
+    ):
+        logger.warning(
+            f"Additional properties not a boolean: {property_details['additionalProperties']}"
+        )
+        # new_type = property_details["additionalProperties"].get("type")
+        # return new_type, new_type
+
+    if "enum" in property_details:
+        return (
+            property_type,
+            " ".join([f"`{str(value)}`" for value in property_details["enum"]]),
+        )
+
+    # Handle array-like properties
+    if any(key in property_details for key in ["oneOf", "anyOf", "allOf"]):
+        t, d = _handle_array_like_property(property_type, property_details, defs)
+        if t and d:
+            return t, d
+
+    if "items" in property_details:
+        if any(key in property_details["items"] for key in ["oneOf", "anyOf", "allOf"]):
+            t, d = _handle_array_like_property(
+                property_type, property_details["items"], defs
             )
+            if t and d:
+                return t, d
 
         ref_type, ref_details = get_property_if_ref(property_details["items"], defs)
         if ref_type or ref_details:
             return property_type, ref_details
         else:
             ref_type, ref_details = _get_property_details(
                 property_details["items"].get("type"), property_details["items"], defs
             )
             return property_type, ref_details
 
     elif "pattern" in property_details:
         pattern = property_details["pattern"]
         res_details = f"[`{pattern}`](https://regex101.com/?regex={urllib.parse.quote_plus(pattern)})"
         return property_type, res_details
-    elif "additionalProperties" in property_details and not isinstance(
-        property_details["additionalProperties"], bool
-    ):
-        new_type = property_details["additionalProperties"].get("type")
-        return new_type, new_type
     elif "const" in property_details:
         res_details = f"`{property_details.get('const')}`"
         return "const", res_details
     elif property_type in ["integer", "number"]:
         # write the range of the integer in the format a <= x <= b
         minimum = property_details.get("minimum")
         maximum = property_details.get("maximum")
```

## jsonschema_markdown/main.py

```diff
@@ -59,8 +59,8 @@
     if title:
         kwargs["title"] = title
 
     # Convert the file contents to markdown
     markdown = jsonschema_markdown.generate(file_contents, **kwargs)
 
     # Output the markdown
-    click.echo(markdown)
+    click.echo(markdown, nl=False)
```

## Comparing `jsonschema_markdown-0.3.2.dist-info/LICENSE` & `jsonschema_markdown-0.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jsonschema_markdown-0.3.2.dist-info/METADATA` & `jsonschema_markdown-0.3.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-markdown
-Version: 0.3.2
+Version: 0.3.3
 Summary: Export a JSON Schema document to Markdown documentation.
 Home-page: https://github.com/elisiariocouto/jsonschema-markdown
 License: MIT
 Keywords: jsonschema,markdown,documentation,docs,json
 Author: Elisiário Couto
 Author-email: elisiario@couto.io
 Requires-Python: >=3.9,<4.0
```

