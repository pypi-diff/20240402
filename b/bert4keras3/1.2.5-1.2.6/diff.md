# Comparing `tmp/bert4keras3-1.2.5-py3-none-any.whl.zip` & `tmp/bert4keras3-1.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 59559 bytes, number of entries: 12
+Zip file size: 59590 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      150 b- defN 24-Mar-27 11:41 bert4keras3/__init__.py
 -rw-rw-rw-  2.0 fat    20229 b- defN 24-Mar-27 11:41 bert4keras3/backend.py
 -rw-rw-rw-  2.0 fat    52459 b- defN 24-Mar-27 14:03 bert4keras3/layers.py
--rw-rw-rw-  2.0 fat   123797 b- defN 24-Mar-27 14:04 bert4keras3/models.py
+-rw-rw-rw-  2.0 fat   123859 b- defN 24-Apr-02 12:31 bert4keras3/models.py
 -rw-rw-rw-  2.0 fat    30152 b- defN 24-Mar-27 11:41 bert4keras3/ops.py
 -rw-rw-rw-  2.0 fat    27955 b- defN 24-Mar-27 11:41 bert4keras3/snippets.py
 -rw-rw-rw-  2.0 fat    15509 b- defN 24-Mar-27 11:41 bert4keras3/tokenizers.py
--rw-rw-rw-  2.0 fat    11358 b- defN 24-Mar-27 14:09 bert4keras3-1.2.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      221 b- defN 24-Mar-27 14:09 bert4keras3-1.2.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-27 14:09 bert4keras3-1.2.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Mar-27 14:09 bert4keras3-1.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      964 b- defN 24-Mar-27 14:09 bert4keras3-1.2.5.dist-info/RECORD
-12 files, 282898 bytes uncompressed, 57961 bytes compressed:  79.5%
+-rw-rw-rw-  2.0 fat    11358 b- defN 24-Apr-02 12:32 bert4keras3-1.2.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      221 b- defN 24-Apr-02 12:32 bert4keras3-1.2.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 12:32 bert4keras3-1.2.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-02 12:32 bert4keras3-1.2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      964 b- defN 24-Apr-02 12:32 bert4keras3-1.2.6.dist-info/RECORD
+12 files, 282960 bytes uncompressed, 57992 bytes compressed:  79.5%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: bert4keras3/snippets.py
 Comment: 
 
 Filename: bert4keras3/tokenizers.py
 Comment: 
 
-Filename: bert4keras3-1.2.5.dist-info/LICENSE
+Filename: bert4keras3-1.2.6.dist-info/LICENSE
 Comment: 
 
-Filename: bert4keras3-1.2.5.dist-info/METADATA
+Filename: bert4keras3-1.2.6.dist-info/METADATA
 Comment: 
 
-Filename: bert4keras3-1.2.5.dist-info/WHEEL
+Filename: bert4keras3-1.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: bert4keras3-1.2.5.dist-info/top_level.txt
+Filename: bert4keras3-1.2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: bert4keras3-1.2.5.dist-info/RECORD
+Filename: bert4keras3-1.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bert4keras3/models.py

```diff
@@ -3488,14 +3488,15 @@
     transformer.build(**configs)
     if keras.__version__>'3.0':
         #keras3不知道为什么attention需要走一次前向才能初始化
         inputs=[]
         for modelin in transformer.model.inputs: 
             shape=keras.ops.shape(modelin)
             shape=[1 if t==None else t for t in shape]
+            shape[0] = len(keras.distribution.list_devices())
             inputs.append(np.zeros(shape,modelin.dtype))
         transformer.model.predict(inputs,verbose=3)
         if keras_weights_path is not None:
             transformer.model.load_weights(keras_weights_path, skip_mismatch=True)
         if lora_model:
             
             def enable_lora(t):
```

## Comparing `bert4keras3-1.2.5.dist-info/LICENSE` & `bert4keras3-1.2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bert4keras3-1.2.5.dist-info/RECORD` & `bert4keras3-1.2.6.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 bert4keras3/__init__.py,sha256=CMb8S8X82Zw-9GhxgUom0I8qs7veKePBxPqa7nStNpk,150
 bert4keras3/backend.py,sha256=6Z7XUI2vjPtrddejf0y2rCKQftucxxCf74jjwGPs1l0,20229
 bert4keras3/layers.py,sha256=PvlMvpDjIZaIgNSJ5gfzyTgoDyK5GhhonPqJhrb16d4,52459
-bert4keras3/models.py,sha256=HC6uDDNuBr9FxcyxA1EiBQEZ90WtLkERib1majhrtqc,123797
+bert4keras3/models.py,sha256=YXsCWUy2L1D8DO3sRUHfdxI8qIjT2jqeLyAeiJGjKEQ,123859
 bert4keras3/ops.py,sha256=H1sbMv6WOJ5iGAB0rosPz9LoqdT0jS8knLRW_6XkFRU,30152
 bert4keras3/snippets.py,sha256=YwdYRvrewhM6g8ax9_Ath0HsJATzuyZksL5Dow9l65A,27955
 bert4keras3/tokenizers.py,sha256=PCxtC4L9tF2w-GUDujdPK8Z5WlnbaL8mYhRfHn1S_Qg,15509
-bert4keras3-1.2.5.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-bert4keras3-1.2.5.dist-info/METADATA,sha256=DuauFeRJ8XeJW50DoBdhSxdUuvxdvzIwmng9n0T-fUs,221
-bert4keras3-1.2.5.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-bert4keras3-1.2.5.dist-info/top_level.txt,sha256=cPWwwxSejEMpgAZFzYQc0WmhPrF3XwP3k1IwRO93gwQ,12
-bert4keras3-1.2.5.dist-info/RECORD,,
+bert4keras3-1.2.6.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+bert4keras3-1.2.6.dist-info/METADATA,sha256=YlQq_Pb8x0xuyrq3oLzizwFEWSxb0AWCP2jR7zAePV0,221
+bert4keras3-1.2.6.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+bert4keras3-1.2.6.dist-info/top_level.txt,sha256=cPWwwxSejEMpgAZFzYQc0WmhPrF3XwP3k1IwRO93gwQ,12
+bert4keras3-1.2.6.dist-info/RECORD,,
```

