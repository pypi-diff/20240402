# Comparing `tmp/increff_runner-3.1.5-py3-none-any.whl.zip` & `tmp/increff_runner-3.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 13186 bytes, number of entries: 16
+Zip file size: 13191 bytes, number of entries: 16
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-05 05:14 increff_runner/__init__.py
 -rw-r--r--  2.0 unx     9762 b- defN 24-Mar-29 08:33 increff_runner/function.py
 -rw-r--r--  2.0 unx     4143 b- defN 24-Feb-22 04:41 increff_runner/commons/algo_block_downloader.py
 -rw-r--r--  2.0 unx     2812 b- defN 24-Mar-29 07:34 increff_runner/commons/callback_helper.py
 -rw-r--r--  2.0 unx      351 b- defN 24-Feb-15 07:21 increff_runner/commons/constants.py
 -rw-r--r--  2.0 unx     3385 b- defN 24-Mar-29 07:29 increff_runner/commons/db_helper.py
 -rw-r--r--  2.0 unx      905 b- defN 24-Feb-22 04:41 increff_runner/commons/db_service.py
 -rw-r--r--  2.0 unx      349 b- defN 24-Feb-22 10:18 increff_runner/commons/event_helper.py
 -rw-r--r--  2.0 unx     8278 b- defN 24-Mar-29 09:53 increff_runner/commons/graphdb_helper.py
--rw-r--r--  2.0 unx     4099 b- defN 24-Mar-29 09:42 increff_runner/commons/mse_helper.py
+-rw-r--r--  2.0 unx     4120 b- defN 24-Apr-02 04:29 increff_runner/commons/mse_helper.py
 -rw-r--r--  2.0 unx      687 b- defN 24-Feb-22 04:41 increff_runner/commons/setup.py
 -rw-r--r--  2.0 unx     2104 b- defN 24-Feb-22 04:41 increff_runner/commons/utils.py
--rw-r--r--  2.0 unx      612 b- defN 24-Mar-29 09:54 increff_runner-3.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-29 09:54 increff_runner-3.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-Mar-29 09:54 increff_runner-3.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1424 b- defN 24-Mar-29 09:54 increff_runner-3.1.5.dist-info/RECORD
-16 files, 39018 bytes uncompressed, 10792 bytes compressed:  72.3%
+-rw-r--r--  2.0 unx      612 b- defN 24-Apr-02 04:30 increff_runner-3.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 04:30 increff_runner-3.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-Apr-02 04:30 increff_runner-3.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1424 b- defN 24-Apr-02 04:30 increff_runner-3.1.6.dist-info/RECORD
+16 files, 39039 bytes uncompressed, 10797 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: increff_runner/commons/setup.py
 Comment: 
 
 Filename: increff_runner/commons/utils.py
 Comment: 
 
-Filename: increff_runner-3.1.5.dist-info/METADATA
+Filename: increff_runner-3.1.6.dist-info/METADATA
 Comment: 
 
-Filename: increff_runner-3.1.5.dist-info/WHEEL
+Filename: increff_runner-3.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: increff_runner-3.1.5.dist-info/top_level.txt
+Filename: increff_runner-3.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: increff_runner-3.1.5.dist-info/RECORD
+Filename: increff_runner-3.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## increff_runner/commons/mse_helper.py

```diff
@@ -47,15 +47,15 @@
     #     job["data"]["level"],
     # )
     # interim_task["status"] = "SUCCESS"
     change_status_of_task_node(job["data"]["algo_name"], job["data"]["task_id"], job["data"]["level"], "SUCCESS")
     
     # persist_value(INTERIM_TASK_TABLE, interim_task["id"], interim_task)
 
-    node = get_task_node(job["data"]["algo_name"],job["data"]["task_id"])
+    node = get_task_node(job["data"]["algo_name"],job["data"]["task_id"],job["data"]["level"])
     if(str(node['last_block'])=="1"):
         status = check_last_block_status(job["data"]["task_id"], job["data"]["algo_name"])
         if status:
             add_info_logs(job["id"], "All levels for the block are completed")
             send_subtask_success_callback(
                 master_url, job["data"]["task_id"], node['parent_task']
             )
```

## Comparing `increff_runner-3.1.5.dist-info/RECORD` & `increff_runner-3.1.6.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 increff_runner/commons/algo_block_downloader.py,sha256=JSZLYpIuWhybRD13sHPu_05X4KoeMApa5qELLkqA9R4,4143
 increff_runner/commons/callback_helper.py,sha256=p-lIfzW7HVV73Y9tqA4aBYPzx6QnWPqbAYHRvGNO41Q,2812
 increff_runner/commons/constants.py,sha256=dJRawPQQduTe1BqN6SrLYYpzI5bVqS6AbuYwj6Qa6is,351
 increff_runner/commons/db_helper.py,sha256=NW4PMZwRM4s636nFrvLOfj7VkarS8EOc2MsZg1YLg2Y,3385
 increff_runner/commons/db_service.py,sha256=5PtU_AQCwm5FVmRXjJprysNoIy_vKt06vN1IlnxuH-c,905
 increff_runner/commons/event_helper.py,sha256=MN1XR6yielNYXLbLxi3uuiDyXZ-lmVKszL9DOL4swBY,349
 increff_runner/commons/graphdb_helper.py,sha256=Uw4vWF2D4u9L5A2SGKVPw18fMfFuwY80Af1fpj1k6G0,8278
-increff_runner/commons/mse_helper.py,sha256=q6Q4VrCJqTcLYvWjmqKhHy3rDgejLeS-XZ5iIj4afZ8,4099
+increff_runner/commons/mse_helper.py,sha256=WMDGy9VQpnEu6QALY8Dcm3jeXgQWUtyGGBNCdIuav-s,4120
 increff_runner/commons/setup.py,sha256=iwg58X1DKaSP8hKlXLvH5OXSEW8N_UuRMDb2CocaAfY,687
 increff_runner/commons/utils.py,sha256=PUKWRMYzTTWK7pTK2S5DM0szru4zGmmVKfPpXhnmPUM,2104
-increff_runner-3.1.5.dist-info/METADATA,sha256=RInvZLHWhrmKOsJlza69_-LimCqh362kHW84PGhj0IU,612
-increff_runner-3.1.5.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-increff_runner-3.1.5.dist-info/top_level.txt,sha256=pL8Rxzd3TVe5jhZdPB1tmORoBiwmdtiDgfNAvJtCl1s,15
-increff_runner-3.1.5.dist-info/RECORD,,
+increff_runner-3.1.6.dist-info/METADATA,sha256=EXc68NGbpccZz581WVSmppO4mBSd9srUyNGhG3u4eI4,612
+increff_runner-3.1.6.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+increff_runner-3.1.6.dist-info/top_level.txt,sha256=pL8Rxzd3TVe5jhZdPB1tmORoBiwmdtiDgfNAvJtCl1s,15
+increff_runner-3.1.6.dist-info/RECORD,,
```

