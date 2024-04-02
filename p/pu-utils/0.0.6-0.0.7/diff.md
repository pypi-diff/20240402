# Comparing `tmp/pu_utils-0.0.6-py3-none-any.whl.zip` & `tmp/pu_utils-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 18894 bytes, number of entries: 13
--rw-r--r--  2.0 unx    14068 b- defN 16-Jan-01 00:00 pu_utils-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 pu_utils-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx    11357 b- defN 16-Jan-01 00:00 pu_utils-0.0.6.dist-info/licenses/LICENSE
+Zip file size: 18925 bytes, number of entries: 13
+-rw-r--r--  2.0 unx    14068 b- defN 16-Jan-01 00:00 pu_utils-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 pu_utils-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx    11357 b- defN 16-Jan-01 00:00 pu_utils-0.0.7.dist-info/licenses/LICENSE
 -rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 pu_utils/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 pu_utils/aws/__init__.py
 -rw-r--r--  2.0 unx     5525 b- defN 16-Jan-01 00:00 pu_utils/aws/iam.py
 -rw-r--r--  2.0 unx     3944 b- defN 16-Jan-01 00:00 pu_utils/aws/iam_test.py
--rw-r--r--  2.0 unx    14710 b- defN 16-Jan-01 00:00 pu_utils/aws/lambda_.py
+-rw-r--r--  2.0 unx    14803 b- defN 16-Jan-01 00:00 pu_utils/aws/lambda_.py
 -rw-r--r--  2.0 unx     1609 b- defN 16-Jan-01 00:00 pu_utils/namer.py
 -rw-r--r--  2.0 unx     1437 b- defN 16-Jan-01 00:00 pu_utils/namer_test.py
 -rw-r--r--  2.0 unx     2754 b- defN 16-Jan-01 00:00 pu_utils/python_zip.py
 -rw-r--r--  2.0 unx     1773 b- defN 16-Jan-01 00:00 pu_utils/python_zip_test.py
-?rw-------  2.0 unx     1015 b- defN 16-Jan-01 00:00 pu_utils-0.0.6.dist-info/RECORD
-13 files, 58282 bytes uncompressed, 17218 bytes compressed:  70.5%
+?rw-------  2.0 unx     1015 b- defN 16-Jan-01 00:00 pu_utils-0.0.7.dist-info/RECORD
+13 files, 58375 bytes uncompressed, 17249 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
-Filename: pu_utils-0.0.6.dist-info/METADATA
+Filename: pu_utils-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: pu_utils-0.0.6.dist-info/WHEEL
+Filename: pu_utils-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: pu_utils-0.0.6.dist-info/licenses/LICENSE
+Filename: pu_utils-0.0.7.dist-info/licenses/LICENSE
 Comment: 
 
 Filename: pu_utils/__init__.py
 Comment: 
 
 Filename: pu_utils/aws/__init__.py
 Comment: 
@@ -30,11 +30,11 @@
 
 Filename: pu_utils/python_zip.py
 Comment: 
 
 Filename: pu_utils/python_zip_test.py
 Comment: 
 
-Filename: pu_utils-0.0.6.dist-info/RECORD
+Filename: pu_utils-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pu_utils/aws/lambda_.py

```diff
@@ -386,14 +386,16 @@
         self._execution_role = self._create_execution_role(
             name,
             role_name=namer.role(name),
             policies=[
                 policy_factory.lambda_log_policy(self.function_name),
                 policy_factory.lambda_vpc_policy(),
                 policy_factory.ssm_params_policy(),
+                # For decrypting SSM parameters
+                policy_factory.kms_policy(),
                 *(policies or []),
             ],
         )
         self._function = self._create_function(
             name,
             image_uri=image_uri,
             function_name=self.function_name,
```

## Comparing `pu_utils-0.0.6.dist-info/METADATA` & `pu_utils-0.0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pu-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Random stuff to help writing Pulumi scripts easier
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

## Comparing `pu_utils-0.0.6.dist-info/licenses/LICENSE` & `pu_utils-0.0.7.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `pu_utils-0.0.6.dist-info/RECORD` & `pu_utils-0.0.7.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-pu_utils-0.0.6.dist-info/METADATA,sha256=NEl1OXaYUKOrHVr7DSBliBrmkc4Jh_QHeII3_9MEXnw,14068
-pu_utils-0.0.6.dist-info/WHEEL,sha256=N2J68yzZqJh3mI_Wg92rwhw0rtJDFpZj9bwQIMJgaVg,90
-pu_utils-0.0.6.dist-info/licenses/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pu_utils-0.0.7.dist-info/METADATA,sha256=vckrpddv9r9F_2nysC-_yb5vD6-4Ng2HjE4j0ICKelQ,14068
+pu_utils-0.0.7.dist-info/WHEEL,sha256=N2J68yzZqJh3mI_Wg92rwhw0rtJDFpZj9bwQIMJgaVg,90
+pu_utils-0.0.7.dist-info/licenses/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
 pu_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pu_utils/aws/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pu_utils/aws/iam.py,sha256=xWMQ2mmYd73uRg5JBO8MFSQcivcmD2c-5I4fDZi2ucY,5525
 pu_utils/aws/iam_test.py,sha256=LNP-cegreyGK0osrVF1FDOdivByFuTukkKsIxt_SPM4,3944
-pu_utils/aws/lambda_.py,sha256=tfYwj3rlkfOYGmitywfWqXCT2uV-AZqIJShiXicZsfg,14710
+pu_utils/aws/lambda_.py,sha256=JLG0qitabpc-lR-cW8xvEXeucbCjh8cxuYC4bcdgWrM,14803
 pu_utils/namer.py,sha256=7Xo0eNtTBq3z1187yV4O7gcRnRTMsI0NiZ1QCDMNWqo,1609
 pu_utils/namer_test.py,sha256=rZ_hSe4Gz5lqtR9I5zYDdf7cohFlID2hmtMr88Lvva8,1437
 pu_utils/python_zip.py,sha256=VB1sHYsz1S28iYt9sjrUpjEkoiiX8HW7IzIFoe9SFog,2754
 pu_utils/python_zip_test.py,sha256=9iEiYI2zCHi3-sEVtF9Kws5kA7oGCdgpHS-Gntz-23Y,1773
-pu_utils-0.0.6.dist-info/RECORD,,
+pu_utils-0.0.7.dist-info/RECORD,,
```

