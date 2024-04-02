# Comparing `tmp/tree_sitter_earthfile-0.1.2-cp38-abi3-win_amd64.whl.zip` & `tmp/tree_sitter_earthfile-0.2.1-cp38-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 107902 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-25 08:21 tree_sitter_earthfile/__init__.py
--rw-rw-rw-  2.0 fat       27 b- defN 24-Mar-25 08:21 tree_sitter_earthfile/__init__.pyi
--rw-rw-rw-  2.0 fat   565248 b- defN 24-Mar-25 08:24 tree_sitter_earthfile/_binding.pyd
--rw-rw-rw-  2.0 fat      642 b- defN 24-Mar-25 08:21 tree_sitter_earthfile/binding.c
--rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-25 08:21 tree_sitter_earthfile/py.typed
--rw-rw-rw-  2.0 fat     1932 b- defN 24-Mar-25 08:21 tree_sitter_earthfile/queries/highlights.scm
--rw-rw-rw-  2.0 fat      234 b- defN 24-Mar-25 08:21 tree_sitter_earthfile/queries/injections.scm
--rw-rw-rw-  2.0 fat     1072 b- defN 24-Mar-25 08:24 tree_sitter_earthfile-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      987 b- defN 24-Mar-25 08:24 tree_sitter_earthfile-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Mar-25 08:24 tree_sitter_earthfile-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       31 b- defN 24-Mar-25 08:23 tree_sitter_earthfile-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1098 b- defN 24-Mar-25 08:24 tree_sitter_earthfile-0.1.2.dist-info/RECORD
-12 files, 571463 bytes uncompressed, 106010 bytes compressed:  81.4%
+Zip file size: 105721 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 15:22 tree_sitter_earthfile/__init__.py
+-rw-rw-rw-  2.0 fat       27 b- defN 24-Apr-02 15:22 tree_sitter_earthfile/__init__.pyi
+-rw-rw-rw-  2.0 fat   526848 b- defN 24-Apr-02 15:25 tree_sitter_earthfile/_binding.pyd
+-rw-rw-rw-  2.0 fat      642 b- defN 24-Apr-02 15:22 tree_sitter_earthfile/binding.c
+-rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-02 15:22 tree_sitter_earthfile/py.typed
+-rw-rw-rw-  2.0 fat     2096 b- defN 24-Apr-02 15:22 tree_sitter_earthfile/queries/highlights.scm
+-rw-rw-rw-  2.0 fat      271 b- defN 24-Apr-02 15:22 tree_sitter_earthfile/queries/injections.scm
+-rw-rw-rw-  2.0 fat     1072 b- defN 24-Apr-02 15:25 tree_sitter_earthfile-0.2.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      987 b- defN 24-Apr-02 15:25 tree_sitter_earthfile-0.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-02 15:25 tree_sitter_earthfile-0.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       31 b- defN 24-Apr-02 15:24 tree_sitter_earthfile-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1098 b- defN 24-Apr-02 15:25 tree_sitter_earthfile-0.2.1.dist-info/RECORD
+12 files, 533264 bytes uncompressed, 103829 bytes compressed:  80.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tree_sitter_earthfile/queries/highlights.scm
 Comment: 
 
 Filename: tree_sitter_earthfile/queries/injections.scm
 Comment: 
 
-Filename: tree_sitter_earthfile-0.1.2.dist-info/LICENSE
+Filename: tree_sitter_earthfile-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: tree_sitter_earthfile-0.1.2.dist-info/METADATA
+Filename: tree_sitter_earthfile-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: tree_sitter_earthfile-0.1.2.dist-info/WHEEL
+Filename: tree_sitter_earthfile-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: tree_sitter_earthfile-0.1.2.dist-info/top_level.txt
+Filename: tree_sitter_earthfile-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: tree_sitter_earthfile-0.1.2.dist-info/RECORD
+Filename: tree_sitter_earthfile-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tree_sitter_earthfile/queries/highlights.scm

```diff
@@ -25,52 +25,50 @@
 (set_command "SET" @keyword)
 (user_command "USER" @keyword)
 (version_command "VERSION" @keyword)
 (volume_command "VOLUME" @keyword)
 (with_docker_command "WITH DOCKER" @keyword)
 (workdir_command "WORKDIR" @keyword)
 
-(for_command ["FOR" "IN" "END"] @keyword.control)
-(if_command ["IF" "ELSE" "ELSE IF" "END"] @keyword.control)
-(import_command ["IMPORT" "AS"] @keyword.control)
-(try_command ["TRY" "FINALLY" "END"] @keyword.control)
+(for_command ["FOR" "IN" "END"] @keyword.control.repeat)
+(if_command ["IF" "END"] @keyword.control.conditional)
+(elif_block ["ELSE IF"] @keyword.control.conditional)
+(else_block ["ELSE"] @keyword.control.conditional)
+(import_command ["IMPORT" "AS"] @keyword.control.import)
+(try_command ["TRY" "FINALLY" "END"] @keyword.control.exception)
+(wait_command ["WAIT" "END"] @keyword.control)
 
 
 [
     (comment)
     (line_continuation_comment)
 ] @comment
 
 (line_continuation) @operator
 
-(function_ref) @function
-
 [
     (target_ref)
     (target_artifact)
-    (image_spec)
-] @module
+    (function_ref)
+] @function
 
-(target (identifier) @module)
+(target (identifier) @function)
 
 [
-  (double_quoted_string)
-  (single_quoted_string)
+    (double_quoted_string)
+    (single_quoted_string)
 ] @string
 (unquoted_string) @string.special
 (escape_sequence) @string.escape
 
 (variable) @variable
 (expansion ["$" "{" "}" "(" ")"] @punctuation.special)
 (build_arg) @variable
+(options (_) @variable.parameter)
 
-[
-    option: (_)
-] @type
-
-option: (_ "=" @operator)
+(options (_ "=" @operator))
 (build_arg "=" @operator)
 (arg_command "=" @operator)
 (env_command "=" @operator)
 (label "=" @operator)
 (set_command "=" @operator)
 (let_command "=" @operator)
```

## tree_sitter_earthfile/queries/injections.scm

```diff
@@ -1,8 +1,9 @@
 ((comment) @injection.content
   (#set! injection.language "comment"))
 
 ((line_continuation_comment) @injection.content
   (#set! injection.language "comment"))
 
 ((shell_fragment) @injection.content
-  (#set! injection.language "bash"))
+  (#set! injection.language "bash")
+  (#set! injection.include-children))
```

## Comparing `tree_sitter_earthfile-0.1.2.dist-info/LICENSE` & `tree_sitter_earthfile-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tree_sitter_earthfile-0.1.2.dist-info/METADATA` & `tree_sitter_earthfile-0.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-sitter-earthfile
-Version: 0.1.2
+Version: 0.2.1
 Summary: Earthfile grammar for tree-sitter
 License: MIT
 Project-URL: Homepage, https://github.com/tree-sitter/tree-sitter-earthfile
 Keywords: incremental,parsing,tree-sitter,earthfile
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Compilers
```

