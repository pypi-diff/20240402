# Comparing `tmp/rg3py-0.0.2-py3-none-win_amd64.whl.zip` & `tmp/rg3py-0.0.3-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7917839 bytes, number of entries: 7
--rw-r--r--  2.0 unx      713 b- defN 24-Mar-16 12:41 rg3py/__init__.py
--rw-r--r--  2.0 unx 20483584 b- defN 24-Mar-16 12:41 rg3py/rg3py.pyd
--rw-r--r--  2.0 unx     8298 b- defN 24-Mar-16 12:41 rg3py/rg3py.pyi
--rw-r--r--  2.0 unx     2973 b- defN 24-Mar-16 12:41 rg3py-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       98 b- defN 24-Mar-16 12:41 rg3py-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Mar-16 12:41 rg3py-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      510 b- defN 24-Mar-16 12:41 rg3py-0.0.2.dist-info/RECORD
-7 files, 20496182 bytes uncompressed, 7916951 bytes compressed:  61.4%
+Zip file size: 7949670 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      916 b- defN 24-Apr-02 19:25 rg3py/__init__.py
+-rw-r--r--  2.0 unx 20607488 b- defN 24-Apr-02 19:26 rg3py/rg3py.pyd
+-rw-r--r--  2.0 unx     8063 b- defN 24-Apr-02 19:26 rg3py/rg3py.pyi
+-rw-r--r--  2.0 unx     4821 b- defN 24-Apr-02 19:26 rg3py-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 24-Apr-02 19:26 rg3py-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-02 19:26 rg3py-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      510 b- defN 24-Apr-02 19:26 rg3py-0.0.3.dist-info/RECORD
+7 files, 20621902 bytes uncompressed, 7948782 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: rg3py/rg3py.pyd
 Comment: 
 
 Filename: rg3py/rg3py.pyi
 Comment: 
 
-Filename: rg3py-0.0.2.dist-info/METADATA
+Filename: rg3py-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: rg3py-0.0.2.dist-info/WHEEL
+Filename: rg3py-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: rg3py-0.0.2.dist-info/top_level.txt
+Filename: rg3py-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: rg3py-0.0.2.dist-info/RECORD
+Filename: rg3py-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rg3py/__init__.py

```diff
@@ -1,22 +1,28 @@
 from .rg3py import CppStandard
+from .rg3py import InheritanceVisibility
 from .rg3py import CppEnumEntry
 from .rg3py import CppTypeKind
 from .rg3py import CppEnum
+from .rg3py import CppAlias
 from .rg3py import CppIncludeKind
 from .rg3py import CppIncludeInfo
 from .rg3py import Location
 from .rg3py import CppNamespace
 from .rg3py import TagArgumentType
 from .rg3py import TagArgument
 from .rg3py import Tag
 from .rg3py import Tags
 from .rg3py import CppBaseType
 from .rg3py import CppClassEntryVisibillity
+from .rg3py import TypeStatement
+from .rg3py import FunctionArgument
 from .rg3py import CppClassFunction
 from .rg3py import CppClassProperty
+from .rg3py import ClassParent
 from .rg3py import CppClass
 from .rg3py import CodeAnalyzer
+from .rg3py import AnalyzerContext
 from .rg3py import CppCompilerIssueKind
 from .rg3py import CppCompilerIssue
 from .rg3py import CppTypeReference
-from .rg3py import ClangRuntime
+from .rg3py import ClangRuntime
```

## rg3py/rg3py.pyi

```diff
@@ -29,40 +29,26 @@
 
 
 class CppTypeKind:
     TK_NONE = 0
     TK_TRIVIAL = 1
     TK_ENUM = 2
     TK_STRUCT_OR_CLASS = 3
-    TK_ALIAS = 4
-    TK_TEMPLATE_SPECIALIZATION = 5
-
 
 class CppEnum:
     @property
     def entries(self) -> List[CppEnumEntry]: ...
 
     @property
     def is_scoped(self) -> bool: ...
 
     @property
     def underlying_type(self) -> str: ...
 
 
-class CppAlias:
-    @property
-    def target(self) -> CppTypeReference: ...
-
-    @property
-    def target_location(self) -> Optional[Location]: ...
-
-    @property
-    def target_description(self) -> TypeStatement: ...
-
-
 class CppIncludeKind:
     IK_PROJECT = 0
     IK_SYSTEM = 1
     IK_SYSROOT = 2
     IK_THIRD_PARTY = 3
     IK_DEFAULT = IK_PROJECT
 
@@ -85,14 +71,17 @@
 
     @property
     def line(self) -> int: ...
 
     @property
     def column(self) -> int: ...
 
+    @property
+    def angled(self) -> bool: ...
+
 
 class CppNamespace:
     def __eq__(self, other) -> bool: ...
     def __ne__(self, other) -> bool: ...
     def __str__(self) -> str: ...
     def __repr__(self) -> str: ...
```

