# Comparing `tmp/shacl2code-0.0.8.tar.gz` & `tmp/shacl2code-0.0.9.tar.gz`

## Comparing `shacl2code-0.0.8.tar` & `shacl2code-0.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 shacl2code-0.0.8/.flake8
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 shacl2code-0.0.8/.github/workflows/coverage-generate.yaml
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 shacl2code-0.0.8/.github/workflows/coverage-report.yaml
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 shacl2code-0.0.8/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 shacl2code-0.0.8/.github/workflows/test.yaml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 shacl2code-0.0.8/src/shacl2code/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 shacl2code-0.0.8/src/shacl2code/__main__.py
--rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 shacl2code-0.0.8/src/shacl2code/context.py
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 shacl2code-0.0.8/src/shacl2code/main.py
--rw-r--r--   0        0        0     9164 2020-02-02 00:00:00.000000 shacl2code-0.0.8/src/shacl2code/model.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 shacl2code-0.0.8/src/shacl2code/urlcontext.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 shacl2code-0.0.8/src/shacl2code/version.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 shacl2code-0.0.8/src/shacl2code/lang/__init__.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 shacl2code-0.0.8/src/shacl2code/lang/common.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 shacl2code-0.0.8/src/shacl2code/lang/jinja.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 shacl2code-0.0.8/src/shacl2code/lang/jsonschema.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 shacl2code-0.0.8/src/shacl2code/lang/lang.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 shacl2code-0.0.8/src/shacl2code/lang/python.py
--rw-r--r--   0        0        0    10606 2020-02-02 00:00:00.000000 shacl2code-0.0.8/src/shacl2code/lang/templates/jsonschema.j2
--rw-r--r--   0        0        0    44242 2020-02-02 00:00:00.000000 shacl2code-0.0.8/src/shacl2code/lang/templates/python.j2
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/conftest.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/test_cli.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/test_common_jinja.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/test_common_prefix.py
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/test_context.py
--rw-r--r--   0        0        0    20284 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/test_jsonschema.py
--rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/test_model_source.py
--rw-r--r--   0        0        0    37933 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/test_python.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/data/abort.j2
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/data/bad-id.j2
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/data/bad-node-kind.ttl
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/data/bad-pattern-class.ttl
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/data/bad-pattern-integer.ttl
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/data/bad-reference.jsonld
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/data/context-url.j2
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/data/context.j2
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/data/missing-range.ttl
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/data/raw.j2
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/data/model/test-context.json
--rw-r--r--   0        0        0    10619 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/data/model/test.ttl
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/data/python/links.json
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/data/python/roundtrip.json
--rwxr-xr-x   0        0        0     2538 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/expect/make_expect.py
--rw-r--r--   0        0        0    28868 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/expect/jsonschema/test-context.json
--rw-r--r--   0        0        0    32185 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/expect/jsonschema/test.json
--rwxr-xr-x   0        0        0    55931 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/expect/python/test-context.py
--rw-r--r--   0        0        0    52747 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/expect/python/test.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/expect/raw/test-context.txt
--rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 shacl2code-0.0.8/tests/expect/raw/test.txt
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 shacl2code-0.0.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 shacl2code-0.0.8/LICENSE
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 shacl2code-0.0.8/README.md
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 shacl2code-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 shacl2code-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 shacl2code-0.0.9/.flake8
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 shacl2code-0.0.9/.github/workflows/coverage-generate.yaml
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 shacl2code-0.0.9/.github/workflows/coverage-report.yaml
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 shacl2code-0.0.9/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 shacl2code-0.0.9/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 shacl2code-0.0.9/src/shacl2code/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 shacl2code-0.0.9/src/shacl2code/__main__.py
+-rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 shacl2code-0.0.9/src/shacl2code/context.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 shacl2code-0.0.9/src/shacl2code/main.py
+-rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 shacl2code-0.0.9/src/shacl2code/model.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 shacl2code-0.0.9/src/shacl2code/urlcontext.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 shacl2code-0.0.9/src/shacl2code/version.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 shacl2code-0.0.9/src/shacl2code/lang/__init__.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 shacl2code-0.0.9/src/shacl2code/lang/common.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 shacl2code-0.0.9/src/shacl2code/lang/jinja.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 shacl2code-0.0.9/src/shacl2code/lang/jsonschema.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 shacl2code-0.0.9/src/shacl2code/lang/lang.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 shacl2code-0.0.9/src/shacl2code/lang/python.py
+-rw-r--r--   0        0        0    11296 2020-02-02 00:00:00.000000 shacl2code-0.0.9/src/shacl2code/lang/templates/jsonschema.j2
+-rw-r--r--   0        0        0    47860 2020-02-02 00:00:00.000000 shacl2code-0.0.9/src/shacl2code/lang/templates/python.j2
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/conftest.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/test_cli.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/test_common_jinja.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/test_common_prefix.py
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/test_context.py
+-rw-r--r--   0        0        0    23313 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/test_jsonschema.py
+-rw-r--r--   0        0        0     9135 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/test_model_source.py
+-rw-r--r--   0        0        0    40576 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/test_python.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/data/abort.j2
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/data/bad-id.j2
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/data/bad-node-kind.ttl
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/data/bad-pattern-class.ttl
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/data/bad-pattern-integer.ttl
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/data/bad-reference.jsonld
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/data/context-url.j2
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/data/context.j2
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/data/missing-range.ttl
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/data/raw.j2
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/data/model/test-context.json
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/data/model/test.ttl
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/data/python/links.json
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/data/python/roundtrip.json
+-rwxr-xr-x   0        0        0     2538 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/expect/make_expect.py
+-rw-r--r--   0        0        0    33894 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/expect/jsonschema/test-context.json
+-rw-r--r--   0        0        0    37567 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/expect/jsonschema/test.json
+-rwxr-xr-x   0        0        0    58223 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/expect/python/test-context.py
+-rw-r--r--   0        0        0    55863 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/expect/python/test.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/expect/raw/test-context.txt
+-rw-r--r--   0        0        0    14121 2020-02-02 00:00:00.000000 shacl2code-0.0.9/tests/expect/raw/test.txt
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 shacl2code-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 shacl2code-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 shacl2code-0.0.9/README.md
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 shacl2code-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 shacl2code-0.0.9/PKG-INFO
```

### Comparing `shacl2code-0.0.8/.github/workflows/coverage-generate.yaml` & `shacl2code-0.0.9/.github/workflows/coverage-generate.yaml`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/.github/workflows/coverage-report.yaml` & `shacl2code-0.0.9/.github/workflows/coverage-report.yaml`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/.github/workflows/publish.yaml` & `shacl2code-0.0.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/.github/workflows/test.yaml` & `shacl2code-0.0.9/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/src/shacl2code/context.py` & `shacl2code-0.0.9/src/shacl2code/context.py`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/src/shacl2code/main.py` & `shacl2code-0.0.9/src/shacl2code/main.py`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/src/shacl2code/model.py` & `shacl2code-0.0.9/src/shacl2code/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     str(XSD.dateTimeStamp),
     str(XSD.anyURI),
 ]
 
 
 class SHACL2CODE(DefinedNamespace):
     idPropertyName: URIRef
+    isExtensible: URIRef
 
     _NS = Namespace("https://jpewdev.github.io/shacl2code/schema#")
 
 
 class ModelException(Exception):
     pass
 
@@ -86,31 +87,30 @@
     clsname: str
     parent_ids: typing.List[str]
     derived_ids: list
     properties: typing.List[Property]
     comment: str = ""
     id_property: str = ""
     node_kind: str = None
+    extensible: bool = False
 
 
 class Model(object):
     def __init__(self, graph, context=None):
         self.model = graph
         self.context = context
         self.compact_ids = {}
         self.objects = {}
         self.enums = []
         self.classes = []
         class_iris = set()
         enum_iris = set()
         classes_by_iri = {}
-        all_class_iris = set()
 
         for cls_iri in self.model.subjects(RDF.type, OWL.Class):
-            all_class_iris.add(cls_iri)
             enum_values = []
 
             for value_iri in self.model.subjects(RDF.type, cls_iri):
                 if (value_iri, RDF.type, OWL.NamedIndividual) not in self.model:
                     continue
 
                 v = EnumValue(
@@ -127,16 +127,15 @@
                     _id=str(cls_iri),
                     clsname=self.get_class_name(cls_iri),
                     comment=str(self.model.value(cls_iri, RDFS.comment, default="")),
                     values=enum_values,
                 )
                 self.enums.append(e)
                 enum_iris.add(cls_iri)
-
-            if (cls_iri, RDF.type, SH.NodeShape) in self.model:
+            else:
                 class_iris.add(cls_iri)
 
         def int_val(v):
             if not v:
                 return None
             return int(v)
 
@@ -162,28 +161,23 @@
             if value is not None:
                 return value
             return default
 
         def set_prop_range(p, range_id):
             nonlocal enum_iris
             nonlocal class_iris
-            nonlocal all_class_iris
 
             if range_id in enum_iris:
                 p.enum_id = str(range_id)
                 return True
 
             if range_id in class_iris:
                 p.class_id = str(range_id)
                 return True
 
-            if range_id in all_class_iris:
-                p.datatype = str(XSD.anyURI)
-                return True
-
             return False
 
         for cls_iri in class_iris:
             c = Class(
                 _id=str(cls_iri),
                 parent_ids=[
                     str(parent_iri)
@@ -194,14 +188,15 @@
                 clsname=self.get_class_name(cls_iri),
                 comment=str(self.model.value(cls_iri, RDFS.comment, default="")),
                 properties=[],
                 id_property=str_val(
                     get_inherited_value(cls_iri, SHACL2CODE.idPropertyName)
                 ),
                 node_kind=get_inherited_value(cls_iri, SH.nodeKind, SH.BlankNodeOrIRI),
+                extensible=bool(self.model.value(cls_iri, SHACL2CODE.isExtensible)),
             )
 
             if c.node_kind not in (SH.IRI, SH.BlankNode, SH.BlankNodeOrIRI):
                 raise ModelException(
                     f"Class {c._id} has unsupported '{SH.nodeKind}' value '{c.node_kind}'"
                 )
```

### Comparing `shacl2code-0.0.8/src/shacl2code/lang/common.py` & `shacl2code-0.0.9/src/shacl2code/lang/common.py`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/src/shacl2code/lang/jinja.py` & `shacl2code-0.0.9/src/shacl2code/lang/jinja.py`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/src/shacl2code/lang/jsonschema.py` & `shacl2code-0.0.9/src/shacl2code/lang/jsonschema.py`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/src/shacl2code/lang/python.py` & `shacl2code-0.0.9/src/shacl2code/lang/python.py`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/src/shacl2code/lang/templates/jsonschema.j2` & `shacl2code-0.0.9/src/shacl2code/lang/templates/jsonschema.j2`

 * *Files 2% similar despite different names*

```diff
@@ -56,41 +56,53 @@
     {%- for class in classes %}
         {#- Classes are divided into 2 parts. The properties are separated into a separate object #}
         {#- so that a object can references the properties of its parent without needing the const #}
         {#- @type tag #}
         "{{ varname(class.clsname) }}": {
             "allOf": [
                 {
+                    {%- if class.extensible %}
+                    "unevaluatedProperties": true,
+                    {%- endif %}
                     "properties": {
                         "{{ class.id_property or "@id" }}": { "$ref": "#/$defs/{{ class.node_kind.split("#")[-1] }}" },
-                        "{{ context.compact("@type") }}": { "const": "{{ context.compact_vocab(class._id) }}" }
+                        "{{ context.compact("@type") }}": {
+                            "oneOf": [
+                                {%- if class.extensible %}
+                                { "$ref": "#/$defs/IRI" },
+                                {%- endif %}
+                                { "const": "{{ context.compact_vocab(class._id) }}" }
+                            ]
+                        }
                     }{%- if class.node_kind == SH.IRI %},
                     "required": ["{{ class.id_property or "@id" }}"]
                     {%- endif %}
                 },
                 { "$ref": "#/$defs/{{ varname(class.clsname) }}_props" }
             ]
         },
         "{{ varname(class.clsname) }}_derived": {
+            {%- if not class.extensible %}
+            "unevaluatedProperties": false,
+            {%- endif %}
             {%- set ns = namespace(external_ref=False, local_ref=False, any_ref=False, json_refs=[]) %}
             {%- for d in get_all_derived(class) + [class._id] %}
                 {%- set ns.json_refs = ns.json_refs + ["#/$defs/" + varname(classes.get(d).clsname)] %}
             {%- endfor %}
             {%- set ns.json_refs = ns.json_refs + ["#/$defs/BlankNodeOrIRI"] %}
 
             {%- if ns.json_refs | length == 1 %}
             "$ref": "{{ ns.json_refs[0] }}",
             {%- elif ns.json_refs %}
-            "oneOf": [
+            "anyOf": [
                 {%- for r in ns.json_refs %}
                 { "$ref": "{{ r }}" }{% if not loop.last %},{% endif %}
                 {%- endfor %}
-            ],
+            ]
             {%- endif %}
-            "unevaluatedProperties": false
         },
         "{{ varname(class.clsname) }}_props": {
             "allOf": [
                 {%- if class.parent_ids %}
                 {%- for parent in class.parent_ids %}
                 { "$ref": "#/$defs/{{ varname(classes.get(parent).clsname) }}_props" },
                 {%- endfor %}
@@ -209,19 +221,19 @@
                 {%- endif %}
             {%- endif %}
         },
         {%- endfor %}
     {%- endfor %}
         "IRI": {
             "type": "string",
-            "pattern": "^(?!_:).*"
+            "pattern": "^(?!_:).+:.+"
         },
         "BlankNode": {
             "type": "string",
-            "pattern": "^_:.*"
+            "pattern": "^_:.+"
         },
         "BlankNodeOrIRI": {
             "oneOf": [
                 { "$ref": "#/$defs/IRI" },
                 { "$ref": "#/$defs/BlankNode" }
             ]
         },
@@ -240,25 +252,30 @@
         "Extension": {
             "type": "string"
         },
         "SHACLClass": {
             "type": "object",
             "properties": {
                 "{{ context.compact("@type") }}": {
-                    "enum": [
-                    {%- for class in classes %}
-                        "{{ context.compact_vocab(class._id) }}"{% if not loop.last %},{% endif %}
-                    {%- endfor %}
+                    "oneOf": [
+                        { "$ref": "#/$defs/IRI" },
+                        {
+                            "enum": [
+                            {%- for class in classes %}
+                                "{{ context.compact_vocab(class._id) }}"{% if not loop.last %},{% endif %}
+                            {%- endfor %}
+                            ]
+                        }
                     ]
                 }
             },
             "required": ["{{ context.compact("@type") }}"]
         },
         "AnyClass": {
-            "oneOf": [
+            "anyOf": [
                 {%- for class in classes %}
                 { "$ref": "#/$defs/{{ varname(class.clsname) }}" }{% if not loop.last %},{% endif %}
                 {%- endfor %}
             ]
         }
     }
 }
```

### Comparing `shacl2code-0.0.8/src/shacl2code/lang/templates/python.j2` & `shacl2code-0.0.9/src/shacl2code/lang/templates/python.j2`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # SPDX-License-Identifier: MIT
 
 import functools
 import hashlib
 import json
 import re
 import time
+import threading
 from contextlib import contextmanager
 from datetime import datetime, timezone, timedelta
 from enum import Enum
 from abc import ABC, abstractmethod
 
 
 def check_type(obj, types):
@@ -58,26 +59,29 @@
 
     def elide(self, value):
         return value is None
 
     def walk(self, value, callback, path):
         callback(value, path)
 
-    def link_prop(self, value, link_cache, missing, visited):
+    def iter_objects(self, value, recursive, visited):
+        return []
+
+    def link_prop(self, value, doc, missing, visited):
         return value
 
     def to_string(self, value):
         return str(value)
 
     @abstractmethod
     def encode(self, encoder, value, state):
         pass
 
     @abstractmethod
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         pass
 
 
 class StringProp(Property):
     """
     A scalar string property for an SHACL object
     """
@@ -86,23 +90,23 @@
 
     def set(self, value):
         return str(value)
 
     def encode(self, encoder, value, state):
         encoder.write_string(value)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         return decoder.read_string()
 
 
 class AnyURIProp(StringProp):
     def encode(self, encoder, value, state):
         encoder.write_iri(value)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         return decoder.read_iri()
 
 
 class DateTimeProp(Property):
     """
     A Date/Time Object with optional timezone
     """
@@ -113,15 +117,15 @@
 
     def set(self, value):
         return self._normalize(value)
 
     def encode(self, encoder, value, state):
         encoder.write_datetime(self.to_string(value))
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         s = decoder.read_datetime()
         if s is None:
             return None
         v = self.from_string(s)
         return self._normalize(v)
 
     def _normalize(self, value):
@@ -167,15 +171,15 @@
 
     def set(self, value):
         return int(value)
 
     def encode(self, encoder, value, state):
         encoder.write_integer(value)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         return decoder.read_integer()
 
 
 class PositiveIntegerProp(IntegerProp):
     def validate(self, value):
         super().validate(value)
         if value < 1:
@@ -194,28 +198,28 @@
 
     def set(self, value):
         return bool(value)
 
     def encode(self, encoder, value, state):
         encoder.write_bool(value)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         return decoder.read_bool()
 
 
 class FloatProp(Property):
     VALID_TYPES = (float, int)
 
     def set(self, value):
         return float(value)
 
     def encode(self, encoder, value, state):
         encoder.write_float(value)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         return decoder.read_float()
 
 
 class ObjectProp(Property):
     """
     A scalar SHACL object property of a SHACL object
     """
@@ -238,51 +242,64 @@
             return
 
         if not isinstance(value, str):
             value.walk(callback, path)
         else:
             callback(value, path)
 
+    def iter_objects(self, value, recursive, visited):
+        if value is None or isinstance(value, str):
+            return
+
+        if value not in visited:
+            visited.add(value)
+            yield value
+
+            if recursive:
+                for c in value.iter_objects(recursive=True, visited=visited):
+                    yield c
+
     def encode(self, encoder, value, state):
         if value is None:
             raise ValueError("Object cannot be None")
 
         if isinstance(value, str):
             encoder.write_iri(value)
             return
 
         return value.encode(encoder, state)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         iri = decoder.read_iri()
         if iri is not None:
-            if object_ids and iri in object_ids:
-                return object_ids[iri]
+            if doc is not None:
+                return doc.find_by_id(iri, iri)
             return iri
 
-        return SHACLObject.decode(decoder, object_ids=object_ids)
+        return SHACLObject.decode(decoder, doc=doc)
 
-    def link_prop(self, value, link_cache, missing, visited):
+    def link_prop(self, value, doc, missing, visited):
         if value is None:
             return value
 
         if isinstance(value, str):
-            if value in link_cache:
-                return link_cache[value]
+            o = doc.find_by_id(value)
+            if o is not None:
+                return o
 
             if missing is not None:
                 missing.add(value)
 
             return value
 
         # De-duplicate IDs
-        if value._id and value._id is not link_cache[value._id]:
-            value = link_cache[value._id]
+        if value._id:
+            value = doc.find_by_id(value._id, value)
 
-        value.link_helper(link_cache, missing, visited)
+        value.link_helper(doc, missing, visited)
         return value
 
 
 class ListProxy(object):
     def __init__(self, prop, data=None):
         if data is None:
             self.__data = []
@@ -381,34 +398,39 @@
         return len(value) == 0
 
     def walk(self, value, callback, path):
         callback(value, path)
         for idx, v in enumerate(value):
             self.prop.walk(v, callback, path + [f"[{idx}]"])
 
-    def link_prop(self, value, link_cache, missing, visited):
+    def iter_objects(self, value, recursive, visited):
+        for v in value:
+            for c in self.prop.iter_objects(v, recursive, visited):
+                yield c
+
+    def link_prop(self, value, doc, missing, visited):
         if isinstance(value, ListProxy):
-            data = [self.prop.link_prop(v, link_cache, missing, visited) for v in value]
+            data = [self.prop.link_prop(v, doc, missing, visited) for v in value]
         else:
-            data = [self.prop.link_prop(v, link_cache, missing, visited) for v in value]
+            data = [self.prop.link_prop(v, doc, missing, visited) for v in value]
 
         return ListProxy(self.prop, data=data)
 
     def encode(self, encoder, value, state):
         check_type(value, ListProxy)
 
         with encoder.write_list() as list_s:
             for v in value:
                 with list_s.write_list_item() as item_s:
                     self.prop.encode(item_s, v, state)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         data = []
         for val_d in decoder.read_list():
-            v = self.prop.decode(val_d, object_ids=object_ids)
+            v = self.prop.decode(val_d, doc=doc)
             self.prop.validate(v)
             data.append(v)
 
         return ListProxy(self.prop, data=data)
 
 
 class EnumProp(Property):
@@ -430,130 +452,166 @@
         for iri, compact in self.context:
             if iri == value:
                 encoder.write_enum(value, self, compact)
                 return
 
         encoder.write_enum(value, self)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         v = decoder.read_enum(self)
         for iri, compact in self.context:
             if v == compact:
                 return iri
         return v
 
 
 class NodeKind(Enum):
     BlankNode = 1
     IRI = 2
     BlankNodeOrIRI = 3
 
 
+def register(type_iri, compact_type=None):
+    def add_deserializer(key, c):
+        assert (
+            key not in SHACLObject.DESERIALIZERS
+        ), f"{key} already registered to {SHACLObject.DESERIALIZERS[key].__name__}"
+        SHACLObject.DESERIALIZERS[key] = c
+
+    def decorator(c):
+        assert issubclass(
+            c, SHACLObject
+        ), f"{c.__name__} is not derived from SHACLObject"
+
+        c.TYPE = type_iri
+        add_deserializer(type_iri, c)
+
+        c.COMPACT_TYPE = compact_type
+        if compact_type:
+            add_deserializer(compact_type, c)
+
+        # Registration is deferred until the first instance of class is created
+        # so that it has access to any other defined class
+        c._NEEDS_REG = True
+        return c
+
+    return decorator
+
+
+register_lock = threading.Lock()
+
+
 @functools.total_ordering
 class SHACLObject(object):
     DESERIALIZERS = {}
     NODE_KIND = NodeKind.BlankNodeOrIRI
     ID_ALIAS = None
     COMPACT_TYPE = None
 
-    def __init__(self):
+    def __init__(self, **kwargs):
+        with register_lock:
+            cls = self.__class__
+            if cls._NEEDS_REG:
+                cls._OBJ_PROPERTIES = {}
+                cls._OBJ_IRIS = {}
+                cls._register_props()
+                cls._NEEDS_REG = False
+
         self._obj_data = {}
-        self._obj_properties = {}
-        self._obj_iris = {}
         self._obj_metadata = {}
 
-        self._add_property("_id", StringProp(), iri="@id")
+        for iri, prop, _, _, _, _ in self.__iter_props():
+            self._obj_data[iri] = prop.init()
 
-    def _set_init_props(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
 
+    @classmethod
+    def _register_props(cls):
+        cls._add_property("_id", StringProp(), iri="@id")
+
+    @classmethod
     def _add_property(
-        self,
+        cls,
         pyname,
         prop,
         iri,
         min_count=None,
         max_count=None,
         compact=None,
     ):
-        if pyname in self._obj_iris:
-            raise KeyError(
-                f"'{pyname}' is already defined for '{self.__class__.__name__}'"
-            )
-        if iri in self._obj_properties:
-            raise KeyError(
-                f"'{iri}' is already defined for '{self.__class__.__name__}'"
-            )
+        if pyname in cls._OBJ_IRIS:
+            raise KeyError(f"'{pyname}' is already defined for '{cls.__name__}'")
+        if iri in cls._OBJ_PROPERTIES:
+            raise KeyError(f"'{iri}' is already defined for '{cls.__name__}'")
 
-        while hasattr(self, pyname):
+        while hasattr(cls, pyname):
             pyname = pyname + "_"
 
-        self._obj_iris[pyname] = iri
-        self._obj_properties[iri] = (prop, min_count, max_count, pyname, compact)
-        self._obj_data[iri] = prop.init()
+        cls._OBJ_IRIS[pyname] = iri
+        cls._OBJ_PROPERTIES[iri] = (prop, min_count, max_count, pyname, compact)
 
     def __setattr__(self, name, value):
         if name.startswith("_obj_"):
             return super().__setattr__(name, value)
 
         if name == self.ID_ALIAS:
             name = "_id"
 
         try:
-            iri = self._obj_iris[name]
+            iri = self._OBJ_IRIS[name]
             self[iri] = value
         except KeyError:
             raise AttributeError(
                 f"'{name}' is not a valid property of {self.__class__.__name__}"
             )
 
     def __getattr__(self, name):
         if name.startswith("_obj_"):
             return self.__dict__[name]
 
         if name == "_metadata":
             return self._obj_metadata
 
         if name == "_IRI":
-            return self._obj_iris
+            return self._OBJ_IRIS
 
         if name == self.ID_ALIAS:
             name = "_id"
 
         try:
-            iri = self._obj_iris[name]
+            iri = self._OBJ_IRIS[name]
             return self[iri]
         except KeyError:
             raise AttributeError(
                 f"'{name}' is not a valid property of {self.__class__.__name__}"
             )
 
     def __delattr__(self, name):
         if name == self.ID_ALIAS:
             name = "_id"
 
         try:
-            iri = self._obj_iris[name]
+            iri = self._OBJ_IRIS[name]
             del self[iri]
         except KeyError:
             raise AttributeError(
                 f"'{name}' is not a valid property of {self.__class__.__name__}"
             )
 
     def __get_prop(self, iri):
-        if iri not in self._obj_properties:
+        if iri not in self._OBJ_PROPERTIES:
             raise KeyError(
                 f"'{iri}' is not a valid property of {self.__class__.__name__}"
             )
 
-        return self._obj_properties[iri]
+        return self._OBJ_PROPERTIES[iri]
 
     def __iter_props(self):
-        for iri, v in self._obj_properties.items():
+        for iri, v in self._OBJ_PROPERTIES.items():
             yield iri, *v
 
     def __getitem__(self, iri):
         return self._obj_data[iri]
 
     def __setitem__(self, iri, value):
         if iri == "@id":
@@ -573,15 +631,15 @@
         self._obj_data[iri] = prop.set(value)
 
     def __delitem__(self, iri):
         prop, _, _, _, _ = self.__get_prop(iri)
         self._obj_data[iri] = prop.init()
 
     def __iter__(self):
-        return self._obj_properties.keys()
+        return self._OBJ_PROPERTIES.keys()
 
     def walk(self, callback, path=None):
         """
         Walk object tree, invoking the callback for each item
 
         Callback has the form:
 
@@ -590,39 +648,35 @@
         if path is None:
             path = ["."]
 
         if callback(self, path):
             for iri, prop, _, _, _, _ in self.__iter_props():
                 prop.walk(self._obj_data[iri], callback, path + [f".{iri}"])
 
-    def child_objects(self):
+    def property_keys(self):
+        for iri, _, _, _, pyname, compact in self.__iter_props():
+            if iri == "@id":
+                compact = self.ID_ALIAS
+            yield pyname, iri, compact
+
+    def iter_objects(self, *, recursive=False, visited=None):
         """
-        Iterate over each object that is a child of this one
+        Iterate of all objects that are a child of this one
         """
-        seen = set()
-
-        def _walk_callback(value, path):
-            nonlocal seen
-
-            if not isinstance(value, SHACLObject):
-                return False
+        if visited is None:
+            visited = set()
 
-            if value in seen:
-                return False
-
-            seen.add(value)
-            return True
-
-        self.walk(_walk_callback)
-
-        for obj in seen:
-            yield obj
+        for iri, prop, _, _, _, _ in self.__iter_props():
+            for c in prop.iter_objects(
+                self._obj_data[iri], recursive=recursive, visited=visited
+            ):
+                yield c
 
     def encode(self, encoder, state):
-        idname = self.ID_ALIAS or self._obj_iris["_id"]
+        idname = self.ID_ALIAS or self._OBJ_IRIS["_id"]
         if not self._id and self.NODE_KIND == NodeKind.IRI:
             raise ValueError(
                 f"{self.__class__.__name__} ({id(self)}) must have a IRI for property '{idname}'"
             )
 
         if state.is_written(self):
             encoder.write_iri(state.get_object_id(self))
@@ -652,77 +706,69 @@
 
                 if max_count is not None:
                     if not prop.check_max_count(value, max_count):
                         raise ValueError(
                             f"Property '{pyname}' in {self.__class__.__name__} ({id(self)}) requires a maximum of {max_count} elements"
                         )
 
-                if iri == self._obj_iris["_id"]:
+                if iri == self._OBJ_IRIS["_id"]:
                     continue
 
                 with obj_s.write_property(iri, compact) as prop_s:
                     prop.encode(prop_s, value, state)
 
     @classmethod
-    def decode(cls, decoder, *, object_ids=None):
+    def decode(cls, decoder, *, doc=None):
         typ, obj_d = decoder.read_object()
         if typ is None:
             raise TypeError("Unable to determine type for object")
 
         if typ not in cls.DESERIALIZERS:
             raise TypeError(f"Unknown type {typ}")
 
         obj = cls.DESERIALIZERS[typ]()
         _id = obj_d.read_object_id(obj.ID_ALIAS)
         if _id is not None:
-            if object_ids is not None:
-                if _id in object_ids:
-                    return object_ids[_id]
-                object_ids[_id] = obj
             obj._id = _id
+            if doc is not None:
+                v = doc.find_by_id(_id)
+                if v is not None:
+                    return v
+
+        if doc is not None:
+            doc.add_index(obj)
 
         for iri, prop, _, _, _, compact in obj.__iter_props():
-            if iri == obj._obj_iris["_id"]:
+            if iri == obj._OBJ_IRIS["_id"]:
                 continue
 
             with obj_d.read_property(iri, compact) as prop_d:
                 if prop_d is None:
                     continue
 
-                v = prop.decode(prop_d, object_ids=object_ids)
+                v = prop.decode(prop_d, doc=doc)
                 prop.validate(v)
                 obj._obj_data[iri] = v
 
         return obj
 
-    def link_helper(self, link_cache, missing, visited):
+    def link_helper(self, doc, missing, visited):
         if self in visited:
             return
 
         visited.add(self)
 
         for iri, prop, _, _, _, _ in self.__iter_props():
             self._obj_data[iri] = prop.link_prop(
                 self._obj_data[iri],
-                link_cache,
+                doc,
                 missing,
                 visited,
             )
 
-    def link(self, link_cache=None):
-        if not link_cache:
-            link_cache = {obj._id: obj for obj in self.child_objects() if obj._id}
-
-        missing = set()
-        visited = set()
-
-        self.link_helper(link_cache, missing, visited)
-
-        return missing
-
     def __str__(self):
         parts = [
             f"{self.__class__.__name__}(",
         ]
         if self._id:
             parts.append(f"@id='{self._id}'")
         parts.append(")")
@@ -744,135 +790,213 @@
                 getattr(obj, "name", None) or "",
                 id(obj),
             )
 
         return sort_key(self) < sort_key(other)
 
 
-class EncodeState(object):
-    def __init__(self):
-        self.ref_objects = set()
-        self.written_objects = set()
-        self.blank_objects = {}
+class SHACLDocument(object):
+    def __init__(self, objects=[], *, link=False):
+        self.objects = set()
+        for o in objects:
+            self.objects.add(o)
+        self.create_index()
+        if link:
+            self._link()
+
+    def create_index(self):
+        self.obj_by_id = {}
+        self.obj_by_type = {}
+        for o in self.foreach():
+            self.add_index(o)
+
+    def add_index(self, obj):
+        for typ in SHACLObject.DESERIALIZERS.values():
+            if isinstance(obj, typ):
+                self.obj_by_type.setdefault(typ, set()).add(obj)
 
-    def get_object_id(self, o):
-        if o._id:
-            return o._id
+        if not obj._id:
+            return
 
-        if o not in self.blank_objects:
-            _id = f"_:{o.__class__.__name__}{len(self.blank_objects)}"
-            self.blank_objects[o] = _id
+        if obj._id in self.obj_by_id:
+            return
 
-        return self.blank_objects[o]
+        self.obj_by_id[obj._id] = obj
 
-    def is_refed(self, o):
-        return o in self.ref_objects
+    def link(self):
+        self.create_index()
+        return self._link()
 
-    def add_refed(self, o):
-        self.ref_objects.add(o)
+    def _link(self):
+        missing = set()
+        visited = set()
 
-    def is_written(self, o):
-        return o in self.written_objects
+        new_objects = set()
 
-    def add_written(self, o):
-        self.written_objects.add(o)
+        for o in self.objects:
+            if o._id:
+                o = self.find_by_id(o._id, o)
+            o.link_helper(self, missing, visited)
+            new_objects.add(o)
+
+        self.objects = new_objects
+
+        # Remove blank nodes
+        obj_by_id = {}
+        for _id, obj in self.obj_by_id.items():
+            if _id.startswith("_:"):
+                del obj._id
+            else:
+                obj_by_id[obj._id] = obj
+        self.obj_by_id = obj_by_id
 
+        return missing
 
-def encode_objects(encoder, objects, force_list=False):
-    """
-    Serialize a list of objects to a serialization encoder
+    def find_by_id(self, _id, default=None):
+        if _id not in self.obj_by_id:
+            return default
+        return self.obj_by_id[_id]
 
-    If force_list is true, a list will always be written using the encoder.
-    """
-    ref_counts = {}
-    state = EncodeState()
+    def foreach(self):
+        visited = set()
+        for o in self.objects:
+            if o not in visited:
+                yield o
+                visited.add(o)
+
+            for child in o.iter_objects(recursive=True, visited=visited):
+                yield child
+
+    def foreach_type(self, typ, *, subclass=False):
+        if isinstance(typ, str):
+            typ = SHACLObject.DESERIALIZERS[typ]
 
-    def walk_callback(value, path):
-        nonlocal state
-        nonlocal ref_counts
+        if typ not in self.obj_by_type:
+            return
 
-        if not isinstance(value, SHACLObject):
-            return True
+        for o in self.obj_by_type[typ]:
+            if subclass or o.__class__ is typ:
+                yield o
 
-        # Remove blank node ID for re-assignment
-        if value._id and value._id.startswith("_:"):
-            del value._id
+    def merge(self, *doc):
+        new_objects = set()
+        new_objects |= self.objects
+        for d in doc:
+            new_objects |= d.objects
 
-        if value._id:
-            state.add_refed(value)
+        return SHACLDocument(new_objects, link=True)
 
-        # If the object is referenced more than once, add it to the set of
-        # referenced objects
-        ref_counts.setdefault(value, 0)
-        ref_counts[value] += 1
-        if ref_counts[value] > 1:
-            state.add_refed(value)
-            return False
+    def encode(self, encoder, force_list=False):
+        """
+        Serialize a list of objects to a serialization encoder
 
-        return True
+        If force_list is true, a list will always be written using the encoder.
+        """
+        ref_counts = {}
+        state = EncodeState()
 
-    for o in objects:
-        if o._id:
-            state.add_refed(o)
-        o.walk(walk_callback)
+        def walk_callback(value, path):
+            nonlocal state
+            nonlocal ref_counts
 
-    use_list = force_list or len(objects) > 1
+            if not isinstance(value, SHACLObject):
+                return True
 
-    objects = set(objects)
+            # Remove blank node ID for re-assignment
+            if value._id and value._id.startswith("_:"):
+                del value._id
+
+            if value._id:
+                state.add_refed(value)
+
+            # If the object is referenced more than once, add it to the set of
+            # referenced objects
+            ref_counts.setdefault(value, 0)
+            ref_counts[value] += 1
+            if ref_counts[value] > 1:
+                state.add_refed(value)
+                return False
 
-    if use_list:
-        # If we are making a list add all the objects referred to by reference
-        # to the list
-        objects |= state.ref_objects
-
-    objects = list(objects)
-    objects.sort()
-
-    if use_list:
-        # Ensure top level objects are only written in the top level graph
-        # node, and referenced by ID everywhere else. This is done by setting
-        # the flag that indicates this object has been written for all the top
-        # level objects, then clearing it right before serializing the object.
-        #
-        # In this way, if an object is referenced before it is supposed to be
-        # serialized into the @graph, it will serialize as a string instead of
-        # the actual object
-        for o in objects:
-            state.written_objects.add(o)
+            return True
 
-        with encoder.write_list() as list_s:
+        for o in self.objects:
+            if o._id:
+                state.add_refed(o)
+            o.walk(walk_callback)
+
+        use_list = force_list or len(self.objects) > 1
+
+        if use_list:
+            # If we are making a list add all the objects referred to by reference
+            # to the list
+            objects = list(self.objects | state.ref_objects)
+        else:
+            objects = list(self.objects)
+
+        objects.sort()
+
+        if use_list:
+            # Ensure top level objects are only written in the top level graph
+            # node, and referenced by ID everywhere else. This is done by setting
+            # the flag that indicates this object has been written for all the top
+            # level objects, then clearing it right before serializing the object.
+            #
+            # In this way, if an object is referenced before it is supposed to be
+            # serialized into the @graph, it will serialize as a string instead of
+            # the actual object
             for o in objects:
-                # Allow this specific object to be written now
-                state.written_objects.remove(o)
-                with list_s.write_list_item() as item_s:
-                    o.encode(item_s, state)
+                state.written_objects.add(o)
 
-    else:
-        objects[0].encode(encoder, state)
+            with encoder.write_list() as list_s:
+                for o in objects:
+                    # Allow this specific object to be written now
+                    state.written_objects.remove(o)
+                    with list_s.write_list_item() as item_s:
+                        o.encode(item_s, state)
 
+        else:
+            objects[0].encode(encoder, state)
 
-def decode_objects(decoder):
-    object_ids = {}
-    objects = [
-        SHACLObject.decode(obj_d, object_ids=object_ids)
-        for obj_d in decoder.read_list()
-    ]
+    def decode(self, decoder):
+        self.create_index()
 
-    for o in objects:
-        o.link(object_ids)
+        for obj_d in decoder.read_list():
+            o = SHACLObject.decode(obj_d, doc=self)
+            self.objects.add(o)
 
-    # Remove blank node IDs
-    for o in objects:
-        for c in o.child_objects():
-            if c._id and c._id.startswith("_:"):
-                del c._id
+        self._link()
+
+
+class EncodeState(object):
+    def __init__(self):
+        self.ref_objects = set()
+        self.written_objects = set()
+        self.blank_objects = {}
+
+    def get_object_id(self, o):
+        if o._id:
+            return o._id
+
+        if o not in self.blank_objects:
+            _id = f"_:{o.__class__.__name__}{len(self.blank_objects)}"
+            self.blank_objects[o] = _id
+
+        return self.blank_objects[o]
+
+    def is_refed(self, o):
+        return o in self.ref_objects
+
+    def add_refed(self, o):
+        self.ref_objects.add(o)
 
-    object_ids = {k: v for k, v in object_ids.items() if not k.startswith("_:")}
+    def is_written(self, o):
+        return o in self.written_objects
 
-    return objects, object_ids
+    def add_written(self, o):
+        self.written_objects.add(o)
 
 
 class Decoder(ABC):
     @abstractmethod
     def read_string(self):
         """
         Consume the next item as a string.
@@ -1076,22 +1200,22 @@
         return None, self
 
     def read_object_id(self, alias=None):
         return self.__get_value(alias, "@id")
 
 
 class JSONLDDeserializer(object):
-    def read(self, f):
+    def read(self, f, doc):
         data = json.load(f)
         if "@graph" in data:
             h = JSONLDDecoder(data["@graph"])
         else:
             h = JSONLDDecoder(data)
 
-        return decode_objects(h)
+        doc.decode(h)
 
 
 class Encoder(ABC):
     @abstractmethod
     def write_string(self, v):
         """
         Write a string value
@@ -1276,41 +1400,46 @@
         s = self.__class__(None)
         yield s
         if s.data is not None:
             self.data.append(s.data)
 
 
 class JSONLDSerializer(object):
-    def serialize_data(self, objects, force_graph=False):
-        h = JSONLDEncoder()
-        encode_objects(h, objects, force_graph)
-        if isinstance(h.data, list):
-            data = {
-                "@graph": h.data,
-            }
-        else:
-            data = h.data
+    def __init__(self, **args):
+        self.args = args
 
+    def serialize_data(self, doc, force_graph=False):
+        h = JSONLDEncoder()
+        doc.encode(h, force_graph)
+        data = {}
         if len(CONTEXT_URLS) == 1:
             data["@context"] = CONTEXT_URLS[0]
         elif CONTEXT_URLS:
             data["@context"] = CONTEXT_URLS
 
+        if isinstance(h.data, list):
+            data["@graph"] = h.data
+        else:
+            for k, v in h.data.items():
+                data[k] = v
+
         return data
 
-    def write(self, objects, f, force_graph=False, **kwargs):
+    def write(self, doc, f, force_graph=False, **kwargs):
         """
-        Write a list of objects to a JSON LD file
+        Write a SHACLDocument to a JSON LD file
 
         If force_graph is True, a @graph node will always be written
         """
-        data = self.serialize_data(objects, force_graph)
+        data = self.serialize_data(doc, force_graph)
+
+        args = {**self.args, **kwargs}
 
         sha1 = hashlib.sha1()
-        for chunk in json.JSONEncoder(**kwargs).iterencode(data):
+        for chunk in json.JSONEncoder(**args).iterencode(data):
             chunk = chunk.encode("utf-8")
             f.write(chunk)
             sha1.update(chunk)
 
         return sha1.hexdigest()
 
 
@@ -1326,19 +1455,16 @@
         self.sha1.update(s)
 
     def _write_comma(self):
         if self.comma:
             self.write(",")
             self.comma = False
 
-    def _need_comma(self):
-        self.comma = True
-
     def write_string(self, v):
-        self.write(f'"{v}"')
+        self.write(json.dumps(v))
 
     def write_datetime(self, v):
         self.write_string(v)
 
     def write_integer(self, v):
         self.write(f"{v}")
 
@@ -1351,36 +1477,40 @@
     def write_bool(self, v):
         if v:
             self.write("true")
         else:
             self.write("false")
 
     def write_float(self, v):
-        self.write(f'"{v}"')
+        self.write(json.dumps(str(v)))
 
     @contextmanager
     def write_property(self, iri, compact=None):
         self._write_comma()
-        self.write(f'"{compact or iri}":')
+        self.write_string(compact or iri)
+        self.write(":")
         yield self
         self.comma = True
 
     @contextmanager
     def write_object(self, o, _id, needs_id):
         self._write_comma()
 
         self.write("{")
+        self.write_string("{{ context.compact('@type') }}")
+        self.write(":")
+        self.write_string(o.COMPACT_TYPE or o.TYPE)
+        self.comma = True
+
         if needs_id:
-            idname = o.ID_ALIAS or "@id"
-            idval = _id
-            self.write(f'"{idname}": "{idval}",')
-
-        typname = "{{ context.compact('@type') }}"
-        typval = o.COMPACT_TYPE or o.TYPE
-        self.write(f'"{typname}":"{typval}"')
+            self._write_comma()
+            self.write_string(o.ID_ALIAS or "@id")
+            self.write(":")
+            self.write_string(_id)
+            self.comma = True
 
         self.comma = True
         yield self
 
         self.write("}")
         self.comma = True
 
@@ -1396,32 +1526,35 @@
     def write_list_item(self):
         self._write_comma()
         yield self.__class__(self.f, self.sha1)
         self.comma = True
 
 
 class JSONLDInlineSerializer(object):
-    def write(self, objects, f):
+    def write(self, doc, f, force_graph=False):
         """
-        Write a list of objects to a JSON LD file
+        Write a SHACLDocument to a JSON LD file
+
+        Note: force_graph is included for compatibility, but ignored. This
+        serializer always writes out a graph
         """
         sha1 = hashlib.sha1()
         h = JSONLDInlineEncoder(f, sha1)
         h.write('{"@context":')
         if len(CONTEXT_URLS) == 1:
             h.write(f'"{CONTEXT_URLS[0]}"')
         elif CONTEXT_URLS:
             h.write('["')
             h.write('","'.join(CONTEXT_URLS))
             h.write('"]')
         h.write(",")
 
         h.write('"@graph":')
 
-        encode_objects(h, objects, True)
+        doc.encode(h, True)
         h.write("}")
         return sha1.hexdigest()
 
 
 def print_tree(objects, all_fields=False):
     """
     Print object tree
@@ -1508,41 +1641,39 @@
 # CLASSES
 {%- for class in classes %}
 {%- if class.comment %}
 {%- for l in class.comment.split("\n") %}
 #{% if l %} {% endif %}{{ l.rstrip() }}
 {%- endfor %}
 {%- endif %}
+@register("{{ class._id }}"{%- if context.compact(class._id) != class._id %}, "{{ context.compact(class._id) }}"{%- endif %})
 class {{ varname(class.clsname) }}(
 {%- if class.parent_ids %}
     {%- for id in class.parent_ids %}
         {{- varname(classes.get(id).clsname) }}{% if not loop.last %}, {% endif %}
     {%- endfor %}
 {%- else -%}
     SHACLObject
 {%- endif -%}):
-    TYPE = "{{ class._id }}"
-{%- if context.compact(class._id) != class._id %}
-    COMPACT_TYPE = "{{ context.compact(class._id) }}"
-{%- endif %}
     NODE_KIND = NodeKind.{{ class.node_kind.split("#")[-1] }}
     {%- if class.id_property %}
     ID_ALIAS = "{{ class.id_property }}"
     {%- endif %}
 
-    def __init__(self, **kwargs):
-        super().__init__()
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
         {%- for prop in class.properties %}
         {%- set is_list = prop.max_count is none or prop.max_count != 1 %}
         {%- if prop.comment %}
         {%- for l in prop.comment.split("\n") %}
         #{% if l %} {% endif %}{{ l.rstrip() }}
         {%- endfor %}
         {%- endif %}
-        self._add_property(
+        cls._add_property(
             "{{ varname(prop.varname) }}",
             {% if is_list -%}ListProp({% endif %}
             {%- if prop.class_id -%}
                 ObjectProp({{ varname(classes.get(prop.class_id).clsname) }}, {% if prop.min_count and not is_list %}True{% else %}False{% endif %})
             {%- elif prop.enum_id -%}
                 {{ varname(enums.get(prop.enum_id).clsname) }}(context=[
             {%- for value in enums.get(prop.enum_id).values %}
@@ -1565,21 +1696,14 @@
             min_count={{ prop.min_count }},
             {%- endif %}
             {%- if context.compact_vocab(prop.path) != prop.path %}
             compact="{{ context.compact_vocab(prop.path) }}",
             {%- endif %}
         )
         {%- endfor %}
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["{{ class._id }}"] = {{ varname(class.clsname) }}
-{%- if context.compact(class._id) != class._id %}
-SHACLObject.DESERIALIZERS["{{ context.compact(class._id) }}"] = {{ varname(class.clsname) }}
-{%- endif %}
 
 {% endfor %}
 {{ '"' }}{{ '"' }}{{ '"' }}Format Guard"""
 # fmt: on
 
 
 def main():
@@ -1589,25 +1713,26 @@
     parser = argparse.ArgumentParser(description="Python SHACL model test")
     parser.add_argument("infile", type=Path, help="Input file")
     parser.add_argument("--print", action="store_true", help="Print object tree")
     parser.add_argument("--outfile", type=Path, help="Output file")
 
     args = parser.parse_args()
 
+    doc = SHACLDocument()
     with args.infile.open("r") as f:
         d = JSONLDDeserializer()
-        objects, _ = d.read(f)
+        d.read(f, doc)
 
     if args.print:
-        print_tree(objects)
+        print_tree(doc.objects)
 
     if args.outfile:
         with args.outfile.open("wb") as f:
             s = JSONLDSerializer()
-            s.write(objects, f)
+            s.write(doc, f)
 
     return 0
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `shacl2code-0.0.8/tests/conftest.py` & `shacl2code-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/tests/test_cli.py` & `shacl2code-0.0.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/tests/test_common_jinja.py` & `shacl2code-0.0.9/tests/test_common_jinja.py`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/tests/test_common_prefix.py` & `shacl2code-0.0.9/tests/test_common_prefix.py`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/tests/test_context.py` & `shacl2code-0.0.9/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/tests/test_jsonschema.py` & `shacl2code-0.0.9/tests/test_jsonschema.py`

 * *Files 12% similar despite different names*

```diff
@@ -252,14 +252,22 @@
                 "@graph": [
                     {
                         "@type": "link-class",
                     }
                 ],
             },
         ),
+        # Missing type
+        (
+            False,
+            {
+                "@context": CONTEXT,
+                "@graph": [{}],
+            },
+        ),
         # Unknown object field
         (
             False,
             {
                 "@context": CONTEXT,
                 "@graph": [
                     {
@@ -502,14 +510,21 @@
         # Root object with missing context
         (
             False,
             {
                 "@type": "test-class",
             },
         ),
+        # Root object with missing type
+        (
+            False,
+            {
+                "@context": CONTEXT,
+            },
+        ),
         # Root object with bad context
         (
             False,
             {
                 "@context": "http://foo.bar",
                 "@type": "test-class",
             },
@@ -559,14 +574,105 @@
             False,
             {
                 "@context": CONTEXT,
                 "@type": "inherited-id-prop-class",
                 "@id": "_:blank",
             },
         ),
+        # Extensible class
+        (
+            True,
+            {
+                "@context": CONTEXT,
+                "@type": "extensible-class",
+                "extensible-class/required": "foo",
+                "link-class-link-prop": {
+                    "@type": "link-class",
+                },
+            },
+        ),
+        # Extensible class with custom type
+        (
+            True,
+            {
+                "@context": CONTEXT,
+                "@type": "http://example.com/extended",
+                "extensible-class/required": "foo",
+                "link-class-link-prop": {
+                    "@type": "link-class",
+                },
+            },
+        ),
+        # Extended class with unknown property
+        (
+            True,
+            {
+                "@context": CONTEXT,
+                "@type": "http://example.com/extended",
+                "extensible-class/required": "foo",
+                "unknown-prop": "foo",
+            },
+        ),
+        # Extended class with missing required property
+        (
+            False,
+            {
+                "@context": CONTEXT,
+                "@type": "http://example.com/extended",
+                "unknown-prop": "foo",
+            },
+        ),
+        # Nested extensible class
+        (
+            True,
+            {
+                "@context": CONTEXT,
+                "@type": "link-class",
+                "link-class-link-prop": {
+                    "@type": "extensible-class",
+                    "extensible-class/required": "foo",
+                },
+            },
+        ),
+        # Nested extensible class with custom type
+        (
+            True,
+            {
+                "@context": CONTEXT,
+                "@type": "link-class",
+                "link-class-link-prop": {
+                    "@type": "http://example.com/extended",
+                    "extensible-class/required": "foo",
+                },
+            },
+        ),
+        # Nested extensible class with custom unknown property
+        (
+            True,
+            {
+                "@context": CONTEXT,
+                "@type": "link-class",
+                "link-class-link-prop": {
+                    "@type": "http://example.com/extended",
+                    "extensible-class/required": "foo",
+                    "unknown-prop": "foo",
+                },
+            },
+        ),
+        # Nested extended class with missing required property
+        (
+            False,
+            {
+                "@context": CONTEXT,
+                "@type": "link-class",
+                "link-class-link-prop": {
+                    "@type": "http://example.com/extended",
+                },
+            },
+        ),
         # Base object for type tests
         (True, BASE_OBJ),
     ],
 )
 def test_schema_validation(test_jsonschema, test_context_url, passes, data):
     replace_context(data, test_context_url)
```

### Comparing `shacl2code-0.0.8/tests/test_model_source.py` & `shacl2code-0.0.9/tests/test_model_source.py`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/tests/test_python.py` & `shacl2code-0.0.9/tests/test_python.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import jsonschema
 import pyshacl
 import pytest
 import rdflib
 import re
 import subprocess
 import sys
+import importlib
 from pathlib import Path
 from datetime import datetime, timezone, timedelta
 
 THIS_FILE = Path(__file__)
 THIS_DIR = THIS_FILE.parent
 
 EXPECT_DIR = THIS_DIR / "expect"
@@ -24,28 +25,14 @@
 TEST_MODEL = THIS_DIR / "data" / "model" / "test.ttl"
 
 TEST_CONTEXT = THIS_DIR / "data" / "model" / "test-context.json"
 
 SPDX3_CONTEXT_URL = "https://spdx.github.io/spdx-3-model/context.json"
 
 
-class ObjectSet(object):
-    def __init__(self, objects, object_ids):
-        self.objects = objects
-        self.object_ids = object_ids
-
-    def get_obj(self, _id, typ):
-        o = self.object_ids.get(_id, None)
-        assert o is not None, f"Unable to find {_id}"
-        assert isinstance(
-            o, typ
-        ), f"Object {_id} has wrong type {type(o)}. Expected {typ}"
-        return o
-
-
 @pytest.fixture(scope="session")
 def roundtrip(tmp_path_factory, model_server):
     outfile = tmp_path_factory.mktemp("python-roundtrip") / "roundtrip.json"
     with (DATA_DIR / "python" / "roundtrip.json").open("r") as f:
         data = f.read()
 
     data = data.replace("@CONTEXT_URL@", model_server + "/test-context.json")
@@ -80,22 +67,25 @@
 
 @pytest.fixture(scope="module")
 def test_script(test_context):
     _, script = test_context
     yield script
 
 
-@pytest.fixture(scope="module")
-def import_test_context(test_context):
+@pytest.fixture(scope="function")
+def model(test_context):
     tmp_directory, _ = test_context
 
     old_path = sys.path[:]
     sys.path.append(str(tmp_directory))
     try:
-        yield
+        import model
+
+        importlib.reload(model)
+        yield model
     finally:
         sys.path = old_path
 
 
 @pytest.mark.parametrize(
     "args,expect",
     [
@@ -200,17 +190,15 @@
             encoding="utf-8",
         )
 
         for num, line in enumerate(p.stdout.splitlines()):
             assert "\t" not in line, f"Line {num + 1} has tabs"
 
 
-def test_roundtrip(import_test_context, tmp_path, roundtrip):
-    import model
-
+def test_roundtrip(model, tmp_path, roundtrip):
     def check_file(p, expect, digest):
         sha1 = hashlib.sha1()
         with p.open("rb") as f:
             while True:
                 d = f.read(4096)
                 if not d:
                     break
@@ -219,31 +207,32 @@
         assert sha1.hexdigest() == digest
 
         with p.open("r") as f:
             data = json.load(f)
 
         assert data == expect
 
+    doc = model.SHACLDocument()
     with roundtrip.open("r") as f:
         d = model.JSONLDDeserializer()
-        objects, _ = d.read(f)
+        d.read(f, doc)
 
     with roundtrip.open("r") as f:
         expect_data = json.load(f)
 
     outfile = tmp_path / "out.json"
     with outfile.open("wb") as f:
         s = model.JSONLDSerializer()
-        digest = s.write(objects, f, indent=4)
+        digest = s.write(doc, f, indent=4)
 
     check_file(outfile, expect_data, digest)
 
     with outfile.open("wb") as f:
         s = model.JSONLDInlineSerializer()
-        digest = s.write(objects, f)
+        digest = s.write(doc, f)
 
     check_file(outfile, expect_data, digest)
 
 
 def test_script_roundtrip(test_script, tmp_path, roundtrip):
     outpath = tmp_path / "out.json"
 
@@ -285,23 +274,25 @@
         ),
         (
             "http://serialize.example.com/derived-to-base",
             "http://serialize.example.com/self",
         ),
     ],
 )
-def test_links(import_test_context, name, expect):
-    import model
-
+def test_links(model, name, expect):
+    doc = model.SHACLDocument()
     with (DATA_DIR / "python" / "links.json").open("r") as f:
         deserializer = model.JSONLDDeserializer()
-        d = ObjectSet(*deserializer.read(f))
+        deserializer.read(f, doc)
+
+    c = doc.find_by_id(name)
+    assert isinstance(c, model.link_class)
 
-    c = d.get_obj(name, model.link_class)
-    link = d.get_obj(expect, model.link_class)
+    link = doc.find_by_id(expect)
+    assert isinstance(c, model.link_class)
 
     assert c.link_class_link_prop is link
     assert c.link_class_link_prop_no_class is link
     assert c.link_class_link_list_prop == [link, link]
 
 
 @pytest.mark.parametrize(
@@ -321,32 +312,30 @@
         ),
         (
             "http://serialize.example.com/derived-to-blank-derived",
             "link_derived_class",
         ),
     ],
 )
-def test_blank_links(import_test_context, name, cls):
-    import model
-
+def test_blank_links(model, name, cls):
+    doc = model.SHACLDocument()
     with (DATA_DIR / "python" / "links.json").open("r") as f:
         deserializer = model.JSONLDDeserializer()
-        d = ObjectSet(*deserializer.read(f))
+        deserializer.read(f, doc)
 
-    c = d.get_obj(name, model.link_class)
+    c = doc.find_by_id(name)
+    assert isinstance(c, model.link_class)
 
     expect = c.link_class_link_prop
     assert type(expect) is getattr(model, cls)
     assert c.link_class_link_prop_no_class is expect
     assert c.link_class_link_list_prop == [expect, expect]
 
 
-def test_node_kind_blank(import_test_context, test_context_url):
-    import model
-
+def test_node_kind_blank(model, test_context_url):
     s = model.JSONLDSerializer()
     c1 = model.link_class()
     c2 = model.link_class()
 
     c1._id = "http://example.com/c1"
     c2._id = "http://example.com/c2"
 
@@ -356,15 +345,15 @@
         ref._id = "http://example.com/name"
 
     # Blank node assignment is fine but not preserved when serializing
     ref._id = "_:blank"
 
     # No blank ID is written out for one reference (inline)
     c1.link_class_link_prop = ref
-    result = s.serialize_data([c1, c2])
+    result = s.serialize_data(model.SHACLDocument([c1, c2]))
     assert result == {
         "@context": test_context_url,
         "@graph": [
             {
                 "@type": "link-class",
                 "@id": "http://example.com/c1",
                 "link-class-link-prop": {
@@ -376,15 +365,15 @@
                 "@id": "http://example.com/c2",
             },
         ],
     }
 
     # Blank node is written out for multiple references
     c2.link_class_link_prop = ref
-    result = s.serialize_data([c1, c2])
+    result = s.serialize_data(model.SHACLDocument([c1, c2]))
     assert result == {
         "@context": test_context_url,
         "@graph": [
             {
                 "@type": "node-kind-blank",
                 "@id": "_:node_kind_blank0",
             },
@@ -398,15 +387,15 @@
                 "@id": "http://example.com/c2",
                 "link-class-link-prop": "_:node_kind_blank0",
             },
         ],
     }
 
     # Listing in the root graph requires a blank node be written
-    result = s.serialize_data([c1, ref])
+    result = s.serialize_data(model.SHACLDocument([c1, ref]))
     assert result == {
         "@context": test_context_url,
         "@graph": [
             {
                 "@type": "node-kind-blank",
                 "@id": "_:node_kind_blank0",
             },
@@ -419,17 +408,15 @@
     }
 
 
 @pytest.mark.parametrize(
     "cls",
     ["node_kind_iri", "derived_node_kind_iri"],
 )
-def test_node_kind_iri(import_test_context, test_context_url, cls):
-    import model
-
+def test_node_kind_iri(model, test_context_url, cls):
     TEST_ID = "http://serialize.example.com/name"
     TYP = cls.replace("_", "-")
 
     s = model.JSONLDSerializer()
     c1 = model.link_class()
     c2 = model.link_class()
 
@@ -439,21 +426,21 @@
     ref = getattr(model, cls)()
 
     with pytest.raises(ValueError):
         ref._id = "_:blank"
 
     # serializing without an ID is not allowed
     with pytest.raises(ValueError):
-        s.serialize_data([ref])
+        s.serialize_data(model.SHACLDocument([ref]))
 
     # Inlining not allowed
     ref._id = TEST_ID
 
     c1.link_class_link_prop = ref
-    result = s.serialize_data([c1, c2])
+    result = s.serialize_data(model.SHACLDocument([c1, c2]))
     assert result == {
         "@context": test_context_url,
         "@graph": [
             {
                 "@type": "link-class",
                 "@id": "http://example.com/c1",
                 "link-class-link-prop": TEST_ID,
@@ -467,15 +454,15 @@
                 "@id": TEST_ID,
             },
         ],
     }
 
     # Multiple references
     c2.link_class_link_prop = ref
-    result = s.serialize_data([c1, c2])
+    result = s.serialize_data(model.SHACLDocument([c1, c2]))
     assert result == {
         "@context": test_context_url,
         "@graph": [
             {
                 "@type": "link-class",
                 "@id": "http://example.com/c1",
                 "link-class-link-prop": TEST_ID,
@@ -489,15 +476,15 @@
                 "@type": TYP,
                 "@id": TEST_ID,
             },
         ],
     }
 
     # Listing in the root graph forces reference
-    result = s.serialize_data([c1, ref])
+    result = s.serialize_data(model.SHACLDocument([c1, ref]))
     assert result == {
         "@context": test_context_url,
         "@graph": [
             {
                 "@type": "link-class",
                 "@id": "http://example.com/c1",
                 "link-class-link-prop": TEST_ID,
@@ -510,17 +497,15 @@
     }
 
 
 @pytest.mark.parametrize(
     "cls",
     ["id_prop_class", "inherited_id_prop_class"],
 )
-def test_id_name(import_test_context, test_context_url, cls):
-    import model
-
+def test_id_name(model, test_context_url, cls):
     s = model.JSONLDSerializer()
     c = getattr(model, cls)()
 
     TEST_ID = "http://serialize.example.com/name"
 
     # Assign alternate ID
     c.testid = TEST_ID
@@ -532,15 +517,15 @@
     # Delete id
     del c.testid
     assert c.testid is None
     assert c._id is None
 
     # Serialization should the alias name
     c._id = TEST_ID
-    result = s.serialize_data([c])
+    result = s.serialize_data(model.SHACLDocument([c]))
     assert result == {
         "@context": test_context_url,
         "@type": cls.replace("_", "-"),
         "testid": TEST_ID,
     }
 
 
@@ -804,32 +789,53 @@
         ("import_", "foo", "foo"),
         # A property that conflicts with an existing attribute
         ("encode_", "foo", "foo"),
         # Verify that existing attributes cannot be overwritten
         ("encode", "foo", AttributeError),
     ],
 )
-def test_scalar_prop_validation(import_test_context, prop, value, expect):
-    import model
-
+def test_scalar_prop_validation(model, prop, value, expect):
     c = model.test_class()
 
     if callable(value):
         value = value(model)
 
     if expect is SAME_AS_VALUE:
         expect = value
 
-    if isinstance(expect, type) and issubclass(expect, Exception):
-        with pytest.raises(expect):
+    kwargs = {prop: value}
+
+    for cls in model.test_class, model.test_derived_class:
+        c = cls()
+
+        if isinstance(expect, type) and issubclass(expect, Exception):
+            with pytest.raises(expect):
+                setattr(c, prop, value)
+
+            with pytest.raises(expect):
+                c = cls(**kwargs)
+        else:
             setattr(c, prop, value)
-    else:
-        setattr(c, prop, value)
-        assert getattr(c, prop) == expect
-        assert type(getattr(c, prop)) is type(expect)
+            assert getattr(c, prop) == expect
+            assert type(getattr(c, prop)) is type(expect)
+
+            c = cls(**kwargs)
+            assert getattr(c, prop) == expect
+            assert type(getattr(c, prop)) is type(expect)
+
+
+def test_derived_property(model):
+    # The test above covers most of the test cases with setting properties, but
+    # it doesn't cover if the property is defined in the derived class, so test
+    # those here
+    c = model.test_derived_class(test_derived_class_string_prop="abc")
+    assert c.test_derived_class_string_prop == "abc"
+
+    c.test_derived_class_string_prop = "def"
+    assert c.test_derived_class_string_prop == "def"
 
 
 def list_type_tests(name, *typ):
     tests = [
         # Non list types
         (name, 1, TypeError),
         (name, 1.0, TypeError),
@@ -988,66 +994,69 @@
         ("test_class_regex_list", ["bar"], ValueError),
         ("test_class_regex_list", ["fooa"], ValueError),
         ("test_class_regex_list", ["afoo1"], ValueError),
         *list_type_tests("test_class_regex_list", str),
         # TODO Add more list tests
     ],
 )
-def test_list_prop_validation(import_test_context, prop, value, expect):
-    import model
-
+def test_list_prop_validation(model, prop, value, expect):
     c = model.test_class()
 
     if callable(value):
         value = value(model)
 
     if expect is SAME_AS_VALUE:
         expect = value
 
-    if isinstance(expect, type) and issubclass(expect, Exception):
-        with pytest.raises(expect):
-            if value is list:
-                for v in value:
-                    getattr(c, prop).append(v)
-            else:
-                setattr(c, prop, value)
-
-    else:
-        for v in value:
-            getattr(c, prop).append(v)
-
-        import pprint
+    kwargs = {prop: value}
+    for cls in model.test_class, model.test_derived_class:
+        c = cls()
+
+        if isinstance(expect, type) and issubclass(expect, Exception):
+            with pytest.raises(expect):
+                if value is list:
+                    for v in value:
+                        getattr(c, prop).append(v)
+                else:
+                    setattr(c, prop, value)
+
+            with pytest.raises(expect):
+                cls(**kwargs)
+
+        else:
+            for v in value:
+                getattr(c, prop).append(v)
+
+            assert getattr(c, prop) == expect
+            for idx, v in enumerate(expect):
+                assert getattr(c, prop)[idx] == v
+                assert type(getattr(c, prop)[idx]) is type(v)
+
+            setattr(c, prop, value[:])
+            assert getattr(c, prop) == expect
+
+            assert list(getattr(c, prop)) == expect
+
+            getattr(c, prop).sort()
+            assert getattr(c, prop) == list(sorted(expect))
+
+            setattr(c, prop, [])
+            getattr(c, prop).extend(value)
+            assert getattr(c, prop) == expect
+
+            setattr(c, prop, [])
+            for v in value:
+                getattr(c, prop).insert(0, v)
+            assert getattr(c, prop) == list(reversed(expect))
 
-        pprint.pprint(getattr(c, prop))
-        pprint.pprint(expect)
+            for v in expect:
+                assert v in getattr(c, prop)
 
-        assert getattr(c, prop) == expect
-        for idx, v in enumerate(expect):
-            assert getattr(c, prop)[idx] == v
-            assert type(getattr(c, prop)[idx]) is type(v)
-
-        setattr(c, prop, value[:])
-        assert getattr(c, prop) == expect
-
-        assert list(getattr(c, prop)) == expect
-
-        getattr(c, prop).sort()
-        assert getattr(c, prop) == list(sorted(expect))
-
-        setattr(c, prop, [])
-        getattr(c, prop).extend(value)
-        assert getattr(c, prop) == expect
-
-        setattr(c, prop, [])
-        for v in value:
-            getattr(c, prop).insert(0, v)
-        assert getattr(c, prop) == list(reversed(expect))
-
-        for v in expect:
-            assert v in getattr(c, prop)
+            c = cls(**kwargs)
+            assert getattr(c, prop) == expect
 
 
 @pytest.mark.parametrize(
     "value,expect",
     [
         (
             "2024-03-11T01:02:03",
@@ -1083,17 +1092,15 @@
         # Timezone with seconds not allowed
         (
             "2024-03-11T01:02:03+03:00:01",
             ValueError,
         ),
     ],
 )
-def test_datetime_from_string(import_test_context, value, expect):
-    import model
-
+def test_datetime_from_string(model, value, expect):
     p = model.DateTimeProp()
 
     if isinstance(expect, type) and issubclass(expect, Exception):
         with pytest.raises(expect):
             p.from_string(value)
     else:
         v = p.from_string(value)
@@ -1138,17 +1145,15 @@
         # Timezone with seconds not allowed
         (
             "2024-03-11T01:02:03+03:00:01",
             ValueError,
         ),
     ],
 )
-def test_datetimestamp_from_string(import_test_context, value, expect):
-    import model
-
+def test_datetimestamp_from_string(model, value, expect):
     p = model.DateTimeStampProp()
 
     if isinstance(expect, type) and issubclass(expect, Exception):
         with pytest.raises(expect):
             p.from_string(value)
     else:
         v = p.from_string(value)
@@ -1208,101 +1213,95 @@
                 3,
                 tzinfo=timezone(timedelta(hours=-3, minutes=-21, seconds=31)),
             ),
             "2024-03-11T01:02:03-03:21",
         ),
     ],
 )
-def test_datetime_to_string(import_test_context, value, expect):
-    import model
-
+def test_datetime_to_string(model, value, expect):
     p = model.DateTimeProp()
 
     if isinstance(expect, type) and issubclass(expect, Exception):
         with pytest.raises(expect):
             p.to_string(value)
     else:
         v = p.to_string(value)
         assert v == expect
         assert re.match(
             model.DateTimeProp.REGEX, v
         ), f"Value '{v}' does not match regex"
 
 
-def test_enum_var_names(import_test_context):
-    import model
-
+def test_enum_var_names(model):
     assert type(model.enumType.foo) is str
     assert model.enumType.foo == "http://example.org/enumType/foo"
 
     c = model.test_class()
 
     for name, value in model.enumType.valid_values:
         c.test_class_enum_prop = value
         assert getattr(model.enumType, name) == value
 
 
-def test_mandatory_properties(import_test_context, tmp_path):
+def test_mandatory_properties(model, tmp_path):
     """
     Tests that property ordinality (e.g. min count & max count) is checked when
     writing out a file
     """
-    import model
-
     s = model.JSONLDSerializer()
     outfile = tmp_path / "test.json"
 
     def base_obj():
         c = model.test_class_required()
         c.test_class_required_string_scalar_prop = "foo"
         c.test_class_required_string_list_prop = ["bar", "baz"]
         return c
 
     # First validate that the base object is actually valid
     c = base_obj()
     with outfile.open("wb") as f:
-        s.write([c], f)
+        s.write(model.SHACLDocument([c]), f)
 
     # Required scalar property
     c = base_obj()
     del c.test_class_required_string_scalar_prop
     with outfile.open("wb") as f:
         with pytest.raises(ValueError):
-            s.write([c], f)
+            s.write(model.SHACLDocument([c]), f)
 
     # Array that is deleted
     c = base_obj()
     del c.test_class_required_string_list_prop
     with outfile.open("wb") as f:
         with pytest.raises(ValueError):
-            s.write([c], f)
+            s.write(model.SHACLDocument([c]), f)
 
     # Array initialized to empty list
     c = base_obj()
     c.test_class_required_string_list_prop = []
     with outfile.open("wb") as f:
         with pytest.raises(ValueError):
-            s.write([c], f)
+            s.write(model.SHACLDocument([c]), f)
 
     # Array with too many items
     c = base_obj()
     c.test_class_required_string_list_prop.append("too many")
     with outfile.open("wb") as f:
         with pytest.raises(ValueError):
-            s.write([c], f)
+            s.write(model.SHACLDocument([c]), f)
 
 
-def test_iri(import_test_context, roundtrip):
-    import model
-
+def test_iri(model, roundtrip):
+    doc = model.SHACLDocument()
     with roundtrip.open("r") as f:
         deserializer = model.JSONLDDeserializer()
-        d = ObjectSet(*deserializer.read(f))
+        deserializer.read(f, doc)
 
-    c = d.get_obj("http://serialize.example.com/test", model.test_class)
+    c = doc.find_by_id("http://serialize.example.com/test")
+    assert isinstance(c, model.test_class)
 
     assert c._IRI["_id"] == "@id"
     assert c._IRI["named_property"] == "http://example.org/test-class/named-property"
 
     for name, iri in c._IRI.items():
         assert c[iri] == getattr(c, name)
 
@@ -1321,7 +1320,62 @@
 
     conforms, result_graph, result_text = pyshacl.validate(
         data,
         shacl_graph=model,
         ont_graph=model,
     )
     assert conforms, result_text
+
+
+def test_single_register(model):
+    # Ensures that class property registration is only called once
+    assert model.test_class._NEEDS_REG
+    c1 = model.test_class()
+    assert not model.test_class._NEEDS_REG
+
+    c2 = model.test_class()
+    assert not model.test_class._NEEDS_REG
+
+    c1.test_class_string_scalar_prop = "abc"
+    c2.test_class_string_scalar_prop = "def"
+
+    assert c1.test_class_string_scalar_prop == "abc"
+    assert c2.test_class_string_scalar_prop == "def"
+
+    assert model.test_derived_class._NEEDS_REG
+    _ = model.test_derived_class()
+    assert not model.test_derived_class._NEEDS_REG
+
+    _ = model.test_derived_class()
+    assert not model.test_derived_class._NEEDS_REG
+
+
+def test_doc_foreach_type(model, roundtrip):
+    doc = model.SHACLDocument()
+    with roundtrip.open("r") as f:
+        model.JSONLDDeserializer().read(f, doc)
+
+    expect = set()
+
+    expect.add(doc.find_by_id("http://serialize.example.com/test"))
+    expect.add(doc.find_by_id("http://serialize.example.com/nested-parent"))
+    expect.add(
+        doc.find_by_id(
+            "http://serialize.example.com/nested-parent"
+        ).test_class_class_prop
+    )
+    expect.add(doc.find_by_id("http://serialize.example.com/test-special-chars"))
+    assert expect != {None}
+
+    assert set(doc.foreach_type(model.test_class)) == expect
+    assert set(doc.foreach_type("test-class")) == expect
+    assert set(doc.foreach_type("http://example.org/test-class")) == expect
+
+    expect.add(doc.find_by_id("http://serialize.example.com/required"))
+    expect.add(doc.find_by_id("http://serialize.example.com/test-derived"))
+    assert expect != {None}
+
+    assert set(doc.foreach_type(model.test_class, subclass=True)) == expect
+    assert set(doc.foreach_type("test-class", subclass=True)) == expect
+    assert (
+        set(doc.foreach_type("http://example.org/test-class", subclass=True)) == expect
+    )
```

### Comparing `shacl2code-0.0.8/tests/data/bad-pattern-class.ttl` & `shacl2code-0.0.9/tests/data/bad-pattern-class.ttl`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/tests/data/bad-pattern-integer.ttl` & `shacl2code-0.0.9/tests/data/bad-pattern-integer.ttl`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/tests/data/bad-reference.jsonld` & `shacl2code-0.0.9/tests/data/bad-reference.jsonld`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/tests/data/missing-range.ttl` & `shacl2code-0.0.9/tests/data/missing-range.ttl`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/tests/data/model/test-context.json` & `shacl2code-0.0.9/tests/data/model/test-context.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'@context'": "{'extensible-class/required': OrderedDict([('@id', "*

 * *               "'test:extensible-class/required'), ('@type', 'xsd:string')])}"}*

```diff
@@ -1,10 +1,14 @@
 {
     "@context": {
         "@base": "http://example.org/",
+        "extensible-class/required": {
+            "@id": "test:extensible-class/required",
+            "@type": "xsd:string"
+        },
         "link-class-link-list-prop": {
             "@id": "test:link-class-list-prop",
             "@type": "@id"
         },
         "link-class-link-prop": {
             "@id": "test:link-class-prop",
             "@type": "@id"
```

### Comparing `shacl2code-0.0.8/tests/data/model/test.ttl` & `shacl2code-0.0.9/tests/data/model/test.ttl`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,20 @@
         sh:minCount 1 ;
         sh:maxCount 2
     ]
     .
 
 <test-derived-class> a sh:NodeShape, owl:Class ;
     rdfs:subClassOf <test-class> ;
-    rdfs:comment "A class derived from test-class"
+    rdfs:comment "A class derived from test-class" ;
+    sh:property [
+        sh:datatype xsd:string ;
+        sh:path <test-derived-class/string-prop> ;
+        sh:maxCount 1
+    ]
     .
 
 <test-another-class> a sh:NodeShape, owl:Class ;
     rdfs:comment "Another class"
     .
 
 
@@ -309,14 +314,19 @@
     .
 
 <test-class/non-shape> a rdf:Property ;
     rdfs:comment "A class with no shape" ;
     rdfs:range <non-shape-class>
     .
 
+<test-derived-class/string-prop> a rdf:Property ;
+    rdfs:comment "A string property in a derived class" ;
+    rdfs:range xsd:string
+    .
+
 <non-shape-class> a owl:Class ;
     rdfs:comment "A class that is not a nodeshape"
     .
 
 <enumType> a owl:Class ;
     rdfs:comment "An enumerated type"
     .
@@ -406,7 +416,24 @@
     sh:nodeKind sh:BlankNodeOrIRI
     .
 
 <derived-node-kind-iri> a rdf:Class, sh:NodeShape, owl:Class ;
     rdfs:subClassOf <node-kind-iri> ;
     rdfs:comment "A class that derives its nodeKind from parent" ;
     .
+
+<extensible-class> a rdf:Class, sh:NodeShape, owl:Class ;
+    rdfs:subClassOf <link-class> ;
+    sh-to-code:isExtensible true ;
+    rdfs:comment "An extensible class" ;
+    sh:property [
+        sh:datatype xsd:string ;
+        sh:path <extensible-class/required> ;
+        sh:maxCount 1 ;
+        sh:minCount 1
+    ]
+    .
+
+<extensible-class/required> a rdf:Property ;
+    rdfs:comment "A required string" ;
+    rdfs:range xsd:string
+    .
```

### Comparing `shacl2code-0.0.8/tests/data/python/links.json` & `shacl2code-0.0.9/tests/data/python/links.json`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/tests/data/python/roundtrip.json` & `shacl2code-0.0.9/tests/data/python/roundtrip.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'@graph'": "{insert: [(6, OrderedDict([('@type', 'test-class'), ('@id', "*

 * *             "'http://serialize.example.com/test-special-chars'), "*

 * *             '(\'test-class/string-scalar-prop\', \'special chars "\\n\\r:{}[]\')]))]}'}*

```diff
@@ -72,10 +72,15 @@
                 "world"
             ],
             "test-class/string-scalar-prop": "hello"
         },
         {
             "@id": "http://serialize.example.com/test-derived",
             "@type": "test-derived-class"
+        },
+        {
+            "@id": "http://serialize.example.com/test-special-chars",
+            "@type": "test-class",
+            "test-class/string-scalar-prop": "special chars \"\n\r:{}[]"
         }
     ]
 }
```

### Comparing `shacl2code-0.0.8/tests/expect/make_expect.py` & `shacl2code-0.0.9/tests/expect/make_expect.py`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/tests/expect/jsonschema/test-context.json` & `shacl2code-0.0.9/tests/expect/jsonschema/test-context.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9904025011446886%*

 * *Differences: {"'$defs'": "{'idpropclass': {'allOf': {0: {'properties': {'@type': {replace: "*

 * *            "OrderedDict([('oneOf', [OrderedDict([('const', 'id-prop-class')])])])}}}}}, "*

 * *            "'idpropclass_derived': {'anyOf': [OrderedDict([('$ref', "*

 * *            "'#/$defs/inheritedidpropclass')]), OrderedDict([('$ref', '#/$defs/idpropclass')]), "*

 * *            "OrderedDict([('$ref', '#/$defs/BlankNodeOrIRI')])], delete: ['oneOf']}, "*

 * *            "'inheritedidpropclass': {'allOf': {0: {'properties': {'@type': {replace: […]*

```diff
@@ -1,12 +1,12 @@
 {
     "$comment": "This file was automatically generated by shacl2code. DO NOT MANUALLY MODIFY IT",
     "$defs": {
         "AnyClass": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/idpropclass"
                 },
                 {
                     "$ref": "#/$defs/inheritedidpropclass"
                 },
                 {
@@ -21,14 +21,17 @@
                 {
                     "$ref": "#/$defs/nodekindiri"
                 },
                 {
                     "$ref": "#/$defs/nodekindiriorblank"
                 },
                 {
+                    "$ref": "#/$defs/nonshapeclass"
+                },
+                {
                     "$ref": "#/$defs/parentclass"
                 },
                 {
                     "$ref": "#/$defs/testanotherclass"
                 },
                 {
                     "$ref": "#/$defs/testclass"
@@ -40,19 +43,22 @@
                     "$ref": "#/$defs/testderivedclass"
                 },
                 {
                     "$ref": "#/$defs/aaaderivedclass"
                 },
                 {
                     "$ref": "#/$defs/derivednodekindiri"
+                },
+                {
+                    "$ref": "#/$defs/extensibleclass"
                 }
             ]
         },
         "BlankNode": {
-            "pattern": "^_:.*",
+            "pattern": "^_:.+",
             "type": "string"
         },
         "BlankNodeOrIRI": {
             "oneOf": [
                 {
                     "$ref": "#/$defs/IRI"
                 },
@@ -64,38 +70,47 @@
         "DateTime": {
             "type": "string"
         },
         "Extension": {
             "type": "string"
         },
         "IRI": {
-            "pattern": "^(?!_:).*",
+            "pattern": "^(?!_:).+:.+",
             "type": "string"
         },
         "MediaType": {
             "type": "string"
         },
         "SHACLClass": {
             "properties": {
                 "@type": {
-                    "enum": [
-                        "id-prop-class",
-                        "inherited-id-prop-class",
-                        "link-class",
-                        "link-derived-class",
-                        "node-kind-blank",
-                        "node-kind-iri",
-                        "node-kind-iri-or-blank",
-                        "parent-class",
-                        "test-another-class",
-                        "test-class",
-                        "test-class-required",
-                        "test-derived-class",
-                        "aaa-derived-class",
-                        "derived-node-kind-iri"
+                    "oneOf": [
+                        {
+                            "$ref": "#/$defs/IRI"
+                        },
+                        {
+                            "enum": [
+                                "id-prop-class",
+                                "inherited-id-prop-class",
+                                "link-class",
+                                "link-derived-class",
+                                "node-kind-blank",
+                                "node-kind-iri",
+                                "node-kind-iri-or-blank",
+                                "non-shape-class",
+                                "parent-class",
+                                "test-another-class",
+                                "test-class",
+                                "test-class-required",
+                                "test-derived-class",
+                                "aaa-derived-class",
+                                "derived-node-kind-iri",
+                                "extensible-class"
+                            ]
+                        }
                     ]
                 }
             },
             "required": [
                 "@type"
             ],
             "type": "object"
@@ -107,25 +122,29 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "aaa-derived-class"
+                            "oneOf": [
+                                {
+                                    "const": "aaa-derived-class"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/aaaderivedclass_props"
                 }
             ]
         },
         "aaaderivedclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/aaaderivedclass"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -148,28 +167,32 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/IRI"
                         },
                         "@type": {
-                            "const": "derived-node-kind-iri"
+                            "oneOf": [
+                                {
+                                    "const": "derived-node-kind-iri"
+                                }
+                            ]
                         }
                     },
                     "required": [
                         "@id"
                     ]
                 },
                 {
                     "$ref": "#/$defs/derivednodekindiri_props"
                 }
             ]
         },
         "derivednodekindiri_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/derivednodekindiri"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -181,33 +204,89 @@
                     "$ref": "#/$defs/nodekindiri_props"
                 },
                 {
                     "properties": {}
                 }
             ]
         },
+        "extensibleclass": {
+            "allOf": [
+                {
+                    "properties": {
+                        "@id": {
+                            "$ref": "#/$defs/BlankNodeOrIRI"
+                        },
+                        "@type": {
+                            "oneOf": [
+                                {
+                                    "$ref": "#/$defs/IRI"
+                                },
+                                {
+                                    "const": "extensible-class"
+                                }
+                            ]
+                        }
+                    },
+                    "unevaluatedProperties": true
+                },
+                {
+                    "$ref": "#/$defs/extensibleclass_props"
+                }
+            ]
+        },
+        "extensibleclass_derived": {
+            "anyOf": [
+                {
+                    "$ref": "#/$defs/extensibleclass"
+                },
+                {
+                    "$ref": "#/$defs/BlankNodeOrIRI"
+                }
+            ]
+        },
+        "extensibleclass_props": {
+            "allOf": [
+                {
+                    "$ref": "#/$defs/linkclass_props"
+                },
+                {
+                    "properties": {
+                        "extensible-class/required": {
+                            "$ref": "#/$defs/prop_extensibleclass_extensibleclassrequired"
+                        }
+                    },
+                    "required": [
+                        "extensible-class/required"
+                    ]
+                }
+            ]
+        },
         "idpropclass": {
             "allOf": [
                 {
                     "properties": {
                         "@type": {
-                            "const": "id-prop-class"
+                            "oneOf": [
+                                {
+                                    "const": "id-prop-class"
+                                }
+                            ]
                         },
                         "testid": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/idpropclass_props"
                 }
             ]
         },
         "idpropclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/inheritedidpropclass"
                 },
                 {
                     "$ref": "#/$defs/idpropclass"
                 },
                 {
@@ -227,28 +306,32 @@
             ]
         },
         "inheritedidpropclass": {
             "allOf": [
                 {
                     "properties": {
                         "@type": {
-                            "const": "inherited-id-prop-class"
+                            "oneOf": [
+                                {
+                                    "const": "inherited-id-prop-class"
+                                }
+                            ]
                         },
                         "testid": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/inheritedidpropclass_props"
                 }
             ]
         },
         "inheritedidpropclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/inheritedidpropclass"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -268,29 +351,36 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "link-class"
+                            "oneOf": [
+                                {
+                                    "const": "link-class"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/linkclass_props"
                 }
             ]
         },
         "linkclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/derivednodekindiri"
                 },
                 {
+                    "$ref": "#/$defs/extensibleclass"
+                },
+                {
                     "$ref": "#/$defs/linkderivedclass"
                 },
                 {
                     "$ref": "#/$defs/nodekindblank"
                 },
                 {
                     "$ref": "#/$defs/nodekindiri"
@@ -338,25 +428,29 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "link-derived-class"
+                            "oneOf": [
+                                {
+                                    "const": "link-derived-class"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/linkderivedclass_props"
                 }
             ]
         },
         "linkderivedclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/linkderivedclass"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -376,25 +470,29 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNode"
                         },
                         "@type": {
-                            "const": "node-kind-blank"
+                            "oneOf": [
+                                {
+                                    "const": "node-kind-blank"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/nodekindblank_props"
                 }
             ]
         },
         "nodekindblank_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/nodekindblank"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -414,28 +512,32 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/IRI"
                         },
                         "@type": {
-                            "const": "node-kind-iri"
+                            "oneOf": [
+                                {
+                                    "const": "node-kind-iri"
+                                }
+                            ]
                         }
                     },
                     "required": [
                         "@id"
                     ]
                 },
                 {
                     "$ref": "#/$defs/nodekindiri_props"
                 }
             ]
         },
         "nodekindiri_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/derivednodekindiri"
                 },
                 {
                     "$ref": "#/$defs/nodekindiri"
                 },
                 {
@@ -458,25 +560,29 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "node-kind-iri-or-blank"
+                            "oneOf": [
+                                {
+                                    "const": "node-kind-iri-or-blank"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/nodekindiriorblank_props"
                 }
             ]
         },
         "nodekindiriorblank_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/nodekindiriorblank"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -488,33 +594,79 @@
                     "$ref": "#/$defs/linkclass_props"
                 },
                 {
                     "properties": {}
                 }
             ]
         },
+        "nonshapeclass": {
+            "allOf": [
+                {
+                    "properties": {
+                        "@id": {
+                            "$ref": "#/$defs/BlankNodeOrIRI"
+                        },
+                        "@type": {
+                            "oneOf": [
+                                {
+                                    "const": "non-shape-class"
+                                }
+                            ]
+                        }
+                    }
+                },
+                {
+                    "$ref": "#/$defs/nonshapeclass_props"
+                }
+            ]
+        },
+        "nonshapeclass_derived": {
+            "anyOf": [
+                {
+                    "$ref": "#/$defs/nonshapeclass"
+                },
+                {
+                    "$ref": "#/$defs/BlankNodeOrIRI"
+                }
+            ],
+            "unevaluatedProperties": false
+        },
+        "nonshapeclass_props": {
+            "allOf": [
+                {
+                    "$ref": "#/$defs/SHACLClass"
+                },
+                {
+                    "properties": {}
+                }
+            ]
+        },
         "parentclass": {
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "parent-class"
+                            "oneOf": [
+                                {
+                                    "const": "parent-class"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/parentclass_props"
                 }
             ]
         },
         "parentclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/aaaderivedclass"
                 },
                 {
                     "$ref": "#/$defs/testclass"
                 },
                 {
@@ -538,14 +690,17 @@
                     "$ref": "#/$defs/SHACLClass"
                 },
                 {
                     "properties": {}
                 }
             ]
         },
+        "prop_extensibleclass_extensibleclassrequired": {
+            "type": "string"
+        },
         "prop_linkclass_linkclasslinklistprop": {
             "$ref": "#/$defs/linkclass_derived"
         },
         "prop_linkclass_linkclasslinkprop": {
             "$ref": "#/$defs/linkclass_derived"
         },
         "prop_linkclass_linkclasslinkpropnoclass": {
@@ -635,15 +790,15 @@
             "type": "integer"
         },
         "prop_testclass_testclassnonnegativeintegerprop": {
             "minimum": 0,
             "type": "integer"
         },
         "prop_testclass_testclassnonshape": {
-            "$ref": "#/$defs/anyURI"
+            "$ref": "#/$defs/nonshapeclass_derived"
         },
         "prop_testclass_testclasspositiveintegerprop": {
             "minimum": 1,
             "type": "integer"
         },
         "prop_testclass_testclassregex": {
             "pattern": "^foo\\d",
@@ -686,33 +841,40 @@
         },
         "prop_testclassrequired_testclassrequiredstringlistprop": {
             "type": "string"
         },
         "prop_testclassrequired_testclassrequiredstringscalarprop": {
             "type": "string"
         },
+        "prop_testderivedclass_testderivedclassstringprop": {
+            "type": "string"
+        },
         "testanotherclass": {
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "test-another-class"
+                            "oneOf": [
+                                {
+                                    "const": "test-another-class"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/testanotherclass_props"
                 }
             ]
         },
         "testanotherclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/testanotherclass"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -732,25 +894,29 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "test-class"
+                            "oneOf": [
+                                {
+                                    "const": "test-class"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/testclass_props"
                 }
             ]
         },
         "testclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/testclassrequired"
                 },
                 {
                     "$ref": "#/$defs/testderivedclass"
                 },
                 {
@@ -897,25 +1063,29 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "test-class-required"
+                            "oneOf": [
+                                {
+                                    "const": "test-class-required"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/testclassrequired_props"
                 }
             ]
         },
         "testclassrequired_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/testclassrequired"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -955,25 +1125,29 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "test-derived-class"
+                            "oneOf": [
+                                {
+                                    "const": "test-derived-class"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/testderivedclass_props"
                 }
             ]
         },
         "testderivedclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/testderivedclass"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -981,15 +1155,19 @@
         },
         "testderivedclass_props": {
             "allOf": [
                 {
                     "$ref": "#/$defs/testclass_props"
                 },
                 {
-                    "properties": {}
+                    "properties": {
+                        "test-derived-class/string-prop": {
+                            "$ref": "#/$defs/prop_testderivedclass_testderivedclassstringprop"
+                        }
+                    }
                 }
             ]
         }
     },
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "oneOf": [
         {
```

### Comparing `shacl2code-0.0.8/tests/expect/jsonschema/test.json` & `shacl2code-0.0.9/tests/expect/jsonschema/test.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9890314298796442%*

 * *Differences: {"'$defs'": "{'http_exampleorgidpropclass': {'allOf': {0: {'properties': {'@type': {replace: "*

 * *            "OrderedDict([('oneOf', [OrderedDict([('const', "*

 * *            "'http://example.org/id-prop-class')])])])}}}}}, 'http_exampleorgidpropclass_derived': "*

 * *            "{'anyOf': [OrderedDict([('$ref', '#/$defs/http_exampleorginheritedidpropclass')]), "*

 * *            "OrderedDict([('$ref', '#/$defs/http_exampleorgidpropclass')]), OrderedDict([('$ref', "*

 * *            "'#/$defs/BlankNodeOrIRI')])], delete: ['one […]*

```diff
@@ -1,12 +1,12 @@
 {
     "$comment": "This file was automatically generated by shacl2code. DO NOT MANUALLY MODIFY IT",
     "$defs": {
         "AnyClass": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/http_exampleorgidpropclass"
                 },
                 {
                     "$ref": "#/$defs/http_exampleorginheritedidpropclass"
                 },
                 {
@@ -21,14 +21,17 @@
                 {
                     "$ref": "#/$defs/http_exampleorgnodekindiri"
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgnodekindiriorblank"
                 },
                 {
+                    "$ref": "#/$defs/http_exampleorgnonshapeclass"
+                },
+                {
                     "$ref": "#/$defs/http_exampleorgparentclass"
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgtestanotherclass"
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgtestclass"
@@ -40,19 +43,22 @@
                     "$ref": "#/$defs/http_exampleorgtestderivedclass"
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgaaaderivedclass"
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgderivednodekindiri"
+                },
+                {
+                    "$ref": "#/$defs/http_exampleorgextensibleclass"
                 }
             ]
         },
         "BlankNode": {
-            "pattern": "^_:.*",
+            "pattern": "^_:.+",
             "type": "string"
         },
         "BlankNodeOrIRI": {
             "oneOf": [
                 {
                     "$ref": "#/$defs/IRI"
                 },
@@ -64,38 +70,47 @@
         "DateTime": {
             "type": "string"
         },
         "Extension": {
             "type": "string"
         },
         "IRI": {
-            "pattern": "^(?!_:).*",
+            "pattern": "^(?!_:).+:.+",
             "type": "string"
         },
         "MediaType": {
             "type": "string"
         },
         "SHACLClass": {
             "properties": {
                 "@type": {
-                    "enum": [
-                        "http://example.org/id-prop-class",
-                        "http://example.org/inherited-id-prop-class",
-                        "http://example.org/link-class",
-                        "http://example.org/link-derived-class",
-                        "http://example.org/node-kind-blank",
-                        "http://example.org/node-kind-iri",
-                        "http://example.org/node-kind-iri-or-blank",
-                        "http://example.org/parent-class",
-                        "http://example.org/test-another-class",
-                        "http://example.org/test-class",
-                        "http://example.org/test-class-required",
-                        "http://example.org/test-derived-class",
-                        "http://example.org/aaa-derived-class",
-                        "http://example.org/derived-node-kind-iri"
+                    "oneOf": [
+                        {
+                            "$ref": "#/$defs/IRI"
+                        },
+                        {
+                            "enum": [
+                                "http://example.org/id-prop-class",
+                                "http://example.org/inherited-id-prop-class",
+                                "http://example.org/link-class",
+                                "http://example.org/link-derived-class",
+                                "http://example.org/node-kind-blank",
+                                "http://example.org/node-kind-iri",
+                                "http://example.org/node-kind-iri-or-blank",
+                                "http://example.org/non-shape-class",
+                                "http://example.org/parent-class",
+                                "http://example.org/test-another-class",
+                                "http://example.org/test-class",
+                                "http://example.org/test-class-required",
+                                "http://example.org/test-derived-class",
+                                "http://example.org/aaa-derived-class",
+                                "http://example.org/derived-node-kind-iri",
+                                "http://example.org/extensible-class"
+                            ]
+                        }
                     ]
                 }
             },
             "required": [
                 "@type"
             ],
             "type": "object"
@@ -110,25 +125,29 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "http://example.org/aaa-derived-class"
+                            "oneOf": [
+                                {
+                                    "const": "http://example.org/aaa-derived-class"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgaaaderivedclass_props"
                 }
             ]
         },
         "http_exampleorgaaaderivedclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/http_exampleorgaaaderivedclass"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -148,28 +167,32 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/IRI"
                         },
                         "@type": {
-                            "const": "http://example.org/derived-node-kind-iri"
+                            "oneOf": [
+                                {
+                                    "const": "http://example.org/derived-node-kind-iri"
+                                }
+                            ]
                         }
                     },
                     "required": [
                         "@id"
                     ]
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgderivednodekindiri_props"
                 }
             ]
         },
         "http_exampleorgderivednodekindiri_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/http_exampleorgderivednodekindiri"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -181,33 +204,89 @@
                     "$ref": "#/$defs/http_exampleorgnodekindiri_props"
                 },
                 {
                     "properties": {}
                 }
             ]
         },
+        "http_exampleorgextensibleclass": {
+            "allOf": [
+                {
+                    "properties": {
+                        "@id": {
+                            "$ref": "#/$defs/BlankNodeOrIRI"
+                        },
+                        "@type": {
+                            "oneOf": [
+                                {
+                                    "$ref": "#/$defs/IRI"
+                                },
+                                {
+                                    "const": "http://example.org/extensible-class"
+                                }
+                            ]
+                        }
+                    },
+                    "unevaluatedProperties": true
+                },
+                {
+                    "$ref": "#/$defs/http_exampleorgextensibleclass_props"
+                }
+            ]
+        },
+        "http_exampleorgextensibleclass_derived": {
+            "anyOf": [
+                {
+                    "$ref": "#/$defs/http_exampleorgextensibleclass"
+                },
+                {
+                    "$ref": "#/$defs/BlankNodeOrIRI"
+                }
+            ]
+        },
+        "http_exampleorgextensibleclass_props": {
+            "allOf": [
+                {
+                    "$ref": "#/$defs/http_exampleorglinkclass_props"
+                },
+                {
+                    "properties": {
+                        "http://example.org/extensible-class/required": {
+                            "$ref": "#/$defs/prop_http_exampleorgextensibleclass_required"
+                        }
+                    },
+                    "required": [
+                        "http://example.org/extensible-class/required"
+                    ]
+                }
+            ]
+        },
         "http_exampleorgidpropclass": {
             "allOf": [
                 {
                     "properties": {
                         "@type": {
-                            "const": "http://example.org/id-prop-class"
+                            "oneOf": [
+                                {
+                                    "const": "http://example.org/id-prop-class"
+                                }
+                            ]
                         },
                         "testid": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgidpropclass_props"
                 }
             ]
         },
         "http_exampleorgidpropclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/http_exampleorginheritedidpropclass"
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgidpropclass"
                 },
                 {
@@ -227,28 +306,32 @@
             ]
         },
         "http_exampleorginheritedidpropclass": {
             "allOf": [
                 {
                     "properties": {
                         "@type": {
-                            "const": "http://example.org/inherited-id-prop-class"
+                            "oneOf": [
+                                {
+                                    "const": "http://example.org/inherited-id-prop-class"
+                                }
+                            ]
                         },
                         "testid": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/http_exampleorginheritedidpropclass_props"
                 }
             ]
         },
         "http_exampleorginheritedidpropclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/http_exampleorginheritedidpropclass"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -268,29 +351,36 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "http://example.org/link-class"
+                            "oneOf": [
+                                {
+                                    "const": "http://example.org/link-class"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/http_exampleorglinkclass_props"
                 }
             ]
         },
         "http_exampleorglinkclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/http_exampleorgderivednodekindiri"
                 },
                 {
+                    "$ref": "#/$defs/http_exampleorgextensibleclass"
+                },
+                {
                     "$ref": "#/$defs/http_exampleorglinkderivedclass"
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgnodekindblank"
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgnodekindiri"
@@ -338,25 +428,29 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "http://example.org/link-derived-class"
+                            "oneOf": [
+                                {
+                                    "const": "http://example.org/link-derived-class"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/http_exampleorglinkderivedclass_props"
                 }
             ]
         },
         "http_exampleorglinkderivedclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/http_exampleorglinkderivedclass"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -376,25 +470,29 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNode"
                         },
                         "@type": {
-                            "const": "http://example.org/node-kind-blank"
+                            "oneOf": [
+                                {
+                                    "const": "http://example.org/node-kind-blank"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgnodekindblank_props"
                 }
             ]
         },
         "http_exampleorgnodekindblank_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/http_exampleorgnodekindblank"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -414,28 +512,32 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/IRI"
                         },
                         "@type": {
-                            "const": "http://example.org/node-kind-iri"
+                            "oneOf": [
+                                {
+                                    "const": "http://example.org/node-kind-iri"
+                                }
+                            ]
                         }
                     },
                     "required": [
                         "@id"
                     ]
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgnodekindiri_props"
                 }
             ]
         },
         "http_exampleorgnodekindiri_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/http_exampleorgderivednodekindiri"
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgnodekindiri"
                 },
                 {
@@ -458,25 +560,29 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "http://example.org/node-kind-iri-or-blank"
+                            "oneOf": [
+                                {
+                                    "const": "http://example.org/node-kind-iri-or-blank"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgnodekindiriorblank_props"
                 }
             ]
         },
         "http_exampleorgnodekindiriorblank_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/http_exampleorgnodekindiriorblank"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -488,33 +594,79 @@
                     "$ref": "#/$defs/http_exampleorglinkclass_props"
                 },
                 {
                     "properties": {}
                 }
             ]
         },
+        "http_exampleorgnonshapeclass": {
+            "allOf": [
+                {
+                    "properties": {
+                        "@id": {
+                            "$ref": "#/$defs/BlankNodeOrIRI"
+                        },
+                        "@type": {
+                            "oneOf": [
+                                {
+                                    "const": "http://example.org/non-shape-class"
+                                }
+                            ]
+                        }
+                    }
+                },
+                {
+                    "$ref": "#/$defs/http_exampleorgnonshapeclass_props"
+                }
+            ]
+        },
+        "http_exampleorgnonshapeclass_derived": {
+            "anyOf": [
+                {
+                    "$ref": "#/$defs/http_exampleorgnonshapeclass"
+                },
+                {
+                    "$ref": "#/$defs/BlankNodeOrIRI"
+                }
+            ],
+            "unevaluatedProperties": false
+        },
+        "http_exampleorgnonshapeclass_props": {
+            "allOf": [
+                {
+                    "$ref": "#/$defs/SHACLClass"
+                },
+                {
+                    "properties": {}
+                }
+            ]
+        },
         "http_exampleorgparentclass": {
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "http://example.org/parent-class"
+                            "oneOf": [
+                                {
+                                    "const": "http://example.org/parent-class"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgparentclass_props"
                 }
             ]
         },
         "http_exampleorgparentclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/http_exampleorgaaaderivedclass"
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgtestclass"
                 },
                 {
@@ -546,25 +698,29 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "http://example.org/test-another-class"
+                            "oneOf": [
+                                {
+                                    "const": "http://example.org/test-another-class"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgtestanotherclass_props"
                 }
             ]
         },
         "http_exampleorgtestanotherclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/http_exampleorgtestanotherclass"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -584,25 +740,29 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "http://example.org/test-class"
+                            "oneOf": [
+                                {
+                                    "const": "http://example.org/test-class"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgtestclass_props"
                 }
             ]
         },
         "http_exampleorgtestclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/http_exampleorgtestclassrequired"
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgtestderivedclass"
                 },
                 {
@@ -749,25 +909,29 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "http://example.org/test-class-required"
+                            "oneOf": [
+                                {
+                                    "const": "http://example.org/test-class-required"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgtestclassrequired_props"
                 }
             ]
         },
         "http_exampleorgtestclassrequired_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/http_exampleorgtestclassrequired"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -807,25 +971,29 @@
             "allOf": [
                 {
                     "properties": {
                         "@id": {
                             "$ref": "#/$defs/BlankNodeOrIRI"
                         },
                         "@type": {
-                            "const": "http://example.org/test-derived-class"
+                            "oneOf": [
+                                {
+                                    "const": "http://example.org/test-derived-class"
+                                }
+                            ]
                         }
                     }
                 },
                 {
                     "$ref": "#/$defs/http_exampleorgtestderivedclass_props"
                 }
             ]
         },
         "http_exampleorgtestderivedclass_derived": {
-            "oneOf": [
+            "anyOf": [
                 {
                     "$ref": "#/$defs/http_exampleorgtestderivedclass"
                 },
                 {
                     "$ref": "#/$defs/BlankNodeOrIRI"
                 }
             ],
@@ -833,18 +1001,25 @@
         },
         "http_exampleorgtestderivedclass_props": {
             "allOf": [
                 {
                     "$ref": "#/$defs/http_exampleorgtestclass_props"
                 },
                 {
-                    "properties": {}
+                    "properties": {
+                        "http://example.org/test-derived-class/string-prop": {
+                            "$ref": "#/$defs/prop_http_exampleorgtestderivedclass_stringprop"
+                        }
+                    }
                 }
             ]
         },
+        "prop_http_exampleorgextensibleclass_required": {
+            "type": "string"
+        },
         "prop_http_exampleorglinkclass_linklistprop": {
             "$ref": "#/$defs/http_exampleorglinkclass_derived"
         },
         "prop_http_exampleorglinkclass_linkprop": {
             "$ref": "#/$defs/http_exampleorglinkclass_derived"
         },
         "prop_http_exampleorglinkclass_linkpropnoclass": {
@@ -934,15 +1109,15 @@
             "type": "string"
         },
         "prop_http_exampleorgtestclass_nonnegativeintegerprop": {
             "minimum": 0,
             "type": "integer"
         },
         "prop_http_exampleorgtestclass_nonshape": {
-            "$ref": "#/$defs/anyURI"
+            "$ref": "#/$defs/http_exampleorgnonshapeclass_derived"
         },
         "prop_http_exampleorgtestclass_positiveintegerprop": {
             "minimum": 1,
             "type": "integer"
         },
         "prop_http_exampleorgtestclass_regex": {
             "pattern": "^foo\\d",
@@ -984,14 +1159,17 @@
             "type": "string"
         },
         "prop_http_exampleorgtestclassrequired_requiredstringlistprop": {
             "type": "string"
         },
         "prop_http_exampleorgtestclassrequired_requiredstringscalarprop": {
             "type": "string"
+        },
+        "prop_http_exampleorgtestderivedclass_stringprop": {
+            "type": "string"
         }
     },
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "oneOf": [
         {
             "properties": {
                 "@graph": {
```

### Comparing `shacl2code-0.0.8/tests/expect/python/test-context.py` & `shacl2code-0.0.9/tests/expect/python/test-context.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # SPDX-License-Identifier: MIT
 
 import functools
 import hashlib
 import json
 import re
 import time
+import threading
 from contextlib import contextmanager
 from datetime import datetime, timezone, timedelta
 from enum import Enum
 from abc import ABC, abstractmethod
 
 
 def check_type(obj, types):
@@ -58,26 +59,29 @@
 
     def elide(self, value):
         return value is None
 
     def walk(self, value, callback, path):
         callback(value, path)
 
-    def link_prop(self, value, link_cache, missing, visited):
+    def iter_objects(self, value, recursive, visited):
+        return []
+
+    def link_prop(self, value, doc, missing, visited):
         return value
 
     def to_string(self, value):
         return str(value)
 
     @abstractmethod
     def encode(self, encoder, value, state):
         pass
 
     @abstractmethod
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         pass
 
 
 class StringProp(Property):
     """
     A scalar string property for an SHACL object
     """
@@ -86,23 +90,23 @@
 
     def set(self, value):
         return str(value)
 
     def encode(self, encoder, value, state):
         encoder.write_string(value)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         return decoder.read_string()
 
 
 class AnyURIProp(StringProp):
     def encode(self, encoder, value, state):
         encoder.write_iri(value)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         return decoder.read_iri()
 
 
 class DateTimeProp(Property):
     """
     A Date/Time Object with optional timezone
     """
@@ -113,15 +117,15 @@
 
     def set(self, value):
         return self._normalize(value)
 
     def encode(self, encoder, value, state):
         encoder.write_datetime(self.to_string(value))
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         s = decoder.read_datetime()
         if s is None:
             return None
         v = self.from_string(s)
         return self._normalize(v)
 
     def _normalize(self, value):
@@ -167,15 +171,15 @@
 
     def set(self, value):
         return int(value)
 
     def encode(self, encoder, value, state):
         encoder.write_integer(value)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         return decoder.read_integer()
 
 
 class PositiveIntegerProp(IntegerProp):
     def validate(self, value):
         super().validate(value)
         if value < 1:
@@ -194,28 +198,28 @@
 
     def set(self, value):
         return bool(value)
 
     def encode(self, encoder, value, state):
         encoder.write_bool(value)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         return decoder.read_bool()
 
 
 class FloatProp(Property):
     VALID_TYPES = (float, int)
 
     def set(self, value):
         return float(value)
 
     def encode(self, encoder, value, state):
         encoder.write_float(value)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         return decoder.read_float()
 
 
 class ObjectProp(Property):
     """
     A scalar SHACL object property of a SHACL object
     """
@@ -238,51 +242,64 @@
             return
 
         if not isinstance(value, str):
             value.walk(callback, path)
         else:
             callback(value, path)
 
+    def iter_objects(self, value, recursive, visited):
+        if value is None or isinstance(value, str):
+            return
+
+        if value not in visited:
+            visited.add(value)
+            yield value
+
+            if recursive:
+                for c in value.iter_objects(recursive=True, visited=visited):
+                    yield c
+
     def encode(self, encoder, value, state):
         if value is None:
             raise ValueError("Object cannot be None")
 
         if isinstance(value, str):
             encoder.write_iri(value)
             return
 
         return value.encode(encoder, state)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         iri = decoder.read_iri()
         if iri is not None:
-            if object_ids and iri in object_ids:
-                return object_ids[iri]
+            if doc is not None:
+                return doc.find_by_id(iri, iri)
             return iri
 
-        return SHACLObject.decode(decoder, object_ids=object_ids)
+        return SHACLObject.decode(decoder, doc=doc)
 
-    def link_prop(self, value, link_cache, missing, visited):
+    def link_prop(self, value, doc, missing, visited):
         if value is None:
             return value
 
         if isinstance(value, str):
-            if value in link_cache:
-                return link_cache[value]
+            o = doc.find_by_id(value)
+            if o is not None:
+                return o
 
             if missing is not None:
                 missing.add(value)
 
             return value
 
         # De-duplicate IDs
-        if value._id and value._id is not link_cache[value._id]:
-            value = link_cache[value._id]
+        if value._id:
+            value = doc.find_by_id(value._id, value)
 
-        value.link_helper(link_cache, missing, visited)
+        value.link_helper(doc, missing, visited)
         return value
 
 
 class ListProxy(object):
     def __init__(self, prop, data=None):
         if data is None:
             self.__data = []
@@ -381,34 +398,39 @@
         return len(value) == 0
 
     def walk(self, value, callback, path):
         callback(value, path)
         for idx, v in enumerate(value):
             self.prop.walk(v, callback, path + [f"[{idx}]"])
 
-    def link_prop(self, value, link_cache, missing, visited):
+    def iter_objects(self, value, recursive, visited):
+        for v in value:
+            for c in self.prop.iter_objects(v, recursive, visited):
+                yield c
+
+    def link_prop(self, value, doc, missing, visited):
         if isinstance(value, ListProxy):
-            data = [self.prop.link_prop(v, link_cache, missing, visited) for v in value]
+            data = [self.prop.link_prop(v, doc, missing, visited) for v in value]
         else:
-            data = [self.prop.link_prop(v, link_cache, missing, visited) for v in value]
+            data = [self.prop.link_prop(v, doc, missing, visited) for v in value]
 
         return ListProxy(self.prop, data=data)
 
     def encode(self, encoder, value, state):
         check_type(value, ListProxy)
 
         with encoder.write_list() as list_s:
             for v in value:
                 with list_s.write_list_item() as item_s:
                     self.prop.encode(item_s, v, state)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         data = []
         for val_d in decoder.read_list():
-            v = self.prop.decode(val_d, object_ids=object_ids)
+            v = self.prop.decode(val_d, doc=doc)
             self.prop.validate(v)
             data.append(v)
 
         return ListProxy(self.prop, data=data)
 
 
 class EnumProp(Property):
@@ -430,130 +452,166 @@
         for iri, compact in self.context:
             if iri == value:
                 encoder.write_enum(value, self, compact)
                 return
 
         encoder.write_enum(value, self)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         v = decoder.read_enum(self)
         for iri, compact in self.context:
             if v == compact:
                 return iri
         return v
 
 
 class NodeKind(Enum):
     BlankNode = 1
     IRI = 2
     BlankNodeOrIRI = 3
 
 
+def register(type_iri, compact_type=None):
+    def add_deserializer(key, c):
+        assert (
+            key not in SHACLObject.DESERIALIZERS
+        ), f"{key} already registered to {SHACLObject.DESERIALIZERS[key].__name__}"
+        SHACLObject.DESERIALIZERS[key] = c
+
+    def decorator(c):
+        assert issubclass(
+            c, SHACLObject
+        ), f"{c.__name__} is not derived from SHACLObject"
+
+        c.TYPE = type_iri
+        add_deserializer(type_iri, c)
+
+        c.COMPACT_TYPE = compact_type
+        if compact_type:
+            add_deserializer(compact_type, c)
+
+        # Registration is deferred until the first instance of class is created
+        # so that it has access to any other defined class
+        c._NEEDS_REG = True
+        return c
+
+    return decorator
+
+
+register_lock = threading.Lock()
+
+
 @functools.total_ordering
 class SHACLObject(object):
     DESERIALIZERS = {}
     NODE_KIND = NodeKind.BlankNodeOrIRI
     ID_ALIAS = None
     COMPACT_TYPE = None
 
-    def __init__(self):
+    def __init__(self, **kwargs):
+        with register_lock:
+            cls = self.__class__
+            if cls._NEEDS_REG:
+                cls._OBJ_PROPERTIES = {}
+                cls._OBJ_IRIS = {}
+                cls._register_props()
+                cls._NEEDS_REG = False
+
         self._obj_data = {}
-        self._obj_properties = {}
-        self._obj_iris = {}
         self._obj_metadata = {}
 
-        self._add_property("_id", StringProp(), iri="@id")
+        for iri, prop, _, _, _, _ in self.__iter_props():
+            self._obj_data[iri] = prop.init()
 
-    def _set_init_props(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
 
+    @classmethod
+    def _register_props(cls):
+        cls._add_property("_id", StringProp(), iri="@id")
+
+    @classmethod
     def _add_property(
-        self,
+        cls,
         pyname,
         prop,
         iri,
         min_count=None,
         max_count=None,
         compact=None,
     ):
-        if pyname in self._obj_iris:
-            raise KeyError(
-                f"'{pyname}' is already defined for '{self.__class__.__name__}'"
-            )
-        if iri in self._obj_properties:
-            raise KeyError(
-                f"'{iri}' is already defined for '{self.__class__.__name__}'"
-            )
+        if pyname in cls._OBJ_IRIS:
+            raise KeyError(f"'{pyname}' is already defined for '{cls.__name__}'")
+        if iri in cls._OBJ_PROPERTIES:
+            raise KeyError(f"'{iri}' is already defined for '{cls.__name__}'")
 
-        while hasattr(self, pyname):
+        while hasattr(cls, pyname):
             pyname = pyname + "_"
 
-        self._obj_iris[pyname] = iri
-        self._obj_properties[iri] = (prop, min_count, max_count, pyname, compact)
-        self._obj_data[iri] = prop.init()
+        cls._OBJ_IRIS[pyname] = iri
+        cls._OBJ_PROPERTIES[iri] = (prop, min_count, max_count, pyname, compact)
 
     def __setattr__(self, name, value):
         if name.startswith("_obj_"):
             return super().__setattr__(name, value)
 
         if name == self.ID_ALIAS:
             name = "_id"
 
         try:
-            iri = self._obj_iris[name]
+            iri = self._OBJ_IRIS[name]
             self[iri] = value
         except KeyError:
             raise AttributeError(
                 f"'{name}' is not a valid property of {self.__class__.__name__}"
             )
 
     def __getattr__(self, name):
         if name.startswith("_obj_"):
             return self.__dict__[name]
 
         if name == "_metadata":
             return self._obj_metadata
 
         if name == "_IRI":
-            return self._obj_iris
+            return self._OBJ_IRIS
 
         if name == self.ID_ALIAS:
             name = "_id"
 
         try:
-            iri = self._obj_iris[name]
+            iri = self._OBJ_IRIS[name]
             return self[iri]
         except KeyError:
             raise AttributeError(
                 f"'{name}' is not a valid property of {self.__class__.__name__}"
             )
 
     def __delattr__(self, name):
         if name == self.ID_ALIAS:
             name = "_id"
 
         try:
-            iri = self._obj_iris[name]
+            iri = self._OBJ_IRIS[name]
             del self[iri]
         except KeyError:
             raise AttributeError(
                 f"'{name}' is not a valid property of {self.__class__.__name__}"
             )
 
     def __get_prop(self, iri):
-        if iri not in self._obj_properties:
+        if iri not in self._OBJ_PROPERTIES:
             raise KeyError(
                 f"'{iri}' is not a valid property of {self.__class__.__name__}"
             )
 
-        return self._obj_properties[iri]
+        return self._OBJ_PROPERTIES[iri]
 
     def __iter_props(self):
-        for iri, v in self._obj_properties.items():
+        for iri, v in self._OBJ_PROPERTIES.items():
             yield iri, *v
 
     def __getitem__(self, iri):
         return self._obj_data[iri]
 
     def __setitem__(self, iri, value):
         if iri == "@id":
@@ -573,15 +631,15 @@
         self._obj_data[iri] = prop.set(value)
 
     def __delitem__(self, iri):
         prop, _, _, _, _ = self.__get_prop(iri)
         self._obj_data[iri] = prop.init()
 
     def __iter__(self):
-        return self._obj_properties.keys()
+        return self._OBJ_PROPERTIES.keys()
 
     def walk(self, callback, path=None):
         """
         Walk object tree, invoking the callback for each item
 
         Callback has the form:
 
@@ -590,39 +648,35 @@
         if path is None:
             path = ["."]
 
         if callback(self, path):
             for iri, prop, _, _, _, _ in self.__iter_props():
                 prop.walk(self._obj_data[iri], callback, path + [f".{iri}"])
 
-    def child_objects(self):
+    def property_keys(self):
+        for iri, _, _, _, pyname, compact in self.__iter_props():
+            if iri == "@id":
+                compact = self.ID_ALIAS
+            yield pyname, iri, compact
+
+    def iter_objects(self, *, recursive=False, visited=None):
         """
-        Iterate over each object that is a child of this one
+        Iterate of all objects that are a child of this one
         """
-        seen = set()
+        if visited is None:
+            visited = set()
 
-        def _walk_callback(value, path):
-            nonlocal seen
-
-            if not isinstance(value, SHACLObject):
-                return False
-
-            if value in seen:
-                return False
-
-            seen.add(value)
-            return True
-
-        self.walk(_walk_callback)
-
-        for obj in seen:
-            yield obj
+        for iri, prop, _, _, _, _ in self.__iter_props():
+            for c in prop.iter_objects(
+                self._obj_data[iri], recursive=recursive, visited=visited
+            ):
+                yield c
 
     def encode(self, encoder, state):
-        idname = self.ID_ALIAS or self._obj_iris["_id"]
+        idname = self.ID_ALIAS or self._OBJ_IRIS["_id"]
         if not self._id and self.NODE_KIND == NodeKind.IRI:
             raise ValueError(
                 f"{self.__class__.__name__} ({id(self)}) must have a IRI for property '{idname}'"
             )
 
         if state.is_written(self):
             encoder.write_iri(state.get_object_id(self))
@@ -652,77 +706,69 @@
 
                 if max_count is not None:
                     if not prop.check_max_count(value, max_count):
                         raise ValueError(
                             f"Property '{pyname}' in {self.__class__.__name__} ({id(self)}) requires a maximum of {max_count} elements"
                         )
 
-                if iri == self._obj_iris["_id"]:
+                if iri == self._OBJ_IRIS["_id"]:
                     continue
 
                 with obj_s.write_property(iri, compact) as prop_s:
                     prop.encode(prop_s, value, state)
 
     @classmethod
-    def decode(cls, decoder, *, object_ids=None):
+    def decode(cls, decoder, *, doc=None):
         typ, obj_d = decoder.read_object()
         if typ is None:
             raise TypeError("Unable to determine type for object")
 
         if typ not in cls.DESERIALIZERS:
             raise TypeError(f"Unknown type {typ}")
 
         obj = cls.DESERIALIZERS[typ]()
         _id = obj_d.read_object_id(obj.ID_ALIAS)
         if _id is not None:
-            if object_ids is not None:
-                if _id in object_ids:
-                    return object_ids[_id]
-                object_ids[_id] = obj
             obj._id = _id
+            if doc is not None:
+                v = doc.find_by_id(_id)
+                if v is not None:
+                    return v
+
+        if doc is not None:
+            doc.add_index(obj)
 
         for iri, prop, _, _, _, compact in obj.__iter_props():
-            if iri == obj._obj_iris["_id"]:
+            if iri == obj._OBJ_IRIS["_id"]:
                 continue
 
             with obj_d.read_property(iri, compact) as prop_d:
                 if prop_d is None:
                     continue
 
-                v = prop.decode(prop_d, object_ids=object_ids)
+                v = prop.decode(prop_d, doc=doc)
                 prop.validate(v)
                 obj._obj_data[iri] = v
 
         return obj
 
-    def link_helper(self, link_cache, missing, visited):
+    def link_helper(self, doc, missing, visited):
         if self in visited:
             return
 
         visited.add(self)
 
         for iri, prop, _, _, _, _ in self.__iter_props():
             self._obj_data[iri] = prop.link_prop(
                 self._obj_data[iri],
-                link_cache,
+                doc,
                 missing,
                 visited,
             )
 
-    def link(self, link_cache=None):
-        if not link_cache:
-            link_cache = {obj._id: obj for obj in self.child_objects() if obj._id}
-
-        missing = set()
-        visited = set()
-
-        self.link_helper(link_cache, missing, visited)
-
-        return missing
-
     def __str__(self):
         parts = [
             f"{self.__class__.__name__}(",
         ]
         if self._id:
             parts.append(f"@id='{self._id}'")
         parts.append(")")
@@ -744,135 +790,213 @@
                 getattr(obj, "name", None) or "",
                 id(obj),
             )
 
         return sort_key(self) < sort_key(other)
 
 
-class EncodeState(object):
-    def __init__(self):
-        self.ref_objects = set()
-        self.written_objects = set()
-        self.blank_objects = {}
+class SHACLDocument(object):
+    def __init__(self, objects=[], *, link=False):
+        self.objects = set()
+        for o in objects:
+            self.objects.add(o)
+        self.create_index()
+        if link:
+            self._link()
+
+    def create_index(self):
+        self.obj_by_id = {}
+        self.obj_by_type = {}
+        for o in self.foreach():
+            self.add_index(o)
+
+    def add_index(self, obj):
+        for typ in SHACLObject.DESERIALIZERS.values():
+            if isinstance(obj, typ):
+                self.obj_by_type.setdefault(typ, set()).add(obj)
 
-    def get_object_id(self, o):
-        if o._id:
-            return o._id
+        if not obj._id:
+            return
 
-        if o not in self.blank_objects:
-            _id = f"_:{o.__class__.__name__}{len(self.blank_objects)}"
-            self.blank_objects[o] = _id
+        if obj._id in self.obj_by_id:
+            return
 
-        return self.blank_objects[o]
+        self.obj_by_id[obj._id] = obj
 
-    def is_refed(self, o):
-        return o in self.ref_objects
+    def link(self):
+        self.create_index()
+        return self._link()
 
-    def add_refed(self, o):
-        self.ref_objects.add(o)
+    def _link(self):
+        missing = set()
+        visited = set()
 
-    def is_written(self, o):
-        return o in self.written_objects
+        new_objects = set()
 
-    def add_written(self, o):
-        self.written_objects.add(o)
+        for o in self.objects:
+            if o._id:
+                o = self.find_by_id(o._id, o)
+            o.link_helper(self, missing, visited)
+            new_objects.add(o)
+
+        self.objects = new_objects
+
+        # Remove blank nodes
+        obj_by_id = {}
+        for _id, obj in self.obj_by_id.items():
+            if _id.startswith("_:"):
+                del obj._id
+            else:
+                obj_by_id[obj._id] = obj
+        self.obj_by_id = obj_by_id
 
+        return missing
 
-def encode_objects(encoder, objects, force_list=False):
-    """
-    Serialize a list of objects to a serialization encoder
+    def find_by_id(self, _id, default=None):
+        if _id not in self.obj_by_id:
+            return default
+        return self.obj_by_id[_id]
 
-    If force_list is true, a list will always be written using the encoder.
-    """
-    ref_counts = {}
-    state = EncodeState()
+    def foreach(self):
+        visited = set()
+        for o in self.objects:
+            if o not in visited:
+                yield o
+                visited.add(o)
+
+            for child in o.iter_objects(recursive=True, visited=visited):
+                yield child
+
+    def foreach_type(self, typ, *, subclass=False):
+        if isinstance(typ, str):
+            typ = SHACLObject.DESERIALIZERS[typ]
 
-    def walk_callback(value, path):
-        nonlocal state
-        nonlocal ref_counts
+        if typ not in self.obj_by_type:
+            return
 
-        if not isinstance(value, SHACLObject):
-            return True
+        for o in self.obj_by_type[typ]:
+            if subclass or o.__class__ is typ:
+                yield o
 
-        # Remove blank node ID for re-assignment
-        if value._id and value._id.startswith("_:"):
-            del value._id
+    def merge(self, *doc):
+        new_objects = set()
+        new_objects |= self.objects
+        for d in doc:
+            new_objects |= d.objects
 
-        if value._id:
-            state.add_refed(value)
+        return SHACLDocument(new_objects, link=True)
 
-        # If the object is referenced more than once, add it to the set of
-        # referenced objects
-        ref_counts.setdefault(value, 0)
-        ref_counts[value] += 1
-        if ref_counts[value] > 1:
-            state.add_refed(value)
-            return False
+    def encode(self, encoder, force_list=False):
+        """
+        Serialize a list of objects to a serialization encoder
 
-        return True
+        If force_list is true, a list will always be written using the encoder.
+        """
+        ref_counts = {}
+        state = EncodeState()
 
-    for o in objects:
-        if o._id:
-            state.add_refed(o)
-        o.walk(walk_callback)
+        def walk_callback(value, path):
+            nonlocal state
+            nonlocal ref_counts
 
-    use_list = force_list or len(objects) > 1
+            if not isinstance(value, SHACLObject):
+                return True
 
-    objects = set(objects)
+            # Remove blank node ID for re-assignment
+            if value._id and value._id.startswith("_:"):
+                del value._id
+
+            if value._id:
+                state.add_refed(value)
+
+            # If the object is referenced more than once, add it to the set of
+            # referenced objects
+            ref_counts.setdefault(value, 0)
+            ref_counts[value] += 1
+            if ref_counts[value] > 1:
+                state.add_refed(value)
+                return False
 
-    if use_list:
-        # If we are making a list add all the objects referred to by reference
-        # to the list
-        objects |= state.ref_objects
-
-    objects = list(objects)
-    objects.sort()
-
-    if use_list:
-        # Ensure top level objects are only written in the top level graph
-        # node, and referenced by ID everywhere else. This is done by setting
-        # the flag that indicates this object has been written for all the top
-        # level objects, then clearing it right before serializing the object.
-        #
-        # In this way, if an object is referenced before it is supposed to be
-        # serialized into the @graph, it will serialize as a string instead of
-        # the actual object
-        for o in objects:
-            state.written_objects.add(o)
+            return True
 
-        with encoder.write_list() as list_s:
+        for o in self.objects:
+            if o._id:
+                state.add_refed(o)
+            o.walk(walk_callback)
+
+        use_list = force_list or len(self.objects) > 1
+
+        if use_list:
+            # If we are making a list add all the objects referred to by reference
+            # to the list
+            objects = list(self.objects | state.ref_objects)
+        else:
+            objects = list(self.objects)
+
+        objects.sort()
+
+        if use_list:
+            # Ensure top level objects are only written in the top level graph
+            # node, and referenced by ID everywhere else. This is done by setting
+            # the flag that indicates this object has been written for all the top
+            # level objects, then clearing it right before serializing the object.
+            #
+            # In this way, if an object is referenced before it is supposed to be
+            # serialized into the @graph, it will serialize as a string instead of
+            # the actual object
             for o in objects:
-                # Allow this specific object to be written now
-                state.written_objects.remove(o)
-                with list_s.write_list_item() as item_s:
-                    o.encode(item_s, state)
+                state.written_objects.add(o)
 
-    else:
-        objects[0].encode(encoder, state)
+            with encoder.write_list() as list_s:
+                for o in objects:
+                    # Allow this specific object to be written now
+                    state.written_objects.remove(o)
+                    with list_s.write_list_item() as item_s:
+                        o.encode(item_s, state)
 
+        else:
+            objects[0].encode(encoder, state)
 
-def decode_objects(decoder):
-    object_ids = {}
-    objects = [
-        SHACLObject.decode(obj_d, object_ids=object_ids)
-        for obj_d in decoder.read_list()
-    ]
+    def decode(self, decoder):
+        self.create_index()
 
-    for o in objects:
-        o.link(object_ids)
+        for obj_d in decoder.read_list():
+            o = SHACLObject.decode(obj_d, doc=self)
+            self.objects.add(o)
 
-    # Remove blank node IDs
-    for o in objects:
-        for c in o.child_objects():
-            if c._id and c._id.startswith("_:"):
-                del c._id
+        self._link()
+
+
+class EncodeState(object):
+    def __init__(self):
+        self.ref_objects = set()
+        self.written_objects = set()
+        self.blank_objects = {}
+
+    def get_object_id(self, o):
+        if o._id:
+            return o._id
+
+        if o not in self.blank_objects:
+            _id = f"_:{o.__class__.__name__}{len(self.blank_objects)}"
+            self.blank_objects[o] = _id
+
+        return self.blank_objects[o]
+
+    def is_refed(self, o):
+        return o in self.ref_objects
 
-    object_ids = {k: v for k, v in object_ids.items() if not k.startswith("_:")}
+    def add_refed(self, o):
+        self.ref_objects.add(o)
 
-    return objects, object_ids
+    def is_written(self, o):
+        return o in self.written_objects
+
+    def add_written(self, o):
+        self.written_objects.add(o)
 
 
 class Decoder(ABC):
     @abstractmethod
     def read_string(self):
         """
         Consume the next item as a string.
@@ -1076,22 +1200,22 @@
         return None, self
 
     def read_object_id(self, alias=None):
         return self.__get_value(alias, "@id")
 
 
 class JSONLDDeserializer(object):
-    def read(self, f):
+    def read(self, f, doc):
         data = json.load(f)
         if "@graph" in data:
             h = JSONLDDecoder(data["@graph"])
         else:
             h = JSONLDDecoder(data)
 
-        return decode_objects(h)
+        doc.decode(h)
 
 
 class Encoder(ABC):
     @abstractmethod
     def write_string(self, v):
         """
         Write a string value
@@ -1276,41 +1400,46 @@
         s = self.__class__(None)
         yield s
         if s.data is not None:
             self.data.append(s.data)
 
 
 class JSONLDSerializer(object):
-    def serialize_data(self, objects, force_graph=False):
-        h = JSONLDEncoder()
-        encode_objects(h, objects, force_graph)
-        if isinstance(h.data, list):
-            data = {
-                "@graph": h.data,
-            }
-        else:
-            data = h.data
+    def __init__(self, **args):
+        self.args = args
 
+    def serialize_data(self, doc, force_graph=False):
+        h = JSONLDEncoder()
+        doc.encode(h, force_graph)
+        data = {}
         if len(CONTEXT_URLS) == 1:
             data["@context"] = CONTEXT_URLS[0]
         elif CONTEXT_URLS:
             data["@context"] = CONTEXT_URLS
 
+        if isinstance(h.data, list):
+            data["@graph"] = h.data
+        else:
+            for k, v in h.data.items():
+                data[k] = v
+
         return data
 
-    def write(self, objects, f, force_graph=False, **kwargs):
+    def write(self, doc, f, force_graph=False, **kwargs):
         """
-        Write a list of objects to a JSON LD file
+        Write a SHACLDocument to a JSON LD file
 
         If force_graph is True, a @graph node will always be written
         """
-        data = self.serialize_data(objects, force_graph)
+        data = self.serialize_data(doc, force_graph)
+
+        args = {**self.args, **kwargs}
 
         sha1 = hashlib.sha1()
-        for chunk in json.JSONEncoder(**kwargs).iterencode(data):
+        for chunk in json.JSONEncoder(**args).iterencode(data):
             chunk = chunk.encode("utf-8")
             f.write(chunk)
             sha1.update(chunk)
 
         return sha1.hexdigest()
 
 
@@ -1326,19 +1455,16 @@
         self.sha1.update(s)
 
     def _write_comma(self):
         if self.comma:
             self.write(",")
             self.comma = False
 
-    def _need_comma(self):
-        self.comma = True
-
     def write_string(self, v):
-        self.write(f'"{v}"')
+        self.write(json.dumps(v))
 
     def write_datetime(self, v):
         self.write_string(v)
 
     def write_integer(self, v):
         self.write(f"{v}")
 
@@ -1351,36 +1477,40 @@
     def write_bool(self, v):
         if v:
             self.write("true")
         else:
             self.write("false")
 
     def write_float(self, v):
-        self.write(f'"{v}"')
+        self.write(json.dumps(str(v)))
 
     @contextmanager
     def write_property(self, iri, compact=None):
         self._write_comma()
-        self.write(f'"{compact or iri}":')
+        self.write_string(compact or iri)
+        self.write(":")
         yield self
         self.comma = True
 
     @contextmanager
     def write_object(self, o, _id, needs_id):
         self._write_comma()
 
         self.write("{")
+        self.write_string("@type")
+        self.write(":")
+        self.write_string(o.COMPACT_TYPE or o.TYPE)
+        self.comma = True
+
         if needs_id:
-            idname = o.ID_ALIAS or "@id"
-            idval = _id
-            self.write(f'"{idname}": "{idval}",')
-
-        typname = "@type"
-        typval = o.COMPACT_TYPE or o.TYPE
-        self.write(f'"{typname}":"{typval}"')
+            self._write_comma()
+            self.write_string(o.ID_ALIAS or "@id")
+            self.write(":")
+            self.write_string(_id)
+            self.comma = True
 
         self.comma = True
         yield self
 
         self.write("}")
         self.comma = True
 
@@ -1396,32 +1526,35 @@
     def write_list_item(self):
         self._write_comma()
         yield self.__class__(self.f, self.sha1)
         self.comma = True
 
 
 class JSONLDInlineSerializer(object):
-    def write(self, objects, f):
+    def write(self, doc, f, force_graph=False):
         """
-        Write a list of objects to a JSON LD file
+        Write a SHACLDocument to a JSON LD file
+
+        Note: force_graph is included for compatibility, but ignored. This
+        serializer always writes out a graph
         """
         sha1 = hashlib.sha1()
         h = JSONLDInlineEncoder(f, sha1)
         h.write('{"@context":')
         if len(CONTEXT_URLS) == 1:
             h.write(f'"{CONTEXT_URLS[0]}"')
         elif CONTEXT_URLS:
             h.write('["')
             h.write('","'.join(CONTEXT_URLS))
             h.write('"]')
         h.write(",")
 
         h.write('"@graph":')
 
-        encode_objects(h, objects, True)
+        doc.encode(h, True)
         h.write("}")
         return sha1.hexdigest()
 
 
 def print_tree(objects, all_fields=False):
     """
     Print object tree
@@ -1482,454 +1615,419 @@
     foo = "http://example.org/enumType/foo"
     # This value has no label
     nolabel = "http://example.org/enumType/nolabel"
 
 
 # CLASSES
 # A class with an ID alias
+@register("http://example.org/id-prop-class", "id-prop-class")
 class id_prop_class(SHACLObject):
-    TYPE = "http://example.org/id-prop-class"
-    COMPACT_TYPE = "id-prop-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
     ID_ALIAS = "testid"
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/id-prop-class"] = id_prop_class
-SHACLObject.DESERIALIZERS["id-prop-class"] = id_prop_class
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # A class that inherits its idPropertyName from the parent
+@register("http://example.org/inherited-id-prop-class", "inherited-id-prop-class")
 class inherited_id_prop_class(id_prop_class):
-    TYPE = "http://example.org/inherited-id-prop-class"
-    COMPACT_TYPE = "inherited-id-prop-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
     ID_ALIAS = "testid"
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/inherited-id-prop-class"] = inherited_id_prop_class
-SHACLObject.DESERIALIZERS["inherited-id-prop-class"] = inherited_id_prop_class
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # A class to test links
+@register("http://example.org/link-class", "link-class")
 class link_class(SHACLObject):
-    TYPE = "http://example.org/link-class"
-    COMPACT_TYPE = "link-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
         # A link-class list property
-        self._add_property(
+        cls._add_property(
             "link_class_link_list_prop",
             ListProp(ObjectProp(link_class, False)),
             iri="http://example.org/link-class-link-list-prop",
             compact="link-class-link-list-prop",
         )
         # A link-class property
-        self._add_property(
+        cls._add_property(
             "link_class_link_prop",
             ObjectProp(link_class, False),
             iri="http://example.org/link-class-link-prop",
             compact="link-class-link-prop",
         )
         # A link-class property with no sh:class
-        self._add_property(
+        cls._add_property(
             "link_class_link_prop_no_class",
             ObjectProp(link_class, False),
             iri="http://example.org/link-class-link-prop-no-class",
             compact="link-class-link-prop-no-class",
         )
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/link-class"] = link_class
-SHACLObject.DESERIALIZERS["link-class"] = link_class
 
 
 # A class derived from link-class
+@register("http://example.org/link-derived-class", "link-derived-class")
 class link_derived_class(link_class):
-    TYPE = "http://example.org/link-derived-class"
-    COMPACT_TYPE = "link-derived-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/link-derived-class"] = link_derived_class
-SHACLObject.DESERIALIZERS["link-derived-class"] = link_derived_class
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # A class that must be a blank node
+@register("http://example.org/node-kind-blank", "node-kind-blank")
 class node_kind_blank(link_class):
-    TYPE = "http://example.org/node-kind-blank"
-    COMPACT_TYPE = "node-kind-blank"
     NODE_KIND = NodeKind.BlankNode
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/node-kind-blank"] = node_kind_blank
-SHACLObject.DESERIALIZERS["node-kind-blank"] = node_kind_blank
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # A class that must be an IRI
+@register("http://example.org/node-kind-iri", "node-kind-iri")
 class node_kind_iri(link_class):
-    TYPE = "http://example.org/node-kind-iri"
-    COMPACT_TYPE = "node-kind-iri"
     NODE_KIND = NodeKind.IRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/node-kind-iri"] = node_kind_iri
-SHACLObject.DESERIALIZERS["node-kind-iri"] = node_kind_iri
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # A class that can be either a blank node or an IRI
+@register("http://example.org/node-kind-iri-or-blank", "node-kind-iri-or-blank")
 class node_kind_iri_or_blank(link_class):
-    TYPE = "http://example.org/node-kind-iri-or-blank"
-    COMPACT_TYPE = "node-kind-iri-or-blank"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
+
 
+# A class that is not a nodeshape
+@register("http://example.org/non-shape-class", "non-shape-class")
+class non_shape_class(SHACLObject):
+    NODE_KIND = NodeKind.BlankNodeOrIRI
 
-SHACLObject.DESERIALIZERS["http://example.org/node-kind-iri-or-blank"] = node_kind_iri_or_blank
-SHACLObject.DESERIALIZERS["node-kind-iri-or-blank"] = node_kind_iri_or_blank
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # The parent class
+@register("http://example.org/parent-class", "parent-class")
 class parent_class(SHACLObject):
-    TYPE = "http://example.org/parent-class"
-    COMPACT_TYPE = "parent-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/parent-class"] = parent_class
-SHACLObject.DESERIALIZERS["parent-class"] = parent_class
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # Another class
+@register("http://example.org/test-another-class", "test-another-class")
 class test_another_class(SHACLObject):
-    TYPE = "http://example.org/test-another-class"
-    COMPACT_TYPE = "test-another-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/test-another-class"] = test_another_class
-SHACLObject.DESERIALIZERS["test-another-class"] = test_another_class
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # The test class
+@register("http://example.org/test-class", "test-class")
 class test_class(parent_class):
-    TYPE = "http://example.org/test-class"
-    COMPACT_TYPE = "test-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
         # A property that conflicts with an existing SHACLObject property
-        self._add_property(
+        cls._add_property(
             "encode",
             StringProp(),
             iri="http://example.org/encode",
             compact="encode",
         )
         # A property that is a keyword
-        self._add_property(
+        cls._add_property(
             "import_",
             StringProp(),
             iri="http://example.org/import",
             compact="import",
         )
         # a URI
-        self._add_property(
+        cls._add_property(
             "test_class_anyuri_prop",
             AnyURIProp(),
             iri="http://example.org/test-class/anyuri-prop",
             compact="test-class/anyuri-prop",
         )
         # a boolean property
-        self._add_property(
+        cls._add_property(
             "test_class_boolean_prop",
             BooleanProp(),
             iri="http://example.org/test-class/boolean-prop",
             compact="test-class/boolean-prop",
         )
         # A test-class list property
-        self._add_property(
+        cls._add_property(
             "test_class_class_list_prop",
             ListProp(ObjectProp(test_class, False)),
             iri="http://example.org/test-class/class-list-prop",
             compact="test-class/class-list-prop",
         )
         # A test-class property
-        self._add_property(
+        cls._add_property(
             "test_class_class_prop",
             ObjectProp(test_class, False),
             iri="http://example.org/test-class/class-prop",
             compact="test-class/class-prop",
         )
         # A test-class property with no sh:class
-        self._add_property(
+        cls._add_property(
             "test_class_class_prop_no_class",
             ObjectProp(test_class, False),
             iri="http://example.org/test-class/class-prop-no-class",
             compact="test-class/class-prop-no-class",
         )
         # A datetime list property
-        self._add_property(
+        cls._add_property(
             "test_class_datetime_list_prop",
             ListProp(DateTimeProp()),
             iri="http://example.org/test-class/datetime-list-prop",
             compact="test-class/datetime-list-prop",
         )
         # A scalar datetime property
-        self._add_property(
+        cls._add_property(
             "test_class_datetime_scalar_prop",
             DateTimeProp(),
             iri="http://example.org/test-class/datetime-scalar-prop",
             compact="test-class/datetime-scalar-prop",
         )
         # A scalar dateTimeStamp property
-        self._add_property(
+        cls._add_property(
             "test_class_datetimestamp_scalar_prop",
             DateTimeStampProp(),
             iri="http://example.org/test-class/datetimestamp-scalar-prop",
             compact="test-class/datetimestamp-scalar-prop",
         )
         # A enum list property
-        self._add_property(
+        cls._add_property(
             "test_class_enum_list_prop",
             ListProp(enumType(context=[
                 ("http://example.org/enumType/bar", "enumType/bar"),
                 ("http://example.org/enumType/foo", "enumType/foo"),
                 ("http://example.org/enumType/nolabel", "enumType/nolabel"),
             ])),
             iri="http://example.org/test-class/enum-list-prop",
             compact="test-class/enum-list-prop",
         )
         # A enum property
-        self._add_property(
+        cls._add_property(
             "test_class_enum_prop",
             enumType(context=[
                 ("http://example.org/enumType/bar", "enumType/bar"),
                 ("http://example.org/enumType/foo", "enumType/foo"),
                 ("http://example.org/enumType/nolabel", "enumType/nolabel"),
             ]),
             iri="http://example.org/test-class/enum-prop",
             compact="test-class/enum-prop",
         )
         # A enum property with no sh:class
-        self._add_property(
+        cls._add_property(
             "test_class_enum_prop_no_class",
             enumType(context=[
                 ("http://example.org/enumType/bar", "enumType/bar"),
                 ("http://example.org/enumType/foo", "enumType/foo"),
                 ("http://example.org/enumType/nolabel", "enumType/nolabel"),
             ]),
             iri="http://example.org/test-class/enum-prop-no-class",
             compact="test-class/enum-prop-no-class",
         )
         # a float property
-        self._add_property(
+        cls._add_property(
             "test_class_float_prop",
             FloatProp(),
             iri="http://example.org/test-class/float-prop",
             compact="test-class/float-prop",
         )
         # a non-negative integer
-        self._add_property(
+        cls._add_property(
             "test_class_integer_prop",
             IntegerProp(),
             iri="http://example.org/test-class/integer-prop",
             compact="test-class/integer-prop",
         )
         # A named property
-        self._add_property(
+        cls._add_property(
             "named_property",
             StringProp(),
             iri="http://example.org/test-class/named-property",
             compact="test-class/named-property",
         )
         # A class with no shape
-        self._add_property(
+        cls._add_property(
             "test_class_non_shape",
-            AnyURIProp(),
+            ObjectProp(non_shape_class, False),
             iri="http://example.org/test-class/non-shape",
             compact="test-class/non-shape",
         )
         # a non-negative integer
-        self._add_property(
+        cls._add_property(
             "test_class_nonnegative_integer_prop",
             NonNegativeIntegerProp(),
             iri="http://example.org/test-class/nonnegative-integer-prop",
             compact="test-class/nonnegative-integer-prop",
         )
         # A positive integer
-        self._add_property(
+        cls._add_property(
             "test_class_positive_integer_prop",
             PositiveIntegerProp(),
             iri="http://example.org/test-class/positive-integer-prop",
             compact="test-class/positive-integer-prop",
         )
         # A regex validated string
-        self._add_property(
+        cls._add_property(
             "test_class_regex",
             StringProp(pattern=r"^foo\d",),
             iri="http://example.org/test-class/regex",
             compact="test-class/regex",
         )
         # A regex dateTime
-        self._add_property(
+        cls._add_property(
             "test_class_regex_datetime",
             DateTimeProp(pattern=r"^\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d\+01:00$",),
             iri="http://example.org/test-class/regex-datetime",
             compact="test-class/regex-datetime",
         )
         # A regex dateTimeStamp
-        self._add_property(
+        cls._add_property(
             "test_class_regex_datetimestamp",
             DateTimeStampProp(pattern=r"^\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\dZ$",),
             iri="http://example.org/test-class/regex-datetimestamp",
             compact="test-class/regex-datetimestamp",
         )
         # A regex validated string list
-        self._add_property(
+        cls._add_property(
             "test_class_regex_list",
             ListProp(StringProp(pattern=r"^foo\d",)),
             iri="http://example.org/test-class/regex-list",
             compact="test-class/regex-list",
         )
         # A string list property with no sh:datatype
-        self._add_property(
+        cls._add_property(
             "test_class_string_list_no_datatype",
             ListProp(StringProp()),
             iri="http://example.org/test-class/string-list-no-datatype",
             compact="test-class/string-list-no-datatype",
         )
         # A string list property
-        self._add_property(
+        cls._add_property(
             "test_class_string_list_prop",
             ListProp(StringProp()),
             iri="http://example.org/test-class/string-list-prop",
             compact="test-class/string-list-prop",
         )
         # A scalar string propery
-        self._add_property(
+        cls._add_property(
             "test_class_string_scalar_prop",
             StringProp(),
             iri="http://example.org/test-class/string-scalar-prop",
             compact="test-class/string-scalar-prop",
         )
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/test-class"] = test_class
-SHACLObject.DESERIALIZERS["test-class"] = test_class
 
 
+@register("http://example.org/test-class-required", "test-class-required")
 class test_class_required(test_class):
-    TYPE = "http://example.org/test-class-required"
-    COMPACT_TYPE = "test-class-required"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
         # A required string list property
-        self._add_property(
+        cls._add_property(
             "test_class_required_string_list_prop",
             ListProp(StringProp()),
             iri="http://example.org/test-class/required-string-list-prop",
             max_count=2,
             min_count=1,
             compact="test-class/required-string-list-prop",
         )
         # A required scalar string property
-        self._add_property(
+        cls._add_property(
             "test_class_required_string_scalar_prop",
             StringProp(),
             iri="http://example.org/test-class/required-string-scalar-prop",
             min_count=1,
             compact="test-class/required-string-scalar-prop",
         )
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/test-class-required"] = test_class_required
-SHACLObject.DESERIALIZERS["test-class-required"] = test_class_required
 
 
 # A class derived from test-class
+@register("http://example.org/test-derived-class", "test-derived-class")
 class test_derived_class(test_class):
-    TYPE = "http://example.org/test-derived-class"
-    COMPACT_TYPE = "test-derived-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/test-derived-class"] = test_derived_class
-SHACLObject.DESERIALIZERS["test-derived-class"] = test_derived_class
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
+        # A string property in a derived class
+        cls._add_property(
+            "test_derived_class_string_prop",
+            StringProp(),
+            iri="http://example.org/test-derived-class/string-prop",
+            compact="test-derived-class/string-prop",
+        )
 
 
 # Derived class that sorts before the parent to test ordering
+@register("http://example.org/aaa-derived-class", "aaa-derived-class")
 class aaa_derived_class(parent_class):
-    TYPE = "http://example.org/aaa-derived-class"
-    COMPACT_TYPE = "aaa-derived-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/aaa-derived-class"] = aaa_derived_class
-SHACLObject.DESERIALIZERS["aaa-derived-class"] = aaa_derived_class
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # A class that derives its nodeKind from parent
+@register("http://example.org/derived-node-kind-iri", "derived-node-kind-iri")
 class derived_node_kind_iri(node_kind_iri):
-    TYPE = "http://example.org/derived-node-kind-iri"
-    COMPACT_TYPE = "derived-node-kind-iri"
     NODE_KIND = NodeKind.IRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
-SHACLObject.DESERIALIZERS["http://example.org/derived-node-kind-iri"] = derived_node_kind_iri
-SHACLObject.DESERIALIZERS["derived-node-kind-iri"] = derived_node_kind_iri
+# An extensible class
+@register("http://example.org/extensible-class", "extensible-class")
+class extensible_class(link_class):
+    NODE_KIND = NodeKind.BlankNodeOrIRI
+
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
+        # A required string
+        cls._add_property(
+            "extensible_class_required",
+            StringProp(),
+            iri="http://example.org/extensible-class/required",
+            min_count=1,
+            compact="extensible-class/required",
+        )
 
 
 """Format Guard"""
 # fmt: on
 
 
 def main():
@@ -1939,25 +2037,26 @@
     parser = argparse.ArgumentParser(description="Python SHACL model test")
     parser.add_argument("infile", type=Path, help="Input file")
     parser.add_argument("--print", action="store_true", help="Print object tree")
     parser.add_argument("--outfile", type=Path, help="Output file")
 
     args = parser.parse_args()
 
+    doc = SHACLDocument()
     with args.infile.open("r") as f:
         d = JSONLDDeserializer()
-        objects, _ = d.read(f)
+        d.read(f, doc)
 
     if args.print:
-        print_tree(objects)
+        print_tree(doc.objects)
 
     if args.outfile:
         with args.outfile.open("wb") as f:
             s = JSONLDSerializer()
-            s.write(objects, f)
+            s.write(doc, f)
 
     return 0
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `shacl2code-0.0.8/tests/expect/python/test.py` & `shacl2code-0.0.9/tests/expect/python/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # SPDX-License-Identifier: MIT
 
 import functools
 import hashlib
 import json
 import re
 import time
+import threading
 from contextlib import contextmanager
 from datetime import datetime, timezone, timedelta
 from enum import Enum
 from abc import ABC, abstractmethod
 
 
 def check_type(obj, types):
@@ -58,26 +59,29 @@
 
     def elide(self, value):
         return value is None
 
     def walk(self, value, callback, path):
         callback(value, path)
 
-    def link_prop(self, value, link_cache, missing, visited):
+    def iter_objects(self, value, recursive, visited):
+        return []
+
+    def link_prop(self, value, doc, missing, visited):
         return value
 
     def to_string(self, value):
         return str(value)
 
     @abstractmethod
     def encode(self, encoder, value, state):
         pass
 
     @abstractmethod
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         pass
 
 
 class StringProp(Property):
     """
     A scalar string property for an SHACL object
     """
@@ -86,23 +90,23 @@
 
     def set(self, value):
         return str(value)
 
     def encode(self, encoder, value, state):
         encoder.write_string(value)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         return decoder.read_string()
 
 
 class AnyURIProp(StringProp):
     def encode(self, encoder, value, state):
         encoder.write_iri(value)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         return decoder.read_iri()
 
 
 class DateTimeProp(Property):
     """
     A Date/Time Object with optional timezone
     """
@@ -113,15 +117,15 @@
 
     def set(self, value):
         return self._normalize(value)
 
     def encode(self, encoder, value, state):
         encoder.write_datetime(self.to_string(value))
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         s = decoder.read_datetime()
         if s is None:
             return None
         v = self.from_string(s)
         return self._normalize(v)
 
     def _normalize(self, value):
@@ -167,15 +171,15 @@
 
     def set(self, value):
         return int(value)
 
     def encode(self, encoder, value, state):
         encoder.write_integer(value)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         return decoder.read_integer()
 
 
 class PositiveIntegerProp(IntegerProp):
     def validate(self, value):
         super().validate(value)
         if value < 1:
@@ -194,28 +198,28 @@
 
     def set(self, value):
         return bool(value)
 
     def encode(self, encoder, value, state):
         encoder.write_bool(value)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         return decoder.read_bool()
 
 
 class FloatProp(Property):
     VALID_TYPES = (float, int)
 
     def set(self, value):
         return float(value)
 
     def encode(self, encoder, value, state):
         encoder.write_float(value)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         return decoder.read_float()
 
 
 class ObjectProp(Property):
     """
     A scalar SHACL object property of a SHACL object
     """
@@ -238,51 +242,64 @@
             return
 
         if not isinstance(value, str):
             value.walk(callback, path)
         else:
             callback(value, path)
 
+    def iter_objects(self, value, recursive, visited):
+        if value is None or isinstance(value, str):
+            return
+
+        if value not in visited:
+            visited.add(value)
+            yield value
+
+            if recursive:
+                for c in value.iter_objects(recursive=True, visited=visited):
+                    yield c
+
     def encode(self, encoder, value, state):
         if value is None:
             raise ValueError("Object cannot be None")
 
         if isinstance(value, str):
             encoder.write_iri(value)
             return
 
         return value.encode(encoder, state)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         iri = decoder.read_iri()
         if iri is not None:
-            if object_ids and iri in object_ids:
-                return object_ids[iri]
+            if doc is not None:
+                return doc.find_by_id(iri, iri)
             return iri
 
-        return SHACLObject.decode(decoder, object_ids=object_ids)
+        return SHACLObject.decode(decoder, doc=doc)
 
-    def link_prop(self, value, link_cache, missing, visited):
+    def link_prop(self, value, doc, missing, visited):
         if value is None:
             return value
 
         if isinstance(value, str):
-            if value in link_cache:
-                return link_cache[value]
+            o = doc.find_by_id(value)
+            if o is not None:
+                return o
 
             if missing is not None:
                 missing.add(value)
 
             return value
 
         # De-duplicate IDs
-        if value._id and value._id is not link_cache[value._id]:
-            value = link_cache[value._id]
+        if value._id:
+            value = doc.find_by_id(value._id, value)
 
-        value.link_helper(link_cache, missing, visited)
+        value.link_helper(doc, missing, visited)
         return value
 
 
 class ListProxy(object):
     def __init__(self, prop, data=None):
         if data is None:
             self.__data = []
@@ -381,34 +398,39 @@
         return len(value) == 0
 
     def walk(self, value, callback, path):
         callback(value, path)
         for idx, v in enumerate(value):
             self.prop.walk(v, callback, path + [f"[{idx}]"])
 
-    def link_prop(self, value, link_cache, missing, visited):
+    def iter_objects(self, value, recursive, visited):
+        for v in value:
+            for c in self.prop.iter_objects(v, recursive, visited):
+                yield c
+
+    def link_prop(self, value, doc, missing, visited):
         if isinstance(value, ListProxy):
-            data = [self.prop.link_prop(v, link_cache, missing, visited) for v in value]
+            data = [self.prop.link_prop(v, doc, missing, visited) for v in value]
         else:
-            data = [self.prop.link_prop(v, link_cache, missing, visited) for v in value]
+            data = [self.prop.link_prop(v, doc, missing, visited) for v in value]
 
         return ListProxy(self.prop, data=data)
 
     def encode(self, encoder, value, state):
         check_type(value, ListProxy)
 
         with encoder.write_list() as list_s:
             for v in value:
                 with list_s.write_list_item() as item_s:
                     self.prop.encode(item_s, v, state)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         data = []
         for val_d in decoder.read_list():
-            v = self.prop.decode(val_d, object_ids=object_ids)
+            v = self.prop.decode(val_d, doc=doc)
             self.prop.validate(v)
             data.append(v)
 
         return ListProxy(self.prop, data=data)
 
 
 class EnumProp(Property):
@@ -430,130 +452,166 @@
         for iri, compact in self.context:
             if iri == value:
                 encoder.write_enum(value, self, compact)
                 return
 
         encoder.write_enum(value, self)
 
-    def decode(self, decoder, *, object_ids=None):
+    def decode(self, decoder, *, doc=None):
         v = decoder.read_enum(self)
         for iri, compact in self.context:
             if v == compact:
                 return iri
         return v
 
 
 class NodeKind(Enum):
     BlankNode = 1
     IRI = 2
     BlankNodeOrIRI = 3
 
 
+def register(type_iri, compact_type=None):
+    def add_deserializer(key, c):
+        assert (
+            key not in SHACLObject.DESERIALIZERS
+        ), f"{key} already registered to {SHACLObject.DESERIALIZERS[key].__name__}"
+        SHACLObject.DESERIALIZERS[key] = c
+
+    def decorator(c):
+        assert issubclass(
+            c, SHACLObject
+        ), f"{c.__name__} is not derived from SHACLObject"
+
+        c.TYPE = type_iri
+        add_deserializer(type_iri, c)
+
+        c.COMPACT_TYPE = compact_type
+        if compact_type:
+            add_deserializer(compact_type, c)
+
+        # Registration is deferred until the first instance of class is created
+        # so that it has access to any other defined class
+        c._NEEDS_REG = True
+        return c
+
+    return decorator
+
+
+register_lock = threading.Lock()
+
+
 @functools.total_ordering
 class SHACLObject(object):
     DESERIALIZERS = {}
     NODE_KIND = NodeKind.BlankNodeOrIRI
     ID_ALIAS = None
     COMPACT_TYPE = None
 
-    def __init__(self):
+    def __init__(self, **kwargs):
+        with register_lock:
+            cls = self.__class__
+            if cls._NEEDS_REG:
+                cls._OBJ_PROPERTIES = {}
+                cls._OBJ_IRIS = {}
+                cls._register_props()
+                cls._NEEDS_REG = False
+
         self._obj_data = {}
-        self._obj_properties = {}
-        self._obj_iris = {}
         self._obj_metadata = {}
 
-        self._add_property("_id", StringProp(), iri="@id")
+        for iri, prop, _, _, _, _ in self.__iter_props():
+            self._obj_data[iri] = prop.init()
 
-    def _set_init_props(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
 
+    @classmethod
+    def _register_props(cls):
+        cls._add_property("_id", StringProp(), iri="@id")
+
+    @classmethod
     def _add_property(
-        self,
+        cls,
         pyname,
         prop,
         iri,
         min_count=None,
         max_count=None,
         compact=None,
     ):
-        if pyname in self._obj_iris:
-            raise KeyError(
-                f"'{pyname}' is already defined for '{self.__class__.__name__}'"
-            )
-        if iri in self._obj_properties:
-            raise KeyError(
-                f"'{iri}' is already defined for '{self.__class__.__name__}'"
-            )
+        if pyname in cls._OBJ_IRIS:
+            raise KeyError(f"'{pyname}' is already defined for '{cls.__name__}'")
+        if iri in cls._OBJ_PROPERTIES:
+            raise KeyError(f"'{iri}' is already defined for '{cls.__name__}'")
 
-        while hasattr(self, pyname):
+        while hasattr(cls, pyname):
             pyname = pyname + "_"
 
-        self._obj_iris[pyname] = iri
-        self._obj_properties[iri] = (prop, min_count, max_count, pyname, compact)
-        self._obj_data[iri] = prop.init()
+        cls._OBJ_IRIS[pyname] = iri
+        cls._OBJ_PROPERTIES[iri] = (prop, min_count, max_count, pyname, compact)
 
     def __setattr__(self, name, value):
         if name.startswith("_obj_"):
             return super().__setattr__(name, value)
 
         if name == self.ID_ALIAS:
             name = "_id"
 
         try:
-            iri = self._obj_iris[name]
+            iri = self._OBJ_IRIS[name]
             self[iri] = value
         except KeyError:
             raise AttributeError(
                 f"'{name}' is not a valid property of {self.__class__.__name__}"
             )
 
     def __getattr__(self, name):
         if name.startswith("_obj_"):
             return self.__dict__[name]
 
         if name == "_metadata":
             return self._obj_metadata
 
         if name == "_IRI":
-            return self._obj_iris
+            return self._OBJ_IRIS
 
         if name == self.ID_ALIAS:
             name = "_id"
 
         try:
-            iri = self._obj_iris[name]
+            iri = self._OBJ_IRIS[name]
             return self[iri]
         except KeyError:
             raise AttributeError(
                 f"'{name}' is not a valid property of {self.__class__.__name__}"
             )
 
     def __delattr__(self, name):
         if name == self.ID_ALIAS:
             name = "_id"
 
         try:
-            iri = self._obj_iris[name]
+            iri = self._OBJ_IRIS[name]
             del self[iri]
         except KeyError:
             raise AttributeError(
                 f"'{name}' is not a valid property of {self.__class__.__name__}"
             )
 
     def __get_prop(self, iri):
-        if iri not in self._obj_properties:
+        if iri not in self._OBJ_PROPERTIES:
             raise KeyError(
                 f"'{iri}' is not a valid property of {self.__class__.__name__}"
             )
 
-        return self._obj_properties[iri]
+        return self._OBJ_PROPERTIES[iri]
 
     def __iter_props(self):
-        for iri, v in self._obj_properties.items():
+        for iri, v in self._OBJ_PROPERTIES.items():
             yield iri, *v
 
     def __getitem__(self, iri):
         return self._obj_data[iri]
 
     def __setitem__(self, iri, value):
         if iri == "@id":
@@ -573,15 +631,15 @@
         self._obj_data[iri] = prop.set(value)
 
     def __delitem__(self, iri):
         prop, _, _, _, _ = self.__get_prop(iri)
         self._obj_data[iri] = prop.init()
 
     def __iter__(self):
-        return self._obj_properties.keys()
+        return self._OBJ_PROPERTIES.keys()
 
     def walk(self, callback, path=None):
         """
         Walk object tree, invoking the callback for each item
 
         Callback has the form:
 
@@ -590,39 +648,35 @@
         if path is None:
             path = ["."]
 
         if callback(self, path):
             for iri, prop, _, _, _, _ in self.__iter_props():
                 prop.walk(self._obj_data[iri], callback, path + [f".{iri}"])
 
-    def child_objects(self):
+    def property_keys(self):
+        for iri, _, _, _, pyname, compact in self.__iter_props():
+            if iri == "@id":
+                compact = self.ID_ALIAS
+            yield pyname, iri, compact
+
+    def iter_objects(self, *, recursive=False, visited=None):
         """
-        Iterate over each object that is a child of this one
+        Iterate of all objects that are a child of this one
         """
-        seen = set()
+        if visited is None:
+            visited = set()
 
-        def _walk_callback(value, path):
-            nonlocal seen
-
-            if not isinstance(value, SHACLObject):
-                return False
-
-            if value in seen:
-                return False
-
-            seen.add(value)
-            return True
-
-        self.walk(_walk_callback)
-
-        for obj in seen:
-            yield obj
+        for iri, prop, _, _, _, _ in self.__iter_props():
+            for c in prop.iter_objects(
+                self._obj_data[iri], recursive=recursive, visited=visited
+            ):
+                yield c
 
     def encode(self, encoder, state):
-        idname = self.ID_ALIAS or self._obj_iris["_id"]
+        idname = self.ID_ALIAS or self._OBJ_IRIS["_id"]
         if not self._id and self.NODE_KIND == NodeKind.IRI:
             raise ValueError(
                 f"{self.__class__.__name__} ({id(self)}) must have a IRI for property '{idname}'"
             )
 
         if state.is_written(self):
             encoder.write_iri(state.get_object_id(self))
@@ -652,77 +706,69 @@
 
                 if max_count is not None:
                     if not prop.check_max_count(value, max_count):
                         raise ValueError(
                             f"Property '{pyname}' in {self.__class__.__name__} ({id(self)}) requires a maximum of {max_count} elements"
                         )
 
-                if iri == self._obj_iris["_id"]:
+                if iri == self._OBJ_IRIS["_id"]:
                     continue
 
                 with obj_s.write_property(iri, compact) as prop_s:
                     prop.encode(prop_s, value, state)
 
     @classmethod
-    def decode(cls, decoder, *, object_ids=None):
+    def decode(cls, decoder, *, doc=None):
         typ, obj_d = decoder.read_object()
         if typ is None:
             raise TypeError("Unable to determine type for object")
 
         if typ not in cls.DESERIALIZERS:
             raise TypeError(f"Unknown type {typ}")
 
         obj = cls.DESERIALIZERS[typ]()
         _id = obj_d.read_object_id(obj.ID_ALIAS)
         if _id is not None:
-            if object_ids is not None:
-                if _id in object_ids:
-                    return object_ids[_id]
-                object_ids[_id] = obj
             obj._id = _id
+            if doc is not None:
+                v = doc.find_by_id(_id)
+                if v is not None:
+                    return v
+
+        if doc is not None:
+            doc.add_index(obj)
 
         for iri, prop, _, _, _, compact in obj.__iter_props():
-            if iri == obj._obj_iris["_id"]:
+            if iri == obj._OBJ_IRIS["_id"]:
                 continue
 
             with obj_d.read_property(iri, compact) as prop_d:
                 if prop_d is None:
                     continue
 
-                v = prop.decode(prop_d, object_ids=object_ids)
+                v = prop.decode(prop_d, doc=doc)
                 prop.validate(v)
                 obj._obj_data[iri] = v
 
         return obj
 
-    def link_helper(self, link_cache, missing, visited):
+    def link_helper(self, doc, missing, visited):
         if self in visited:
             return
 
         visited.add(self)
 
         for iri, prop, _, _, _, _ in self.__iter_props():
             self._obj_data[iri] = prop.link_prop(
                 self._obj_data[iri],
-                link_cache,
+                doc,
                 missing,
                 visited,
             )
 
-    def link(self, link_cache=None):
-        if not link_cache:
-            link_cache = {obj._id: obj for obj in self.child_objects() if obj._id}
-
-        missing = set()
-        visited = set()
-
-        self.link_helper(link_cache, missing, visited)
-
-        return missing
-
     def __str__(self):
         parts = [
             f"{self.__class__.__name__}(",
         ]
         if self._id:
             parts.append(f"@id='{self._id}'")
         parts.append(")")
@@ -744,135 +790,213 @@
                 getattr(obj, "name", None) or "",
                 id(obj),
             )
 
         return sort_key(self) < sort_key(other)
 
 
-class EncodeState(object):
-    def __init__(self):
-        self.ref_objects = set()
-        self.written_objects = set()
-        self.blank_objects = {}
+class SHACLDocument(object):
+    def __init__(self, objects=[], *, link=False):
+        self.objects = set()
+        for o in objects:
+            self.objects.add(o)
+        self.create_index()
+        if link:
+            self._link()
+
+    def create_index(self):
+        self.obj_by_id = {}
+        self.obj_by_type = {}
+        for o in self.foreach():
+            self.add_index(o)
+
+    def add_index(self, obj):
+        for typ in SHACLObject.DESERIALIZERS.values():
+            if isinstance(obj, typ):
+                self.obj_by_type.setdefault(typ, set()).add(obj)
 
-    def get_object_id(self, o):
-        if o._id:
-            return o._id
+        if not obj._id:
+            return
 
-        if o not in self.blank_objects:
-            _id = f"_:{o.__class__.__name__}{len(self.blank_objects)}"
-            self.blank_objects[o] = _id
+        if obj._id in self.obj_by_id:
+            return
 
-        return self.blank_objects[o]
+        self.obj_by_id[obj._id] = obj
 
-    def is_refed(self, o):
-        return o in self.ref_objects
+    def link(self):
+        self.create_index()
+        return self._link()
 
-    def add_refed(self, o):
-        self.ref_objects.add(o)
+    def _link(self):
+        missing = set()
+        visited = set()
 
-    def is_written(self, o):
-        return o in self.written_objects
+        new_objects = set()
 
-    def add_written(self, o):
-        self.written_objects.add(o)
+        for o in self.objects:
+            if o._id:
+                o = self.find_by_id(o._id, o)
+            o.link_helper(self, missing, visited)
+            new_objects.add(o)
+
+        self.objects = new_objects
+
+        # Remove blank nodes
+        obj_by_id = {}
+        for _id, obj in self.obj_by_id.items():
+            if _id.startswith("_:"):
+                del obj._id
+            else:
+                obj_by_id[obj._id] = obj
+        self.obj_by_id = obj_by_id
 
+        return missing
 
-def encode_objects(encoder, objects, force_list=False):
-    """
-    Serialize a list of objects to a serialization encoder
+    def find_by_id(self, _id, default=None):
+        if _id not in self.obj_by_id:
+            return default
+        return self.obj_by_id[_id]
 
-    If force_list is true, a list will always be written using the encoder.
-    """
-    ref_counts = {}
-    state = EncodeState()
+    def foreach(self):
+        visited = set()
+        for o in self.objects:
+            if o not in visited:
+                yield o
+                visited.add(o)
+
+            for child in o.iter_objects(recursive=True, visited=visited):
+                yield child
+
+    def foreach_type(self, typ, *, subclass=False):
+        if isinstance(typ, str):
+            typ = SHACLObject.DESERIALIZERS[typ]
 
-    def walk_callback(value, path):
-        nonlocal state
-        nonlocal ref_counts
+        if typ not in self.obj_by_type:
+            return
 
-        if not isinstance(value, SHACLObject):
-            return True
+        for o in self.obj_by_type[typ]:
+            if subclass or o.__class__ is typ:
+                yield o
 
-        # Remove blank node ID for re-assignment
-        if value._id and value._id.startswith("_:"):
-            del value._id
+    def merge(self, *doc):
+        new_objects = set()
+        new_objects |= self.objects
+        for d in doc:
+            new_objects |= d.objects
 
-        if value._id:
-            state.add_refed(value)
+        return SHACLDocument(new_objects, link=True)
 
-        # If the object is referenced more than once, add it to the set of
-        # referenced objects
-        ref_counts.setdefault(value, 0)
-        ref_counts[value] += 1
-        if ref_counts[value] > 1:
-            state.add_refed(value)
-            return False
+    def encode(self, encoder, force_list=False):
+        """
+        Serialize a list of objects to a serialization encoder
 
-        return True
+        If force_list is true, a list will always be written using the encoder.
+        """
+        ref_counts = {}
+        state = EncodeState()
 
-    for o in objects:
-        if o._id:
-            state.add_refed(o)
-        o.walk(walk_callback)
+        def walk_callback(value, path):
+            nonlocal state
+            nonlocal ref_counts
 
-    use_list = force_list or len(objects) > 1
+            if not isinstance(value, SHACLObject):
+                return True
 
-    objects = set(objects)
+            # Remove blank node ID for re-assignment
+            if value._id and value._id.startswith("_:"):
+                del value._id
+
+            if value._id:
+                state.add_refed(value)
+
+            # If the object is referenced more than once, add it to the set of
+            # referenced objects
+            ref_counts.setdefault(value, 0)
+            ref_counts[value] += 1
+            if ref_counts[value] > 1:
+                state.add_refed(value)
+                return False
 
-    if use_list:
-        # If we are making a list add all the objects referred to by reference
-        # to the list
-        objects |= state.ref_objects
-
-    objects = list(objects)
-    objects.sort()
-
-    if use_list:
-        # Ensure top level objects are only written in the top level graph
-        # node, and referenced by ID everywhere else. This is done by setting
-        # the flag that indicates this object has been written for all the top
-        # level objects, then clearing it right before serializing the object.
-        #
-        # In this way, if an object is referenced before it is supposed to be
-        # serialized into the @graph, it will serialize as a string instead of
-        # the actual object
-        for o in objects:
-            state.written_objects.add(o)
+            return True
 
-        with encoder.write_list() as list_s:
+        for o in self.objects:
+            if o._id:
+                state.add_refed(o)
+            o.walk(walk_callback)
+
+        use_list = force_list or len(self.objects) > 1
+
+        if use_list:
+            # If we are making a list add all the objects referred to by reference
+            # to the list
+            objects = list(self.objects | state.ref_objects)
+        else:
+            objects = list(self.objects)
+
+        objects.sort()
+
+        if use_list:
+            # Ensure top level objects are only written in the top level graph
+            # node, and referenced by ID everywhere else. This is done by setting
+            # the flag that indicates this object has been written for all the top
+            # level objects, then clearing it right before serializing the object.
+            #
+            # In this way, if an object is referenced before it is supposed to be
+            # serialized into the @graph, it will serialize as a string instead of
+            # the actual object
             for o in objects:
-                # Allow this specific object to be written now
-                state.written_objects.remove(o)
-                with list_s.write_list_item() as item_s:
-                    o.encode(item_s, state)
+                state.written_objects.add(o)
 
-    else:
-        objects[0].encode(encoder, state)
+            with encoder.write_list() as list_s:
+                for o in objects:
+                    # Allow this specific object to be written now
+                    state.written_objects.remove(o)
+                    with list_s.write_list_item() as item_s:
+                        o.encode(item_s, state)
 
+        else:
+            objects[0].encode(encoder, state)
 
-def decode_objects(decoder):
-    object_ids = {}
-    objects = [
-        SHACLObject.decode(obj_d, object_ids=object_ids)
-        for obj_d in decoder.read_list()
-    ]
+    def decode(self, decoder):
+        self.create_index()
 
-    for o in objects:
-        o.link(object_ids)
+        for obj_d in decoder.read_list():
+            o = SHACLObject.decode(obj_d, doc=self)
+            self.objects.add(o)
 
-    # Remove blank node IDs
-    for o in objects:
-        for c in o.child_objects():
-            if c._id and c._id.startswith("_:"):
-                del c._id
+        self._link()
+
+
+class EncodeState(object):
+    def __init__(self):
+        self.ref_objects = set()
+        self.written_objects = set()
+        self.blank_objects = {}
+
+    def get_object_id(self, o):
+        if o._id:
+            return o._id
+
+        if o not in self.blank_objects:
+            _id = f"_:{o.__class__.__name__}{len(self.blank_objects)}"
+            self.blank_objects[o] = _id
+
+        return self.blank_objects[o]
+
+    def is_refed(self, o):
+        return o in self.ref_objects
 
-    object_ids = {k: v for k, v in object_ids.items() if not k.startswith("_:")}
+    def add_refed(self, o):
+        self.ref_objects.add(o)
 
-    return objects, object_ids
+    def is_written(self, o):
+        return o in self.written_objects
+
+    def add_written(self, o):
+        self.written_objects.add(o)
 
 
 class Decoder(ABC):
     @abstractmethod
     def read_string(self):
         """
         Consume the next item as a string.
@@ -1076,22 +1200,22 @@
         return None, self
 
     def read_object_id(self, alias=None):
         return self.__get_value(alias, "@id")
 
 
 class JSONLDDeserializer(object):
-    def read(self, f):
+    def read(self, f, doc):
         data = json.load(f)
         if "@graph" in data:
             h = JSONLDDecoder(data["@graph"])
         else:
             h = JSONLDDecoder(data)
 
-        return decode_objects(h)
+        doc.decode(h)
 
 
 class Encoder(ABC):
     @abstractmethod
     def write_string(self, v):
         """
         Write a string value
@@ -1276,41 +1400,46 @@
         s = self.__class__(None)
         yield s
         if s.data is not None:
             self.data.append(s.data)
 
 
 class JSONLDSerializer(object):
-    def serialize_data(self, objects, force_graph=False):
-        h = JSONLDEncoder()
-        encode_objects(h, objects, force_graph)
-        if isinstance(h.data, list):
-            data = {
-                "@graph": h.data,
-            }
-        else:
-            data = h.data
+    def __init__(self, **args):
+        self.args = args
 
+    def serialize_data(self, doc, force_graph=False):
+        h = JSONLDEncoder()
+        doc.encode(h, force_graph)
+        data = {}
         if len(CONTEXT_URLS) == 1:
             data["@context"] = CONTEXT_URLS[0]
         elif CONTEXT_URLS:
             data["@context"] = CONTEXT_URLS
 
+        if isinstance(h.data, list):
+            data["@graph"] = h.data
+        else:
+            for k, v in h.data.items():
+                data[k] = v
+
         return data
 
-    def write(self, objects, f, force_graph=False, **kwargs):
+    def write(self, doc, f, force_graph=False, **kwargs):
         """
-        Write a list of objects to a JSON LD file
+        Write a SHACLDocument to a JSON LD file
 
         If force_graph is True, a @graph node will always be written
         """
-        data = self.serialize_data(objects, force_graph)
+        data = self.serialize_data(doc, force_graph)
+
+        args = {**self.args, **kwargs}
 
         sha1 = hashlib.sha1()
-        for chunk in json.JSONEncoder(**kwargs).iterencode(data):
+        for chunk in json.JSONEncoder(**args).iterencode(data):
             chunk = chunk.encode("utf-8")
             f.write(chunk)
             sha1.update(chunk)
 
         return sha1.hexdigest()
 
 
@@ -1326,19 +1455,16 @@
         self.sha1.update(s)
 
     def _write_comma(self):
         if self.comma:
             self.write(",")
             self.comma = False
 
-    def _need_comma(self):
-        self.comma = True
-
     def write_string(self, v):
-        self.write(f'"{v}"')
+        self.write(json.dumps(v))
 
     def write_datetime(self, v):
         self.write_string(v)
 
     def write_integer(self, v):
         self.write(f"{v}")
 
@@ -1351,36 +1477,40 @@
     def write_bool(self, v):
         if v:
             self.write("true")
         else:
             self.write("false")
 
     def write_float(self, v):
-        self.write(f'"{v}"')
+        self.write(json.dumps(str(v)))
 
     @contextmanager
     def write_property(self, iri, compact=None):
         self._write_comma()
-        self.write(f'"{compact or iri}":')
+        self.write_string(compact or iri)
+        self.write(":")
         yield self
         self.comma = True
 
     @contextmanager
     def write_object(self, o, _id, needs_id):
         self._write_comma()
 
         self.write("{")
+        self.write_string("@type")
+        self.write(":")
+        self.write_string(o.COMPACT_TYPE or o.TYPE)
+        self.comma = True
+
         if needs_id:
-            idname = o.ID_ALIAS or "@id"
-            idval = _id
-            self.write(f'"{idname}": "{idval}",')
-
-        typname = "@type"
-        typval = o.COMPACT_TYPE or o.TYPE
-        self.write(f'"{typname}":"{typval}"')
+            self._write_comma()
+            self.write_string(o.ID_ALIAS or "@id")
+            self.write(":")
+            self.write_string(_id)
+            self.comma = True
 
         self.comma = True
         yield self
 
         self.write("}")
         self.comma = True
 
@@ -1396,32 +1526,35 @@
     def write_list_item(self):
         self._write_comma()
         yield self.__class__(self.f, self.sha1)
         self.comma = True
 
 
 class JSONLDInlineSerializer(object):
-    def write(self, objects, f):
+    def write(self, doc, f, force_graph=False):
         """
-        Write a list of objects to a JSON LD file
+        Write a SHACLDocument to a JSON LD file
+
+        Note: force_graph is included for compatibility, but ignored. This
+        serializer always writes out a graph
         """
         sha1 = hashlib.sha1()
         h = JSONLDInlineEncoder(f, sha1)
         h.write('{"@context":')
         if len(CONTEXT_URLS) == 1:
             h.write(f'"{CONTEXT_URLS[0]}"')
         elif CONTEXT_URLS:
             h.write('["')
             h.write('","'.join(CONTEXT_URLS))
             h.write('"]')
         h.write(",")
 
         h.write('"@graph":')
 
-        encode_objects(h, objects, True)
+        doc.encode(h, True)
         h.write("}")
         return sha1.hexdigest()
 
 
 def print_tree(objects, all_fields=False):
     """
     Print object tree
@@ -1481,386 +1614,377 @@
     foo = "http://example.org/enumType/foo"
     # This value has no label
     nolabel = "http://example.org/enumType/nolabel"
 
 
 # CLASSES
 # A class with an ID alias
+@register("http://example.org/id-prop-class")
 class http_example_org_id_prop_class(SHACLObject):
-    TYPE = "http://example.org/id-prop-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
     ID_ALIAS = "testid"
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/id-prop-class"] = http_example_org_id_prop_class
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # A class that inherits its idPropertyName from the parent
+@register("http://example.org/inherited-id-prop-class")
 class http_example_org_inherited_id_prop_class(http_example_org_id_prop_class):
-    TYPE = "http://example.org/inherited-id-prop-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
     ID_ALIAS = "testid"
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/inherited-id-prop-class"] = http_example_org_inherited_id_prop_class
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # A class to test links
+@register("http://example.org/link-class")
 class http_example_org_link_class(SHACLObject):
-    TYPE = "http://example.org/link-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
         # A link-class list property
-        self._add_property(
+        cls._add_property(
             "link_list_prop",
             ListProp(ObjectProp(http_example_org_link_class, False)),
             iri="http://example.org/link-class-link-list-prop",
         )
         # A link-class property
-        self._add_property(
+        cls._add_property(
             "link_prop",
             ObjectProp(http_example_org_link_class, False),
             iri="http://example.org/link-class-link-prop",
         )
         # A link-class property with no sh:class
-        self._add_property(
+        cls._add_property(
             "link_prop_no_class",
             ObjectProp(http_example_org_link_class, False),
             iri="http://example.org/link-class-link-prop-no-class",
         )
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/link-class"] = http_example_org_link_class
 
 
 # A class derived from link-class
+@register("http://example.org/link-derived-class")
 class http_example_org_link_derived_class(http_example_org_link_class):
-    TYPE = "http://example.org/link-derived-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/link-derived-class"] = http_example_org_link_derived_class
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # A class that must be a blank node
+@register("http://example.org/node-kind-blank")
 class http_example_org_node_kind_blank(http_example_org_link_class):
-    TYPE = "http://example.org/node-kind-blank"
     NODE_KIND = NodeKind.BlankNode
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/node-kind-blank"] = http_example_org_node_kind_blank
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # A class that must be an IRI
+@register("http://example.org/node-kind-iri")
 class http_example_org_node_kind_iri(http_example_org_link_class):
-    TYPE = "http://example.org/node-kind-iri"
     NODE_KIND = NodeKind.IRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/node-kind-iri"] = http_example_org_node_kind_iri
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # A class that can be either a blank node or an IRI
+@register("http://example.org/node-kind-iri-or-blank")
 class http_example_org_node_kind_iri_or_blank(http_example_org_link_class):
-    TYPE = "http://example.org/node-kind-iri-or-blank"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
+
 
+# A class that is not a nodeshape
+@register("http://example.org/non-shape-class")
+class http_example_org_non_shape_class(SHACLObject):
+    NODE_KIND = NodeKind.BlankNodeOrIRI
 
-SHACLObject.DESERIALIZERS["http://example.org/node-kind-iri-or-blank"] = http_example_org_node_kind_iri_or_blank
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # The parent class
+@register("http://example.org/parent-class")
 class http_example_org_parent_class(SHACLObject):
-    TYPE = "http://example.org/parent-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/parent-class"] = http_example_org_parent_class
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # Another class
+@register("http://example.org/test-another-class")
 class http_example_org_test_another_class(SHACLObject):
-    TYPE = "http://example.org/test-another-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/test-another-class"] = http_example_org_test_another_class
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # The test class
+@register("http://example.org/test-class")
 class http_example_org_test_class(http_example_org_parent_class):
-    TYPE = "http://example.org/test-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
         # A property that conflicts with an existing SHACLObject property
-        self._add_property(
+        cls._add_property(
             "encode",
             StringProp(),
             iri="http://example.org/encode",
         )
         # A property that is a keyword
-        self._add_property(
+        cls._add_property(
             "import_",
             StringProp(),
             iri="http://example.org/import",
         )
         # a URI
-        self._add_property(
+        cls._add_property(
             "anyuri_prop",
             AnyURIProp(),
             iri="http://example.org/test-class/anyuri-prop",
         )
         # a boolean property
-        self._add_property(
+        cls._add_property(
             "boolean_prop",
             BooleanProp(),
             iri="http://example.org/test-class/boolean-prop",
         )
         # A test-class list property
-        self._add_property(
+        cls._add_property(
             "class_list_prop",
             ListProp(ObjectProp(http_example_org_test_class, False)),
             iri="http://example.org/test-class/class-list-prop",
         )
         # A test-class property
-        self._add_property(
+        cls._add_property(
             "class_prop",
             ObjectProp(http_example_org_test_class, False),
             iri="http://example.org/test-class/class-prop",
         )
         # A test-class property with no sh:class
-        self._add_property(
+        cls._add_property(
             "class_prop_no_class",
             ObjectProp(http_example_org_test_class, False),
             iri="http://example.org/test-class/class-prop-no-class",
         )
         # A datetime list property
-        self._add_property(
+        cls._add_property(
             "datetime_list_prop",
             ListProp(DateTimeProp()),
             iri="http://example.org/test-class/datetime-list-prop",
         )
         # A scalar datetime property
-        self._add_property(
+        cls._add_property(
             "datetime_scalar_prop",
             DateTimeProp(),
             iri="http://example.org/test-class/datetime-scalar-prop",
         )
         # A scalar dateTimeStamp property
-        self._add_property(
+        cls._add_property(
             "datetimestamp_scalar_prop",
             DateTimeStampProp(),
             iri="http://example.org/test-class/datetimestamp-scalar-prop",
         )
         # A enum list property
-        self._add_property(
+        cls._add_property(
             "enum_list_prop",
             ListProp(http_example_org_enumType(context=[
             ])),
             iri="http://example.org/test-class/enum-list-prop",
         )
         # A enum property
-        self._add_property(
+        cls._add_property(
             "enum_prop",
             http_example_org_enumType(context=[
             ]),
             iri="http://example.org/test-class/enum-prop",
         )
         # A enum property with no sh:class
-        self._add_property(
+        cls._add_property(
             "enum_prop_no_class",
             http_example_org_enumType(context=[
             ]),
             iri="http://example.org/test-class/enum-prop-no-class",
         )
         # a float property
-        self._add_property(
+        cls._add_property(
             "float_prop",
             FloatProp(),
             iri="http://example.org/test-class/float-prop",
         )
         # a non-negative integer
-        self._add_property(
+        cls._add_property(
             "integer_prop",
             IntegerProp(),
             iri="http://example.org/test-class/integer-prop",
         )
         # A named property
-        self._add_property(
+        cls._add_property(
             "named_property",
             StringProp(),
             iri="http://example.org/test-class/named-property",
         )
         # A class with no shape
-        self._add_property(
+        cls._add_property(
             "non_shape",
-            AnyURIProp(),
+            ObjectProp(http_example_org_non_shape_class, False),
             iri="http://example.org/test-class/non-shape",
         )
         # a non-negative integer
-        self._add_property(
+        cls._add_property(
             "nonnegative_integer_prop",
             NonNegativeIntegerProp(),
             iri="http://example.org/test-class/nonnegative-integer-prop",
         )
         # A positive integer
-        self._add_property(
+        cls._add_property(
             "positive_integer_prop",
             PositiveIntegerProp(),
             iri="http://example.org/test-class/positive-integer-prop",
         )
         # A regex validated string
-        self._add_property(
+        cls._add_property(
             "regex",
             StringProp(pattern=r"^foo\d",),
             iri="http://example.org/test-class/regex",
         )
         # A regex dateTime
-        self._add_property(
+        cls._add_property(
             "regex_datetime",
             DateTimeProp(pattern=r"^\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d\+01:00$",),
             iri="http://example.org/test-class/regex-datetime",
         )
         # A regex dateTimeStamp
-        self._add_property(
+        cls._add_property(
             "regex_datetimestamp",
             DateTimeStampProp(pattern=r"^\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\dZ$",),
             iri="http://example.org/test-class/regex-datetimestamp",
         )
         # A regex validated string list
-        self._add_property(
+        cls._add_property(
             "regex_list",
             ListProp(StringProp(pattern=r"^foo\d",)),
             iri="http://example.org/test-class/regex-list",
         )
         # A string list property with no sh:datatype
-        self._add_property(
+        cls._add_property(
             "string_list_no_datatype",
             ListProp(StringProp()),
             iri="http://example.org/test-class/string-list-no-datatype",
         )
         # A string list property
-        self._add_property(
+        cls._add_property(
             "string_list_prop",
             ListProp(StringProp()),
             iri="http://example.org/test-class/string-list-prop",
         )
         # A scalar string propery
-        self._add_property(
+        cls._add_property(
             "string_scalar_prop",
             StringProp(),
             iri="http://example.org/test-class/string-scalar-prop",
         )
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/test-class"] = http_example_org_test_class
 
 
+@register("http://example.org/test-class-required")
 class http_example_org_test_class_required(http_example_org_test_class):
-    TYPE = "http://example.org/test-class-required"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
         # A required string list property
-        self._add_property(
+        cls._add_property(
             "required_string_list_prop",
             ListProp(StringProp()),
             iri="http://example.org/test-class/required-string-list-prop",
             max_count=2,
             min_count=1,
         )
         # A required scalar string property
-        self._add_property(
+        cls._add_property(
             "required_string_scalar_prop",
             StringProp(),
             iri="http://example.org/test-class/required-string-scalar-prop",
             min_count=1,
         )
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/test-class-required"] = http_example_org_test_class_required
 
 
 # A class derived from test-class
+@register("http://example.org/test-derived-class")
 class http_example_org_test_derived_class(http_example_org_test_class):
-    TYPE = "http://example.org/test-derived-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/test-derived-class"] = http_example_org_test_derived_class
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
+        # A string property in a derived class
+        cls._add_property(
+            "string_prop",
+            StringProp(),
+            iri="http://example.org/test-derived-class/string-prop",
+        )
 
 
 # Derived class that sorts before the parent to test ordering
+@register("http://example.org/aaa-derived-class")
 class http_example_org_aaa_derived_class(http_example_org_parent_class):
-    TYPE = "http://example.org/aaa-derived-class"
     NODE_KIND = NodeKind.BlankNodeOrIRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
-
-
-SHACLObject.DESERIALIZERS["http://example.org/aaa-derived-class"] = http_example_org_aaa_derived_class
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
 # A class that derives its nodeKind from parent
+@register("http://example.org/derived-node-kind-iri")
 class http_example_org_derived_node_kind_iri(http_example_org_node_kind_iri):
-    TYPE = "http://example.org/derived-node-kind-iri"
     NODE_KIND = NodeKind.IRI
 
-    def __init__(self, **kwargs):
-        super().__init__()
-        self._set_init_props(**kwargs)
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
 
 
-SHACLObject.DESERIALIZERS["http://example.org/derived-node-kind-iri"] = http_example_org_derived_node_kind_iri
+# An extensible class
+@register("http://example.org/extensible-class")
+class http_example_org_extensible_class(http_example_org_link_class):
+    NODE_KIND = NodeKind.BlankNodeOrIRI
+
+    @classmethod
+    def _register_props(cls):
+        super()._register_props()
+        # A required string
+        cls._add_property(
+            "required",
+            StringProp(),
+            iri="http://example.org/extensible-class/required",
+            min_count=1,
+        )
 
 
 """Format Guard"""
 # fmt: on
 
 
 def main():
@@ -1870,25 +1994,26 @@
     parser = argparse.ArgumentParser(description="Python SHACL model test")
     parser.add_argument("infile", type=Path, help="Input file")
     parser.add_argument("--print", action="store_true", help="Print object tree")
     parser.add_argument("--outfile", type=Path, help="Output file")
 
     args = parser.parse_args()
 
+    doc = SHACLDocument()
     with args.infile.open("r") as f:
         d = JSONLDDeserializer()
-        objects, _ = d.read(f)
+        d.read(f, doc)
 
     if args.print:
-        print_tree(objects)
+        print_tree(doc.objects)
 
     if args.outfile:
         with args.outfile.open("wb") as f:
             s = JSONLDSerializer()
-            s.write(objects, f)
+            s.write(doc, f)
 
     return 0
 
 
 if __name__ == "__main__":
     import sys
```

### Comparing `shacl2code-0.0.8/tests/expect/raw/test-context.txt` & `shacl2code-0.0.9/tests/expect/raw/test-context.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,20 +13,24 @@
 
 http://example.org/node-kind-blank: node-kind-blank
 
 http://example.org/node-kind-iri: node-kind-iri
 
 http://example.org/node-kind-iri-or-blank: node-kind-iri-or-blank
 
+http://example.org/non-shape-class: non-shape-class
+
 http://example.org/parent-class: parent-class
 
 http://example.org/test-another-class: test-another-class
 
 http://example.org/test-class: test-class
 
 http://example.org/test-class-required: test-class-required
 
 http://example.org/test-derived-class: test-derived-class
 
 http://example.org/aaa-derived-class: aaa-derived-class
 
 http://example.org/derived-node-kind-iri: derived-node-kind-iri
+
+http://example.org/extensible-class: extensible-class
```

### Comparing `shacl2code-0.0.8/tests/expect/raw/test.txt` & `shacl2code-0.0.9/tests/expect/raw/test.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 
 Enum(_id='http://example.org/enumType', clsname='http_//example.org/enumType', values=[EnumValue(_id='http://example.org/enumType/bar', varname='bar', comment='The bar value of enumType'), EnumValue(_id='http://example.org/enumType/foo', varname='foo', comment='The foo value of enumType'), EnumValue(_id='http://example.org/enumType/nolabel', varname='nolabel', comment='This value has no label')], comment='An enumerated type')
 
-Class(_id='http://example.org/id-prop-class', clsname='http_//example.org/id-prop-class', parent_ids=[], derived_ids=['http://example.org/inherited-id-prop-class'], properties=[], comment='A class with an ID alias', id_property='testid', node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'))
-Class(_id='http://example.org/inherited-id-prop-class', clsname='http_//example.org/inherited-id-prop-class', parent_ids=['http://example.org/id-prop-class'], derived_ids=[], properties=[], comment='A class that inherits its idPropertyName from the parent', id_property='testid', node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'))
-Class(_id='http://example.org/link-class', clsname='http_//example.org/link-class', parent_ids=[], derived_ids=['http://example.org/link-derived-class', 'http://example.org/node-kind-blank', 'http://example.org/node-kind-iri', 'http://example.org/node-kind-iri-or-blank'], properties=[Property(path='http://example.org/link-class-link-list-prop', varname='-link-list-prop', comment='A link-class list property', max_count=None, min_count=None, enum_id='', class_id='http://example.org/link-class', datatype='', pattern=''), Property(path='http://example.org/link-class-link-prop', varname='-link-prop', comment='A link-class property', max_count=1, min_count=None, enum_id='', class_id='http://example.org/link-class', datatype='', pattern=''), Property(path='http://example.org/link-class-link-prop-no-class', varname='-link-prop-no-class', comment='A link-class property with no sh:class', max_count=1, min_count=None, enum_id='', class_id='http://example.org/link-class', datatype='', pattern='')], comment='A class to test links', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'))
-Class(_id='http://example.org/link-derived-class', clsname='http_//example.org/link-derived-class', parent_ids=['http://example.org/link-class'], derived_ids=[], properties=[], comment='A class derived from link-class', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'))
-Class(_id='http://example.org/node-kind-blank', clsname='http_//example.org/node-kind-blank', parent_ids=['http://example.org/link-class'], derived_ids=[], properties=[], comment='A class that must be a blank node', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNode'))
-Class(_id='http://example.org/node-kind-iri', clsname='http_//example.org/node-kind-iri', parent_ids=['http://example.org/link-class'], derived_ids=['http://example.org/derived-node-kind-iri'], properties=[], comment='A class that must be an IRI', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#IRI'))
-Class(_id='http://example.org/node-kind-iri-or-blank', clsname='http_//example.org/node-kind-iri-or-blank', parent_ids=['http://example.org/link-class'], derived_ids=[], properties=[], comment='A class that can be either a blank node or an IRI', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'))
-Class(_id='http://example.org/parent-class', clsname='http_//example.org/parent-class', parent_ids=[], derived_ids=['http://example.org/aaa-derived-class', 'http://example.org/test-class'], properties=[], comment='The parent class', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'))
-Class(_id='http://example.org/test-another-class', clsname='http_//example.org/test-another-class', parent_ids=[], derived_ids=[], properties=[], comment='Another class', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'))
-Class(_id='http://example.org/test-class', clsname='http_//example.org/test-class', parent_ids=['http://example.org/parent-class'], derived_ids=['http://example.org/test-class-required', 'http://example.org/test-derived-class'], properties=[Property(path='http://example.org/encode', varname='encode', comment='A property that conflicts with an existing SHACLObject property', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern=''), Property(path='http://example.org/import', varname='import', comment='A property that is a keyword', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern=''), Property(path='http://example.org/test-class/anyuri-prop', varname='anyuri-prop', comment='a URI', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#anyURI', pattern=''), Property(path='http://example.org/test-class/boolean-prop', varname='boolean-prop', comment='a boolean property', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#boolean', pattern=''), Property(path='http://example.org/test-class/class-list-prop', varname='class-list-prop', comment='A test-class list property', max_count=None, min_count=None, enum_id='', class_id='http://example.org/test-class', datatype='', pattern=''), Property(path='http://example.org/test-class/class-prop', varname='class-prop', comment='A test-class property', max_count=1, min_count=None, enum_id='', class_id='http://example.org/test-class', datatype='', pattern=''), Property(path='http://example.org/test-class/class-prop-no-class', varname='class-prop-no-class', comment='A test-class property with no sh:class', max_count=1, min_count=None, enum_id='', class_id='http://example.org/test-class', datatype='', pattern=''), Property(path='http://example.org/test-class/datetime-list-prop', varname='datetime-list-prop', comment='A datetime list property', max_count=None, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#dateTime', pattern=''), Property(path='http://example.org/test-class/datetime-scalar-prop', varname='datetime-scalar-prop', comment='A scalar datetime property', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#dateTime', pattern=''), Property(path='http://example.org/test-class/datetimestamp-scalar-prop', varname='datetimestamp-scalar-prop', comment='A scalar dateTimeStamp property', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#dateTimeStamp', pattern=''), Property(path='http://example.org/test-class/enum-list-prop', varname='enum-list-prop', comment='A enum list property', max_count=None, min_count=None, enum_id='http://example.org/enumType', class_id='', datatype='', pattern=''), Property(path='http://example.org/test-class/enum-prop', varname='enum-prop', comment='A enum property', max_count=1, min_count=None, enum_id='http://example.org/enumType', class_id='', datatype='', pattern=''), Property(path='http://example.org/test-class/enum-prop-no-class', varname='enum-prop-no-class', comment='A enum property with no sh:class', max_count=1, min_count=None, enum_id='http://example.org/enumType', class_id='', datatype='', pattern=''), Property(path='http://example.org/test-class/float-prop', varname='float-prop', comment='a float property', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#decimal', pattern=''), Property(path='http://example.org/test-class/integer-prop', varname='integer-prop', comment='a non-negative integer', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#integer', pattern=''), Property(path='http://example.org/test-class/named-property', varname=rdflib.term.Literal('named_property'), comment='A named property', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern=''), Property(path='http://example.org/test-class/non-shape', varname='non-shape', comment='A class with no shape', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#anyURI', pattern=''), Property(path='http://example.org/test-class/nonnegative-integer-prop', varname='nonnegative-integer-prop', comment='a non-negative integer', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#nonNegativeInteger', pattern=''), Property(path='http://example.org/test-class/positive-integer-prop', varname='positive-integer-prop', comment='A positive integer', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#positiveInteger', pattern=''), Property(path='http://example.org/test-class/regex', varname='regex', comment='A regex validated string', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern='^foo\\d'), Property(path='http://example.org/test-class/regex-datetime', varname='regex-datetime', comment='A regex dateTime', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#dateTime', pattern='^\\d\\d\\d\\d-\\d\\d-\\d\\dT\\d\\d:\\d\\d:\\d\\d\\+01:00$'), Property(path='http://example.org/test-class/regex-datetimestamp', varname='regex-datetimestamp', comment='A regex dateTimeStamp', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#dateTimeStamp', pattern='^\\d\\d\\d\\d-\\d\\d-\\d\\dT\\d\\d:\\d\\d:\\d\\dZ$'), Property(path='http://example.org/test-class/regex-list', varname='regex-list', comment='A regex validated string list', max_count=None, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern='^foo\\d'), Property(path='http://example.org/test-class/string-list-no-datatype', varname='string-list-no-datatype', comment='A string list property with no sh:datatype', max_count=None, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern=''), Property(path='http://example.org/test-class/string-list-prop', varname='string-list-prop', comment='A string list property', max_count=None, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern=''), Property(path='http://example.org/test-class/string-scalar-prop', varname='string-scalar-prop', comment='A scalar string propery', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern='')], comment='The test class', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'))
-Class(_id='http://example.org/test-class-required', clsname='http_//example.org/test-class-required', parent_ids=['http://example.org/test-class'], derived_ids=[], properties=[Property(path='http://example.org/test-class/required-string-list-prop', varname='required-string-list-prop', comment='A required string list property', max_count=2, min_count=1, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern=''), Property(path='http://example.org/test-class/required-string-scalar-prop', varname='required-string-scalar-prop', comment='A required scalar string property', max_count=1, min_count=1, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern='')], comment='', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'))
-Class(_id='http://example.org/test-derived-class', clsname='http_//example.org/test-derived-class', parent_ids=['http://example.org/test-class'], derived_ids=[], properties=[], comment='A class derived from test-class', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'))
-Class(_id='http://example.org/aaa-derived-class', clsname='http_//example.org/aaa-derived-class', parent_ids=['http://example.org/parent-class'], derived_ids=[], properties=[], comment='Derived class that sorts before the parent to test ordering', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'))
-Class(_id='http://example.org/derived-node-kind-iri', clsname='http_//example.org/derived-node-kind-iri', parent_ids=['http://example.org/node-kind-iri'], derived_ids=[], properties=[], comment='A class that derives its nodeKind from parent', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#IRI'))
+Class(_id='http://example.org/id-prop-class', clsname='http_//example.org/id-prop-class', parent_ids=[], derived_ids=['http://example.org/inherited-id-prop-class'], properties=[], comment='A class with an ID alias', id_property='testid', node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'), extensible=False)
+Class(_id='http://example.org/inherited-id-prop-class', clsname='http_//example.org/inherited-id-prop-class', parent_ids=['http://example.org/id-prop-class'], derived_ids=[], properties=[], comment='A class that inherits its idPropertyName from the parent', id_property='testid', node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'), extensible=False)
+Class(_id='http://example.org/link-class', clsname='http_//example.org/link-class', parent_ids=[], derived_ids=['http://example.org/extensible-class', 'http://example.org/link-derived-class', 'http://example.org/node-kind-blank', 'http://example.org/node-kind-iri', 'http://example.org/node-kind-iri-or-blank'], properties=[Property(path='http://example.org/link-class-link-list-prop', varname='-link-list-prop', comment='A link-class list property', max_count=None, min_count=None, enum_id='', class_id='http://example.org/link-class', datatype='', pattern=''), Property(path='http://example.org/link-class-link-prop', varname='-link-prop', comment='A link-class property', max_count=1, min_count=None, enum_id='', class_id='http://example.org/link-class', datatype='', pattern=''), Property(path='http://example.org/link-class-link-prop-no-class', varname='-link-prop-no-class', comment='A link-class property with no sh:class', max_count=1, min_count=None, enum_id='', class_id='http://example.org/link-class', datatype='', pattern='')], comment='A class to test links', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'), extensible=False)
+Class(_id='http://example.org/link-derived-class', clsname='http_//example.org/link-derived-class', parent_ids=['http://example.org/link-class'], derived_ids=[], properties=[], comment='A class derived from link-class', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'), extensible=False)
+Class(_id='http://example.org/node-kind-blank', clsname='http_//example.org/node-kind-blank', parent_ids=['http://example.org/link-class'], derived_ids=[], properties=[], comment='A class that must be a blank node', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNode'), extensible=False)
+Class(_id='http://example.org/node-kind-iri', clsname='http_//example.org/node-kind-iri', parent_ids=['http://example.org/link-class'], derived_ids=['http://example.org/derived-node-kind-iri'], properties=[], comment='A class that must be an IRI', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#IRI'), extensible=False)
+Class(_id='http://example.org/node-kind-iri-or-blank', clsname='http_//example.org/node-kind-iri-or-blank', parent_ids=['http://example.org/link-class'], derived_ids=[], properties=[], comment='A class that can be either a blank node or an IRI', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'), extensible=False)
+Class(_id='http://example.org/non-shape-class', clsname='http_//example.org/non-shape-class', parent_ids=[], derived_ids=[], properties=[], comment='A class that is not a nodeshape', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'), extensible=False)
+Class(_id='http://example.org/parent-class', clsname='http_//example.org/parent-class', parent_ids=[], derived_ids=['http://example.org/aaa-derived-class', 'http://example.org/test-class'], properties=[], comment='The parent class', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'), extensible=False)
+Class(_id='http://example.org/test-another-class', clsname='http_//example.org/test-another-class', parent_ids=[], derived_ids=[], properties=[], comment='Another class', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'), extensible=False)
+Class(_id='http://example.org/test-class', clsname='http_//example.org/test-class', parent_ids=['http://example.org/parent-class'], derived_ids=['http://example.org/test-class-required', 'http://example.org/test-derived-class'], properties=[Property(path='http://example.org/encode', varname='encode', comment='A property that conflicts with an existing SHACLObject property', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern=''), Property(path='http://example.org/import', varname='import', comment='A property that is a keyword', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern=''), Property(path='http://example.org/test-class/anyuri-prop', varname='anyuri-prop', comment='a URI', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#anyURI', pattern=''), Property(path='http://example.org/test-class/boolean-prop', varname='boolean-prop', comment='a boolean property', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#boolean', pattern=''), Property(path='http://example.org/test-class/class-list-prop', varname='class-list-prop', comment='A test-class list property', max_count=None, min_count=None, enum_id='', class_id='http://example.org/test-class', datatype='', pattern=''), Property(path='http://example.org/test-class/class-prop', varname='class-prop', comment='A test-class property', max_count=1, min_count=None, enum_id='', class_id='http://example.org/test-class', datatype='', pattern=''), Property(path='http://example.org/test-class/class-prop-no-class', varname='class-prop-no-class', comment='A test-class property with no sh:class', max_count=1, min_count=None, enum_id='', class_id='http://example.org/test-class', datatype='', pattern=''), Property(path='http://example.org/test-class/datetime-list-prop', varname='datetime-list-prop', comment='A datetime list property', max_count=None, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#dateTime', pattern=''), Property(path='http://example.org/test-class/datetime-scalar-prop', varname='datetime-scalar-prop', comment='A scalar datetime property', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#dateTime', pattern=''), Property(path='http://example.org/test-class/datetimestamp-scalar-prop', varname='datetimestamp-scalar-prop', comment='A scalar dateTimeStamp property', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#dateTimeStamp', pattern=''), Property(path='http://example.org/test-class/enum-list-prop', varname='enum-list-prop', comment='A enum list property', max_count=None, min_count=None, enum_id='http://example.org/enumType', class_id='', datatype='', pattern=''), Property(path='http://example.org/test-class/enum-prop', varname='enum-prop', comment='A enum property', max_count=1, min_count=None, enum_id='http://example.org/enumType', class_id='', datatype='', pattern=''), Property(path='http://example.org/test-class/enum-prop-no-class', varname='enum-prop-no-class', comment='A enum property with no sh:class', max_count=1, min_count=None, enum_id='http://example.org/enumType', class_id='', datatype='', pattern=''), Property(path='http://example.org/test-class/float-prop', varname='float-prop', comment='a float property', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#decimal', pattern=''), Property(path='http://example.org/test-class/integer-prop', varname='integer-prop', comment='a non-negative integer', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#integer', pattern=''), Property(path='http://example.org/test-class/named-property', varname=rdflib.term.Literal('named_property'), comment='A named property', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern=''), Property(path='http://example.org/test-class/non-shape', varname='non-shape', comment='A class with no shape', max_count=1, min_count=None, enum_id='', class_id='http://example.org/non-shape-class', datatype='', pattern=''), Property(path='http://example.org/test-class/nonnegative-integer-prop', varname='nonnegative-integer-prop', comment='a non-negative integer', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#nonNegativeInteger', pattern=''), Property(path='http://example.org/test-class/positive-integer-prop', varname='positive-integer-prop', comment='A positive integer', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#positiveInteger', pattern=''), Property(path='http://example.org/test-class/regex', varname='regex', comment='A regex validated string', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern='^foo\\d'), Property(path='http://example.org/test-class/regex-datetime', varname='regex-datetime', comment='A regex dateTime', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#dateTime', pattern='^\\d\\d\\d\\d-\\d\\d-\\d\\dT\\d\\d:\\d\\d:\\d\\d\\+01:00$'), Property(path='http://example.org/test-class/regex-datetimestamp', varname='regex-datetimestamp', comment='A regex dateTimeStamp', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#dateTimeStamp', pattern='^\\d\\d\\d\\d-\\d\\d-\\d\\dT\\d\\d:\\d\\d:\\d\\dZ$'), Property(path='http://example.org/test-class/regex-list', varname='regex-list', comment='A regex validated string list', max_count=None, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern='^foo\\d'), Property(path='http://example.org/test-class/string-list-no-datatype', varname='string-list-no-datatype', comment='A string list property with no sh:datatype', max_count=None, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern=''), Property(path='http://example.org/test-class/string-list-prop', varname='string-list-prop', comment='A string list property', max_count=None, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern=''), Property(path='http://example.org/test-class/string-scalar-prop', varname='string-scalar-prop', comment='A scalar string propery', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern='')], comment='The test class', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'), extensible=False)
+Class(_id='http://example.org/test-class-required', clsname='http_//example.org/test-class-required', parent_ids=['http://example.org/test-class'], derived_ids=[], properties=[Property(path='http://example.org/test-class/required-string-list-prop', varname='required-string-list-prop', comment='A required string list property', max_count=2, min_count=1, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern=''), Property(path='http://example.org/test-class/required-string-scalar-prop', varname='required-string-scalar-prop', comment='A required scalar string property', max_count=1, min_count=1, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern='')], comment='', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'), extensible=False)
+Class(_id='http://example.org/test-derived-class', clsname='http_//example.org/test-derived-class', parent_ids=['http://example.org/test-class'], derived_ids=[], properties=[Property(path='http://example.org/test-derived-class/string-prop', varname='string-prop', comment='A string property in a derived class', max_count=1, min_count=None, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern='')], comment='A class derived from test-class', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'), extensible=False)
+Class(_id='http://example.org/aaa-derived-class', clsname='http_//example.org/aaa-derived-class', parent_ids=['http://example.org/parent-class'], derived_ids=[], properties=[], comment='Derived class that sorts before the parent to test ordering', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'), extensible=False)
+Class(_id='http://example.org/derived-node-kind-iri', clsname='http_//example.org/derived-node-kind-iri', parent_ids=['http://example.org/node-kind-iri'], derived_ids=[], properties=[], comment='A class that derives its nodeKind from parent', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#IRI'), extensible=False)
+Class(_id='http://example.org/extensible-class', clsname='http_//example.org/extensible-class', parent_ids=['http://example.org/link-class'], derived_ids=[], properties=[Property(path='http://example.org/extensible-class/required', varname='required', comment='A required string', max_count=1, min_count=1, enum_id='', class_id='', datatype='http://www.w3.org/2001/XMLSchema#string', pattern='')], comment='An extensible class', id_property=None, node_kind=rdflib.term.URIRef('http://www.w3.org/ns/shacl#BlankNodeOrIRI'), extensible=True)
```

### Comparing `shacl2code-0.0.8/.gitignore` & `shacl2code-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/LICENSE` & `shacl2code-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/README.md` & `shacl2code-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/pyproject.toml` & `shacl2code-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shacl2code-0.0.8/PKG-INFO` & `shacl2code-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: shacl2code
-Version: 0.0.8
+Version: 0.0.9
 Summary: Convert SHACL model file to code bindings
 Project-URL: Homepage, https://github.com/JPEWdev/shacl2code
 Project-URL: Repository, https://github.com/JPEWdev/shacl2code.git
 Project-URL: Issues, https://github.com/JPEWdev/shacl2code/issues
 Author-email: Joshua Watt <JPEWhacker@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

