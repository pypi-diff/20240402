# Comparing `tmp/oarepo-model-builder-nr-2.0.8.tar.gz` & `tmp/oarepo-model-builder-nr-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-nr-2.0.8.tar", last modified: Wed Jan 10 09:43:15 2024, max compression
+gzip compressed data, was "oarepo-model-builder-nr-2.0.9.tar", last modified: Thu Feb 29 06:42:25 2024, max compression
```

## Comparing `oarepo-model-builder-nr-2.0.8.tar` & `oarepo-model-builder-nr-2.0.9.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.506608 oarepo-model-builder-nr-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-10 09:40:26.000000 oarepo-model-builder-nr-2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-01-10 09:43:15.506608 oarepo-model-builder-nr-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-01-10 09:43:15.000000 oarepo-model-builder-nr-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.506608 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:40:26.000000 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-01-10 09:40:26.000000 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr/components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.506608 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 09:40:26.000000 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-01-10 09:43:15.000000 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr/models/nr_common_metadata_2.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17259 2024-01-10 09:43:15.000000 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr/models/nr_datatypes_2.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-01-10 09:43:15.000000 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr/models/nr_documents_2.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-10 09:43:15.000000 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 09:43:15.506608 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-01-10 09:43:15.000000 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-01-10 09:43:15.000000 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 09:43:15.000000 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-01-10 09:43:15.000000 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 09:43:15.000000 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-10 09:43:15.000000 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-10 09:43:15.000000 oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-10 09:40:26.000000 oarepo-model-builder-nr-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-01-10 09:43:15.506608 oarepo-model-builder-nr-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-10 09:40:26.000000 oarepo-model-builder-nr-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:25.061905 oarepo-model-builder-nr-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-29 06:39:09.000000 oarepo-model-builder-nr-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-02-29 06:42:25.061905 oarepo-model-builder-nr-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-02-29 06:42:24.000000 oarepo-model-builder-nr-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:25.061905 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-29 06:39:09.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr/components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:25.061905 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 06:39:09.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-02-29 06:42:24.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr/models/datacite_4.5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13897 2024-02-29 06:42:24.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr/models/datacite_datatypes_4.5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-02-29 06:42:24.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr/models/nr_common_metadata_2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-02-29 06:42:24.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr/models/nr_data_2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19500 2024-02-29 06:42:24.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr/models/nr_datatypes_2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-02-29 06:42:24.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr/models/nr_documents_2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-29 06:42:24.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 06:42:25.061905 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-02-29 06:42:25.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-29 06:42:25.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 06:42:25.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-29 06:42:25.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 06:42:25.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-29 06:42:25.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-29 06:42:25.000000 oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-29 06:39:09.000000 oarepo-model-builder-nr-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-29 06:42:25.061905 oarepo-model-builder-nr-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 06:39:09.000000 oarepo-model-builder-nr-2.0.9/setup.py
```

### Comparing `oarepo-model-builder-nr-2.0.8/PKG-INFO` & `oarepo-model-builder-nr-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-nr
-Version: 2.0.8
+Version: 2.0.9
 Summary: "A model builder plugin with Czech National Repository compatible metadata schema"
 Home-page: https://github.com/Narodni-repozitar/oarepo-model-builder-nr
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio Czech NR model builder
 Platform: any
```

### Comparing `oarepo-model-builder-nr-2.0.8/README.md` & `oarepo-model-builder-nr-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr/components.py` & `oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr/components.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr/models/nr_datatypes_2.0.yaml` & `oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr/models/nr_datatypes_2.0.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,88 @@
 # Copyright (c) 2022, 2023 NTK, CESNET
 #
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
-NRAuthorityIdentifier:
-  $id: NRAuthorityIdentifier
+NRPerson:
+  $id: NRPerson
+  properties:
+    nameType:
+      type: keyword
+      enum:
+        - Personal
+      label.cs: Typ
+      label.en: Type
+    fullName:
+      type: keyword
+      required: true
+      label.cs: Jméno autora
+      label.en: Author name
+      sample:
+        faker: name
+    givenName:
+      type: keyword
+    familyName:
+      type: keyword
+    authorityIdentifiers[]:
+      use: 'nr-datatypes#NRPersonIdentifier'
+    affiliations[]:
+      type: taxonomy
+      vocabulary-type: institutions
+      keys: [ id, title, props.ror ]
+      ui:
+        marshmallow:
+          class: nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema
+      marshmallow:
+        class: nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema
+      sample:
+        faker: company
+
+      #^uniqueItems: true
+      label.cs: Afiliace
+      label.en: Affiliation
+      hint.cs: Uveďte instituci/instituce, pod jejíž záštitou jste se na tvorbě objektu podíleli.
+  ui:
+    detail: nr_person
+    marshmallow:
+      class: nr_metadata.common.services.records.ui_schema_datatypes.NRPersonUISchema
+  marshmallow:
+    class: nr_metadata.common.services.records.schema_datatypes.NRPersonSchema
+
+
+NROrganization:
+  $id: NROrganization
+  properties:
+    nameType:
+      type: keyword
+      enum: 
+        - Organizational
+      sample: 
+        - Organizational
+      label.cs: Typ
+      label.en: Type
+    fullName:
+      type: keyword
+      required: true
+      label.cs: Jméno autora
+      label.en: Author name
+      sample:
+        faker: name
+    authorityIdentifiers[]:
+      use: 'nr-datatypes#NROrganizationIdentifier'
+      #^uniqueItems: true
+  ui:
+    detail: nr_organization
+    marshmallow:
+      class: nr_metadata.common.services.records.ui_schema_datatypes.NROrganizationUISchema
+  marshmallow:
+    class: nr_metadata.common.services.records.schema_datatypes.NROrganizationSchema
+
+NRPersonIdentifier:
+  $id: NRPersonIdentifier
   properties:
     identifier:
       type: keyword
       required: true
       sample:
         faker: isbn13
       i18n.key: identifier
@@ -21,78 +95,90 @@
         [
           orcid,
           scopusID,
           researcherID,
           czenasAutID,
           vedidk,
           institutionalID,
+          ISNI
+        ]
+      i18n.key: identifier_type
+      label.cs: Typ identifikátoru
+      label.en: Identifier type
+      hint.cs: |
+        Doporučujeme zadat alespoň jeden z typů identifikátorů.
+        Pokud potřebujete rozšířit nabídku typů identifikátorů, kontaktujte nás na support@narodni-repozitar.cz.
+      hint.en: |
+        We recommend providing at least one of the identifier types.
+        If you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.
+  ui:
+    detail: nr_person_identifier
+    marshmallow:
+      class: nr_metadata.ui_schema.identifiers.NRPersonIdentifierUISchema
+      generate: false
+  marshmallow:
+    class: nr_metadata.schema.identifiers.NRPersonIdentifierSchema
+    generate: false
+
+NROrganizationIdentifier:
+  $id: NROrganizationIdentifier
+  properties:
+    identifier:
+      type: keyword
+      required: true
+      sample:
+        faker: isbn13
+      i18n.key: identifier
+      label.cs: Identifikátor
+      label.en: Identifier
+    scheme:
+      type: keyword
+      required: true
+      enum:
+        [
           ISNI,
           ROR,
           ICO,
-          DOI,
+          DOI
         ]
       i18n.key: identifier_type
       label.cs: Typ identifikátoru
       label.en: Identifier type
       hint.cs: |
         Doporučujeme zadat alespoň jeden z typů identifikátorů.
         Pokud potřebujete rozšířit nabídku typů identifikátorů, kontaktujte nás na support@narodni-repozitar.cz.
       hint.en: |
         We recommend providing at least one of the identifier types.
         If you need to expand the range of identifier types, contact us at support@narodni-repozitar.cz.
   ui:
-    detail: nr_authority_identifier
+    detail: nr_organization_identifier
     marshmallow:
-      class: nr_metadata.ui_schema.identifiers.NRAuthorityIdentifierUISchema
+      class: nr_metadata.ui_schema.identifiers.NROrganizationIdentifierUISchema
       generate: false
   marshmallow:
-    class: nr_metadata.schema.identifiers.NRAuthorityIdentifierSchema
+    class: nr_metadata.schema.identifiers.NROrganizationIdentifierSchema
     generate: false
 
 NRAuthority:
   $id: NRAuthority
-  properties:
-    nameType:
-      type: keyword
-      enum: [Organizational, Personal]
-      sample: [Organizational, Personal]
-      label.cs: Typ
-      label.en: Type
-      hint.cs: Jako tvůrce je možné označit osobu nebo instituci.
-      hint.en: It is possible to designate a person or an institution as the creator/contributor.
-    fullName:
-      type: keyword
-      required: true
-      label.cs: Jméno autora
-      label.en: Author name
-      sample:
-        faker: name
-    authorityIdentifiers[]:
-      use: 'nr-datatypes#NRAuthorityIdentifier'
-      #^uniqueItems: true
-    affiliations[]:
-      ui:
-        marshmallow:
-          class: nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema
-      marshmallow:
-        class: nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema
-      sample:
-        faker: company
-      type: taxonomy
-      vocabulary-type: institutions
-      #^uniqueItems: true
-      label.cs: Afiliace
-      label.en: Affiliation
-      hint.cs: Uveďte instituci/instituce, pod jejíž záštitou jste se na tvorbě objektu podíleli.
+  schemas:
+    Personal:
+      use: 'nr-datatypes#NRPerson'
+    Organizational:
+      use: 'nr-datatypes#NROrganization'
+  type: polymorphic
+  discriminator: nameType
+  hint.cs: Jako tvůrce je možné označit osobu nebo instituci.
+  hint.en: It is possible to designate a person or an institution as the creator/contributor.
   ui:
     detail: nr_authority
     marshmallow:
-      class: nr_metadata.common.services.records.ui_schema_datatypes.NRAuthorityUIUISchema
+      class: nr_metadata.common.services.records.ui_schema_datatypes.NRAuthorityUISchema
   marshmallow:
-    class: nr_metadata.common.services.records.schema_datatypes.NRAuthoritySchema
+    class: nr_metadata.common.services.records.ui_schema_datatypes.NRAuthoritySchema
 
 NRObjectPID:
   $id: NRObjectPID
   label.cs: Identifikátor objektu
   label.en: Object identifier
   properties:
     identifier:
@@ -101,15 +187,15 @@
       sample:
         faker: isbn13
       label.cs: Identifikátor objektu
       label.en: Object identifier
     scheme:
       type: keyword
       required: true
-      enum: [DOI, Handle, ISBN, ISSN, RIV]
+      enum: [DOI, Handle, ISBN, ISSN, RIV, IGSN]
       label.cs: Typ identifikátoru
       label.en: Identifier type
   ui:
     detail: nr_object_pid
     marshmallow:
       class: nr_metadata.ui_schema.identifiers.NRObjectIdentifierUISchema
       generate: false
@@ -168,25 +254,25 @@
   $id: NRLatitude
   type: double
   minimum: -90
   maximum: 90
   label.cs: Zeměpisná šířka
   label.en: Latitude
 
-NRAuthorityRole:
-  $id: NRAuthorityRole
+NRContributorType:
+  $id: NRContributorType
   type: vocabulary
-  vocabulary-type: contributor-roles
-  label.cs: Role přispěvatele
-  label.en: Contributor's role
+  vocabulary-type: contributor-types
+  label.cs: Typ přispěvatele
+  label.en: Contributor's type
   ui:
     marshmallow:
-      class: nr_metadata.common.services.records.ui_schema_datatypes.NRAuthorityRoleVocabularyUISchema
+      class: nr_metadata.common.services.records.ui_schema_datatypes.NRContributorTypeVocabularyUISchema
   marshmallow:
-    class: nr_metadata.common.services.records.schema_datatypes.NRAuthorityRoleVocabularySchema
+    class: nr_metadata.common.services.records.schema_datatypes.NRContributorTypeVocabularySchema
 
 NRRelatedItem:
   $id: NRRelatedItem
   label.cs: 'Vazba na/z dalších zdrojů:'
   label.en: 'Link to/from other resources:'
   description: linkdata, propojení přidružených dokumentů a datasetů.
   ui:
@@ -203,61 +289,55 @@
       type: fulltext
       required: true
 
     itemCreators[]:
       #^uniqueItems: true
       ^label.cs: Autoři
       ^label.en: Authors
-
       use: 'nr-datatypes#NRAuthority'
       ui:
         detail: creator
         marshmallow:
           class: nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemCreatorUISchema
       marshmallow:
         class: nr_metadata.common.services.records.schema_datatypes.NRRelatedItemCreatorSchema
-      properties:
-        affiliations[]:
-          ^label.cs: Afiliace
-          ^label.en: Affiliation
-
-          type: taxonomy
-          vocabulary-type: institutions
-          ui:
-            marshmallow:
-              class: nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema
-          marshmallow:
-            class: nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema
 
     itemContributors[]:
       #^uniqueItems: true
       ^label.cs: Přispěvatelé
       ^label.en: Contributors
 
       use: 'nr-datatypes#NRAuthority'
       ui:
         detail: contributor
         marshmallow:
           class: nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemContributorUISchema
       marshmallow:
         class: nr_metadata.common.services.records.schema_datatypes.NRRelatedItemContributorSchema
-      properties:
-        role:
-          use: 'nr-datatypes#NRAuthorityRole'
-        affiliations[]:
-          ^label.cs: Afiliace
-          ^label.en: Affiliation
-
-          type: taxonomy
-          vocabulary-type: institutions
+      schemas:
+        Personal:
           ui:
+            detail: nr_contributor_person
             marshmallow:
-              class: nr_metadata.common.services.records.ui_schema_datatypes.NRAffiliationVocabularyUISchema
+              class: nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemContributorPersonUISchema
           marshmallow:
-            class: nr_metadata.common.services.records.schema_datatypes.NRAffiliationVocabularySchema
+            class: nr_metadata.common.services.records.schema_datatypes.NRRelatedItemContributorPersonSchema
+          properties:
+            contributorType:
+              use: 'nr-datatypes#NRContributorType'
+        Organizational:
+          ui:
+            detail: nr_contributor_organization
+            marshmallow:
+              class: nr_metadata.common.services.records.ui_schema_datatypes.NRRelatedItemContributorOrganizationUISchema
+          marshmallow:
+            class: nr_metadata.common.services.records.schema_datatypes.NRRelatedItemContributorOrganizationSchema
+          properties:
+            contributorType:
+              use: 'nr-datatypes#NRContributorType'
 
     itemPIDs[]:
       use: 'nr-datatypes#NRObjectPID'
       #^uniqueItems: true
 
     itemURL:
       type: url
@@ -424,15 +504,14 @@
       class: nr_metadata.common.services.records.ui_schema_datatypes.NRGeoLocationUISchema
   marshmallow:
     class: nr_metadata.common.services.records.schema_datatypes.NRGeoLocationSchema
   properties:
     geoLocationPlace:
       description: Free description of the location; ie. Atlantic Ocean
       type: keyword
-      required: true
     geoLocationPoint:
       properties:
         pointLongitude:
           use: 'nr-datatypes#NRLongitude'
           required: true
         pointLatitude:
           use: 'nr-datatypes#NRLatitude'
@@ -513,32 +592,33 @@
   label.en: Language
   ui:
     marshmallow:
       class: nr_metadata.common.services.records.ui_schema_datatypes.NRLanguageVocabularyUISchema
   marshmallow:
     class: nr_metadata.common.services.records.schema_datatypes.NRLanguageVocabularySchema
 
-NRLicense:
-  $id: NRLicense
+NRRights:
+  $id: NRRights
+
   type: vocabulary
-  vocabulary-type: licenses
+  vocabulary-type: rights
   sample:
     - 'CC BY'
     - 'CC BY-SA'
     - 'CC BY-NC'
     - 'CC BY-ND'
     - 'CC BY-NC-SA'
     - 'CC BY-NC-ND'
-  label.cs: Licence
-  label.en: License
+  label.cs: Práva/Licence
+  label.en: Rights/Licenses
   ui:
     marshmallow:
-      class: nr_metadata.common.services.records.ui_schema_datatypes.NRLicenseVocabularyUISchema
+      class: nr_metadata.common.services.records.ui_schema_datatypes.NRRightsVocabularyUISchema
   marshmallow:
-    class: nr_metadata.common.services.records.schema_datatypes.NRLicenseVocabularySchema
+    class: nr_metadata.common.services.records.schema_datatypes.NRRightsVocabularySchema
 
 NRAccessRights:
   $id: NRAccessRights
   type: vocabulary
   vocabulary-type: access-rights
   sample: [open, embargoed, restricted, 'metadata only']
   label.cs: Přístupová práva
@@ -547,15 +627,15 @@
     marshmallow:
       class: nr_metadata.common.services.records.ui_schema_datatypes.NRAccessRightsVocabularyUISchema
   marshmallow:
     class: nr_metadata.common.services.records.schema_datatypes.NRAccessRightsVocabularySchema
 
 NRSeries:
   $id: NRSeries
-  label.cs: Série
+  label.cs: Edice
   label.en: Series
   # edice; tématicky sdružuje podobné věci, nemusí se jednat o pravou edici,
   # ale tagování/grupování podobných záznamů
   ui:
     detail: series
     marshmallow:
       class: nr_metadata.common.services.records.ui_schema_datatypes.NRSeriesUISchema
@@ -595,8 +675,8 @@
         faker: url
       label.cs: Externí umístění zdroje
       label.en: Resource external location
 
     externalLocationNote:
       type: fulltext
       label.cs: Poznámka
-      label.en: Note
+      label.en: Note
```

### Comparing `oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr.egg-info/PKG-INFO` & `oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-nr
-Version: 2.0.8
+Version: 2.0.9
 Summary: "A model builder plugin with Czech National Repository compatible metadata schema"
 Home-page: https://github.com/Narodni-repozitar/oarepo-model-builder-nr
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio Czech NR model builder
 Platform: any
```

### Comparing `oarepo-model-builder-nr-2.0.8/oarepo_model_builder_nr.egg-info/SOURCES.txt` & `oarepo-model-builder-nr-2.0.9/oarepo_model_builder_nr.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,10 +10,13 @@
 oarepo_model_builder_nr.egg-info/SOURCES.txt
 oarepo_model_builder_nr.egg-info/dependency_links.txt
 oarepo_model_builder_nr.egg-info/entry_points.txt
 oarepo_model_builder_nr.egg-info/not-zip-safe
 oarepo_model_builder_nr.egg-info/requires.txt
 oarepo_model_builder_nr.egg-info/top_level.txt
 oarepo_model_builder_nr/models/__init__.py
+oarepo_model_builder_nr/models/datacite_4.5.yaml
+oarepo_model_builder_nr/models/datacite_datatypes_4.5.yaml
 oarepo_model_builder_nr/models/nr_common_metadata_2.0.yaml
+oarepo_model_builder_nr/models/nr_data_2.0.yaml
 oarepo_model_builder_nr/models/nr_datatypes_2.0.yaml
 oarepo_model_builder_nr/models/nr_documents_2.0.yaml
```

### Comparing `oarepo-model-builder-nr-2.0.8/setup.cfg` & `oarepo-model-builder-nr-2.0.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 	pytest
 
 [options.entry_points]
 oarepo.models = 
 	nr-datatypes = oarepo_model_builder_nr.models:nr_datatypes_2.0.yaml
 	nr-common-metadata = oarepo_model_builder_nr.models:nr_common_metadata_2.0.yaml
 	nr-documents = oarepo_model_builder_nr.models:nr_documents_2.0.yaml
+	datacite = oarepo_model_builder_nr.models:datacite_4.5.yaml
+	datacite-datatypes = oarepo_model_builder_nr.models:datacite_datatypes_4.5.yaml
 oarepo_model_builder.datatypes.components = 
 	0100-nr-datatypes = oarepo_model_builder_nr.components:COMPONENTS
 
 [build_sphinx]
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
```

