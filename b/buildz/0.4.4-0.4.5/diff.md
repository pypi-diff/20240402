# Comparing `tmp/buildz-0.4.4.tar.gz` & `tmp/buildz-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.4.4.tar", last modified: Mon Apr  1 13:52:43 2024, max compression
+gzip compressed data, was "buildz-0.4.5.tar", last modified: Mon Apr  1 17:54:19 2024, max compression
```

## Comparing `buildz-0.4.4.tar` & `buildz-0.4.5.tar`

### file list

```diff
@@ -1,143 +1,172 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.719395 buildz-0.4.4/
--rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.4.4/LICENSE
--rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5750 2024-04-01 13:52:43.719395 buildz-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     5335 2023-10-16 14:40:02.000000 buildz-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.294190 buildz-0.4.4/buildz/
--rw-rw-rw-   0        0        0       81 2024-04-01 13:50:26.000000 buildz-0.4.4/buildz/__init__.py
--rw-rw-rw-   0        0        0     1165 2024-04-01 13:42:56.000000 buildz-0.4.4/buildz/argx.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.238638 buildz-0.4.4/buildz/demo/
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.309809 buildz-0.4.4/buildz/demo/ioc/
--rw-rw-rw-   0        0        0      964 2024-04-01 13:51:18.000000 buildz-0.4.4/buildz/demo/ioc/test.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.325412 buildz-0.4.4/buildz/demo/ioc/test_conf/
--rw-rw-rw-   0        0        0      573 2024-03-30 10:09:18.000000 buildz-0.4.4/buildz/demo/ioc/test_conf/base.js
--rw-rw-rw-   0        0        0     1328 2024-04-01 11:15:14.000000 buildz-0.4.4/buildz/demo/ioc/test_conf/data1.js
--rw-rw-rw-   0        0        0      398 2024-03-31 08:55:33.000000 buildz-0.4.4/buildz/demo/ioc/test_conf/data2.js
--rw-rw-rw-   0        0        0      362 2024-03-30 15:22:31.000000 buildz-0.4.4/buildz/demo/ioc/test_conf/data3.js
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.325412 buildz-0.4.4/buildz/demo/xf/
--rw-rw-rw-   0        0        0      162 2024-04-01 11:24:41.000000 buildz-0.4.4/buildz/demo/xf/test.js
--rw-rw-rw-   0        0        0      251 2024-04-01 12:36:42.000000 buildz-0.4.4/buildz/demo/xf/test.py
--rw-rw-rw-   0        0        0        0 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/dj.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.341064 buildz-0.4.4/buildz/ioc/
--rw-rw-rw-   0        0        0       40 2024-03-31 10:20:19.000000 buildz-0.4.4/buildz/ioc/__init__.py
--rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.4.4/buildz/ioc/init.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.356691 buildz-0.4.4/buildz/ioc/ioc/
--rw-rw-rw-   0        0        0      971 2024-03-31 09:07:56.000000 buildz-0.4.4/buildz/ioc/ioc/base.py
--rw-rw-rw-   0        0        0     4266 2024-03-31 10:19:09.000000 buildz-0.4.4/buildz/ioc/ioc/conf.py
--rw-rw-rw-   0        0        0     9786 2024-03-31 08:54:57.000000 buildz-0.4.4/buildz/ioc/ioc/confs.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.404564 buildz-0.4.4/buildz/ioc/ioc_deal/
--rw-rw-rw-   0        0        0     4522 2024-03-31 09:45:12.000000 buildz-0.4.4/buildz/ioc/ioc_deal/base.py
--rw-rw-rw-   0        0        0     1128 2024-03-31 09:56:22.000000 buildz-0.4.4/buildz/ioc/ioc_deal/call.py
--rw-rw-rw-   0        0        0      936 2024-03-31 10:45:14.000000 buildz-0.4.4/buildz/ioc/ioc_deal/calls.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.419600 buildz-0.4.4/buildz/ioc/ioc_deal/conf/
--rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/call_defaults.js
--rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/call_lists.js
--rw-rw-rw-   0        0        0       19 2024-03-31 10:41:23.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/calls_defaults.js
--rw-rw-rw-   0        0        0      376 2024-03-31 10:41:10.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/calls_lists.js
--rw-rw-rw-   0        0        0     1089 2024-04-01 11:12:34.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/deals.js
--rw-rw-rw-   0        0        0      307 2024-03-31 09:29:07.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/env_lists.js
--rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/ioc_lists.js
--rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/mcall_defaults.js
--rw-rw-rw-   0        0        0      476 2024-03-31 09:44:23.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/mcall_lists.js
--rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
--rw-rw-rw-   0        0        0       94 2024-03-31 03:42:49.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/obj_defaults.js
--rw-rw-rw-   0        0        0      626 2024-03-31 09:33:20.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/obj_lists.js
--rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/obj_set_lists.js
--rw-rw-rw-   0        0        0      411 2024-03-31 10:04:44.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/ovar_lists.js
--rw-rw-rw-   0        0        0      416 2024-03-31 07:52:50.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/ref_lists.js
--rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.4.4/buildz/ioc/ioc_deal/conf/var_lists.js
--rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.4.4/buildz/ioc/ioc_deal/demo.py
--rw-rw-rw-   0        0        0      524 2024-03-31 09:08:42.000000 buildz-0.4.4/buildz/ioc/ioc_deal/env.py
--rw-rw-rw-   0        0        0      606 2024-04-01 11:11:54.000000 buildz-0.4.4/buildz/ioc/ioc_deal/ioc.py
--rw-rw-rw-   0        0        0     1487 2024-03-31 10:48:09.000000 buildz-0.4.4/buildz/ioc/ioc_deal/mcall.py
--rw-rw-rw-   0        0        0     2861 2024-03-31 10:00:11.000000 buildz-0.4.4/buildz/ioc/ioc_deal/obj.py
--rw-rw-rw-   0        0        0     1096 2024-03-31 10:05:27.000000 buildz-0.4.4/buildz/ioc/ioc_deal/ovar.py
--rw-rw-rw-   0        0        0      536 2024-03-31 09:09:01.000000 buildz-0.4.4/buildz/ioc/ioc_deal/ref.py
--rw-rw-rw-   0        0        0      279 2024-03-31 07:26:16.000000 buildz-0.4.4/buildz/ioc/ioc_deal/val.py
--rw-rw-rw-   0        0        0      823 2024-03-31 10:07:06.000000 buildz-0.4.4/buildz/ioc/ioc_deal/var.py
--rw-rw-rw-   0        0        0     5405 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/keys.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.450893 buildz-0.4.4/buildz/old_version/
--rw-rw-rw-   0        0        0     1055 2024-04-01 11:19:41.000000 buildz-0.4.4/buildz/old_version/__init__.py
--rw-rw-rw-   0        0        0      344 2024-04-01 11:19:32.000000 buildz-0.4.4/buildz/old_version/__main__.py
--rw-rw-rw-   0        0        0     1775 2024-02-28 03:15:25.000000 buildz-0.4.4/buildz/old_version/base.py
--rw-rw-rw-   0        0        0     7859 2024-04-01 11:19:19.000000 buildz-0.4.4/buildz/old_version/build.py
--rw-rw-rw-   0        0        0    10964 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/confz.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.242235 buildz-0.4.4/buildz/old_version/demo/
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.513811 buildz-0.4.4/buildz/old_version/demo/x/
--rw-rw-rw-   0        0        0      546 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/demo.confz
--rw-rw-rw-   0        0        0      522 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/demo.py
--rw-rw-rw-   0        0        0      476 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/run.confz
--rw-rw-rw-   0        0        0      464 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/test.confz
--rw-rw-rw-   0        0        0      217 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/test.py
--rw-rw-rw-   0        0        0      240 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/testc.py
--rw-rw-rw-   0        0        0      780 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/testf.py
--rw-rw-rw-   0        0        0     1197 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/testz.py
--rw-rw-rw-   0        0        0      375 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/value.confz
--rw-rw-rw-   0        0        0      174 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/demo/x/x.py
--rw-rw-rw-   0        0        0     5405 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/keys.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.593439 buildz-0.4.4/buildz/old_version/xconfz/
--rw-rw-rw-   0        0        0      524 2024-04-01 11:20:18.000000 buildz-0.4.4/buildz/old_version/xconfz/__init__.py
--rw-rw-rw-   0        0        0     6026 2024-04-01 11:20:26.000000 buildz-0.4.4/buildz/old_version/xconfz/base.py
--rw-rw-rw-   0        0        0     1675 2024-04-01 11:20:36.000000 buildz-0.4.4/buildz/old_version/xconfz/buff.py
--rw-rw-rw-   0        0        0      156 2024-04-01 11:21:03.000000 buildz-0.4.4/buildz/old_version/xconfz/fc.py
--rw-rw-rw-   0        0        0     2281 2024-04-01 11:20:44.000000 buildz-0.4.4/buildz/old_version/xconfz/fc_item.py
--rw-rw-rw-   0        0        0     2678 2024-04-01 11:20:47.000000 buildz-0.4.4/buildz/old_version/xconfz/fc_list.py
--rw-rw-rw-   0        0        0     3017 2024-04-01 11:20:50.000000 buildz-0.4.4/buildz/old_version/xconfz/fc_map.py
--rw-rw-rw-   0        0        0     1778 2024-04-01 11:20:53.000000 buildz-0.4.4/buildz/old_version/xconfz/fc_set.py
--rw-rw-rw-   0        0        0     2887 2024-04-01 11:20:56.000000 buildz-0.4.4/buildz/old_version/xconfz/fc_str.py
--rw-rw-rw-   0        0        0     2823 2024-04-01 11:20:59.000000 buildz-0.4.4/buildz/old_version/xconfz/fc_type.py
--rw-rw-rw-   0        0        0      841 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/old_version/xconfz/file.py
--rw-rw-rw-   0        0        0     4018 2024-04-01 11:21:08.000000 buildz-0.4.4/buildz/old_version/xconfz/fmt_base.py
--rw-rw-rw-   0        0        0     1322 2024-04-01 11:21:16.000000 buildz-0.4.4/buildz/old_version/xconfz/fmt_str.py
--rw-rw-rw-   0        0        0     2069 2024-04-01 11:21:20.000000 buildz-0.4.4/buildz/old_version/xconfz/fmt_type.py
--rw-rw-rw-   0        0        0     4326 2024-04-01 11:21:30.000000 buildz-0.4.4/buildz/old_version/xconfz/mg.py
--rw-rw-rw-   0        0        0     4186 2024-04-01 11:21:23.000000 buildz-0.4.4/buildz/old_version/xconfz/mg_fmt.py
--rw-rw-rw-   0        0        0     1112 2024-03-31 02:32:18.000000 buildz-0.4.4/buildz/pyz.py
--rw-rw-rw-   0        0        0     1750 2024-02-22 17:23:17.000000 buildz-0.4.4/buildz/test_loader copy.py
--rw-rw-rw-   0        0        0      336 2024-03-01 16:45:49.000000 buildz-0.4.4/buildz/test_loader.py
--rw-rw-rw-   0        0        0      658 2024-03-01 16:51:21.000000 buildz-0.4.4/buildz/test_writer.py
--rw-rw-rw-   0        0        0      843 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.624698 buildz-0.4.4/buildz/xf/
--rw-rw-rw-   0        0        0      139 2024-04-01 13:46:42.000000 buildz-0.4.4/buildz/xf/__init__.py
--rw-rw-rw-   0        0        0      841 2023-10-16 14:40:02.000000 buildz-0.4.4/buildz/xf/file.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.646804 buildz-0.4.4/buildz/xf/loader/
--rw-rw-rw-   0        0        0     1696 2024-03-01 16:40:46.000000 buildz-0.4.4/buildz/xf/loader/base.py
--rw-rw-rw-   0        0        0     2456 2024-02-22 16:50:58.000000 buildz-0.4.4/buildz/xf/loader/buffer.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.688145 buildz-0.4.4/buildz/xf/loader/deal/
--rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.4.4/buildz/xf/loader/deal/listz.py
--rw-rw-rw-   0        0        0     2619 2024-03-31 10:34:46.000000 buildz-0.4.4/buildz/xf/loader/deal/lr.py
--rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.4.4/buildz/xf/loader/deal/lrval.py
--rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.4.4/buildz/xf/loader/deal/mapz.py
--rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.4.4/buildz/xf/loader/deal/nextz.py
--rw-rw-rw-   0        0        0     1156 2024-03-01 16:45:20.000000 buildz-0.4.4/buildz/xf/loader/deal/reval.py
--rw-rw-rw-   0        0        0     1134 2024-02-22 13:17:44.000000 buildz-0.4.4/buildz/xf/loader/deal/setz.py
--rw-rw-rw-   0        0        0      390 2024-02-22 17:15:53.000000 buildz-0.4.4/buildz/xf/loader/deal/spc.py
--rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.4.4/buildz/xf/loader/deal/spt.py
--rw-rw-rw-   0        0        0     2806 2024-03-21 08:07:18.000000 buildz-0.4.4/buildz/xf/loader/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.4.4/buildz/xf/loader/exp.py
--rw-rw-rw-   0        0        0     1490 2024-02-22 16:35:35.000000 buildz-0.4.4/buildz/xf/loader/item.py
--rw-rw-rw-   0        0        0     1693 2024-02-22 16:18:29.000000 buildz-0.4.4/buildz/xf/loader/mg.py
--rw-rw-rw-   0        0        0     1339 2024-02-22 12:37:04.000000 buildz-0.4.4/buildz/xf/loader/pos.py
--rw-rw-rw-   0        0        0     1093 2024-03-31 03:05:04.000000 buildz-0.4.4/buildz/xf/mapz.py
--rw-rw-rw-   0        0        0     2385 2024-03-06 07:06:32.000000 buildz-0.4.4/buildz/xf/read.py
--rw-rw-rw-   0        0        0     1314 2024-02-24 09:19:50.000000 buildz-0.4.4/buildz/xf/test_write.py
--rw-rw-rw-   0        0        0     1203 2024-03-01 16:51:07.000000 buildz-0.4.4/buildz/xf/write.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.703801 buildz-0.4.4/buildz/xf/writer/
--rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.4.4/buildz/xf/writer/base.py
--rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.4.4/buildz/xf/writer/conf.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.719395 buildz-0.4.4/buildz/xf/writer/deal/
--rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.4.4/buildz/xf/writer/deal/jsonval.py
--rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.4.4/buildz/xf/writer/deal/listz.py
--rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.4.4/buildz/xf/writer/deal/mapz.py
--rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.4.4/buildz/xf/writer/deal/reval.py
--rw-rw-rw-   0        0        0     1377 2024-02-24 09:43:55.000000 buildz-0.4.4/buildz/xf/writer/deal/strz.py
--rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.4.4/buildz/xf/writer/itemz.py
--rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.4.4/buildz/xf/writer/mg.py
--rw-rw-rw-   0        0        0      509 2024-04-01 13:44:50.000000 buildz-0.4.4/buildz/xf/xargs.py
-drwxrwxrwx   0        0        0        0 2024-04-01 13:52:43.309809 buildz-0.4.4/buildz.egg-info/
--rw-rw-rw-   0        0        0     5750 2024-04-01 13:52:43.000000 buildz-0.4.4/buildz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3546 2024-04-01 13:52:43.000000 buildz-0.4.4/buildz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 13:52:43.000000 buildz-0.4.4/buildz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-01 13:52:43.000000 buildz-0.4.4/buildz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 13:52:43.719395 buildz-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      770 2024-04-01 11:15:48.000000 buildz-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.361896 buildz-0.4.5/
+-rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     5750 2024-04-01 17:54:19.361896 buildz-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5335 2023-10-16 14:40:02.000000 buildz-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.235931 buildz-0.4.5/buildz/
+-rw-rw-rw-   0        0        0      139 2024-04-01 15:22:30.000000 buildz-0.4.5/buildz/__init__.py
+-rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.4.5/buildz/__main__.py
+-rw-rw-rw-   0        0        0     1382 2024-04-01 16:58:33.000000 buildz-0.4.5/buildz/argx.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.252353 buildz-0.4.5/buildz/demo/
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.252353 buildz-0.4.5/buildz/demo/ioc/
+-rw-rw-rw-   0        0        0      482 2024-04-01 17:50:54.000000 buildz-0.4.5/buildz/demo/ioc/deal.py
+-rw-rw-rw-   0        0        0      132 2024-04-01 16:27:59.000000 buildz-0.4.5/buildz/demo/ioc/help.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.262541 buildz-0.4.5/buildz/demo/res/
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.262541 buildz-0.4.5/buildz/demo/res/conf/
+-rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.4.5/buildz/demo/res/conf/ioc.js
+-rw-rw-rw-   0        0        0     1601 2024-04-01 16:39:00.000000 buildz-0.4.5/buildz/demo/res/conf/main.js
+-rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.4.5/buildz/demo/res/conf/xf.js
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.265403 buildz-0.4.5/buildz/demo/res/help/
+-rw-rw-rw-   0        0        0      100 2024-04-01 16:29:54.000000 buildz-0.4.5/buildz/demo/res/help/default.js
+-rw-rw-rw-   0        0        0     3083 2024-04-01 17:51:58.000000 buildz-0.4.5/buildz/demo/res/help/ioc.js
+-rw-rw-rw-   0        0        0     1039 2024-04-01 17:28:35.000000 buildz-0.4.5/buildz/demo/res/help/xf.js
+-rw-rw-rw-   0        0        0      282 2024-04-01 16:32:30.000000 buildz-0.4.5/buildz/demo/res/test.js
+-rw-rw-rw-   0        0        0     1098 2024-04-01 16:47:51.000000 buildz-0.4.5/buildz/demo/test.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.269075 buildz-0.4.5/buildz/demo/xf/
+-rw-rw-rw-   0        0        0      362 2024-04-01 16:41:35.000000 buildz-0.4.5/buildz/demo/xf/deal.py
+-rw-rw-rw-   0        0        0      140 2024-04-01 16:27:54.000000 buildz-0.4.5/buildz/demo/xf/help.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.220306 buildz-0.4.5/buildz/demos/
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.269075 buildz-0.4.5/buildz/demos/ioc/
+-rw-rw-rw-   0        0        0      964 2024-04-01 13:51:18.000000 buildz-0.4.5/buildz/demos/ioc/test.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.269075 buildz-0.4.5/buildz/demos/ioc/test_conf/
+-rw-rw-rw-   0        0        0      573 2024-03-30 10:09:18.000000 buildz-0.4.5/buildz/demos/ioc/test_conf/base.js
+-rw-rw-rw-   0        0        0     1329 2024-04-01 16:05:37.000000 buildz-0.4.5/buildz/demos/ioc/test_conf/data1.js
+-rw-rw-rw-   0        0        0      398 2024-03-31 08:55:33.000000 buildz-0.4.5/buildz/demos/ioc/test_conf/data2.js
+-rw-rw-rw-   0        0        0      362 2024-03-30 15:22:31.000000 buildz-0.4.5/buildz/demos/ioc/test_conf/data3.js
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.283078 buildz-0.4.5/buildz/demos/xf/
+-rw-rw-rw-   0        0        0      162 2024-04-01 11:24:41.000000 buildz-0.4.5/buildz/demos/xf/test.js
+-rw-rw-rw-   0        0        0      251 2024-04-01 12:36:42.000000 buildz-0.4.5/buildz/demos/xf/test.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.283078 buildz-0.4.5/buildz/fz/
+-rw-rw-rw-   0        0        0      159 2024-04-01 15:24:04.000000 buildz-0.4.5/buildz/fz/__init__.py
+-rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.4.5/buildz/fz/dirz.py
+-rw-rw-rw-   0        0        0     1584 2024-04-01 14:56:51.000000 buildz-0.4.5/buildz/fz/lsf.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.283078 buildz-0.4.5/buildz/ioc/
+-rw-rw-rw-   0        0        0      110 2024-04-01 15:22:59.000000 buildz-0.4.5/buildz/ioc/__init__.py
+-rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.4.5/buildz/ioc/init.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.283078 buildz-0.4.5/buildz/ioc/ioc/
+-rw-rw-rw-   0        0        0      971 2024-04-01 15:06:27.000000 buildz-0.4.5/buildz/ioc/ioc/base.py
+-rw-rw-rw-   0        0        0     4266 2024-04-01 15:06:31.000000 buildz-0.4.5/buildz/ioc/ioc/conf.py
+-rw-rw-rw-   0        0        0    12380 2024-04-01 17:23:56.000000 buildz-0.4.5/buildz/ioc/ioc/confs.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.298708 buildz-0.4.5/buildz/ioc/ioc_deal/
+-rw-rw-rw-   0        0        0     4536 2024-04-01 16:04:44.000000 buildz-0.4.5/buildz/ioc/ioc_deal/base.py
+-rw-rw-rw-   0        0        0     1128 2024-03-31 09:56:22.000000 buildz-0.4.5/buildz/ioc/ioc_deal/call.py
+-rw-rw-rw-   0        0        0      956 2024-04-01 14:23:38.000000 buildz-0.4.5/buildz/ioc/ioc_deal/calls.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.314333 buildz-0.4.5/buildz/ioc/ioc_deal/conf/
+-rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/call_defaults.js
+-rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/call_lists.js
+-rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/calls_defaults.js
+-rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/calls_lists.js
+-rw-rw-rw-   0        0        0     1392 2024-04-01 16:37:04.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/deals.js
+-rw-rw-rw-   0        0        0      307 2024-04-01 14:20:24.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/env_lists.js
+-rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/ioc_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/join_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/list_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/map_lists.js
+-rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/mcall_defaults.js
+-rw-rw-rw-   0        0        0      476 2024-03-31 09:44:23.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/mcall_lists.js
+-rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
+-rw-rw-rw-   0        0        0       94 2024-03-31 03:42:49.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/obj_defaults.js
+-rw-rw-rw-   0        0        0      626 2024-03-31 09:33:20.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/obj_lists.js
+-rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/obj_set_lists.js
+-rw-rw-rw-   0        0        0      411 2024-03-31 10:04:44.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/ovar_lists.js
+-rw-rw-rw-   0        0        0      416 2024-04-01 14:20:26.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/ref_lists.js
+-rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.4.5/buildz/ioc/ioc_deal/conf/var_lists.js
+-rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.4.5/buildz/ioc/ioc_deal/demo.py
+-rw-rw-rw-   0        0        0      524 2024-03-31 09:08:42.000000 buildz-0.4.5/buildz/ioc/ioc_deal/env.py
+-rw-rw-rw-   0        0        0      606 2024-04-01 11:11:54.000000 buildz-0.4.5/buildz/ioc/ioc_deal/ioc.py
+-rw-rw-rw-   0        0        0      617 2024-04-01 16:39:12.000000 buildz-0.4.5/buildz/ioc/ioc_deal/join.py
+-rw-rw-rw-   0        0        0      610 2024-04-01 16:09:38.000000 buildz-0.4.5/buildz/ioc/ioc_deal/list.py
+-rw-rw-rw-   0        0        0      612 2024-04-01 16:09:21.000000 buildz-0.4.5/buildz/ioc/ioc_deal/map.py
+-rw-rw-rw-   0        0        0     1487 2024-03-31 10:48:09.000000 buildz-0.4.5/buildz/ioc/ioc_deal/mcall.py
+-rw-rw-rw-   0        0        0     2862 2024-04-01 16:12:27.000000 buildz-0.4.5/buildz/ioc/ioc_deal/obj.py
+-rw-rw-rw-   0        0        0     1096 2024-03-31 10:05:27.000000 buildz-0.4.5/buildz/ioc/ioc_deal/ovar.py
+-rw-rw-rw-   0        0        0      536 2024-04-01 16:24:19.000000 buildz-0.4.5/buildz/ioc/ioc_deal/ref.py
+-rw-rw-rw-   0        0        0      280 2024-04-01 16:05:46.000000 buildz-0.4.5/buildz/ioc/ioc_deal/val.py
+-rw-rw-rw-   0        0        0      823 2024-03-31 10:07:06.000000 buildz-0.4.5/buildz/ioc/ioc_deal/var.py
+-rw-rw-rw-   0        0        0     5405 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/keys.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.314333 buildz-0.4.5/buildz/old_version/
+-rw-rw-rw-   0        0        0     1055 2024-04-01 11:19:41.000000 buildz-0.4.5/buildz/old_version/__init__.py
+-rw-rw-rw-   0        0        0      344 2024-04-01 11:19:32.000000 buildz-0.4.5/buildz/old_version/__main__.py
+-rw-rw-rw-   0        0        0     1775 2024-02-28 03:15:25.000000 buildz-0.4.5/buildz/old_version/base.py
+-rw-rw-rw-   0        0        0     7859 2024-04-01 11:19:19.000000 buildz-0.4.5/buildz/old_version/build.py
+-rw-rw-rw-   0        0        0    10964 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/old_version/confz.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.220306 buildz-0.4.5/buildz/old_version/demo/
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.329958 buildz-0.4.5/buildz/old_version/demo/x/
+-rw-rw-rw-   0        0        0      546 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/old_version/demo/x/demo.confz
+-rw-rw-rw-   0        0        0      522 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/old_version/demo/x/demo.py
+-rw-rw-rw-   0        0        0      476 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/old_version/demo/x/run.confz
+-rw-rw-rw-   0        0        0      464 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/old_version/demo/x/test.confz
+-rw-rw-rw-   0        0        0      217 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/old_version/demo/x/test.py
+-rw-rw-rw-   0        0        0      240 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/old_version/demo/x/testc.py
+-rw-rw-rw-   0        0        0      780 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/old_version/demo/x/testf.py
+-rw-rw-rw-   0        0        0     1197 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/old_version/demo/x/testz.py
+-rw-rw-rw-   0        0        0      375 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/old_version/demo/x/value.confz
+-rw-rw-rw-   0        0        0      174 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/old_version/demo/x/x.py
+-rw-rw-rw-   0        0        0        0 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/old_version/dj.txt
+-rw-rw-rw-   0        0        0     5405 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/old_version/keys.py
+-rw-rw-rw-   0        0        0     1750 2024-04-01 14:37:34.000000 buildz-0.4.5/buildz/old_version/test_loader copy.py
+-rw-rw-rw-   0        0        0      336 2024-03-01 16:45:49.000000 buildz-0.4.5/buildz/old_version/test_loader.py
+-rw-rw-rw-   0        0        0      658 2024-03-01 16:51:21.000000 buildz-0.4.5/buildz/old_version/test_writer.py
+-rw-rw-rw-   0        0        0      843 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/old_version/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.332313 buildz-0.4.5/buildz/old_version/xconfz/
+-rw-rw-rw-   0        0        0      524 2024-04-01 11:20:18.000000 buildz-0.4.5/buildz/old_version/xconfz/__init__.py
+-rw-rw-rw-   0        0        0     6026 2024-04-01 11:20:26.000000 buildz-0.4.5/buildz/old_version/xconfz/base.py
+-rw-rw-rw-   0        0        0     1675 2024-04-01 11:20:36.000000 buildz-0.4.5/buildz/old_version/xconfz/buff.py
+-rw-rw-rw-   0        0        0      156 2024-04-01 11:21:03.000000 buildz-0.4.5/buildz/old_version/xconfz/fc.py
+-rw-rw-rw-   0        0        0     2281 2024-04-01 11:20:44.000000 buildz-0.4.5/buildz/old_version/xconfz/fc_item.py
+-rw-rw-rw-   0        0        0     2678 2024-04-01 11:20:47.000000 buildz-0.4.5/buildz/old_version/xconfz/fc_list.py
+-rw-rw-rw-   0        0        0     3017 2024-04-01 11:20:50.000000 buildz-0.4.5/buildz/old_version/xconfz/fc_map.py
+-rw-rw-rw-   0        0        0     1778 2024-04-01 11:20:53.000000 buildz-0.4.5/buildz/old_version/xconfz/fc_set.py
+-rw-rw-rw-   0        0        0     2887 2024-04-01 11:20:56.000000 buildz-0.4.5/buildz/old_version/xconfz/fc_str.py
+-rw-rw-rw-   0        0        0     2823 2024-04-01 11:20:59.000000 buildz-0.4.5/buildz/old_version/xconfz/fc_type.py
+-rw-rw-rw-   0        0        0      841 2023-10-16 14:40:02.000000 buildz-0.4.5/buildz/old_version/xconfz/file.py
+-rw-rw-rw-   0        0        0     4018 2024-04-01 11:21:08.000000 buildz-0.4.5/buildz/old_version/xconfz/fmt_base.py
+-rw-rw-rw-   0        0        0     1322 2024-04-01 11:21:16.000000 buildz-0.4.5/buildz/old_version/xconfz/fmt_str.py
+-rw-rw-rw-   0        0        0     2069 2024-04-01 11:21:20.000000 buildz-0.4.5/buildz/old_version/xconfz/fmt_type.py
+-rw-rw-rw-   0        0        0     4326 2024-04-01 11:21:30.000000 buildz-0.4.5/buildz/old_version/xconfz/mg.py
+-rw-rw-rw-   0        0        0     4186 2024-04-01 11:21:23.000000 buildz-0.4.5/buildz/old_version/xconfz/mg_fmt.py
+-rw-rw-rw-   0        0        0     1112 2024-03-31 02:32:18.000000 buildz-0.4.5/buildz/pyz.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.346393 buildz-0.4.5/buildz/xf/
+-rw-rw-rw-   0        0        0      209 2024-04-01 15:22:54.000000 buildz-0.4.5/buildz/xf/__init__.py
+-rw-rw-rw-   0        0        0      841 2024-04-01 17:49:56.000000 buildz-0.4.5/buildz/xf/file.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.346393 buildz-0.4.5/buildz/xf/loader/
+-rw-rw-rw-   0        0        0     1696 2024-03-01 16:40:46.000000 buildz-0.4.5/buildz/xf/loader/base.py
+-rw-rw-rw-   0        0        0     2456 2024-02-22 16:50:58.000000 buildz-0.4.5/buildz/xf/loader/buffer.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.346393 buildz-0.4.5/buildz/xf/loader/deal/
+-rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.4.5/buildz/xf/loader/deal/listz.py
+-rw-rw-rw-   0        0        0     2619 2024-03-31 10:34:46.000000 buildz-0.4.5/buildz/xf/loader/deal/lr.py
+-rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.4.5/buildz/xf/loader/deal/lrval.py
+-rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.4.5/buildz/xf/loader/deal/mapz.py
+-rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.4.5/buildz/xf/loader/deal/nextz.py
+-rw-rw-rw-   0        0        0     1156 2024-03-01 16:45:20.000000 buildz-0.4.5/buildz/xf/loader/deal/reval.py
+-rw-rw-rw-   0        0        0     1134 2024-02-22 13:17:44.000000 buildz-0.4.5/buildz/xf/loader/deal/setz.py
+-rw-rw-rw-   0        0        0      390 2024-02-22 17:15:53.000000 buildz-0.4.5/buildz/xf/loader/deal/spc.py
+-rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.4.5/buildz/xf/loader/deal/spt.py
+-rw-rw-rw-   0        0        0     3070 2024-04-01 16:46:08.000000 buildz-0.4.5/buildz/xf/loader/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.4.5/buildz/xf/loader/exp.py
+-rw-rw-rw-   0        0        0     1490 2024-02-22 16:35:35.000000 buildz-0.4.5/buildz/xf/loader/item.py
+-rw-rw-rw-   0        0        0     1693 2024-02-22 16:18:29.000000 buildz-0.4.5/buildz/xf/loader/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-02-22 12:37:04.000000 buildz-0.4.5/buildz/xf/loader/pos.py
+-rw-rw-rw-   0        0        0     1093 2024-03-31 03:05:04.000000 buildz-0.4.5/buildz/xf/mapz.py
+-rw-rw-rw-   0        0        0     2591 2024-04-01 16:46:39.000000 buildz-0.4.5/buildz/xf/read.py
+-rw-rw-rw-   0        0        0     1314 2024-02-24 09:19:50.000000 buildz-0.4.5/buildz/xf/test_write.py
+-rw-rw-rw-   0        0        0     1203 2024-03-01 16:51:07.000000 buildz-0.4.5/buildz/xf/write.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.361896 buildz-0.4.5/buildz/xf/writer/
+-rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.4.5/buildz/xf/writer/base.py
+-rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.4.5/buildz/xf/writer/conf.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.361896 buildz-0.4.5/buildz/xf/writer/deal/
+-rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.4.5/buildz/xf/writer/deal/jsonval.py
+-rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.4.5/buildz/xf/writer/deal/listz.py
+-rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.4.5/buildz/xf/writer/deal/mapz.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.4.5/buildz/xf/writer/deal/reval.py
+-rw-rw-rw-   0        0        0     1377 2024-02-24 09:43:55.000000 buildz-0.4.5/buildz/xf/writer/deal/strz.py
+-rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.4.5/buildz/xf/writer/itemz.py
+-rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.4.5/buildz/xf/writer/mg.py
+-rw-rw-rw-   0        0        0      509 2024-04-01 13:44:50.000000 buildz-0.4.5/buildz/xf/xargs.py
+drwxrwxrwx   0        0        0        0 2024-04-01 17:54:19.252353 buildz-0.4.5/buildz.egg-info/
+-rw-rw-rw-   0        0        0     5750 2024-04-01 17:54:19.000000 buildz-0.4.5/buildz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4197 2024-04-01 17:54:19.000000 buildz-0.4.5/buildz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 17:54:19.000000 buildz-0.4.5/buildz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-01 17:54:19.000000 buildz-0.4.5/buildz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-01 17:54:19.361896 buildz-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      770 2024-04-01 15:13:28.000000 buildz-0.4.5/setup.py
```

### Comparing `buildz-0.4.4/LICENSE` & `buildz-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/PKG-INFO` & `buildz-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.4.4
+Version: 0.4.5
 Summary: a json-like file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.4.4/README.md` & `buildz-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/argx.py` & `buildz-0.4.5/buildz/argx.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,25 +22,33 @@
             val = 1
         else:
             if v[1]=="-":
                 kv = v[2:]
                 x = kv.split("=")
                 key = x[0]
                 val = "=".join(x[1:])
+                if len(val)==0:
+                    val = 1
             else:
                 key = v[1]
                 if len(v)>2:
                     val = argv[2:]
                 else:
                     if i+1>=len(argv):
                         val = 1
                     else:
                         val = argv[i+1]
                         i+=1
-        maps[key] = val
+        if key not in maps:
+            maps[key] = []
+        maps[key].append(val)
         i+=1
+    for k in maps:
+        v = maps[k]
+        if len(v)==1:
+            maps[k] = v[0]
     return lists, maps
 
 pass
```

### Comparing `buildz-0.4.4/buildz/demo/ioc/test.py` & `buildz-0.4.5/buildz/demos/ioc/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/demo/ioc/test_conf/base.js` & `buildz-0.4.5/buildz/demos/ioc/test_conf/base.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/demo/ioc/test_conf/data1.js` & `buildz-0.4.5/buildz/demos/ioc/test_conf/data1.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -37,15 +37,15 @@
         type: mcall
         source: test
         method: run
         args: []
         maps: {}
     } {
         id: test.obj
-        val: test.show
+        data: test.show
     } {
         id: calls
         type: calls
         calls: [
             [mcall, test, run, , , ]
             [call, test.show]
         ]
```

### Comparing `buildz-0.4.4/buildz/ioc/ioc/base.py` & `buildz-0.4.5/buildz/ioc/ioc/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/ioc/ioc/conf.py` & `buildz-0.4.5/buildz/ioc/ioc/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/ioc/ioc/confs.py` & `buildz-0.4.5/buildz/ioc/ioc/confs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #coding=utf-8
 from buildz import xf, pyz
 from buildz.xf import g as xg
+from buildz import argx
 import json
 from .base import Base, EncapeData
 from .conf import Conf
 import os
 class ConfsNode(Base):
     def init(self):
         self.confs = []
@@ -43,15 +44,61 @@
                 self.update_maps(tval, val)
             else:
                 tmp[id] = val
     def env_ids(self, id):
         return id.split(self.env_spt)
     def env_id(self, ids):
         return self.env_spt.join(ids)
+    def get_env_sys(self, id, sid=None):
+        sysdt = os.getenv(id)
+        return sysdt
+    def build_env_args_xf(self):
+        data = xf.args()
+        env = data['env']
+        self.envs_args = env
+    def build_env_args_buildz(self):
+        args, maps = argx.fetch()
+        e = xf.get(maps, e = [])
+        env = xf.get(maps, env=[])
+        env += e
+        env = [k.split("=") for k in env]
+        env = {k[0]:"=".join(k[1:]) for k in env}
+        self.envs_args = env
+    def get_env_args(self, id, sid=None):
+        if self.envs_args is not None:
+            if self.args_type == "xf":
+                self.build_env_args_xf()
+            else:
+                self.build_env_args_buildz()
+        return xf.get(self.envs_args, id)
+    def get_env_local(self, id, sid=None):
+        if sid is not None and not self.global_env:
+            val = self.confs[sid].get_env(id, False)
+            if val is not None:
+                return val
+        return None
+    def get_env_conf(self, id, sid=None):
+        ids = self.env_ids(id)
+        envs = self.envs
+        for id in ids:
+            if type(envs)!=dict:
+                envs = None
+                break
+            if id not in envs:
+                envs = None
+                break 
+            envs = envs[id]
+        return envs
     def get_env(self, id, sid=None):
+        for key in self.env_orders:
+            fc = self.env_fcs[key]
+            obj = fc(id, sid)
+            if obj is not None:
+                return obj
+        return None
         if sid is not None and not self.global_env:
             val = self.confs[sid].get_env(id, False)
             if val is not None:
                 return val
         sysdt = os.getenv(id)
         if sysdt is not None:
             return sysdt
@@ -107,14 +154,21 @@
             default_type: default
             // 全局查id的时候是从最上层开始找还是从最下层开始找（每一层都可能有配置文件）
             // default = false
             deep_first: false
             // true=环境变量env都是全局的（全局查找），否则优先每个配置文件里查环境变量，查不到才查全局
             // default = true
             global_env: true
+            // 环境变量读取顺序，默认先命令行配置，然后系统变量，然后本地配置文件配置(设置全局则不查)，最后配置文件配置，不想读哪个把哪个删了就可以
+            // 命令行配置格式:
+            //     -e a=b --env=a=b --env=c=d
+            //     env: {a=b, c=d}
+            env_orders: [args, sys, local, conf]
+            // 命令行读取方式：默认xf(xf.args),可选: buildz(buidlz.argx)
+            args_type: 'xf'
             // true=类型处理函数deal都是全局的（全局查找），否则优先每个配置文件里查处理函数，查不到才查全局
             // default = true 
             global_deal: true
             // 数据的id字段名
             // default = 'id'
             data_key_id: id
             // 数据的type字段名
@@ -147,20 +201,29 @@
         self.global_deal = xf.g(conf, global_deal = True)
         self.data_key_id = xf.g(conf, data_key_id = 'id')
         self.data_key_type = xf.g(conf, data_key_type = 'type')
         self.data_index_id = xf.g(conf, data_index_id = [0,0])
         self.data_index_type = xf.g(conf, data_index_type = [0,1])
         self.deal_key_type = xf.g(conf, deal_key_type = 'type')
         self.deal_index_type = xf.g(conf, deal_index_type = 0)
+        self.env_orders = xf.g(conf, env_orders = ['args', 'sys', 'local', 'conf'])
+        self.env_fcs = {
+            'args': self.get_env_args,
+            'sys': self.get_env_sys,
+            'local': self.get_env_local,
+            'conf': self.get_env_conf
+        }
+        self.args_type = xf.g(conf, args_type = "xf")
         self._conf_id = 0
         self.conf = conf
         self.node = ConfsNode()
         self.confs = {}
         self.deals = {}
         self.envs = {}
+        self.envs_args = None
     def get_deal_type(self, obj):
         if type(obj)==dict:
             return obj[self.deal_key_type]
         return obj[self.deal_index_type]
     def get_data_id(self, obj):
         if type(obj)==dict:
             return obj[self.data_key_id]
@@ -196,17 +259,23 @@
         return id.split(self.spt)
     def id(self, ids):
         """
             data的id列表转id，外部不调用
             例: ids = ['a','b','c'], spt = ".", id = 'a.b.c', 
         """
         return self.spt.join(ids)
+    def add_fps(self, fps):
+        for fp in fps:
+            self.add_fp(fp)
     def add_fp(self, fp):
         conf = self.loads(xf.fread(fp))
         return self.add(conf)
+    def adds(self, confs):
+        for conf in confs:
+            self.add(conf)
     def add(self, conf):
         """
             {
                 deals:[{build: fc_path,args: [],maps: {}}]
                 envs: {id: val}
                 id: default null
                 namespace: default null
```

### Comparing `buildz-0.4.4/buildz/ioc/ioc_deal/base.py` & `buildz-0.4.5/buildz/ioc/ioc_deal/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-#
+#coding=utf-8
+
 from ..ioc.base import Base, EncapeData
 from buildz import xf
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
 default_deals = join(dp, 'conf', 'deals.js')
 class FormatData(Base):
```

### Comparing `buildz-0.4.4/buildz/ioc/ioc_deal/call.py` & `buildz-0.4.5/buildz/ioc/ioc_deal/call.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/ioc/ioc_deal/calls.py` & `buildz-0.4.5/buildz/ioc/ioc_deal/calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,12 +25,13 @@
     def deal(self, edata:EncapeData):
         sid = edata.sid
         data = edata.data
         conf = edata.conf
         data = self.format(data)
         src = edata.src
         calls = xf.g(data, calls=[])
+        rst = None
         for call in calls:
             rst = self.get_obj(call, conf, src)
         return rst
 
 pass
```

### Comparing `buildz-0.4.4/buildz/ioc/ioc_deal/conf/deals.js` & `buildz-0.4.5/buildz/ioc/ioc_deal/conf/deals.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -26,9 +26,18 @@
         build: buildz.ioc.ioc_deal.var.VarDeal
     }, {
         type: calls,
         build: buildz.ioc.ioc_deal.calls.CallsDeal
     }, {
         type: ioc,
         build: buildz.ioc.ioc_deal.ioc.IOCObjectDeal
+    }, {
+        type: list,
+        build: buildz.ioc.ioc_deal.list.ListDeal
+    }, {
+        type: map,
+        build: buildz.ioc.ioc_deal.map.MapDeal
+    }, {
+        type: join,
+        build: buildz.ioc.ioc_deal.join.JoinDeal
     }]
 }
```

### Comparing `buildz-0.4.4/buildz/ioc/ioc_deal/conf/obj_lists.js` & `buildz-0.4.5/buildz/ioc/ioc_deal/conf/obj_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/ioc/ioc_deal/env.py` & `buildz-0.4.5/buildz/ioc/ioc_deal/env.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/ioc/ioc_deal/ioc.py` & `buildz-0.4.5/buildz/ioc/ioc_deal/ioc.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/ioc/ioc_deal/mcall.py` & `buildz-0.4.5/buildz/ioc/ioc_deal/mcall.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/ioc/ioc_deal/obj.py` & `buildz-0.4.5/buildz/ioc/ioc_deal/obj.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         conf = edata.conf
         confs = edata.confs
         source = xf.g(data, source=0)
         fc = xf.get(self.sources, source, None)
         if fc is None:
             fc = pyz.load(source)
             self.sources[source]=fc
-        cst = xf.g(data, construct = 0)
+        cst = xf.g(data, construct = [])
         cst = self.fmt_cst(cst)
         args = xf.g(cst, args=[])
         maps = xf.g(cst, maps={})
         args = [self.get_obj(v, conf) for v in args]
         maps = {k:self.get_obj(maps[k], conf) for k in maps}
         obj = fc(*args, **maps)
         if single:
```

### Comparing `buildz-0.4.4/buildz/ioc/ioc_deal/ovar.py` & `buildz-0.4.5/buildz/ioc/ioc_deal/ovar.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/ioc/ioc_deal/ref.py` & `buildz-0.4.5/buildz/ioc/ioc_deal/ref.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .base import FormatData,BaseDeal
 from buildz import xf, pyz
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
 class RefDeal(BaseDeal):
     def init(self, fp_lists=None, fp_defaults=None):
-        super().init("EnvDeal", fp_lists, fp_defaults, join(dp, "conf", "ref_lists.js"), None)
+        super().init("RefDeal", fp_lists, fp_defaults, join(dp, "conf", "ref_lists.js"), None)
     def deal(self, edata:EncapeData):
         data = edata.data
         data = self.fill(data)
         key = data['key']
         return edata.conf.get_obj(key)
 
 pass
```

### Comparing `buildz-0.4.4/buildz/ioc/ioc_deal/var.py` & `buildz-0.4.5/buildz/ioc/ioc_deal/var.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/keys.py` & `buildz-0.4.5/buildz/keys.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/__init__.py` & `buildz-0.4.5/buildz/old_version/__init__.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/base.py` & `buildz-0.4.5/buildz/old_version/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/build.py` & `buildz-0.4.5/buildz/old_version/build.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/confz.py` & `buildz-0.4.5/buildz/old_version/confz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/demo/x/demo.confz` & `buildz-0.4.5/buildz/old_version/demo/x/demo.confz`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/demo/x/demo.py` & `buildz-0.4.5/buildz/old_version/demo/x/demo.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/demo/x/testf.py` & `buildz-0.4.5/buildz/old_version/demo/x/testf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/demo/x/testz.py` & `buildz-0.4.5/buildz/old_version/demo/x/testz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/keys.py` & `buildz-0.4.5/buildz/old_version/keys.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/xconfz/__init__.py` & `buildz-0.4.5/buildz/old_version/xconfz/__init__.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/xconfz/base.py` & `buildz-0.4.5/buildz/old_version/xconfz/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/xconfz/buff.py` & `buildz-0.4.5/buildz/old_version/xconfz/buff.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/xconfz/fc_item.py` & `buildz-0.4.5/buildz/old_version/xconfz/fc_item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/xconfz/fc_list.py` & `buildz-0.4.5/buildz/old_version/xconfz/fc_list.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/xconfz/fc_map.py` & `buildz-0.4.5/buildz/old_version/xconfz/fc_map.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/xconfz/fc_set.py` & `buildz-0.4.5/buildz/old_version/xconfz/fc_set.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/xconfz/fc_str.py` & `buildz-0.4.5/buildz/old_version/xconfz/fc_str.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/xconfz/fc_type.py` & `buildz-0.4.5/buildz/old_version/xconfz/fc_type.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/xconfz/file.py` & `buildz-0.4.5/buildz/old_version/xconfz/file.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/xconfz/fmt_base.py` & `buildz-0.4.5/buildz/old_version/xconfz/fmt_base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/xconfz/fmt_str.py` & `buildz-0.4.5/buildz/old_version/xconfz/fmt_str.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/xconfz/fmt_type.py` & `buildz-0.4.5/buildz/old_version/xconfz/fmt_type.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/xconfz/mg.py` & `buildz-0.4.5/buildz/old_version/xconfz/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/old_version/xconfz/mg_fmt.py` & `buildz-0.4.5/buildz/old_version/xconfz/mg_fmt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/pyz.py` & `buildz-0.4.5/buildz/pyz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/test_loader copy.py` & `buildz-0.4.5/buildz/old_version/test_loader copy.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/test_writer.py` & `buildz-0.4.5/buildz/old_version/test_writer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/tools.py` & `buildz-0.4.5/buildz/old_version/tools.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/file.py` & `buildz-0.4.5/buildz/xf/file.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/loader/base.py` & `buildz-0.4.5/buildz/xf/loader/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/loader/buffer.py` & `buildz-0.4.5/buildz/xf/loader/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/loader/deal/listz.py` & `buildz-0.4.5/buildz/xf/loader/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/loader/deal/lr.py` & `buildz-0.4.5/buildz/xf/loader/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/loader/deal/lrval.py` & `buildz-0.4.5/buildz/xf/loader/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/loader/deal/mapz.py` & `buildz-0.4.5/buildz/xf/loader/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/loader/deal/nextz.py` & `buildz-0.4.5/buildz/xf/loader/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/loader/deal/reval.py` & `buildz-0.4.5/buildz/xf/loader/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/loader/deal/setz.py` & `buildz-0.4.5/buildz/xf/loader/deal/setz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/loader/deal/spt.py` & `buildz-0.4.5/buildz/xf/loader/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/loader/deal/strz.py` & `buildz-0.4.5/buildz/xf/loader/deal/strz.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 from .. import base
 from .. import item
 from .. import exp
+from ... import file
 import json
 class PrevStrDeal(base.BaseDeal):
     def init(self, left = '"', right= '"', single_line = False, note = False, translate = False):
         self.left = left
         self.right = right
         self.ll = len(left)
         self.lr = len(right)
         self.single_line = single_line
         self.note = note
         self.translate = translate
+    def json_loads(self, s):
+        x = s
+        cd = None
+        if type(x)==bytes:
+            x, cd = file.decode_c(x)
+        rs = json.loads(x)
+        if type(s)==bytes:
+            rs = rs.encode(cd)
+        return rs
     def do_translate(self, s):
         """
             取巧直接调用json
         """
         qt = self.like('"',s)
         ql = self.like("\\", s)
         et = self.like("\n", s)
@@ -23,15 +33,15 @@
         pt = ql+qt
         arr = s.split(pt)
         arr = [k.replace(qt, pt) for k in arr]
         s = pt.join(arr)
         #s = s.replace(qt, ql+qt)
         s = s.replace(tr, nt)
         arr = s.split(et)
-        outs = [json.loads(qt+k+qt) for k in arr]
+        outs = [self.json_loads(qt+k+qt) for k in arr]
         outs = et.join(outs)
         return outs
     def prev(self, buffer, queue, pos):
         cl = buffer.read(self.ll)
         if not self.same(self.left, cl):
             return False
         buffer.pop_read(self.ll)
```

### Comparing `buildz-0.4.4/buildz/xf/loader/item.py` & `buildz-0.4.5/buildz/xf/loader/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/loader/mg.py` & `buildz-0.4.5/buildz/xf/loader/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/loader/pos.py` & `buildz-0.4.5/buildz/xf/loader/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/mapz.py` & `buildz-0.4.5/buildz/xf/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/read.py` & `buildz-0.4.5/buildz/xf/read.py`

 * *Files 25% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     fcs.set("nil", lambda x:None)
     fcs.set("n", lambda x:None)
     mgs.add(lrval.LRValDeal("<",">",fcs))
 
 pass
 def build_val(mgs):
     mgs.add(reval.ValDeal("[\+\-]?\d+", int))
-    mgs.add(reval.ValDeal("[\+\-]?\d+\.\d+", float))
+    mgs.add(reval.ValDeal("[\+\-]?\d*\.\d+", float))
     mgs.add(reval.ValDeal("[\+\-]?\d+e[\+\-]?\d+", float))
     mgs.add(reval.ValDeal("null", lambda x:None))
     mgs.add(reval.ValDeal("true", lambda x:True))
     mgs.add(reval.ValDeal("false", lambda x:False))
 
 pass
 def build():
@@ -67,12 +67,20 @@
     return mgs
 
 pass
 def load(read):
     mgs = build()
     return msg.load(read)
 def loads(s):
+    # lr = "{}"
+    # ls = "{[("
+    # if type(s)==bytes:
+    #     lr = lr.encode()
+    #     ls = ls.encode()
+    # x = s.strip()
+    # if len(x)>0 and x[0] not in ls:
+    #     s = lr[0]+s+lr[1]
     mgs = build()
     input = buffer.BufferInput(s)
     return mgs.load(input)
 
 pass
```

### Comparing `buildz-0.4.4/buildz/xf/test_write.py` & `buildz-0.4.5/buildz/xf/test_write.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/write.py` & `buildz-0.4.5/buildz/xf/write.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/writer/base.py` & `buildz-0.4.5/buildz/xf/writer/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/writer/conf.py` & `buildz-0.4.5/buildz/xf/writer/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/writer/deal/listz.py` & `buildz-0.4.5/buildz/xf/writer/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/writer/deal/mapz.py` & `buildz-0.4.5/buildz/xf/writer/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/writer/deal/strz.py` & `buildz-0.4.5/buildz/xf/writer/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/writer/itemz.py` & `buildz-0.4.5/buildz/xf/writer/itemz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz/xf/writer/mg.py` & `buildz-0.4.5/buildz/xf/writer/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.4/buildz.egg-info/PKG-INFO` & `buildz-0.4.5/buildz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.4.4
+Version: 0.4.5
 Summary: a json-like file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.4.4/buildz.egg-info/SOURCES.txt` & `buildz-0.4.5/buildz.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,92 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 buildz/__init__.py
+buildz/__main__.py
 buildz/argx.py
-buildz/dj.txt
 buildz/keys.py
 buildz/pyz.py
-buildz/test_loader copy.py
-buildz/test_loader.py
-buildz/test_writer.py
-buildz/tools.py
 buildz.egg-info/PKG-INFO
 buildz.egg-info/SOURCES.txt
 buildz.egg-info/dependency_links.txt
 buildz.egg-info/top_level.txt
-buildz/demo/ioc/test.py
-buildz/demo/ioc/test_conf/base.js
-buildz/demo/ioc/test_conf/data1.js
-buildz/demo/ioc/test_conf/data2.js
-buildz/demo/ioc/test_conf/data3.js
-buildz/demo/xf/test.js
-buildz/demo/xf/test.py
+buildz/demo/test.py
+buildz/demo/ioc/deal.py
+buildz/demo/ioc/help.py
+buildz/demo/res/test.js
+buildz/demo/res/conf/ioc.js
+buildz/demo/res/conf/main.js
+buildz/demo/res/conf/xf.js
+buildz/demo/res/help/default.js
+buildz/demo/res/help/ioc.js
+buildz/demo/res/help/xf.js
+buildz/demo/xf/deal.py
+buildz/demo/xf/help.py
+buildz/demos/ioc/test.py
+buildz/demos/ioc/test_conf/base.js
+buildz/demos/ioc/test_conf/data1.js
+buildz/demos/ioc/test_conf/data2.js
+buildz/demos/ioc/test_conf/data3.js
+buildz/demos/xf/test.js
+buildz/demos/xf/test.py
+buildz/fz/__init__.py
+buildz/fz/dirz.py
+buildz/fz/lsf.py
 buildz/ioc/__init__.py
 buildz/ioc/init.py
 buildz/ioc/ioc/base.py
 buildz/ioc/ioc/conf.py
 buildz/ioc/ioc/confs.py
 buildz/ioc/ioc_deal/base.py
 buildz/ioc/ioc_deal/call.py
 buildz/ioc/ioc_deal/calls.py
 buildz/ioc/ioc_deal/demo.py
 buildz/ioc/ioc_deal/env.py
 buildz/ioc/ioc_deal/ioc.py
+buildz/ioc/ioc_deal/join.py
+buildz/ioc/ioc_deal/list.py
+buildz/ioc/ioc_deal/map.py
 buildz/ioc/ioc_deal/mcall.py
 buildz/ioc/ioc_deal/obj.py
 buildz/ioc/ioc_deal/ovar.py
 buildz/ioc/ioc_deal/ref.py
 buildz/ioc/ioc_deal/val.py
 buildz/ioc/ioc_deal/var.py
 buildz/ioc/ioc_deal/conf/call_defaults.js
 buildz/ioc/ioc_deal/conf/call_lists.js
 buildz/ioc/ioc_deal/conf/calls_defaults.js
 buildz/ioc/ioc_deal/conf/calls_lists.js
 buildz/ioc/ioc_deal/conf/deals.js
 buildz/ioc/ioc_deal/conf/env_lists.js
 buildz/ioc/ioc_deal/conf/ioc_lists.js
+buildz/ioc/ioc_deal/conf/join_lists.js
+buildz/ioc/ioc_deal/conf/list_lists.js
+buildz/ioc/ioc_deal/conf/map_lists.js
 buildz/ioc/ioc_deal/conf/mcall_defaults.js
 buildz/ioc/ioc_deal/conf/mcall_lists.js
 buildz/ioc/ioc_deal/conf/obj_cst_lists.js
 buildz/ioc/ioc_deal/conf/obj_defaults.js
 buildz/ioc/ioc_deal/conf/obj_lists.js
 buildz/ioc/ioc_deal/conf/obj_set_lists.js
 buildz/ioc/ioc_deal/conf/ovar_lists.js
 buildz/ioc/ioc_deal/conf/ref_lists.js
 buildz/ioc/ioc_deal/conf/var_lists.js
 buildz/old_version/__init__.py
 buildz/old_version/__main__.py
 buildz/old_version/base.py
 buildz/old_version/build.py
 buildz/old_version/confz.py
+buildz/old_version/dj.txt
 buildz/old_version/keys.py
+buildz/old_version/test_loader copy.py
+buildz/old_version/test_loader.py
+buildz/old_version/test_writer.py
+buildz/old_version/tools.py
 buildz/old_version/demo/x/demo.confz
 buildz/old_version/demo/x/demo.py
 buildz/old_version/demo/x/run.confz
 buildz/old_version/demo/x/test.confz
 buildz/old_version/demo/x/test.py
 buildz/old_version/demo/x/testc.py
 buildz/old_version/demo/x/testf.py
```

### Comparing `buildz-0.4.4/setup.py` & `buildz-0.4.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: Zzz(1309458652@qq.com)
 # Description:
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'buildz',
-    version = '0.4.4',
+    version = '0.4.5',
     keywords='buildz',
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     description = "a json-like file format's read and write code by python, and codes to read and product object from configure file in such format",
     license = 'Apache License 2.0',
     url = 'https://github.com/buildCodeZ/buildz',
     author = 'Zzz',
```

