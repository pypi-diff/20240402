# Comparing `tmp/sssom-schema-0.9.3.tar.gz` & `tmp/sssom-schema-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sssom-schema-0.9.3.tar", max compression
+gzip compressed data, was "sssom-schema-0.9.4.tar", max compression
```

## Comparing `sssom-schema-0.9.3.tar` & `sssom-schema-0.9.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1523 2022-06-09 20:49:09.853059 sssom-schema-0.9.3/LICENSE
--rw-r--r--   0        0        0     6755 2022-06-09 20:49:09.853059 sssom-schema-0.9.3/README.md
--rw-r--r--   0        0        0      579 2022-06-09 20:50:31.973934 sssom-schema-0.9.3/pyproject.toml
--rw-r--r--   0        0        0       37 2022-06-09 20:49:09.861059 sssom-schema-0.9.3/src/sssom_schema/__init__.py
--rw-r--r--   0        0        0        0 2022-06-09 20:49:09.861059 sssom-schema-0.9.3/src/sssom_schema/datamodel/__init__.py
--rw-r--r--   0        0        0    40519 2022-06-09 20:49:09.861059 sssom-schema-0.9.3/src/sssom_schema/datamodel/sssom_schema.py
--rw-r--r--   0        0        0    21401 2022-06-09 20:49:09.861059 sssom-schema-0.9.3/src/sssom_schema/schema/sssom_schema.yaml
--rw-r--r--   0        0        0     7629 2022-06-09 20:50:33.109680 sssom-schema-0.9.3/setup.py
--rw-r--r--   0        0        0     7356 2022-06-09 20:50:33.110480 sssom-schema-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1523 2022-06-20 10:42:01.034533 sssom-schema-0.9.4/LICENSE
+-rw-r--r--   0        0        0     6828 2022-06-20 10:42:01.034533 sssom-schema-0.9.4/README.md
+-rw-r--r--   0        0        0      579 2022-06-20 10:43:07.071432 sssom-schema-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0       37 2022-06-20 10:42:01.038533 sssom-schema-0.9.4/src/sssom_schema/__init__.py
+-rw-r--r--   0        0        0        0 2022-06-20 10:42:01.038533 sssom-schema-0.9.4/src/sssom_schema/datamodel/__init__.py
+-rw-r--r--   0        0        0    40519 2022-06-20 10:42:01.038533 sssom-schema-0.9.4/src/sssom_schema/datamodel/sssom_schema.py
+-rw-r--r--   0        0        0    21386 2022-06-20 10:42:01.038533 sssom-schema-0.9.4/src/sssom_schema/schema/sssom_schema.yaml
+-rw-r--r--   0        0        0     7702 2022-06-20 10:43:07.957501 sssom-schema-0.9.4/setup.py
+-rw-r--r--   0        0        0     7429 2022-06-20 10:43:07.958177 sssom-schema-0.9.4/PKG-INFO
```

### Comparing `sssom-schema-0.9.3/LICENSE` & `sssom-schema-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sssom-schema-0.9.3/README.md` & `sssom-schema-0.9.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 
 1. a TSV-based representation for ontology term mappings
 1. a comprehensive set of standard metadata elements to describe mappings and 
 1. a standard translation between the TSV and the Web Ontology Language (OWL). 
 
 The SSSOM TSV format in particular is geared towards the needs of the wider bioinformatics community as a way to safely exchange mappings in an easily readable yet semantically well-specified manner. Consider this example of a simple mapping file:
 
-| subject_id	| predicate_id	| object_id	| match_type | subject_label	| object_label |
+| subject_id	| predicate_id	| object_id	| mapping_justification | subject_label	| object_label |
 | --- | --- | --- | --- | --- | --- |
-| HP:0009124	| skos:exactMatch	| MP:0000003	| Lexical	| Abnormal adipose tissue morphology	| abnormal adipose tissue morphology |
-| HP:0008551	| skos:exactMatch	| MP:0000018	| Lexical	| Microtia	| small ears |
-| HP:0000411	| skos:exactMatch	| MP:0000021	| Lexical	| Protruding ear	| prominent ears |
+| HP:0009124	| skos:exactMatch	| MP:0000003	| semapv:LexicalMatching	| Abnormal adipose tissue morphology	| abnormal adipose tissue morphology |
+| HP:0008551	| skos:exactMatch	| MP:0000018	| semapv:LexicalMatching	| Microtia	| small ears |
+| HP:0000411	| skos:exactMatch	| MP:0000021	| semapv:LexicalMatching	| Protruding ear	| prominent ears |
 
 SSSOM specifies all its metadata elements:
 
 - subject_id
 - predicate_id
 - object_id
-- match_type (*NOTE June 2022*: `match_type` is being replaced by `mapping_justification` see [here](https://github.com/mapping-commons/sssom/issues/150))
+- mapping_justification (*NOTE: Since June 2022* `match_type` is being replaced by `mapping_justification` see [here](https://github.com/mapping-commons/sssom/issues/150))
 - subject_label
 - object_label
 
 including clear definitions, examples of use and controlled vocabulary where necessary, along with 30 other optional metadata elements to provide additional provenance.
 
 SSSOM further provides a standard way to 
 - augment the TSV file with mapping set - level metadata, such as creator_id, mapping_date or license and
```

### Comparing `sssom-schema-0.9.3/pyproject.toml` & `sssom-schema-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sssom-schema"
-version = "0.9.3"
+version = "0.9.4"
 description = "SSSOM is a Simple Standard for Sharing Ontology Mappings."
 readme = "README.md"
 authors = [
     "Nicolas Matentzoglu <nicolas.matentzoglu@gmail.com>",
     "Harshad Hegde <hhegde@lbl.gov>"
     ]
 license = "MIT"
```

### Comparing `sssom-schema-0.9.3/src/sssom_schema/datamodel/sssom_schema.py` & `sssom-schema-0.9.4/src/sssom_schema/datamodel/sssom_schema.py`

 * *Files identical despite different names*

### Comparing `sssom-schema-0.9.3/src/sssom_schema/schema/sssom_schema.yaml` & `sssom-schema-0.9.4/src/sssom_schema/schema/sssom_schema.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         description: The subject and the object are sufficiently similar that they can be used interchangeably in some information retrieval applications.
       - value: skos:exactMatch
         description: The subject and the object can, with a high degree of confidence, be used interchangeably across a wide range of information retrieval applications.
       - value: skos:narrowMatch
         description: "From the SKOS primer: A triple skos:narrower (and skos:narrowMatch) asserts that , the object of the triple, is a narrower concept than , the subject of the triple."
       - value: skos:broadMatch
         description: "From the SKOS primer: A triple skos:broader (and skos:broadMatch) asserts that , the object of the triple, is a broader concept than , the subject of the triple."
-      - value: oboInOwl:database_cross_reference
+      - value: oboInOwl:hasDbXref
         description: Two terms are related in some way. The meaning is frequently consistent across a single set of mappings. Note this property is often overloaded even where the terms are of a different nature (e.g. interpro2go)
       - value: rdfs:seeAlso
         description: The subject and the object are associated in some unspecified way. The object IRI often resolves to a resource on the web that provides additional information.
   predicate_type:
     description: The type of entity that is being mapped.
     range: entity_type_enum
     examples:
```

### Comparing `sssom-schema-0.9.3/setup.py` & `sssom-schema-0.9.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 {'': ['*'], 'sssom_schema': ['schema/*']}
 
 install_requires = \
 ['linkml-runtime>=1.1.24,<2.0.0']
 
 setup_kwargs = {
     'name': 'sssom-schema',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'SSSOM is a Simple Standard for Sharing Ontology Mappings.',
-    'long_description': '<!--[![DOI](https://zenodo.org/badge/13996/mapping-commons/sssom.svg)](https://zenodo.org/badge/latestdoi/13996/mapping-commons/sssom)-->\n\n# A Simple Standard for Sharing Ontological Mappings (SSSOM)\n\n<img src="https://github.com/jmcmurry/closed-illustrations/raw/master/logos/sssom-logos/sssom_logo_black-banner.png" />\n\n\nSSSOM is a Simple Standard for Sharing Ontological Mappings, providing \n\n1. a TSV-based representation for ontology term mappings\n1. a comprehensive set of standard metadata elements to describe mappings and \n1. a standard translation between the TSV and the Web Ontology Language (OWL). \n\nThe SSSOM TSV format in particular is geared towards the needs of the wider bioinformatics community as a way to safely exchange mappings in an easily readable yet semantically well-specified manner. Consider this example of a simple mapping file:\n\n| subject_id\t| predicate_id\t| object_id\t| match_type | subject_label\t| object_label |\n| --- | --- | --- | --- | --- | --- |\n| HP:0009124\t| skos:exactMatch\t| MP:0000003\t| Lexical\t| Abnormal adipose tissue morphology\t| abnormal adipose tissue morphology |\n| HP:0008551\t| skos:exactMatch\t| MP:0000018\t| Lexical\t| Microtia\t| small ears |\n| HP:0000411\t| skos:exactMatch\t| MP:0000021\t| Lexical\t| Protruding ear\t| prominent ears |\n\nSSSOM specifies all its metadata elements:\n\n- subject_id\n- predicate_id\n- object_id\n- match_type (*NOTE June 2022*: `match_type` is being replaced by `mapping_justification` see [here](https://github.com/mapping-commons/sssom/issues/150))\n- subject_label\n- object_label\n\nincluding clear definitions, examples of use and controlled vocabulary where necessary, along with 30 other optional metadata elements to provide additional provenance.\n\nSSSOM further provides a standard way to \n- augment the TSV file with mapping set - level metadata, such as creator_id, mapping_date or license and\n- translate a SSSOM compliant TSV files into _OWL reified axioms_. This will allow the easy loading, and merging of SSSOM mapping tables into existing ontologies using standard tools such as ROBOT (under development).\n\nNote that SSSOM is currently under development and subject to change. Please leave us a comment on the [issue tracker](https://github.com/OBOFoundry/SSSOM/issues) if you want to be involved. The full specification can be found [here](https://w3id.org/sssom/spec).\n\n## Citation\n\nIf you have found SSSOM to be helpful in your work, please consider citing:\n\nNicolas Matentzoglu, James P Balhoff, Susan M Bello, Chris Bizon, Matthew Brush, Tiffany J Callahan, Christopher G Chute, William D Duncan, Chris T Evelo, Davera Gabriel, John Graybeal, Alasdair Gray, Benjamin M Gyori, Melissa Haendel, Henriette Harmse, Nomi L Harris, Ian Harrow, Harshad B Hegde, Amelia L Hoyt, Charles T Hoyt, Dazhi Jiao, Ernesto Jiménez-Ruiz, Simon Jupp, Hyeongsik Kim, Sebastian Koehler, Thomas Liener, Qinqin Long, James Malone, James A McLaughlin, Julie A McMurry, Sierra Moxon, Monica C Munoz-Torres, David Osumi-Sutherland, James A Overton, Bjoern Peters, Tim Putman, Núria Queralt-Rosinach, Kent Shefchek, Harold Solbrig, Anne Thessen, Tania Tudorache, Nicole Vasilevsky, Alex H Wagner, Christopher J Mungall, A Simple Standard for Sharing Ontological Mappings (SSSOM), Database, Volume 2022, 2022, baac035, https://doi.org/10.1093/database/baac035\n\n```bibtex\n@article{10.1093/database/baac035,\n    author = {Matentzoglu, Nicolas and Balhoff, James P and Bello, Susan M and Bizon, Chris and Brush, Matthew and Callahan, Tiffany J and Chute, Christopher G and Duncan, William D and Evelo, Chris T and Gabriel, Davera and Graybeal, John and Gray, Alasdair and Gyori, Benjamin M and Haendel, Melissa and Harmse, Henriette and Harris, Nomi L and Harrow, Ian and Hegde, Harshad B and Hoyt, Amelia L and Hoyt, Charles T and Jiao, Dazhi and Jiménez-Ruiz, Ernesto and Jupp, Simon and Kim, Hyeongsik and Koehler, Sebastian and Liener, Thomas and Long, Qinqin and Malone, James and McLaughlin, James A and McMurry, Julie A and Moxon, Sierra and Munoz-Torres, Monica C and Osumi-Sutherland, David and Overton, James A and Peters, Bjoern and Putman, Tim and Queralt-Rosinach, Núria and Shefchek, Kent and Solbrig, Harold and Thessen, Anne and Tudorache, Tania and Vasilevsky, Nicole and Wagner, Alex H and Mungall, Christopher J},\n    title = "{A Simple Standard for Sharing Ontological Mappings (SSSOM)}",\n    journal = {Database},\n    volume = {2022},\n    year = {2022},\n    month = {05},\n    abstract = "{Despite progress in the development of standards for describing and exchanging scientific information, the lack of easy-to-use standards for mapping between different representations of the same or similar objects in different databases poses a major impediment to data integration and interoperability. Mappings often lack the metadata needed to be correctly interpreted and applied. For example, are two terms equivalent or merely related? Are they narrow or broad matches? Or are they associated in some other way? Such relationships between the mapped terms are often not documented, which leads to incorrect assumptions and makes them hard to use in scenarios that require a high degree of precision (such as diagnostics or risk prediction). Furthermore, the lack of descriptions of how mappings were done makes it hard to combine and reconcile mappings, particularly curated and automated ones. We have developed the Simple Standard for Sharing Ontological Mappings (SSSOM) which addresses these problems by: (i) Introducing a machine-readable and extensible vocabulary to describe metadata that makes imprecision, inaccuracy and incompleteness in mappings explicit. (ii) Defining an easy-to-use simple table-based format that can be integrated into existing data science pipelines without the need to parse or query ontologies, and that integrates seamlessly with Linked Data principles. (iii) Implementing open and community-driven collaborative workflows that are designed to evolve the standard continuously to address changing requirements and mapping practices. (iv) Providing reference tools and software libraries for working with the standard. In this paper, we present the SSSOM standard, describe several use cases in detail and survey some of the existing work on standardizing the exchange of mappings, with the goal of making mappings Findable, Accessible, Interoperable and Reusable (FAIR). The SSSOM specification can be found at http://w3id.org/sssom/spec.Database URL: http://w3id.org/sssom/spec}",\n    issn = {1758-0463},\n    doi = {10.1093/database/baac035},\n    url = {https://doi.org/10.1093/database/baac035},\n    note = {baac035},\n    eprint = {https://academic.oup.com/database/article-pdf/doi/10.1093/database/baac035/43832024/baac035.pdf},\n}\n```\n',
+    'long_description': '<!--[![DOI](https://zenodo.org/badge/13996/mapping-commons/sssom.svg)](https://zenodo.org/badge/latestdoi/13996/mapping-commons/sssom)-->\n\n# A Simple Standard for Sharing Ontological Mappings (SSSOM)\n\n<img src="https://github.com/jmcmurry/closed-illustrations/raw/master/logos/sssom-logos/sssom_logo_black-banner.png" />\n\n\nSSSOM is a Simple Standard for Sharing Ontological Mappings, providing \n\n1. a TSV-based representation for ontology term mappings\n1. a comprehensive set of standard metadata elements to describe mappings and \n1. a standard translation between the TSV and the Web Ontology Language (OWL). \n\nThe SSSOM TSV format in particular is geared towards the needs of the wider bioinformatics community as a way to safely exchange mappings in an easily readable yet semantically well-specified manner. Consider this example of a simple mapping file:\n\n| subject_id\t| predicate_id\t| object_id\t| mapping_justification | subject_label\t| object_label |\n| --- | --- | --- | --- | --- | --- |\n| HP:0009124\t| skos:exactMatch\t| MP:0000003\t| semapv:LexicalMatching\t| Abnormal adipose tissue morphology\t| abnormal adipose tissue morphology |\n| HP:0008551\t| skos:exactMatch\t| MP:0000018\t| semapv:LexicalMatching\t| Microtia\t| small ears |\n| HP:0000411\t| skos:exactMatch\t| MP:0000021\t| semapv:LexicalMatching\t| Protruding ear\t| prominent ears |\n\nSSSOM specifies all its metadata elements:\n\n- subject_id\n- predicate_id\n- object_id\n- mapping_justification (*NOTE: Since June 2022* `match_type` is being replaced by `mapping_justification` see [here](https://github.com/mapping-commons/sssom/issues/150))\n- subject_label\n- object_label\n\nincluding clear definitions, examples of use and controlled vocabulary where necessary, along with 30 other optional metadata elements to provide additional provenance.\n\nSSSOM further provides a standard way to \n- augment the TSV file with mapping set - level metadata, such as creator_id, mapping_date or license and\n- translate a SSSOM compliant TSV files into _OWL reified axioms_. This will allow the easy loading, and merging of SSSOM mapping tables into existing ontologies using standard tools such as ROBOT (under development).\n\nNote that SSSOM is currently under development and subject to change. Please leave us a comment on the [issue tracker](https://github.com/OBOFoundry/SSSOM/issues) if you want to be involved. The full specification can be found [here](https://w3id.org/sssom/spec).\n\n## Citation\n\nIf you have found SSSOM to be helpful in your work, please consider citing:\n\nNicolas Matentzoglu, James P Balhoff, Susan M Bello, Chris Bizon, Matthew Brush, Tiffany J Callahan, Christopher G Chute, William D Duncan, Chris T Evelo, Davera Gabriel, John Graybeal, Alasdair Gray, Benjamin M Gyori, Melissa Haendel, Henriette Harmse, Nomi L Harris, Ian Harrow, Harshad B Hegde, Amelia L Hoyt, Charles T Hoyt, Dazhi Jiao, Ernesto Jiménez-Ruiz, Simon Jupp, Hyeongsik Kim, Sebastian Koehler, Thomas Liener, Qinqin Long, James Malone, James A McLaughlin, Julie A McMurry, Sierra Moxon, Monica C Munoz-Torres, David Osumi-Sutherland, James A Overton, Bjoern Peters, Tim Putman, Núria Queralt-Rosinach, Kent Shefchek, Harold Solbrig, Anne Thessen, Tania Tudorache, Nicole Vasilevsky, Alex H Wagner, Christopher J Mungall, A Simple Standard for Sharing Ontological Mappings (SSSOM), Database, Volume 2022, 2022, baac035, https://doi.org/10.1093/database/baac035\n\n```bibtex\n@article{10.1093/database/baac035,\n    author = {Matentzoglu, Nicolas and Balhoff, James P and Bello, Susan M and Bizon, Chris and Brush, Matthew and Callahan, Tiffany J and Chute, Christopher G and Duncan, William D and Evelo, Chris T and Gabriel, Davera and Graybeal, John and Gray, Alasdair and Gyori, Benjamin M and Haendel, Melissa and Harmse, Henriette and Harris, Nomi L and Harrow, Ian and Hegde, Harshad B and Hoyt, Amelia L and Hoyt, Charles T and Jiao, Dazhi and Jiménez-Ruiz, Ernesto and Jupp, Simon and Kim, Hyeongsik and Koehler, Sebastian and Liener, Thomas and Long, Qinqin and Malone, James and McLaughlin, James A and McMurry, Julie A and Moxon, Sierra and Munoz-Torres, Monica C and Osumi-Sutherland, David and Overton, James A and Peters, Bjoern and Putman, Tim and Queralt-Rosinach, Núria and Shefchek, Kent and Solbrig, Harold and Thessen, Anne and Tudorache, Tania and Vasilevsky, Nicole and Wagner, Alex H and Mungall, Christopher J},\n    title = "{A Simple Standard for Sharing Ontological Mappings (SSSOM)}",\n    journal = {Database},\n    volume = {2022},\n    year = {2022},\n    month = {05},\n    abstract = "{Despite progress in the development of standards for describing and exchanging scientific information, the lack of easy-to-use standards for mapping between different representations of the same or similar objects in different databases poses a major impediment to data integration and interoperability. Mappings often lack the metadata needed to be correctly interpreted and applied. For example, are two terms equivalent or merely related? Are they narrow or broad matches? Or are they associated in some other way? Such relationships between the mapped terms are often not documented, which leads to incorrect assumptions and makes them hard to use in scenarios that require a high degree of precision (such as diagnostics or risk prediction). Furthermore, the lack of descriptions of how mappings were done makes it hard to combine and reconcile mappings, particularly curated and automated ones. We have developed the Simple Standard for Sharing Ontological Mappings (SSSOM) which addresses these problems by: (i) Introducing a machine-readable and extensible vocabulary to describe metadata that makes imprecision, inaccuracy and incompleteness in mappings explicit. (ii) Defining an easy-to-use simple table-based format that can be integrated into existing data science pipelines without the need to parse or query ontologies, and that integrates seamlessly with Linked Data principles. (iii) Implementing open and community-driven collaborative workflows that are designed to evolve the standard continuously to address changing requirements and mapping practices. (iv) Providing reference tools and software libraries for working with the standard. In this paper, we present the SSSOM standard, describe several use cases in detail and survey some of the existing work on standardizing the exchange of mappings, with the goal of making mappings Findable, Accessible, Interoperable and Reusable (FAIR). The SSSOM specification can be found at http://w3id.org/sssom/spec.Database URL: http://w3id.org/sssom/spec}",\n    issn = {1758-0463},\n    doi = {10.1093/database/baac035},\n    url = {https://doi.org/10.1093/database/baac035},\n    note = {baac035},\n    eprint = {https://academic.oup.com/database/article-pdf/doi/10.1093/database/baac035/43832024/baac035.pdf},\n}\n```\n',
     'author': 'Nicolas Matentzoglu',
     'author_email': 'nicolas.matentzoglu@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `sssom-schema-0.9.3/PKG-INFO` & `sssom-schema-0.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sssom-schema
-Version: 0.9.3
+Version: 0.9.4
 Summary: SSSOM is a Simple Standard for Sharing Ontology Mappings.
 License: MIT
 Author: Nicolas Matentzoglu
 Author-email: nicolas.matentzoglu@gmail.com
 Requires-Python: >=3.7.6,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -26,26 +26,26 @@
 
 1. a TSV-based representation for ontology term mappings
 1. a comprehensive set of standard metadata elements to describe mappings and 
 1. a standard translation between the TSV and the Web Ontology Language (OWL). 
 
 The SSSOM TSV format in particular is geared towards the needs of the wider bioinformatics community as a way to safely exchange mappings in an easily readable yet semantically well-specified manner. Consider this example of a simple mapping file:
 
-| subject_id	| predicate_id	| object_id	| match_type | subject_label	| object_label |
+| subject_id	| predicate_id	| object_id	| mapping_justification | subject_label	| object_label |
 | --- | --- | --- | --- | --- | --- |
-| HP:0009124	| skos:exactMatch	| MP:0000003	| Lexical	| Abnormal adipose tissue morphology	| abnormal adipose tissue morphology |
-| HP:0008551	| skos:exactMatch	| MP:0000018	| Lexical	| Microtia	| small ears |
-| HP:0000411	| skos:exactMatch	| MP:0000021	| Lexical	| Protruding ear	| prominent ears |
+| HP:0009124	| skos:exactMatch	| MP:0000003	| semapv:LexicalMatching	| Abnormal adipose tissue morphology	| abnormal adipose tissue morphology |
+| HP:0008551	| skos:exactMatch	| MP:0000018	| semapv:LexicalMatching	| Microtia	| small ears |
+| HP:0000411	| skos:exactMatch	| MP:0000021	| semapv:LexicalMatching	| Protruding ear	| prominent ears |
 
 SSSOM specifies all its metadata elements:
 
 - subject_id
 - predicate_id
 - object_id
-- match_type (*NOTE June 2022*: `match_type` is being replaced by `mapping_justification` see [here](https://github.com/mapping-commons/sssom/issues/150))
+- mapping_justification (*NOTE: Since June 2022* `match_type` is being replaced by `mapping_justification` see [here](https://github.com/mapping-commons/sssom/issues/150))
 - subject_label
 - object_label
 
 including clear definitions, examples of use and controlled vocabulary where necessary, along with 30 other optional metadata elements to provide additional provenance.
 
 SSSOM further provides a standard way to 
 - augment the TSV file with mapping set - level metadata, such as creator_id, mapping_date or license and
```

