# Comparing `tmp/turnkeyml-2.0.1.tar.gz` & `tmp/turnkeyml-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turnkeyml-2.0.1.tar", last modified: Thu Mar 21 15:01:29 2024, max compression
+gzip compressed data, was "turnkeyml-2.0.2.tar", last modified: Tue Apr  2 19:24:00 2024, max compression
```

## Comparing `turnkeyml-2.0.1.tar` & `turnkeyml-2.0.2.tar`

### file list

```diff
@@ -1,1348 +1,1348 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.582609 turnkeyml-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (127)    13824 2024-03-21 15:01:29.582609 turnkeyml-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.370606 turnkeyml-2.0.1/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.374606 turnkeyml-2.0.1/models/graph_convolutions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/graph_convolutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/graph_convolutions/chebconv.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/graph_convolutions/dnaconv.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/graph_convolutions/feastconv.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/graph_convolutions/gatedgraphconv.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/graph_convolutions/generalconv.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/graph_convolutions/leconv.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/graph_convolutions/pnaconv.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/graph_convolutions/resgatedgraphconv.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/graph_convolutions/sageconv.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/graph_convolutions/tagconv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.374606 turnkeyml-2.0.1/models/selftest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/selftest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/selftest/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/selftest/twolayer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.510608 turnkeyml-2.0.1/models/timm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/adv_inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/bat_resnext26ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/beit_base_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/beit_base_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/beit_large_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/beit_large_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/beit_large_patch16_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/botnet26t_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/botnet50ts_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cait_m36_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cait_m48_448.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cait_s24_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cait_s24_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cait_s36_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cait_xs24_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cait_xxs24_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cait_xxs24_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cait_xxs36_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cait_xxs36_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/coat_lite_mini.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/coat_lite_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/coat_lite_tiny.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/coat_mini.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/coat_tiny.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convit_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convit_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convit_tiny.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convmixer_1024_20_ks9_p14.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convmixer_1536_20.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convmixer_768_32.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_base_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_base_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_base_in22k.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_large_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_large_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_large_in22k.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_nano.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_nano_ols.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_small_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_small_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_small_in22k.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_tiny.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_tiny_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_tiny_hnf.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_tiny_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_tiny_in22k.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_xlarge_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_xlarge_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/convnext_xlarge_in22k.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/crossvit_15_240.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/crossvit_15_dagger_240.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/crossvit_15_dagger_408.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/crossvit_18_240.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/crossvit_18_dagger_240.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/crossvit_18_dagger_408.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/crossvit_9_240.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/crossvit_9_dagger_240.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/crossvit_base_240.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/crossvit_small_240.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/crossvit_tiny_240.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cs3darknet_focus_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cs3darknet_focus_m.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cs3darknet_focus_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cs3darknet_focus_x.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cs3darknet_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cs3darknet_m.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cs3darknet_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cs3darknet_x.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cs3edgenet_x.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cs3se_edgenet_x.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cs3sedarknet_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cs3sedarknet_x.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cs3sedarknet_xdw.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cspdarknet53.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cspresnet50.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cspresnet50d.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cspresnet50w.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/cspresnext50.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/darknet17.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/darknet21.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/darknet53.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/darknetaa53.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit3_base_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit3_base_patch16_224_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit3_base_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit3_base_patch16_384_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit3_huge_patch14_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit3_huge_patch14_224_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit3_large_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit3_large_patch16_224_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit3_large_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit3_large_patch16_384_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit3_small_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit3_small_patch16_224_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit3_small_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit3_small_patch16_384_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit_base_distilled_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit_base_distilled_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit_base_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit_base_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit_small_distilled_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit_small_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit_tiny_distilled_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/deit_tiny_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/densenet121.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/densenet161.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/densenet169.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/densenet201.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/densenetblur121d.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dla102.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dla102x.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dla102x2.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dla169.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dla34.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dla46_c.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dla46x_c.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dla60.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dla60_res2net.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dla60_res2next.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dla60x.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dla60x_c.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dm_nfnet_f0.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dm_nfnet_f1.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dm_nfnet_f2.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dm_nfnet_f3.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dm_nfnet_f4.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dm_nfnet_f5.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dm_nfnet_f6.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dpn107.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dpn131.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dpn68.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dpn68b.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dpn92.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/dpn98.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/eca_botnext26ts_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/eca_halonext26ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/eca_nfnet_l0.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/eca_nfnet_l1.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/eca_nfnet_l2.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/eca_nfnet_l3.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/eca_resnet33ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/eca_resnext26ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/eca_vovnet39b.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ecaresnet101d.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ecaresnet200d.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ecaresnet269d.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ecaresnet26t.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ecaresnet50d.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ecaresnet50t.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ecaresnetlight.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ecaresnext26t_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ecaresnext50t_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/edgenext_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/edgenext_small_rw.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/edgenext_x_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/edgenext_xx_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b0.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b0_g16_evos.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b0_g8_gn.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b0_gn.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b1.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b2.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b2a.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b3.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b3_g8_gn.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b3_gn.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b3a.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b4.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b5.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b6.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b7.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_b8.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_cc_b0_4e.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_cc_b0_8e.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_cc_b1_8e.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_el.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_el_pruned.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_em.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_es.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_es_pruned.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_l2.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_lite0.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_lite1.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_lite2.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_lite3.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnet_lite4.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnetv2_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnetv2_m.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnetv2_rw_m.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnetv2_rw_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnetv2_rw_t.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnetv2_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/efficientnetv2_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ens_adv_inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ese_vovnet19b_dw.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ese_vovnet19b_slim.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ese_vovnet19b_slim_dw.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ese_vovnet39b.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ese_vovnet39b_evos.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ese_vovnet57b.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ese_vovnet99b.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/fbnetc_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/fbnetv3_b.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/fbnetv3_d.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/fbnetv3_g.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gc_efficientnetv2_rw_t.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gcresnet33ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gcresnet50t.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gcresnext26ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gcresnext50ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gernet_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gernet_m.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gernet_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ghostnet_050.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ghostnet_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ghostnet_130.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnet101_v1b.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnet101_v1c.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnet101_v1d.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnet101_v1s.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnet152_v1b.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnet152_v1c.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnet152_v1d.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnet152_v1s.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnet18_v1b.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnet34_v1b.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnet50_v1b.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnet50_v1c.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnet50_v1d.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnet50_v1s.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnext101_64x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_resnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_senet154.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_seresnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_seresnext101_64x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gluon_seresnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gmixer_12_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gmixer_24_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gmlp_b16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gmlp_s16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/gmlp_ti16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/halo2botnet50ts_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/halonet26t.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/halonet50ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/halonet_h1.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/haloregnetz_b.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/hardcorenas_a.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/hardcorenas_b.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/hardcorenas_c.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/hardcorenas_d.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/hardcorenas_e.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/hardcorenas_f.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/hrnet_w18.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/hrnet_w18_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/hrnet_w18_small_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/hrnet_w30.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/hrnet_w32.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/hrnet_w40.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/hrnet_w44.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/hrnet_w48.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/hrnet_w64.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ig_resnext101_32x16d.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ig_resnext101_32x32d.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ig_resnext101_32x48d.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ig_resnext101_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/inception_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/jx_nest_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/jx_nest_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/jx_nest_tiny.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/lambda_resnet26rpt_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/lambda_resnet26t.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/lambda_resnet50ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/lamhalobotnet50ts_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/lcnet_035.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/lcnet_050.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/lcnet_075.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/lcnet_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/lcnet_150.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/legacy_senet154.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/legacy_seresnet101.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/legacy_seresnet152.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/legacy_seresnet18.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/legacy_seresnet34.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/legacy_seresnet50.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/legacy_seresnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/legacy_seresnext26_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/legacy_seresnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/levit_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/levit_128s.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/levit_192.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/levit_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/levit_256d.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/levit_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mixer_b16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mixer_b16_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mixer_b16_224_miil.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mixer_b16_224_miil_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mixer_b32_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mixer_l16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mixer_l16_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mixer_l32_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mixer_s16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mixer_s32_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mixnet_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mixnet_m.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mixnet_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mixnet_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mixnet_xxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mnasnet_050.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mnasnet_075.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mnasnet_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mnasnet_140.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mnasnet_a1.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mnasnet_b1.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mnasnet_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilenetv2_035.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilenetv2_050.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilenetv2_075.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilenetv2_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilenetv2_110d.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilenetv2_120d.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilenetv2_140.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilenetv3_large_075.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilenetv3_large_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilenetv3_large_100_miil.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilenetv3_large_100_miil_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilenetv3_rw.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilenetv3_small_050.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilenetv3_small_075.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilenetv3_small_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevit_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevit_xs.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevit_xxs.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevitv2_050.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevitv2_075.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevitv2_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevitv2_125.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevitv2_150.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevitv2_150_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevitv2_150_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevitv2_175.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevitv2_175_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevitv2_175_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevitv2_200.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevitv2_200_384_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/mobilevitv2_200_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nasnetalarge.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nest_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nest_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nest_tiny.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nf_ecaresnet101.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nf_ecaresnet26.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nf_ecaresnet50.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nf_regnet_b0.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nf_regnet_b1.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nf_regnet_b2.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nf_regnet_b3.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nf_regnet_b4.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nf_regnet_b5.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nf_resnet101.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nf_resnet26.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nf_resnet50.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nf_seresnet101.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nf_seresnet26.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nf_seresnet50.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nfnet_f0.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nfnet_f1.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nfnet_f2.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nfnet_f3.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nfnet_f4.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nfnet_f5.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nfnet_f6.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nfnet_f7.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/nfnet_l0.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/pit_b_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/pit_b_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/pit_s_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/pit_s_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/pit_ti_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/pit_ti_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/pit_xs_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/pit_xs_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/pnasnet5large.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/poolformer_m36.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/poolformer_m48.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/poolformer_s12.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/poolformer_s24.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/poolformer_s36.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetv_040.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetv_064.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetx_002.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetx_004.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetx_006.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetx_008.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetx_016.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetx_032.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetx_040.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetx_064.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetx_080.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetx_120.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetx_160.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetx_320.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnety_002.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnety_004.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnety_006.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnety_008.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnety_016.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnety_032.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnety_040.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnety_064.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnety_080.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnety_120.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnety_160.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnety_320.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetz_005.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetz_040.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetz_040h.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetz_b16.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetz_b16_evos.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetz_c16.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetz_c16_evos.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetz_d32.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetz_d8.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetz_d8_evos.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/regnetz_e8.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/repvgg_a2.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/repvgg_b0.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/repvgg_b1.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/repvgg_b1g4.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/repvgg_b2.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/repvgg_b2g4.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/repvgg_b3.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/repvgg_b3g4.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/res2net101_26w_4s.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/res2net50_14w_8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/res2net50_26w_4s.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/res2net50_26w_6s.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/res2net50_26w_8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/res2net50_48w_2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/res2next50.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resmlp_12_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resmlp_12_224_dino.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resmlp_12_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resmlp_24_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resmlp_24_224_dino.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resmlp_24_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resmlp_36_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resmlp_36_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resmlp_big_24_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resmlp_big_24_224_in22ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resmlp_big_24_distilled_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnest101e.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnest14d.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnest200e.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnest269e.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnest26d.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnest50d.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnest50d_1s4x24d.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnest50d_4s2x40d.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet101.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet101d.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet10t.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet14t.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet152.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet152d.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet18.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet18d.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet200.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet200d.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet26.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet26d.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet26t.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet32ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet33ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet34.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet34d.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet50.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet50_gn.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet50d.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet50t.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet51q.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnet61q.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetaa101d.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetaa50.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetaa50d.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetblur101d.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetblur18.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetblur50.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetblur50d.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetrs101.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetrs152.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetrs200.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetrs270.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetrs350.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetrs420.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetrs50.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_101.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_101d.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_101x1_bitm.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_101x1_bitm_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_101x3_bitm.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_101x3_bitm_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_152.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_152d.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_152x2_bit_teacher.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_152x2_bit_teacher_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_152x2_bitm.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_152x2_bitm_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_152x4_bitm.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_152x4_bitm_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_50.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_50d.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_50d_evos.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_50d_frn.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_50d_gn.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_50t.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_50x1_bit_distilled.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_50x1_bitm.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_50x1_bitm_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_50x3_bitm.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnetv2_50x3_bitm_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnext101_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnext101_64x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnext26ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/resnext50d_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/rexnet_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/rexnet_130.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/rexnet_150.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/rexnet_200.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/rexnetr_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/rexnetr_130.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/rexnetr_150.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/rexnetr_200.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/sebotnet33ts_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/sedarknet21.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/sehalonet33ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/selecsls42.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/selecsls42b.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/selecsls60.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/selecsls60b.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/selecsls84.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/semnasnet_050.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/semnasnet_075.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/semnasnet_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/semnasnet_140.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/senet154.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/sequencer2d_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/sequencer2d_m.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/sequencer2d_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnet101.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnet152.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnet152d.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnet18.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnet200d.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnet269d.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnet33ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnet34.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnet50.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnet50t.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnetaa50d.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnext101_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnext101d_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnext26d_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnext26t_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnext26tn_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnext26ts.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/seresnextaa101d_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/skresnet18.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/skresnet34.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/skresnet50.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/skresnet50d.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/skresnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/spnasnet_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ssl_resnet18.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ssl_resnet50.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ssl_resnext101_32x16d.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ssl_resnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ssl_resnext101_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/ssl_resnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swin_base_patch4_window12_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swin_base_patch4_window12_384_in22k.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swin_base_patch4_window7_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swin_base_patch4_window7_224_in22k.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swin_large_patch4_window12_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swin_large_patch4_window12_384_in22k.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swin_large_patch4_window7_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swin_large_patch4_window7_224_in22k.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swin_s3_base_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swin_s3_small_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swin_s3_tiny_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swin_small_patch4_window7_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swin_tiny_patch4_window7_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_base_window12_192_22k.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_base_window12to16_192to256_22kft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_base_window12to24_192to384_22kft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_base_window16_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_base_window8_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_cr_base_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_cr_base_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_cr_base_ns_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_cr_giant_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_cr_giant_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_cr_huge_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_cr_huge_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_cr_large_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_cr_large_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_cr_small_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_cr_small_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_cr_small_ns_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_cr_tiny_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_cr_tiny_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_cr_tiny_ns_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_large_window12_192_22k.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_large_window12to16_192to256_22kft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_large_window12to24_192to384_22kft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_small_window16_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_small_window8_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_tiny_window16_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swinv2_tiny_window8_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swsl_resnet18.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swsl_resnet50.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swsl_resnext101_32x16d.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swsl_resnext101_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swsl_resnext101_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/swsl_resnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b0.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b0_ap.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b0_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b1.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b1_ap.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b1_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b2.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b2_ap.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b2_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b3.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b3_ap.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b3_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b4.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b4_ap.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b4_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b5.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b5_ap.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b5_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b6.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b6_ap.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b6_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b7.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b7_ap.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b7_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b8.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_b8_ap.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_cc_b0_4e.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_cc_b0_8e.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_cc_b1_8e.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_el.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_em.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_es.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_l2_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_l2_ns_475.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_lite0.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_lite1.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_lite2.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_lite3.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnet_lite4.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnetv2_b0.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnetv2_b1.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnetv2_b2.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnetv2_b3.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnetv2_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnetv2_l_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnetv2_l_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnetv2_m.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnetv2_m_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnetv2_m_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnetv2_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnetv2_s_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnetv2_s_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnetv2_xl_in21ft1k.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_efficientnetv2_xl_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_mixnet_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_mixnet_m.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_mixnet_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_mobilenetv3_large_075.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_mobilenetv3_large_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_mobilenetv3_large_minimal_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_mobilenetv3_small_075.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_mobilenetv3_small_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tf_mobilenetv3_small_minimal_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tinynet_a.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tinynet_b.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tinynet_c.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tinynet_d.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tinynet_e.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tnt_b_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tnt_s_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tv_resnet101.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tv_resnet152.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tv_resnet34.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tv_resnet50.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/tv_resnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/twins_pcpvt_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/twins_pcpvt_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/twins_pcpvt_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/twins_svt_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/twins_svt_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/twins_svt_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vgg11.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vgg11_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vgg13.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vgg13_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vgg16_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vgg19_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/visformer_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/visformer_tiny.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch16_18x2_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch16_224_dino.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch16_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch16_224_miil.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch16_224_miil_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch16_plus_240.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch16_rpn_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch32_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch32_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch32_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch32_plus_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch8_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch8_224_dino.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_base_patch8_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_giant_patch14_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_gigantic_patch14_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_huge_patch14_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_huge_patch14_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_large_patch14_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_large_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_large_patch16_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_large_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_large_patch32_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_large_patch32_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_large_patch32_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_relpos_base_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_relpos_base_patch16_cls_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_relpos_base_patch16_clsgap_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_relpos_base_patch16_plus_240.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_relpos_base_patch16_rpn_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_relpos_base_patch32_plus_rpn_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_relpos_medium_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_relpos_medium_patch16_cls_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_relpos_medium_patch16_rpn_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_relpos_small_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_relpos_small_patch16_rpn_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_small_patch16_18x2_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_small_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_small_patch16_224_dino.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_small_patch16_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_small_patch16_36x1_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_small_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_small_patch32_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_small_patch32_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_small_patch32_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_small_patch8_224_dino.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_srelpos_medium_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_srelpos_small_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_tiny_patch16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_tiny_patch16_224_in21k.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vit_tiny_patch16_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/volo_d1_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/volo_d1_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/volo_d2_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/volo_d2_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/volo_d3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/volo_d3_448.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/volo_d4_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/volo_d4_448.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/volo_d5_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/volo_d5_448.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/volo_d5_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vovnet39a.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/vovnet57a.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/wide_resnet101_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/wide_resnet50_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xception.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xception41.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xception41p.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xception65.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xception65p.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xception71.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_large_24_p16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_large_24_p16_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_large_24_p16_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_large_24_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_large_24_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_large_24_p8_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_medium_24_p16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_medium_24_p16_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_medium_24_p16_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_medium_24_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_medium_24_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_medium_24_p8_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_nano_12_p16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_nano_12_p16_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_nano_12_p16_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_nano_12_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_nano_12_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_nano_12_p8_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_small_12_p16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_small_12_p16_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_small_12_p16_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_small_12_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_small_12_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_small_12_p8_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_small_24_p16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_small_24_p16_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_small_24_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_small_24_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_small_24_p8_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_tiny_12_p16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_tiny_12_p16_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_tiny_12_p16_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_tiny_12_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_tiny_12_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_tiny_12_p8_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_tiny_24_p16_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_tiny_24_p16_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_tiny_24_p16_384_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_tiny_24_p8_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_tiny_24_p8_224_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/timm/xcit_tiny_24_p8_384_dist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.526608 turnkeyml-2.0.1/models/torch_hub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/alexnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/convnext_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/convnext_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/convnext_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/convnext_tiny.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/densenet121.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/densenet161.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/densenet169.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/densenet201.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/efficientnet_b1.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/efficientnet_v2_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/efficientnet_v2_m.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/efficientnet_v2_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/googlenet.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/hardnet39ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/hardnet68.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/hardnet68ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/hardnet85.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/mealv1_resnest50.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/mealv2_efficientnet_b0.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/mealv2_mobilenet_v3_large_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/mealv2_mobilenetv3_small_075.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/mealv2_mobilenetv3_small_100.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/mealv2_resnest50.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/mealv2_resnest50_380x380.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/mealv2_resnest50_cutmix.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/midas_v2.1_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/midas_v3_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/mnasnet0_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/mnasnet0_75.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/mnasnet1_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/mnasnet1_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/mobilenet_v3_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/mobilenet_v3_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/proxyless_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/proxyless_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/proxyless_mobile.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/proxyless_mobile_14.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/regnet_x_16gf.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/regnet_x_1_6gf.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/regnet_x_32gf.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/regnet_x_3_2gf.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/regnet_x_400mf.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/regnet_x_800mf.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/regnet_x_8gf.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/regnet_y_128gf.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/regnet_y_16gf.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/regnet_y_1_6gf.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/regnet_y_32gf.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/regnet_y_3_2gf.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/regnet_y_400mf.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/regnet_y_800mf.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/regnet_y_8gf.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnest101.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnest200.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnest269.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnest50.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnest50_fast_1s1x64d.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnest50_fast_1s2x40d.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnest50_fast_1s4x24d.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnest50_fast_2s1x64d.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnest50_fast_2s2x40d.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnest50_fast_4s1x64d.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnest50_fast_4s2x40d.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnet101.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnet101_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnet101_ibn_b.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnet152.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnet18.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnet18_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnet18_ibn_b.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnet34.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnet34_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnet34_ibn_b.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnet50.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnet50_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnet50_ibn_b.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnext101_32x8d.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnext101_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/resnext50_32x4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/se_resnet101_ibn_a.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/shufflenet_v2_x0_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/shufflenet_v2_x1_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/shufflenet_v2_x1_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/shufflenet_v2_x2_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/squeezenet1_0.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/squeezenet1_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/swin_b.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/swin_s.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/swin_t.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/vgg11.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/vgg11_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/vgg13.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/vgg13_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/vgg16_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/vgg19_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/vit_b_16.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/vit_b_32.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/vit_l_16.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/vit_l_32.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/wide_resnet101_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torch_hub/wide_resnet50_2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.526608 turnkeyml-2.0.1/models/torchvision/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torchvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torchvision/fasterrcnn_mobilenet_v3_large_320_fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torchvision/fasterrcnn_mobilenet_v3_large_fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torchvision/fasterrcnn_resnet50_fpn_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torchvision/fcos_resnet50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torchvision/maskrcnn_resnet50_fpn_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/torchvision/retinanet_resnet50_fpn_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.574609 turnkeyml-2.0.1/models/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/albert.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/albert_base_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/albert_large_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/albert_large_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/albert_xlarge_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/albert_xlarge_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/albert_xxlarge_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/albert_xxlarge_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/auto.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bart.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bart_large.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/barthez.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/barthez_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/barthez_summarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bartpho_syllable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bartpho_syllable_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bartpho_word.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bartpho_word_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bert.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bert_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bertjapanese.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bertjapanese_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bertlmhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bertweet.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bertweet_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bigbird.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bigbirdpegasus.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/biogpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/biogpt_large.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/blenderbot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/blenderbotsmall.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bloom.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bloom_1b1.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bloom_1b7.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bloom_3b.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/bloom_7b1.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/camembert.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/camembert_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/canine.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/codegen_350m.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/codegen_6b.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/convbert.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/convbert_medium_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/convbert_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/ctrl.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/ctrllmhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/deberta.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/deberta_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/deberta_xlarge.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/debertav2.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/debertav2_xxlarge.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/debertav3_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/debertav3_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/debertav3_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/debertav3_xsmall.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/distilbert.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/dpr_context_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/dpr_question_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/dpr_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/electra.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/electra_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/electra_generator_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/electra_generator_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/electra_generator_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/electra_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/encoderdecoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/ernie.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/ernie2_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/ernie2_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/ernie3_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/ernie3_medium.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/ernie3_micro.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/ernie3_mini.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/ernie3_nano.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/ernie_health.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/erniem.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/erniem_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/esm.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/esm2_150M.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/esm2_15B.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/esm2_35M.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/esm2_3B.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/esm2_650M.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/falcon_40b.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/falcon_7b.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/flaubert.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/flaubert_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/flaubert_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/flaubertwithlmhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/flaubertwithlmhead_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/flaubertwithlmhead_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/fnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/fnet_large.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/fsmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/fsmt_de_en.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/fsmt_en_de.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/fsmt_en_ru.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/funnel_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/funnel_intermediate_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/funnel_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/funnel_large_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/funnel_medium.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/funnel_medium_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/funnel_small_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/funnel_xlarge.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/funnel_xlarge_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/gpt2doubleheads.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/gpt2lmhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/gptbigcode.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/gptj.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/gptj_tiny.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/gptneo.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/gptneo_125M.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/gptneo_2B7.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/gptneox.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/gptneoxjapanese.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/ibert.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/ibert_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/led.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/led_large.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/llama2_13b.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/llama2_34b.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/llama2_70b.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/llama2_7b.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/longformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/longformer_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/longt5.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/longt5_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/longt5_tglobal_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/longt5_tglobal_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/longt5_tglobal_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/longt5encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/luke.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/luke_base_lite.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/luke_japanese_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/luke_japanese_base_lite.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/luke_japanese_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/luke_japanese_large_lite.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/luke_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/luke_large_lite.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/m2m100.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/m2m100_12B.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/m2m100_1B2.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/madlad400_10b.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/madlad400_3b.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/madlad400_7b.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/marian.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/markuplm.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/markuplm_large.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mbart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mbart_50.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mbarthez.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mega.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mistral_7b.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mixtral_7bx8.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mluke_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mluke_base_lite.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mluke_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mluke_large_lite.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mobilebert.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mpnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mpt_30b.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mpt_7b_8k.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mra.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mra_4096.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mt5.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mt5_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mt5_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mt5_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mt5_xxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mt5encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mt5encoder_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mt5encoder_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mt5encoder_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mt5encoder_xxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/mvp.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/nezha.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/nezha_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/nystromformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/nystromformer_1024.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/nystromformer_2048.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/nystromformer_4096.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/openaigpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/openaigptdoubleheads.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/openaigptlmhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/opt.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/opt_125m.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/opt_13B.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/opt_1B3.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/opt_2B7.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/opt_30B.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/opt_66B.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/opt_6B7.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/pegasus_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/pegasus_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/pegasus_x_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/pegasus_x_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/persimmon_8b.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/phi1.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/phi1point5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/phi2.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/phobert_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/phobert_large.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/plbart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/plbart_large.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/prophetnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/reformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/rembert.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/roberta.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/roberta_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/robertaprelayernorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/rocbert.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/roformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/roformer_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/splinter.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/splinter_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/squeezebert.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformers_base_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformers_base_16.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformers_base_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformers_base_32.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformers_base_64.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformers_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformers_xxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformersencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformersencoder_base_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformersencoder_base_16.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformersencoder_base_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformersencoder_base_32.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformersencoder_base_64.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformersencoder_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/switchtransformersencoder_xxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/t5.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/t5_11b.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/t5_3b.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/t5_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/t5_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/t5encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/t5encoder_11b.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/t5encoder_3b.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/t5encoder_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/t5encoder_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/t5v1dot1_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/t5v1dot1_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/t5v1dot1_small.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/t5v1dot1_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/t5v1dot1_xxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/transfoxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/transfoxllmhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/umt5.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/umt5_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/umt5_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/umt5_xxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/umt5encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/umt5encoder_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/umt5encoder_xl.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/umt5encoder_xxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xglm.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xglm_1B7.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xglm_2B9.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xglm_4B5.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xglm_7B5.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xlm.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xlm_1024.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xlm_1280.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xlmroberta.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xlmroberta_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xlmrobertaxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xlmrobertaxl_xxl.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xlmv.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xlmwithlmhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xlmwithlmhead_1024.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xlmwithlmhead_1280.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xlnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xlnet_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xlnetlmhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xlnetlmhead_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xmod.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xmod_base_13_125k.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xmod_base_30_125k.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xmod_base_30_195k.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xmod_base_60_125k.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xmod_base_60_265k.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xmod_base_75_125k.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xmod_base_75_269k.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/xmod_large.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/models/transformers/yoso.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 15:01:29.582609 turnkeyml-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.370606 turnkeyml-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.574609 turnkeyml-2.0.1/src/turnkeyml/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.574609 turnkeyml-2.0.1/src/turnkeyml/analyze/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/analyze/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    36655 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/analyze/script.py
--rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/analyze/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.578609 turnkeyml-2.0.1/src/turnkeyml/build/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/build/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/build/hummingbird.py
--rw-r--r--   0 runner    (1001) docker     (127)    19624 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/build/ignition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/build/onnx_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/build/sequences.py
--rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/build/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/build/tensor_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/build_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.578609 turnkeyml-2.0.1/src/turnkeyml/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20537 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/cli/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/cli/parser_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7821 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/cli/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/cli/spawn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.578609 turnkeyml-2.0.1/src/turnkeyml/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21414 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/common/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17450 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/common/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/common/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/common/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/common/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/common/printing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/common/tf_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16406 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/files_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.578609 turnkeyml-2.0.1/src/turnkeyml/run/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/run/basert.py
--rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/run/benchmark_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/run/devices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.582609 turnkeyml-2.0.1/src/turnkeyml/run/onnxrt/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/run/onnxrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/run/onnxrt/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/run/onnxrt/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/run/onnxrt/within_conda.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/run/plugin_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.582609 turnkeyml-2.0.1/src/turnkeyml/run/tensorrt/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/run/tensorrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/run/tensorrt/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/run/tensorrt/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.582609 turnkeyml-2.0.1/src/turnkeyml/run/torchrt/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/run/torchrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/run/torchrt/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-21 15:00:55.000000 turnkeyml-2.0.1/src/turnkeyml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:01:29.582609 turnkeyml-2.0.1/src/turnkeyml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13824 2024-03-21 15:01:29.000000 turnkeyml-2.0.1/src/turnkeyml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    44571 2024-03-21 15:01:29.000000 turnkeyml-2.0.1/src/turnkeyml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 15:01:29.000000 turnkeyml-2.0.1/src/turnkeyml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-21 15:01:29.000000 turnkeyml-2.0.1/src/turnkeyml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-21 15:01:29.000000 turnkeyml-2.0.1/src/turnkeyml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-21 15:01:29.000000 turnkeyml-2.0.1/src/turnkeyml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.650653 turnkeyml-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-04-02 19:24:00.650653 turnkeyml-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.446652 turnkeyml-2.0.2/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.446652 turnkeyml-2.0.2/models/graph_convolutions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/graph_convolutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/graph_convolutions/chebconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/graph_convolutions/dnaconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/graph_convolutions/feastconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/graph_convolutions/gatedgraphconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/graph_convolutions/generalconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/graph_convolutions/leconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/graph_convolutions/pnaconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/graph_convolutions/resgatedgraphconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/graph_convolutions/sageconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/graph_convolutions/tagconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.450652 turnkeyml-2.0.2/models/selftest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/selftest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/selftest/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/selftest/twolayer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.590653 turnkeyml-2.0.2/models/timm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/adv_inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/bat_resnext26ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/beit_base_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/beit_base_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/beit_large_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/beit_large_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/beit_large_patch16_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/botnet26t_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/botnet50ts_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cait_m36_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cait_m48_448.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cait_s24_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cait_s24_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cait_s36_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cait_xs24_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cait_xxs24_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cait_xxs24_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cait_xxs36_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cait_xxs36_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/coat_lite_mini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/coat_lite_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/coat_lite_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/coat_mini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/coat_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convit_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convit_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convit_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convmixer_1024_20_ks9_p14.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convmixer_1536_20.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convmixer_768_32.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_base_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_base_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_base_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_large_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_large_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_large_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_nano.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_nano_ols.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_small_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_small_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_small_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_tiny_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_tiny_hnf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_tiny_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_tiny_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_xlarge_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_xlarge_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/convnext_xlarge_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/crossvit_15_240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/crossvit_15_dagger_240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/crossvit_15_dagger_408.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/crossvit_18_240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/crossvit_18_dagger_240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/crossvit_18_dagger_408.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/crossvit_9_240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/crossvit_9_dagger_240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/crossvit_base_240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/crossvit_small_240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/crossvit_tiny_240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cs3darknet_focus_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cs3darknet_focus_m.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cs3darknet_focus_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cs3darknet_focus_x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cs3darknet_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cs3darknet_m.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cs3darknet_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cs3darknet_x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cs3edgenet_x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cs3se_edgenet_x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cs3sedarknet_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cs3sedarknet_x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cs3sedarknet_xdw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cspdarknet53.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cspresnet50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cspresnet50d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cspresnet50w.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/cspresnext50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/darknet17.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/darknet21.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/darknet53.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/darknetaa53.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit3_base_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit3_base_patch16_224_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit3_base_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit3_base_patch16_384_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit3_huge_patch14_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit3_huge_patch14_224_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit3_large_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit3_large_patch16_224_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit3_large_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit3_large_patch16_384_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit3_small_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit3_small_patch16_224_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit3_small_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit3_small_patch16_384_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit_base_distilled_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit_base_distilled_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit_base_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit_base_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit_small_distilled_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit_small_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit_tiny_distilled_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/deit_tiny_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/densenet121.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/densenet161.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/densenet169.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/densenet201.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/densenetblur121d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dla102.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dla102x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dla102x2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dla169.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dla34.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dla46_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dla46x_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dla60.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dla60_res2net.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dla60_res2next.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dla60x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dla60x_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dm_nfnet_f0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dm_nfnet_f1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dm_nfnet_f2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dm_nfnet_f3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dm_nfnet_f4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dm_nfnet_f5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dm_nfnet_f6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dpn107.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dpn131.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dpn68.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dpn68b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dpn92.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/dpn98.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/eca_botnext26ts_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/eca_halonext26ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/eca_nfnet_l0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/eca_nfnet_l1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/eca_nfnet_l2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/eca_nfnet_l3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/eca_resnet33ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/eca_resnext26ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/eca_vovnet39b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ecaresnet101d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ecaresnet200d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ecaresnet269d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ecaresnet26t.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ecaresnet50d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ecaresnet50t.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ecaresnetlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ecaresnext26t_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ecaresnext50t_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/edgenext_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/edgenext_small_rw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/edgenext_x_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/edgenext_xx_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b0_g16_evos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b0_g8_gn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b0_gn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b2a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b3_g8_gn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b3_gn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b3a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_b8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_cc_b0_4e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_cc_b0_8e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_cc_b1_8e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_el.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_el_pruned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_em.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_es_pruned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_l2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_lite0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_lite1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_lite2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_lite3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnet_lite4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnetv2_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnetv2_m.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnetv2_rw_m.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnetv2_rw_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnetv2_rw_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnetv2_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/efficientnetv2_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ens_adv_inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ese_vovnet19b_dw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ese_vovnet19b_slim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ese_vovnet19b_slim_dw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ese_vovnet39b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ese_vovnet39b_evos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ese_vovnet57b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ese_vovnet99b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/fbnetc_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/fbnetv3_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/fbnetv3_d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/fbnetv3_g.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gc_efficientnetv2_rw_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gcresnet33ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gcresnet50t.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gcresnext26ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gcresnext50ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gernet_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gernet_m.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gernet_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ghostnet_050.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ghostnet_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ghostnet_130.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnet101_v1b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnet101_v1c.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnet101_v1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnet101_v1s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnet152_v1b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnet152_v1c.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnet152_v1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnet152_v1s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnet18_v1b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnet34_v1b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnet50_v1b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnet50_v1c.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnet50_v1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnet50_v1s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnext101_64x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_resnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_senet154.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_seresnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_seresnext101_64x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gluon_seresnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gmixer_12_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gmixer_24_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gmlp_b16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gmlp_s16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/gmlp_ti16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/halo2botnet50ts_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/halonet26t.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/halonet50ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/halonet_h1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/haloregnetz_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/hardcorenas_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/hardcorenas_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/hardcorenas_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/hardcorenas_d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/hardcorenas_e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/hardcorenas_f.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/hrnet_w18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/hrnet_w18_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/hrnet_w18_small_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/hrnet_w30.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/hrnet_w32.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/hrnet_w40.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/hrnet_w44.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/hrnet_w48.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/hrnet_w64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ig_resnext101_32x16d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ig_resnext101_32x32d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ig_resnext101_32x48d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ig_resnext101_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/inception_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/jx_nest_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/jx_nest_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/jx_nest_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/lambda_resnet26rpt_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/lambda_resnet26t.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/lambda_resnet50ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/lamhalobotnet50ts_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/lcnet_035.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/lcnet_050.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/lcnet_075.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/lcnet_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/lcnet_150.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/legacy_senet154.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/legacy_seresnet101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/legacy_seresnet152.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/legacy_seresnet18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/legacy_seresnet34.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/legacy_seresnet50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/legacy_seresnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/legacy_seresnext26_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/legacy_seresnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/levit_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/levit_128s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/levit_192.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/levit_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/levit_256d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/levit_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mixer_b16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mixer_b16_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mixer_b16_224_miil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mixer_b16_224_miil_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mixer_b32_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mixer_l16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mixer_l16_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mixer_l32_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mixer_s16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mixer_s32_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mixnet_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mixnet_m.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mixnet_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mixnet_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mixnet_xxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mnasnet_050.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mnasnet_075.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mnasnet_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mnasnet_140.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mnasnet_a1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mnasnet_b1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mnasnet_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilenetv2_035.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilenetv2_050.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilenetv2_075.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilenetv2_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilenetv2_110d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilenetv2_120d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilenetv2_140.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilenetv3_large_075.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilenetv3_large_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilenetv3_large_100_miil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilenetv3_large_100_miil_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilenetv3_rw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilenetv3_small_050.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilenetv3_small_075.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilenetv3_small_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevit_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevit_xs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevit_xxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevitv2_050.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevitv2_075.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevitv2_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevitv2_125.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevitv2_150.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevitv2_150_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevitv2_150_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevitv2_175.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevitv2_175_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevitv2_175_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevitv2_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevitv2_200_384_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/mobilevitv2_200_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nasnetalarge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nest_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nest_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nest_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nf_ecaresnet101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nf_ecaresnet26.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nf_ecaresnet50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nf_regnet_b0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nf_regnet_b1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nf_regnet_b2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nf_regnet_b3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nf_regnet_b4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nf_regnet_b5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nf_resnet101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nf_resnet26.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nf_resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nf_seresnet101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nf_seresnet26.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nf_seresnet50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nfnet_f0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nfnet_f1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nfnet_f2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nfnet_f3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nfnet_f4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nfnet_f5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nfnet_f6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nfnet_f7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/nfnet_l0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/pit_b_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/pit_b_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/pit_s_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/pit_s_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/pit_ti_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/pit_ti_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/pit_xs_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/pit_xs_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/pnasnet5large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/poolformer_m36.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/poolformer_m48.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/poolformer_s12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/poolformer_s24.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/poolformer_s36.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetv_040.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetv_064.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetx_002.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetx_004.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetx_006.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetx_008.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetx_016.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetx_032.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetx_040.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetx_064.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetx_080.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetx_120.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetx_160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetx_320.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnety_002.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnety_004.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnety_006.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnety_008.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnety_016.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnety_032.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnety_040.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnety_064.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnety_080.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnety_120.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnety_160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnety_320.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetz_005.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetz_040.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetz_040h.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetz_b16.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetz_b16_evos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetz_c16.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetz_c16_evos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetz_d32.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetz_d8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetz_d8_evos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/regnetz_e8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/repvgg_a2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/repvgg_b0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/repvgg_b1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/repvgg_b1g4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/repvgg_b2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/repvgg_b2g4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/repvgg_b3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/repvgg_b3g4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/res2net101_26w_4s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/res2net50_14w_8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/res2net50_26w_4s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/res2net50_26w_6s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/res2net50_26w_8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/res2net50_48w_2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/res2next50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resmlp_12_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resmlp_12_224_dino.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resmlp_12_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resmlp_24_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resmlp_24_224_dino.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resmlp_24_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resmlp_36_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resmlp_36_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resmlp_big_24_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resmlp_big_24_224_in22ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resmlp_big_24_distilled_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnest101e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnest14d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnest200e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnest269e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnest26d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnest50d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnest50d_1s4x24d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnest50d_4s2x40d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet101d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet10t.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet14t.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet152.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet152d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet18d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet200d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet26.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet26d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet26t.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet32ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet33ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet34.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet34d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet50_gn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet50d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet50t.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet51q.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnet61q.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetaa101d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetaa50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetaa50d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetblur101d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetblur18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetblur50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetblur50d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetrs101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetrs152.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetrs200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetrs270.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetrs350.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetrs420.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetrs50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_101d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_101x1_bitm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_101x1_bitm_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_101x3_bitm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_101x3_bitm_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_152.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_152d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_152x2_bit_teacher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_152x2_bit_teacher_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_152x2_bitm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_152x2_bitm_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_152x4_bitm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_152x4_bitm_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_50d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_50d_evos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_50d_frn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_50d_gn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_50t.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_50x1_bit_distilled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_50x1_bitm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_50x1_bitm_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_50x3_bitm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnetv2_50x3_bitm_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnext101_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnext101_64x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnext26ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/resnext50d_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/rexnet_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/rexnet_130.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/rexnet_150.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/rexnet_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/rexnetr_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/rexnetr_130.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/rexnetr_150.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/rexnetr_200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/sebotnet33ts_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/sedarknet21.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/sehalonet33ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/selecsls42.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/selecsls42b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/selecsls60.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/selecsls60b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/selecsls84.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/semnasnet_050.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/semnasnet_075.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/semnasnet_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/semnasnet_140.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/senet154.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/sequencer2d_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/sequencer2d_m.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/sequencer2d_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnet101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnet152.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnet152d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnet18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnet200d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnet269d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnet33ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnet34.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnet50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnet50t.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnetaa50d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnext101_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnext101d_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnext26d_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnext26t_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnext26tn_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnext26ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/seresnextaa101d_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/skresnet18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/skresnet34.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/skresnet50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/skresnet50d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/skresnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/spnasnet_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ssl_resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ssl_resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ssl_resnext101_32x16d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ssl_resnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ssl_resnext101_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/ssl_resnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swin_base_patch4_window12_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swin_base_patch4_window12_384_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swin_base_patch4_window7_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swin_base_patch4_window7_224_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swin_large_patch4_window12_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swin_large_patch4_window12_384_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swin_large_patch4_window7_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swin_large_patch4_window7_224_in22k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swin_s3_base_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swin_s3_small_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swin_s3_tiny_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swin_small_patch4_window7_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swin_tiny_patch4_window7_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_base_window12_192_22k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_base_window12to16_192to256_22kft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_base_window12to24_192to384_22kft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_base_window16_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_base_window8_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_cr_base_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_cr_base_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_cr_base_ns_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_cr_giant_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_cr_giant_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_cr_huge_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_cr_huge_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_cr_large_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_cr_large_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_cr_small_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_cr_small_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_cr_small_ns_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_cr_tiny_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_cr_tiny_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_cr_tiny_ns_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_large_window12_192_22k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_large_window12to16_192to256_22kft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_large_window12to24_192to384_22kft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_small_window16_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_small_window8_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_tiny_window16_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swinv2_tiny_window8_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swsl_resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swsl_resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swsl_resnext101_32x16d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swsl_resnext101_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swsl_resnext101_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/swsl_resnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b0_ap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b0_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b1_ap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b1_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b2_ap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b2_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b3_ap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b3_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b4_ap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b4_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b5_ap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b5_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b6_ap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b6_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b7_ap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b7_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_b8_ap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_cc_b0_4e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_cc_b0_8e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_cc_b1_8e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_el.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_em.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_l2_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_l2_ns_475.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_lite0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_lite1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_lite2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_lite3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnet_lite4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnetv2_b0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnetv2_b1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnetv2_b2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnetv2_b3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnetv2_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnetv2_l_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnetv2_l_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnetv2_m.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnetv2_m_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnetv2_m_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnetv2_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnetv2_s_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnetv2_s_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnetv2_xl_in21ft1k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_efficientnetv2_xl_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_mixnet_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_mixnet_m.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_mixnet_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_mobilenetv3_large_075.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_mobilenetv3_large_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_mobilenetv3_large_minimal_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_mobilenetv3_small_075.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_mobilenetv3_small_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tf_mobilenetv3_small_minimal_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tinynet_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tinynet_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tinynet_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tinynet_d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tinynet_e.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tnt_b_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tnt_s_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tv_resnet101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tv_resnet152.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tv_resnet34.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tv_resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/tv_resnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/twins_pcpvt_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/twins_pcpvt_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/twins_pcpvt_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/twins_svt_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/twins_svt_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/twins_svt_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vgg11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vgg11_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vgg13.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vgg13_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vgg16_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vgg19_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/visformer_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/visformer_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch16_18x2_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch16_224_dino.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch16_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch16_224_miil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch16_224_miil_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch16_plus_240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch16_rpn_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch32_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch32_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch32_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch32_plus_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch8_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch8_224_dino.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_base_patch8_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_giant_patch14_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_gigantic_patch14_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_huge_patch14_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_huge_patch14_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_large_patch14_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_large_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_large_patch16_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_large_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_large_patch32_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_large_patch32_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_large_patch32_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_relpos_base_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_relpos_base_patch16_cls_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_relpos_base_patch16_clsgap_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_relpos_base_patch16_plus_240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_relpos_base_patch16_rpn_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_relpos_base_patch32_plus_rpn_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_relpos_medium_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_relpos_medium_patch16_cls_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_relpos_medium_patch16_rpn_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_relpos_small_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_relpos_small_patch16_rpn_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_small_patch16_18x2_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_small_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_small_patch16_224_dino.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_small_patch16_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_small_patch16_36x1_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_small_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_small_patch32_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_small_patch32_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_small_patch32_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_small_patch8_224_dino.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_srelpos_medium_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_srelpos_small_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_tiny_patch16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_tiny_patch16_224_in21k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vit_tiny_patch16_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/volo_d1_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/volo_d1_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/volo_d2_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/volo_d2_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/volo_d3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/volo_d3_448.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/volo_d4_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/volo_d4_448.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/volo_d5_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/volo_d5_448.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/volo_d5_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vovnet39a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/vovnet57a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/wide_resnet101_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/wide_resnet50_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xception41.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xception41p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xception65.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xception65p.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xception71.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_large_24_p16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_large_24_p16_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_large_24_p16_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_large_24_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_large_24_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_large_24_p8_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_medium_24_p16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_medium_24_p16_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_medium_24_p16_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_medium_24_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_medium_24_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_medium_24_p8_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_nano_12_p16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_nano_12_p16_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_nano_12_p16_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_nano_12_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_nano_12_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_nano_12_p8_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_small_12_p16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_small_12_p16_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_small_12_p16_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_small_12_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_small_12_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_small_12_p8_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_small_24_p16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_small_24_p16_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_small_24_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_small_24_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_small_24_p8_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_tiny_12_p16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_tiny_12_p16_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_tiny_12_p16_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_tiny_12_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_tiny_12_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_tiny_12_p8_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_tiny_24_p16_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_tiny_24_p16_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_tiny_24_p16_384_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_tiny_24_p8_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_tiny_24_p8_224_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/timm/xcit_tiny_24_p8_384_dist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.602653 turnkeyml-2.0.2/models/torch_hub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/alexnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/convnext_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/convnext_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/convnext_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/convnext_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/densenet121.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/densenet161.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/densenet169.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/densenet201.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/efficientnet_b1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/efficientnet_v2_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/efficientnet_v2_m.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/efficientnet_v2_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/googlenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/hardnet39ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/hardnet68.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/hardnet68ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/hardnet85.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/mealv1_resnest50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/mealv2_efficientnet_b0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/mealv2_mobilenet_v3_large_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/mealv2_mobilenetv3_small_075.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/mealv2_mobilenetv3_small_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/mealv2_resnest50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/mealv2_resnest50_380x380.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/mealv2_resnest50_cutmix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/midas_v2.1_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/midas_v3_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/mnasnet0_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/mnasnet0_75.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/mnasnet1_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/mnasnet1_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/mobilenet_v3_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/mobilenet_v3_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/proxyless_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/proxyless_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/proxyless_mobile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/proxyless_mobile_14.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/regnet_x_16gf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/regnet_x_1_6gf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/regnet_x_32gf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/regnet_x_3_2gf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/regnet_x_400mf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/regnet_x_800mf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/regnet_x_8gf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/regnet_y_128gf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/regnet_y_16gf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/regnet_y_1_6gf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/regnet_y_32gf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/regnet_y_3_2gf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/regnet_y_400mf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/regnet_y_800mf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/regnet_y_8gf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnest101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnest200.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnest269.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnest50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnest50_fast_1s1x64d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnest50_fast_1s2x40d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnest50_fast_1s4x24d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnest50_fast_2s1x64d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnest50_fast_2s2x40d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnest50_fast_4s1x64d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnest50_fast_4s2x40d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnet101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnet101_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnet101_ibn_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnet152.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnet18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnet18_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnet18_ibn_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnet34.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnet34_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnet34_ibn_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnet50.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnet50_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnet50_ibn_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnext101_32x8d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnext101_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/resnext50_32x4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/se_resnet101_ibn_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/shufflenet_v2_x0_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/shufflenet_v2_x1_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/shufflenet_v2_x1_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/shufflenet_v2_x2_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/squeezenet1_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/squeezenet1_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/swin_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/swin_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/swin_t.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/vgg11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/vgg11_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/vgg13.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/vgg13_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/vgg16_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/vgg19_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/vit_b_16.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/vit_b_32.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/vit_l_16.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/vit_l_32.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/wide_resnet101_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torch_hub/wide_resnet50_2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.602653 turnkeyml-2.0.2/models/torchvision/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torchvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torchvision/fasterrcnn_mobilenet_v3_large_320_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torchvision/fasterrcnn_mobilenet_v3_large_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torchvision/fasterrcnn_resnet50_fpn_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torchvision/fcos_resnet50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torchvision/maskrcnn_resnet50_fpn_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/torchvision/retinanet_resnet50_fpn_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.642653 turnkeyml-2.0.2/models/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/albert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/albert_base_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/albert_large_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/albert_large_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/albert_xlarge_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/albert_xlarge_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/albert_xxlarge_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/albert_xxlarge_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bart_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/barthez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/barthez_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/barthez_summarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bartpho_syllable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bartpho_syllable_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bartpho_word.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bartpho_word_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bert_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bertjapanese.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bertjapanese_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bertlmhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bertweet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bertweet_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bigbird.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bigbirdpegasus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/biogpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/biogpt_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/blenderbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/blenderbotsmall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bloom_1b1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bloom_1b7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bloom_3b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/bloom_7b1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/camembert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/camembert_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/canine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/codegen_350m.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/codegen_6b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/convbert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/convbert_medium_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/convbert_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/ctrllmhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/deberta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/deberta_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/deberta_xlarge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/debertav2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/debertav2_xxlarge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/debertav3_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/debertav3_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/debertav3_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/debertav3_xsmall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/distilbert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/dpr_context_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/dpr_question_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/dpr_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/electra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/electra_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/electra_generator_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/electra_generator_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/electra_generator_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/electra_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/encoderdecoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/ernie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/ernie2_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/ernie2_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/ernie3_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/ernie3_medium.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/ernie3_micro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/ernie3_mini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/ernie3_nano.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/ernie_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/erniem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/erniem_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/esm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/esm2_150M.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/esm2_15B.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/esm2_35M.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/esm2_3B.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/esm2_650M.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/falcon_40b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/falcon_7b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/flaubert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/flaubert_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/flaubert_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/flaubertwithlmhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/flaubertwithlmhead_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/flaubertwithlmhead_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/fnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/fnet_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/fsmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/fsmt_de_en.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/fsmt_en_de.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/fsmt_en_ru.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/funnel_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/funnel_intermediate_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/funnel_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/funnel_large_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/funnel_medium.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/funnel_medium_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/funnel_small_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/funnel_xlarge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/funnel_xlarge_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/gpt2doubleheads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/gpt2lmhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/gptbigcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/gptj.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/gptj_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/gptneo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/gptneo_125M.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/gptneo_2B7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/gptneox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/gptneoxjapanese.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/ibert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/ibert_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/led.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/led_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/llama2_13b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/llama2_34b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/llama2_70b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/llama2_7b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/longformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/longformer_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/longt5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/longt5_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/longt5_tglobal_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/longt5_tglobal_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/longt5_tglobal_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/longt5encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/luke.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/luke_base_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/luke_japanese_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/luke_japanese_base_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/luke_japanese_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/luke_japanese_large_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/luke_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/luke_large_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/m2m100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/m2m100_12B.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/m2m100_1B2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/madlad400_10b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/madlad400_3b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/madlad400_7b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/marian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/markuplm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/markuplm_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mbart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mbart_50.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mbarthez.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mega.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mistral_7b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mixtral_7bx8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mluke_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mluke_base_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mluke_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mluke_large_lite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mobilebert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mpnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mpt_30b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mpt_7b_8k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mra_4096.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mt5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mt5_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mt5_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mt5_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mt5_xxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mt5encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mt5encoder_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mt5encoder_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mt5encoder_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mt5encoder_xxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/mvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/nezha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/nezha_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/nystromformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/nystromformer_1024.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/nystromformer_2048.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/nystromformer_4096.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/openaigpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/openaigptdoubleheads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/openaigptlmhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/opt_125m.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/opt_13B.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/opt_1B3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/opt_2B7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/opt_30B.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/opt_66B.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/opt_6B7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/pegasus_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/pegasus_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/pegasus_x_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/pegasus_x_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/persimmon_8b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/phi1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/phi1point5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/phi2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/phobert_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/phobert_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/plbart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/plbart_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/prophetnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/reformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/rembert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/roberta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/roberta_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/robertaprelayernorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/rocbert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/roformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/roformer_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/splinter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/splinter_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/squeezebert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformers_base_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformers_base_16.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformers_base_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformers_base_32.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformers_base_64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformers_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformers_xxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformersencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformersencoder_base_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformersencoder_base_16.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformersencoder_base_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformersencoder_base_32.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformersencoder_base_64.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformersencoder_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/switchtransformersencoder_xxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/t5_11b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/t5_3b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/t5_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/t5_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/t5encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/t5encoder_11b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/t5encoder_3b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/t5encoder_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/t5encoder_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/t5v1dot1_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/t5v1dot1_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/t5v1dot1_small.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/t5v1dot1_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/t5v1dot1_xxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/transfoxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/transfoxllmhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/umt5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/umt5_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/umt5_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/umt5_xxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/umt5encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/umt5encoder_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/umt5encoder_xl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/umt5encoder_xxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xglm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xglm_1B7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xglm_2B9.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xglm_4B5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xglm_7B5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xlm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xlm_1024.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xlm_1280.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xlmroberta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xlmroberta_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xlmrobertaxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xlmrobertaxl_xxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xlmv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xlmwithlmhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xlmwithlmhead_1024.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xlmwithlmhead_1280.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xlnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xlnet_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xlnetlmhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xlnetlmhead_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xmod_base_13_125k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xmod_base_30_125k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xmod_base_30_195k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xmod_base_60_125k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xmod_base_60_265k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xmod_base_75_125k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xmod_base_75_269k.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/xmod_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/models/transformers/yoso.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:24:00.650653 turnkeyml-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.442652 turnkeyml-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.642653 turnkeyml-2.0.2/src/turnkeyml/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.646653 turnkeyml-2.0.2/src/turnkeyml/analyze/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/analyze/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36655 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/analyze/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/analyze/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.646653 turnkeyml-2.0.2/src/turnkeyml/build/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/build/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/build/hummingbird.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19624 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/build/ignition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/build/onnx_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/build/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/build/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/build/tensor_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/build_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.646653 turnkeyml-2.0.2/src/turnkeyml/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20537 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/cli/parser_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7821 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/cli/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14403 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/cli/spawn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.650653 turnkeyml-2.0.2/src/turnkeyml/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21414 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/common/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17450 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/common/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/common/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/common/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/common/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/common/printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/common/tf_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16406 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/files_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.650653 turnkeyml-2.0.2/src/turnkeyml/run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/run/basert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11271 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/run/benchmark_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/run/devices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.650653 turnkeyml-2.0.2/src/turnkeyml/run/onnxrt/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/run/onnxrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/run/onnxrt/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/run/onnxrt/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/run/onnxrt/within_conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/run/plugin_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.650653 turnkeyml-2.0.2/src/turnkeyml/run/tensorrt/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/run/tensorrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/run/tensorrt/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/run/tensorrt/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.650653 turnkeyml-2.0.2/src/turnkeyml/run/torchrt/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/run/torchrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/run/torchrt/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 19:23:39.000000 turnkeyml-2.0.2/src/turnkeyml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:24:00.650653 turnkeyml-2.0.2/src/turnkeyml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-04-02 19:24:00.000000 turnkeyml-2.0.2/src/turnkeyml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    44571 2024-04-02 19:24:00.000000 turnkeyml-2.0.2/src/turnkeyml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:24:00.000000 turnkeyml-2.0.2/src/turnkeyml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 19:24:00.000000 turnkeyml-2.0.2/src/turnkeyml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-02 19:24:00.000000 turnkeyml-2.0.2/src/turnkeyml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:24:00.000000 turnkeyml-2.0.2/src/turnkeyml.egg-info/top_level.txt
```

### Comparing `turnkeyml-2.0.1/LICENSE` & `turnkeyml-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/NOTICE.md` & `turnkeyml-2.0.2/NOTICE.md`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/PKG-INFO` & `turnkeyml-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: turnkeyml
-Version: 2.0.1
+Version: 2.0.2
 Summary: TurnkeyML Tools and Models
 Author: Jeremy Fowers, Daniel Holanda, Ramakrishnan Sivakumar, Victoria Godsoe
 Author-email: jeremy.fowers@amd.com, daniel.holandanoronha@amd.com, krishna.sivakumar@amd.com, victoria.godsoe@amd.com
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE.md
 Requires-Dist: invoke>=2.0.0
 Requires-Dist: onnx>=1.11.0
 Requires-Dist: onnxmltools==1.10.0
 Requires-Dist: hummingbird-ml==0.4.4
 Requires-Dist: scikit-learn==1.1.1
 Requires-Dist: xgboost==1.6.1
 Requires-Dist: lightgbm==3.3.5
-Requires-Dist: onnxruntime<1.16.0,>=1.10.1
+Requires-Dist: onnxruntime>=1.10.1
 Requires-Dist: torch>=1.12.1
 Requires-Dist: protobuf<3.21,>=3.17.3
 Requires-Dist: pyyaml>=5.4
 Requires-Dist: typeguard>=2.3.13
 Requires-Dist: packaging>=20.9
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: fasteners
```

### Comparing `turnkeyml-2.0.1/README.md` & `turnkeyml-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/graph_convolutions/chebconv.py` & `turnkeyml-2.0.2/models/graph_convolutions/chebconv.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/graph_convolutions/dnaconv.py` & `turnkeyml-2.0.2/models/graph_convolutions/dnaconv.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/graph_convolutions/feastconv.py` & `turnkeyml-2.0.2/models/graph_convolutions/feastconv.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/graph_convolutions/gatedgraphconv.py` & `turnkeyml-2.0.2/models/graph_convolutions/gatedgraphconv.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/graph_convolutions/generalconv.py` & `turnkeyml-2.0.2/models/graph_convolutions/generalconv.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/graph_convolutions/leconv.py` & `turnkeyml-2.0.2/models/graph_convolutions/leconv.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/graph_convolutions/pnaconv.py` & `turnkeyml-2.0.2/models/graph_convolutions/pnaconv.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/graph_convolutions/resgatedgraphconv.py` & `turnkeyml-2.0.2/models/graph_convolutions/resgatedgraphconv.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/graph_convolutions/sageconv.py` & `turnkeyml-2.0.2/models/graph_convolutions/sageconv.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/graph_convolutions/tagconv.py` & `turnkeyml-2.0.2/models/graph_convolutions/tagconv.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/readme.md` & `turnkeyml-2.0.2/models/readme.md`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/selftest/linear.py` & `turnkeyml-2.0.2/models/selftest/linear.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/selftest/twolayer.py` & `turnkeyml-2.0.2/models/selftest/twolayer.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/adv_inception_v3.py` & `turnkeyml-2.0.2/models/timm/adv_inception_v3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/bat_resnext26ts.py` & `turnkeyml-2.0.2/models/timm/bat_resnext26ts.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/beit_base_patch16_224.py` & `turnkeyml-2.0.2/models/timm/beit_base_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/beit_base_patch16_384.py` & `turnkeyml-2.0.2/models/timm/beit_base_patch16_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/beit_large_patch16_224.py` & `turnkeyml-2.0.2/models/timm/beit_large_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/beit_large_patch16_384.py` & `turnkeyml-2.0.2/models/timm/beit_large_patch16_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/beit_large_patch16_512.py` & `turnkeyml-2.0.2/models/timm/beit_large_patch16_512.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/botnet26t_256.py` & `turnkeyml-2.0.2/models/timm/botnet26t_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/botnet50ts_256.py` & `turnkeyml-2.0.2/models/timm/botnet50ts_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cait_m36_384.py` & `turnkeyml-2.0.2/models/timm/cait_m36_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cait_m48_448.py` & `turnkeyml-2.0.2/models/timm/cait_m48_448.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cait_s24_224.py` & `turnkeyml-2.0.2/models/timm/cait_s24_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cait_s24_384.py` & `turnkeyml-2.0.2/models/timm/cait_s24_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cait_s36_384.py` & `turnkeyml-2.0.2/models/timm/cait_s36_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cait_xs24_384.py` & `turnkeyml-2.0.2/models/timm/cait_xs24_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cait_xxs24_224.py` & `turnkeyml-2.0.2/models/timm/cait_xxs24_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cait_xxs24_384.py` & `turnkeyml-2.0.2/models/timm/cait_xxs24_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cait_xxs36_224.py` & `turnkeyml-2.0.2/models/timm/cait_xxs36_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cait_xxs36_384.py` & `turnkeyml-2.0.2/models/timm/cait_xxs36_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/coat_lite_mini.py` & `turnkeyml-2.0.2/models/timm/coat_lite_mini.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/coat_lite_small.py` & `turnkeyml-2.0.2/models/timm/coat_lite_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/coat_lite_tiny.py` & `turnkeyml-2.0.2/models/timm/coat_lite_tiny.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/coat_mini.py` & `turnkeyml-2.0.2/models/timm/coat_mini.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/coat_tiny.py` & `turnkeyml-2.0.2/models/timm/coat_tiny.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convit_base.py` & `turnkeyml-2.0.2/models/timm/convit_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convit_small.py` & `turnkeyml-2.0.2/models/timm/convit_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convit_tiny.py` & `turnkeyml-2.0.2/models/timm/convit_tiny.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convmixer_1024_20_ks9_p14.py` & `turnkeyml-2.0.2/models/timm/convmixer_1024_20_ks9_p14.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convmixer_1536_20.py` & `turnkeyml-2.0.2/models/timm/convmixer_1536_20.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convmixer_768_32.py` & `turnkeyml-2.0.2/models/timm/convmixer_768_32.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_base.py` & `turnkeyml-2.0.2/models/timm/convnext_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_base_384_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/convnext_base_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_base_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/convnext_base_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_base_in22k.py` & `turnkeyml-2.0.2/models/timm/convnext_base_in22k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_large.py` & `turnkeyml-2.0.2/models/timm/convnext_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_large_384_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/convnext_large_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_large_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/convnext_large_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_large_in22k.py` & `turnkeyml-2.0.2/models/timm/convnext_large_in22k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_nano.py` & `turnkeyml-2.0.2/models/timm/convnext_nano.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_nano_ols.py` & `turnkeyml-2.0.2/models/timm/convnext_nano_ols.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_small.py` & `turnkeyml-2.0.2/models/timm/convnext_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_small_384_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/convnext_small_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_small_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/convnext_small_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_small_in22k.py` & `turnkeyml-2.0.2/models/timm/convnext_small_in22k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_tiny.py` & `turnkeyml-2.0.2/models/timm/convnext_tiny.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_tiny_384_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/convnext_tiny_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_tiny_hnf.py` & `turnkeyml-2.0.2/models/timm/convnext_tiny_hnf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_tiny_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/convnext_tiny_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_tiny_in22k.py` & `turnkeyml-2.0.2/models/timm/convnext_tiny_in22k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_xlarge_384_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/convnext_xlarge_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_xlarge_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/convnext_xlarge_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/convnext_xlarge_in22k.py` & `turnkeyml-2.0.2/models/timm/convnext_xlarge_in22k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/crossvit_15_240.py` & `turnkeyml-2.0.2/models/timm/crossvit_15_240.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/crossvit_15_dagger_240.py` & `turnkeyml-2.0.2/models/timm/crossvit_15_dagger_240.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/crossvit_15_dagger_408.py` & `turnkeyml-2.0.2/models/timm/crossvit_15_dagger_408.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/crossvit_18_240.py` & `turnkeyml-2.0.2/models/timm/crossvit_18_240.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/crossvit_18_dagger_240.py` & `turnkeyml-2.0.2/models/timm/crossvit_18_dagger_240.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/crossvit_18_dagger_408.py` & `turnkeyml-2.0.2/models/timm/crossvit_18_dagger_408.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/crossvit_9_240.py` & `turnkeyml-2.0.2/models/timm/crossvit_9_240.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/crossvit_9_dagger_240.py` & `turnkeyml-2.0.2/models/timm/crossvit_9_dagger_240.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/crossvit_base_240.py` & `turnkeyml-2.0.2/models/timm/crossvit_base_240.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/crossvit_small_240.py` & `turnkeyml-2.0.2/models/timm/crossvit_small_240.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/crossvit_tiny_240.py` & `turnkeyml-2.0.2/models/timm/crossvit_tiny_240.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cs3darknet_focus_l.py` & `turnkeyml-2.0.2/models/timm/cs3darknet_focus_l.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cs3darknet_focus_m.py` & `turnkeyml-2.0.2/models/timm/cs3darknet_focus_m.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cs3darknet_focus_s.py` & `turnkeyml-2.0.2/models/timm/cs3darknet_focus_s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cs3darknet_focus_x.py` & `turnkeyml-2.0.2/models/timm/cs3darknet_focus_x.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cs3darknet_l.py` & `turnkeyml-2.0.2/models/timm/cs3darknet_l.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cs3darknet_m.py` & `turnkeyml-2.0.2/models/timm/cs3darknet_m.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cs3darknet_s.py` & `turnkeyml-2.0.2/models/timm/cs3darknet_s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cs3darknet_x.py` & `turnkeyml-2.0.2/models/timm/cs3darknet_x.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cs3edgenet_x.py` & `turnkeyml-2.0.2/models/timm/cs3edgenet_x.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cs3se_edgenet_x.py` & `turnkeyml-2.0.2/models/timm/cs3se_edgenet_x.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cs3sedarknet_l.py` & `turnkeyml-2.0.2/models/timm/cs3sedarknet_l.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cs3sedarknet_x.py` & `turnkeyml-2.0.2/models/timm/cs3sedarknet_x.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cs3sedarknet_xdw.py` & `turnkeyml-2.0.2/models/timm/cs3sedarknet_xdw.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cspdarknet53.py` & `turnkeyml-2.0.2/models/timm/cspdarknet53.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cspresnet50.py` & `turnkeyml-2.0.2/models/timm/cspresnet50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cspresnet50d.py` & `turnkeyml-2.0.2/models/timm/cspresnet50d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cspresnet50w.py` & `turnkeyml-2.0.2/models/timm/cspresnet50w.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/cspresnext50.py` & `turnkeyml-2.0.2/models/timm/cspresnext50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/darknet17.py` & `turnkeyml-2.0.2/models/timm/darknet17.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/darknet21.py` & `turnkeyml-2.0.2/models/timm/darknet21.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/darknet53.py` & `turnkeyml-2.0.2/models/timm/darknet53.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/darknetaa53.py` & `turnkeyml-2.0.2/models/timm/darknetaa53.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit3_base_patch16_224.py` & `turnkeyml-2.0.2/models/timm/deit3_base_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit3_base_patch16_224_in21ft1k.py` & `turnkeyml-2.0.2/models/timm/deit3_base_patch16_224_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit3_base_patch16_384.py` & `turnkeyml-2.0.2/models/timm/deit3_base_patch16_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit3_base_patch16_384_in21ft1k.py` & `turnkeyml-2.0.2/models/timm/deit3_base_patch16_384_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit3_huge_patch14_224.py` & `turnkeyml-2.0.2/models/timm/deit3_huge_patch14_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit3_huge_patch14_224_in21ft1k.py` & `turnkeyml-2.0.2/models/timm/deit3_huge_patch14_224_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit3_large_patch16_224.py` & `turnkeyml-2.0.2/models/timm/deit3_large_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit3_large_patch16_224_in21ft1k.py` & `turnkeyml-2.0.2/models/timm/deit3_large_patch16_224_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit3_large_patch16_384.py` & `turnkeyml-2.0.2/models/timm/deit3_large_patch16_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit3_large_patch16_384_in21ft1k.py` & `turnkeyml-2.0.2/models/timm/deit3_large_patch16_384_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit3_small_patch16_224.py` & `turnkeyml-2.0.2/models/timm/deit3_small_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit3_small_patch16_224_in21ft1k.py` & `turnkeyml-2.0.2/models/timm/deit3_small_patch16_224_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit3_small_patch16_384.py` & `turnkeyml-2.0.2/models/timm/deit3_small_patch16_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit3_small_patch16_384_in21ft1k.py` & `turnkeyml-2.0.2/models/timm/deit3_small_patch16_384_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit_base_distilled_patch16_224.py` & `turnkeyml-2.0.2/models/timm/deit_base_distilled_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit_base_distilled_patch16_384.py` & `turnkeyml-2.0.2/models/timm/deit_base_distilled_patch16_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit_base_patch16_224.py` & `turnkeyml-2.0.2/models/timm/deit_base_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit_base_patch16_384.py` & `turnkeyml-2.0.2/models/timm/deit_base_patch16_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit_small_distilled_patch16_224.py` & `turnkeyml-2.0.2/models/timm/deit_small_distilled_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit_small_patch16_224.py` & `turnkeyml-2.0.2/models/timm/deit_small_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit_tiny_distilled_patch16_224.py` & `turnkeyml-2.0.2/models/timm/deit_tiny_distilled_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/deit_tiny_patch16_224.py` & `turnkeyml-2.0.2/models/timm/deit_tiny_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/densenet121.py` & `turnkeyml-2.0.2/models/timm/densenet121.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/densenet161.py` & `turnkeyml-2.0.2/models/timm/densenet161.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/densenet169.py` & `turnkeyml-2.0.2/models/timm/densenet169.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/densenet201.py` & `turnkeyml-2.0.2/models/timm/densenet201.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/densenetblur121d.py` & `turnkeyml-2.0.2/models/timm/densenetblur121d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dla102.py` & `turnkeyml-2.0.2/models/timm/dla102.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dla102x.py` & `turnkeyml-2.0.2/models/timm/dla102x.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dla102x2.py` & `turnkeyml-2.0.2/models/timm/dla102x2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dla169.py` & `turnkeyml-2.0.2/models/timm/dla169.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dla34.py` & `turnkeyml-2.0.2/models/timm/dla34.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dla46_c.py` & `turnkeyml-2.0.2/models/timm/dla46_c.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dla46x_c.py` & `turnkeyml-2.0.2/models/timm/dla46x_c.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dla60.py` & `turnkeyml-2.0.2/models/timm/dla60.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dla60_res2net.py` & `turnkeyml-2.0.2/models/timm/dla60_res2net.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dla60_res2next.py` & `turnkeyml-2.0.2/models/timm/dla60_res2next.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dla60x.py` & `turnkeyml-2.0.2/models/timm/dla60x.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dla60x_c.py` & `turnkeyml-2.0.2/models/timm/dla60x_c.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dm_nfnet_f0.py` & `turnkeyml-2.0.2/models/timm/dm_nfnet_f0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dm_nfnet_f1.py` & `turnkeyml-2.0.2/models/timm/dm_nfnet_f1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dm_nfnet_f2.py` & `turnkeyml-2.0.2/models/timm/dm_nfnet_f2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dm_nfnet_f3.py` & `turnkeyml-2.0.2/models/timm/dm_nfnet_f3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dm_nfnet_f4.py` & `turnkeyml-2.0.2/models/timm/dm_nfnet_f4.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dm_nfnet_f5.py` & `turnkeyml-2.0.2/models/timm/dm_nfnet_f5.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dm_nfnet_f6.py` & `turnkeyml-2.0.2/models/timm/dm_nfnet_f6.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dpn107.py` & `turnkeyml-2.0.2/models/timm/dpn107.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dpn131.py` & `turnkeyml-2.0.2/models/timm/dpn131.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dpn68.py` & `turnkeyml-2.0.2/models/timm/dpn68.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dpn68b.py` & `turnkeyml-2.0.2/models/timm/dpn68b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dpn92.py` & `turnkeyml-2.0.2/models/timm/dpn92.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/dpn98.py` & `turnkeyml-2.0.2/models/timm/dpn98.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/eca_botnext26ts_256.py` & `turnkeyml-2.0.2/models/timm/eca_botnext26ts_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/eca_halonext26ts.py` & `turnkeyml-2.0.2/models/timm/eca_halonext26ts.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/eca_nfnet_l0.py` & `turnkeyml-2.0.2/models/timm/eca_nfnet_l0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/eca_nfnet_l1.py` & `turnkeyml-2.0.2/models/timm/eca_nfnet_l1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/eca_nfnet_l2.py` & `turnkeyml-2.0.2/models/timm/eca_nfnet_l2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/eca_nfnet_l3.py` & `turnkeyml-2.0.2/models/timm/eca_nfnet_l3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/eca_resnet33ts.py` & `turnkeyml-2.0.2/models/timm/eca_resnet33ts.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/eca_resnext26ts.py` & `turnkeyml-2.0.2/models/timm/eca_resnext26ts.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/eca_vovnet39b.py` & `turnkeyml-2.0.2/models/timm/eca_vovnet39b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ecaresnet101d.py` & `turnkeyml-2.0.2/models/timm/ecaresnet101d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ecaresnet200d.py` & `turnkeyml-2.0.2/models/timm/ecaresnet200d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ecaresnet269d.py` & `turnkeyml-2.0.2/models/timm/ecaresnet269d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ecaresnet26t.py` & `turnkeyml-2.0.2/models/timm/ecaresnet26t.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ecaresnet50d.py` & `turnkeyml-2.0.2/models/timm/ecaresnet50d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ecaresnet50t.py` & `turnkeyml-2.0.2/models/timm/ecaresnet50t.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ecaresnetlight.py` & `turnkeyml-2.0.2/models/timm/ecaresnetlight.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ecaresnext26t_32x4d.py` & `turnkeyml-2.0.2/models/timm/ecaresnext26t_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ecaresnext50t_32x4d.py` & `turnkeyml-2.0.2/models/timm/ecaresnext50t_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/edgenext_small.py` & `turnkeyml-2.0.2/models/timm/edgenext_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/edgenext_small_rw.py` & `turnkeyml-2.0.2/models/timm/edgenext_small_rw.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/edgenext_x_small.py` & `turnkeyml-2.0.2/models/timm/edgenext_x_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/edgenext_xx_small.py` & `turnkeyml-2.0.2/models/timm/edgenext_xx_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b0.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b0_g16_evos.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b0_g16_evos.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b0_g8_gn.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b0_g8_gn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b0_gn.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b0_gn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b1.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b2.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b2a.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b2a.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b3.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b3_g8_gn.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b3_g8_gn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b3_gn.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b3_gn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b3a.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b3a.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b4.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b4.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b5.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b5.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b6.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b6.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b7.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b7.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_b8.py` & `turnkeyml-2.0.2/models/timm/efficientnet_b8.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_cc_b0_4e.py` & `turnkeyml-2.0.2/models/timm/efficientnet_cc_b0_4e.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_cc_b0_8e.py` & `turnkeyml-2.0.2/models/timm/efficientnet_cc_b0_8e.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_cc_b1_8e.py` & `turnkeyml-2.0.2/models/timm/efficientnet_cc_b1_8e.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_el.py` & `turnkeyml-2.0.2/models/timm/efficientnet_el.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_el_pruned.py` & `turnkeyml-2.0.2/models/timm/efficientnet_el_pruned.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_em.py` & `turnkeyml-2.0.2/models/timm/efficientnet_em.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_es.py` & `turnkeyml-2.0.2/models/timm/efficientnet_es.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_es_pruned.py` & `turnkeyml-2.0.2/models/timm/efficientnet_es_pruned.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_l2.py` & `turnkeyml-2.0.2/models/timm/efficientnet_l2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_lite0.py` & `turnkeyml-2.0.2/models/timm/efficientnet_lite0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_lite1.py` & `turnkeyml-2.0.2/models/timm/efficientnet_lite1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_lite2.py` & `turnkeyml-2.0.2/models/timm/efficientnet_lite2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_lite3.py` & `turnkeyml-2.0.2/models/timm/efficientnet_lite3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnet_lite4.py` & `turnkeyml-2.0.2/models/timm/efficientnet_lite4.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnetv2_l.py` & `turnkeyml-2.0.2/models/timm/efficientnetv2_l.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnetv2_m.py` & `turnkeyml-2.0.2/models/timm/efficientnetv2_m.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnetv2_rw_m.py` & `turnkeyml-2.0.2/models/timm/efficientnetv2_rw_m.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnetv2_rw_s.py` & `turnkeyml-2.0.2/models/timm/efficientnetv2_rw_s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnetv2_rw_t.py` & `turnkeyml-2.0.2/models/timm/efficientnetv2_rw_t.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnetv2_s.py` & `turnkeyml-2.0.2/models/timm/efficientnetv2_s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/efficientnetv2_xl.py` & `turnkeyml-2.0.2/models/timm/efficientnetv2_xl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ens_adv_inception_resnet_v2.py` & `turnkeyml-2.0.2/models/timm/ens_adv_inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ese_vovnet19b_dw.py` & `turnkeyml-2.0.2/models/timm/ese_vovnet19b_dw.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ese_vovnet19b_slim.py` & `turnkeyml-2.0.2/models/timm/ese_vovnet19b_slim.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ese_vovnet19b_slim_dw.py` & `turnkeyml-2.0.2/models/timm/ese_vovnet19b_slim_dw.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ese_vovnet39b.py` & `turnkeyml-2.0.2/models/timm/ese_vovnet39b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ese_vovnet39b_evos.py` & `turnkeyml-2.0.2/models/timm/ese_vovnet39b_evos.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ese_vovnet57b.py` & `turnkeyml-2.0.2/models/timm/ese_vovnet57b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ese_vovnet99b.py` & `turnkeyml-2.0.2/models/timm/ese_vovnet99b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/fbnetc_100.py` & `turnkeyml-2.0.2/models/timm/fbnetc_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/fbnetv3_b.py` & `turnkeyml-2.0.2/models/timm/fbnetv3_b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/fbnetv3_d.py` & `turnkeyml-2.0.2/models/timm/fbnetv3_d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/fbnetv3_g.py` & `turnkeyml-2.0.2/models/timm/fbnetv3_g.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gc_efficientnetv2_rw_t.py` & `turnkeyml-2.0.2/models/timm/gc_efficientnetv2_rw_t.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gcresnet33ts.py` & `turnkeyml-2.0.2/models/timm/gcresnet33ts.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gcresnet50t.py` & `turnkeyml-2.0.2/models/timm/gcresnet50t.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gcresnext26ts.py` & `turnkeyml-2.0.2/models/timm/gcresnext26ts.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gcresnext50ts.py` & `turnkeyml-2.0.2/models/timm/gcresnext50ts.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gernet_l.py` & `turnkeyml-2.0.2/models/timm/gernet_l.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gernet_m.py` & `turnkeyml-2.0.2/models/timm/gernet_m.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gernet_s.py` & `turnkeyml-2.0.2/models/timm/gernet_s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ghostnet_050.py` & `turnkeyml-2.0.2/models/timm/ghostnet_050.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ghostnet_100.py` & `turnkeyml-2.0.2/models/timm/ghostnet_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ghostnet_130.py` & `turnkeyml-2.0.2/models/timm/ghostnet_130.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_inception_v3.py` & `turnkeyml-2.0.2/models/timm/gluon_inception_v3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnet101_v1b.py` & `turnkeyml-2.0.2/models/timm/gluon_resnet101_v1b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnet101_v1c.py` & `turnkeyml-2.0.2/models/timm/gluon_resnet101_v1c.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnet101_v1d.py` & `turnkeyml-2.0.2/models/timm/gluon_resnet101_v1d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnet101_v1s.py` & `turnkeyml-2.0.2/models/timm/gluon_resnet101_v1s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnet152_v1b.py` & `turnkeyml-2.0.2/models/timm/gluon_resnet152_v1b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnet152_v1c.py` & `turnkeyml-2.0.2/models/timm/gluon_resnet152_v1c.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnet152_v1d.py` & `turnkeyml-2.0.2/models/timm/gluon_resnet152_v1d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnet152_v1s.py` & `turnkeyml-2.0.2/models/timm/gluon_resnet152_v1s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnet18_v1b.py` & `turnkeyml-2.0.2/models/timm/gluon_resnet18_v1b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnet34_v1b.py` & `turnkeyml-2.0.2/models/timm/gluon_resnet34_v1b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnet50_v1b.py` & `turnkeyml-2.0.2/models/timm/gluon_resnet50_v1b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnet50_v1c.py` & `turnkeyml-2.0.2/models/timm/gluon_resnet50_v1c.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnet50_v1d.py` & `turnkeyml-2.0.2/models/timm/gluon_resnet50_v1d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnet50_v1s.py` & `turnkeyml-2.0.2/models/timm/gluon_resnet50_v1s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnext101_32x4d.py` & `turnkeyml-2.0.2/models/timm/gluon_resnext101_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnext101_64x4d.py` & `turnkeyml-2.0.2/models/timm/gluon_resnext101_64x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_resnext50_32x4d.py` & `turnkeyml-2.0.2/models/timm/gluon_resnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_senet154.py` & `turnkeyml-2.0.2/models/timm/gluon_senet154.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_seresnext101_32x4d.py` & `turnkeyml-2.0.2/models/timm/gluon_seresnext101_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_seresnext101_64x4d.py` & `turnkeyml-2.0.2/models/timm/gluon_seresnext101_64x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gluon_seresnext50_32x4d.py` & `turnkeyml-2.0.2/models/timm/gluon_seresnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gmixer_12_224.py` & `turnkeyml-2.0.2/models/timm/gmixer_12_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gmixer_24_224.py` & `turnkeyml-2.0.2/models/timm/gmixer_24_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gmlp_b16_224.py` & `turnkeyml-2.0.2/models/timm/gmlp_b16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gmlp_s16_224.py` & `turnkeyml-2.0.2/models/timm/gmlp_s16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/gmlp_ti16_224.py` & `turnkeyml-2.0.2/models/timm/gmlp_ti16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/halo2botnet50ts_256.py` & `turnkeyml-2.0.2/models/timm/halo2botnet50ts_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/halonet26t.py` & `turnkeyml-2.0.2/models/timm/halonet26t.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/halonet50ts.py` & `turnkeyml-2.0.2/models/timm/halonet50ts.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/halonet_h1.py` & `turnkeyml-2.0.2/models/timm/halonet_h1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/haloregnetz_b.py` & `turnkeyml-2.0.2/models/timm/haloregnetz_b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/hardcorenas_a.py` & `turnkeyml-2.0.2/models/timm/hardcorenas_a.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/hardcorenas_b.py` & `turnkeyml-2.0.2/models/timm/hardcorenas_b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/hardcorenas_c.py` & `turnkeyml-2.0.2/models/timm/hardcorenas_c.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/hardcorenas_d.py` & `turnkeyml-2.0.2/models/timm/hardcorenas_d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/hardcorenas_e.py` & `turnkeyml-2.0.2/models/timm/hardcorenas_e.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/hardcorenas_f.py` & `turnkeyml-2.0.2/models/timm/hardcorenas_f.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/hrnet_w18.py` & `turnkeyml-2.0.2/models/timm/hrnet_w18.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/hrnet_w18_small.py` & `turnkeyml-2.0.2/models/timm/hrnet_w18_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/hrnet_w18_small_v2.py` & `turnkeyml-2.0.2/models/timm/hrnet_w18_small_v2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/hrnet_w30.py` & `turnkeyml-2.0.2/models/timm/hrnet_w30.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/hrnet_w32.py` & `turnkeyml-2.0.2/models/timm/hrnet_w32.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/hrnet_w40.py` & `turnkeyml-2.0.2/models/timm/hrnet_w40.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/hrnet_w44.py` & `turnkeyml-2.0.2/models/timm/hrnet_w44.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/hrnet_w48.py` & `turnkeyml-2.0.2/models/timm/hrnet_w48.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/hrnet_w64.py` & `turnkeyml-2.0.2/models/timm/hrnet_w64.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ig_resnext101_32x16d.py` & `turnkeyml-2.0.2/models/timm/ig_resnext101_32x16d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ig_resnext101_32x32d.py` & `turnkeyml-2.0.2/models/timm/ig_resnext101_32x32d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ig_resnext101_32x48d.py` & `turnkeyml-2.0.2/models/timm/ig_resnext101_32x48d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ig_resnext101_32x8d.py` & `turnkeyml-2.0.2/models/timm/ig_resnext101_32x8d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/inception_resnet_v2.py` & `turnkeyml-2.0.2/models/timm/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/inception_v3.py` & `turnkeyml-2.0.2/models/timm/inception_v3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/inception_v4.py` & `turnkeyml-2.0.2/models/timm/inception_v4.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/jx_nest_base.py` & `turnkeyml-2.0.2/models/timm/jx_nest_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/jx_nest_small.py` & `turnkeyml-2.0.2/models/timm/jx_nest_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/jx_nest_tiny.py` & `turnkeyml-2.0.2/models/timm/jx_nest_tiny.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/lambda_resnet26rpt_256.py` & `turnkeyml-2.0.2/models/timm/lambda_resnet26rpt_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/lambda_resnet26t.py` & `turnkeyml-2.0.2/models/timm/lambda_resnet26t.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/lambda_resnet50ts.py` & `turnkeyml-2.0.2/models/timm/lambda_resnet50ts.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/lamhalobotnet50ts_256.py` & `turnkeyml-2.0.2/models/timm/lamhalobotnet50ts_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/lcnet_035.py` & `turnkeyml-2.0.2/models/timm/lcnet_035.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/lcnet_050.py` & `turnkeyml-2.0.2/models/timm/lcnet_050.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/lcnet_075.py` & `turnkeyml-2.0.2/models/timm/lcnet_075.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/lcnet_100.py` & `turnkeyml-2.0.2/models/timm/lcnet_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/lcnet_150.py` & `turnkeyml-2.0.2/models/timm/lcnet_150.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/legacy_senet154.py` & `turnkeyml-2.0.2/models/timm/legacy_senet154.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/legacy_seresnet101.py` & `turnkeyml-2.0.2/models/timm/legacy_seresnet101.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/legacy_seresnet152.py` & `turnkeyml-2.0.2/models/timm/legacy_seresnet152.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/legacy_seresnet18.py` & `turnkeyml-2.0.2/models/timm/legacy_seresnet18.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/legacy_seresnet34.py` & `turnkeyml-2.0.2/models/timm/legacy_seresnet34.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/legacy_seresnet50.py` & `turnkeyml-2.0.2/models/timm/legacy_seresnet50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/legacy_seresnext101_32x4d.py` & `turnkeyml-2.0.2/models/timm/legacy_seresnext101_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/legacy_seresnext26_32x4d.py` & `turnkeyml-2.0.2/models/timm/legacy_seresnext26_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/legacy_seresnext50_32x4d.py` & `turnkeyml-2.0.2/models/timm/legacy_seresnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/levit_128.py` & `turnkeyml-2.0.2/models/timm/levit_128.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/levit_128s.py` & `turnkeyml-2.0.2/models/timm/levit_128s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/levit_192.py` & `turnkeyml-2.0.2/models/timm/levit_192.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/levit_256.py` & `turnkeyml-2.0.2/models/timm/levit_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/levit_256d.py` & `turnkeyml-2.0.2/models/timm/levit_256d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/levit_384.py` & `turnkeyml-2.0.2/models/timm/levit_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mixer_b16_224.py` & `turnkeyml-2.0.2/models/timm/mixer_b16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mixer_b16_224_in21k.py` & `turnkeyml-2.0.2/models/timm/mixer_b16_224_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mixer_b16_224_miil.py` & `turnkeyml-2.0.2/models/timm/mixer_b16_224_miil.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mixer_b16_224_miil_in21k.py` & `turnkeyml-2.0.2/models/timm/mixer_b16_224_miil_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mixer_b32_224.py` & `turnkeyml-2.0.2/models/timm/mixer_b32_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mixer_l16_224.py` & `turnkeyml-2.0.2/models/timm/mixer_l16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mixer_l16_224_in21k.py` & `turnkeyml-2.0.2/models/timm/mixer_l16_224_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mixer_l32_224.py` & `turnkeyml-2.0.2/models/timm/mixer_l32_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mixer_s16_224.py` & `turnkeyml-2.0.2/models/timm/mixer_s16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mixer_s32_224.py` & `turnkeyml-2.0.2/models/timm/mixer_s32_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mixnet_l.py` & `turnkeyml-2.0.2/models/timm/mixnet_l.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mixnet_m.py` & `turnkeyml-2.0.2/models/timm/mixnet_m.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mixnet_s.py` & `turnkeyml-2.0.2/models/timm/mixnet_s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mixnet_xl.py` & `turnkeyml-2.0.2/models/timm/mixnet_xl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mixnet_xxl.py` & `turnkeyml-2.0.2/models/timm/mixnet_xxl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mnasnet_050.py` & `turnkeyml-2.0.2/models/timm/mnasnet_050.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mnasnet_075.py` & `turnkeyml-2.0.2/models/timm/mnasnet_075.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mnasnet_100.py` & `turnkeyml-2.0.2/models/timm/mnasnet_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mnasnet_140.py` & `turnkeyml-2.0.2/models/timm/mnasnet_140.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mnasnet_a1.py` & `turnkeyml-2.0.2/models/timm/mnasnet_a1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mnasnet_b1.py` & `turnkeyml-2.0.2/models/timm/mnasnet_b1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mnasnet_small.py` & `turnkeyml-2.0.2/models/timm/mnasnet_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilenetv2_035.py` & `turnkeyml-2.0.2/models/timm/mobilenetv2_035.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilenetv2_050.py` & `turnkeyml-2.0.2/models/timm/mobilenetv2_050.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilenetv2_075.py` & `turnkeyml-2.0.2/models/timm/mobilenetv2_075.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilenetv2_100.py` & `turnkeyml-2.0.2/models/timm/mobilenetv2_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilenetv2_110d.py` & `turnkeyml-2.0.2/models/timm/mobilenetv2_110d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilenetv2_120d.py` & `turnkeyml-2.0.2/models/timm/mobilenetv2_120d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilenetv2_140.py` & `turnkeyml-2.0.2/models/timm/mobilenetv2_140.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilenetv3_large_075.py` & `turnkeyml-2.0.2/models/timm/mobilenetv3_large_075.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilenetv3_large_100.py` & `turnkeyml-2.0.2/models/timm/mobilenetv3_large_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilenetv3_large_100_miil.py` & `turnkeyml-2.0.2/models/timm/mobilenetv3_large_100_miil.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilenetv3_large_100_miil_in21k.py` & `turnkeyml-2.0.2/models/timm/mobilenetv3_large_100_miil_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilenetv3_rw.py` & `turnkeyml-2.0.2/models/timm/mobilenetv3_rw.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilenetv3_small_050.py` & `turnkeyml-2.0.2/models/timm/mobilenetv3_small_050.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilenetv3_small_075.py` & `turnkeyml-2.0.2/models/timm/mobilenetv3_small_075.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilenetv3_small_100.py` & `turnkeyml-2.0.2/models/timm/mobilenetv3_small_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevit_s.py` & `turnkeyml-2.0.2/models/timm/mobilevit_s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevit_xs.py` & `turnkeyml-2.0.2/models/timm/mobilevit_xs.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevit_xxs.py` & `turnkeyml-2.0.2/models/timm/mobilevit_xxs.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevitv2_050.py` & `turnkeyml-2.0.2/models/timm/mobilevitv2_050.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevitv2_075.py` & `turnkeyml-2.0.2/models/timm/mobilevitv2_075.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevitv2_100.py` & `turnkeyml-2.0.2/models/timm/mobilevitv2_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevitv2_125.py` & `turnkeyml-2.0.2/models/timm/mobilevitv2_125.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevitv2_150.py` & `turnkeyml-2.0.2/models/timm/mobilevitv2_150.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevitv2_150_384_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/mobilevitv2_150_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevitv2_150_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/mobilevitv2_150_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevitv2_175.py` & `turnkeyml-2.0.2/models/timm/mobilevitv2_175.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevitv2_175_384_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/mobilevitv2_175_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevitv2_175_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/mobilevitv2_175_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevitv2_200.py` & `turnkeyml-2.0.2/models/timm/mobilevitv2_200.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevitv2_200_384_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/mobilevitv2_200_384_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/mobilevitv2_200_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/mobilevitv2_200_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nasnetalarge.py` & `turnkeyml-2.0.2/models/timm/nasnetalarge.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nest_base.py` & `turnkeyml-2.0.2/models/timm/nest_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nest_small.py` & `turnkeyml-2.0.2/models/timm/nest_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nest_tiny.py` & `turnkeyml-2.0.2/models/timm/nest_tiny.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nf_ecaresnet101.py` & `turnkeyml-2.0.2/models/timm/nf_ecaresnet101.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nf_ecaresnet26.py` & `turnkeyml-2.0.2/models/timm/nf_ecaresnet26.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nf_ecaresnet50.py` & `turnkeyml-2.0.2/models/timm/nf_ecaresnet50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nf_regnet_b0.py` & `turnkeyml-2.0.2/models/timm/nf_regnet_b0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nf_regnet_b1.py` & `turnkeyml-2.0.2/models/timm/nf_regnet_b1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nf_regnet_b2.py` & `turnkeyml-2.0.2/models/timm/nf_regnet_b2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nf_regnet_b3.py` & `turnkeyml-2.0.2/models/timm/nf_regnet_b3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nf_regnet_b4.py` & `turnkeyml-2.0.2/models/timm/nf_regnet_b4.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nf_regnet_b5.py` & `turnkeyml-2.0.2/models/timm/nf_regnet_b5.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nf_resnet101.py` & `turnkeyml-2.0.2/models/timm/nf_resnet101.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nf_resnet26.py` & `turnkeyml-2.0.2/models/timm/nf_resnet26.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nf_resnet50.py` & `turnkeyml-2.0.2/models/timm/nf_resnet50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nf_seresnet101.py` & `turnkeyml-2.0.2/models/timm/nf_seresnet101.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nf_seresnet26.py` & `turnkeyml-2.0.2/models/timm/nf_seresnet26.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nf_seresnet50.py` & `turnkeyml-2.0.2/models/timm/nf_seresnet50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nfnet_f0.py` & `turnkeyml-2.0.2/models/timm/nfnet_f0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nfnet_f1.py` & `turnkeyml-2.0.2/models/timm/nfnet_f1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nfnet_f2.py` & `turnkeyml-2.0.2/models/timm/nfnet_f2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nfnet_f3.py` & `turnkeyml-2.0.2/models/timm/nfnet_f3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nfnet_f4.py` & `turnkeyml-2.0.2/models/timm/nfnet_f4.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nfnet_f5.py` & `turnkeyml-2.0.2/models/timm/nfnet_f5.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nfnet_f6.py` & `turnkeyml-2.0.2/models/timm/nfnet_f6.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nfnet_f7.py` & `turnkeyml-2.0.2/models/timm/nfnet_f7.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/nfnet_l0.py` & `turnkeyml-2.0.2/models/timm/nfnet_l0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/pit_b_224.py` & `turnkeyml-2.0.2/models/timm/pit_b_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/pit_b_distilled_224.py` & `turnkeyml-2.0.2/models/timm/pit_b_distilled_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/pit_s_224.py` & `turnkeyml-2.0.2/models/timm/pit_s_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/pit_s_distilled_224.py` & `turnkeyml-2.0.2/models/timm/pit_s_distilled_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/pit_ti_224.py` & `turnkeyml-2.0.2/models/timm/pit_ti_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/pit_ti_distilled_224.py` & `turnkeyml-2.0.2/models/timm/pit_ti_distilled_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/pit_xs_224.py` & `turnkeyml-2.0.2/models/timm/pit_xs_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/pit_xs_distilled_224.py` & `turnkeyml-2.0.2/models/timm/pit_xs_distilled_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/pnasnet5large.py` & `turnkeyml-2.0.2/models/timm/pnasnet5large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/poolformer_m36.py` & `turnkeyml-2.0.2/models/timm/poolformer_m36.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/poolformer_m48.py` & `turnkeyml-2.0.2/models/timm/poolformer_m48.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/poolformer_s12.py` & `turnkeyml-2.0.2/models/timm/poolformer_s12.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/poolformer_s24.py` & `turnkeyml-2.0.2/models/timm/poolformer_s24.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/poolformer_s36.py` & `turnkeyml-2.0.2/models/timm/poolformer_s36.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetv_040.py` & `turnkeyml-2.0.2/models/timm/regnetv_040.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetv_064.py` & `turnkeyml-2.0.2/models/timm/regnetv_064.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetx_002.py` & `turnkeyml-2.0.2/models/timm/regnetx_002.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetx_004.py` & `turnkeyml-2.0.2/models/timm/regnetx_004.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetx_006.py` & `turnkeyml-2.0.2/models/timm/regnetx_006.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetx_008.py` & `turnkeyml-2.0.2/models/timm/regnetx_008.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetx_016.py` & `turnkeyml-2.0.2/models/timm/regnetx_016.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetx_032.py` & `turnkeyml-2.0.2/models/timm/regnetx_032.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetx_040.py` & `turnkeyml-2.0.2/models/timm/regnetx_040.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetx_064.py` & `turnkeyml-2.0.2/models/timm/regnetx_064.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetx_080.py` & `turnkeyml-2.0.2/models/timm/regnetx_080.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetx_120.py` & `turnkeyml-2.0.2/models/timm/regnetx_120.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetx_160.py` & `turnkeyml-2.0.2/models/timm/regnetx_160.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetx_320.py` & `turnkeyml-2.0.2/models/timm/regnetx_320.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnety_002.py` & `turnkeyml-2.0.2/models/timm/regnety_002.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnety_004.py` & `turnkeyml-2.0.2/models/timm/regnety_004.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnety_006.py` & `turnkeyml-2.0.2/models/timm/regnety_006.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnety_008.py` & `turnkeyml-2.0.2/models/timm/regnety_008.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnety_016.py` & `turnkeyml-2.0.2/models/timm/regnety_016.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnety_032.py` & `turnkeyml-2.0.2/models/timm/regnety_032.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnety_040.py` & `turnkeyml-2.0.2/models/timm/regnety_040.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnety_064.py` & `turnkeyml-2.0.2/models/timm/regnety_064.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnety_080.py` & `turnkeyml-2.0.2/models/timm/regnety_080.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnety_120.py` & `turnkeyml-2.0.2/models/timm/regnety_120.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnety_160.py` & `turnkeyml-2.0.2/models/timm/regnety_160.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnety_320.py` & `turnkeyml-2.0.2/models/timm/regnety_320.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetz_005.py` & `turnkeyml-2.0.2/models/timm/regnetz_005.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetz_040.py` & `turnkeyml-2.0.2/models/timm/regnetz_040.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetz_040h.py` & `turnkeyml-2.0.2/models/timm/regnetz_040h.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetz_b16.py` & `turnkeyml-2.0.2/models/timm/regnetz_b16.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetz_b16_evos.py` & `turnkeyml-2.0.2/models/timm/regnetz_b16_evos.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetz_c16.py` & `turnkeyml-2.0.2/models/timm/regnetz_c16.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetz_c16_evos.py` & `turnkeyml-2.0.2/models/timm/regnetz_c16_evos.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetz_d32.py` & `turnkeyml-2.0.2/models/timm/regnetz_d32.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetz_d8.py` & `turnkeyml-2.0.2/models/timm/regnetz_d8.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetz_d8_evos.py` & `turnkeyml-2.0.2/models/timm/regnetz_d8_evos.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/regnetz_e8.py` & `turnkeyml-2.0.2/models/timm/regnetz_e8.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/repvgg_a2.py` & `turnkeyml-2.0.2/models/timm/repvgg_a2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/repvgg_b0.py` & `turnkeyml-2.0.2/models/timm/repvgg_b0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/repvgg_b1.py` & `turnkeyml-2.0.2/models/timm/repvgg_b1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/repvgg_b1g4.py` & `turnkeyml-2.0.2/models/timm/repvgg_b1g4.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/repvgg_b2.py` & `turnkeyml-2.0.2/models/timm/repvgg_b2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/repvgg_b2g4.py` & `turnkeyml-2.0.2/models/timm/repvgg_b2g4.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/repvgg_b3.py` & `turnkeyml-2.0.2/models/timm/repvgg_b3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/repvgg_b3g4.py` & `turnkeyml-2.0.2/models/timm/repvgg_b3g4.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/res2net101_26w_4s.py` & `turnkeyml-2.0.2/models/timm/res2net101_26w_4s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/res2net50_14w_8s.py` & `turnkeyml-2.0.2/models/timm/res2net50_14w_8s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/res2net50_26w_4s.py` & `turnkeyml-2.0.2/models/timm/res2net50_26w_4s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/res2net50_26w_6s.py` & `turnkeyml-2.0.2/models/timm/res2net50_26w_6s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/res2net50_26w_8s.py` & `turnkeyml-2.0.2/models/timm/res2net50_26w_8s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/res2net50_48w_2s.py` & `turnkeyml-2.0.2/models/timm/res2net50_48w_2s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/res2next50.py` & `turnkeyml-2.0.2/models/timm/res2next50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resmlp_12_224.py` & `turnkeyml-2.0.2/models/timm/resmlp_12_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resmlp_12_224_dino.py` & `turnkeyml-2.0.2/models/timm/resmlp_12_224_dino.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resmlp_12_distilled_224.py` & `turnkeyml-2.0.2/models/timm/resmlp_12_distilled_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resmlp_24_224.py` & `turnkeyml-2.0.2/models/timm/resmlp_24_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resmlp_24_224_dino.py` & `turnkeyml-2.0.2/models/timm/resmlp_24_224_dino.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resmlp_24_distilled_224.py` & `turnkeyml-2.0.2/models/timm/resmlp_24_distilled_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resmlp_36_224.py` & `turnkeyml-2.0.2/models/timm/resmlp_36_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resmlp_36_distilled_224.py` & `turnkeyml-2.0.2/models/timm/resmlp_36_distilled_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resmlp_big_24_224.py` & `turnkeyml-2.0.2/models/timm/resmlp_big_24_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resmlp_big_24_224_in22ft1k.py` & `turnkeyml-2.0.2/models/timm/resmlp_big_24_224_in22ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resmlp_big_24_distilled_224.py` & `turnkeyml-2.0.2/models/timm/resmlp_big_24_distilled_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnest101e.py` & `turnkeyml-2.0.2/models/timm/resnest101e.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnest14d.py` & `turnkeyml-2.0.2/models/timm/resnest14d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnest200e.py` & `turnkeyml-2.0.2/models/timm/resnest200e.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnest269e.py` & `turnkeyml-2.0.2/models/timm/resnest269e.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnest26d.py` & `turnkeyml-2.0.2/models/timm/resnest26d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnest50d.py` & `turnkeyml-2.0.2/models/timm/resnest50d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnest50d_1s4x24d.py` & `turnkeyml-2.0.2/models/timm/resnest50d_1s4x24d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnest50d_4s2x40d.py` & `turnkeyml-2.0.2/models/timm/resnest50d_4s2x40d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet101.py` & `turnkeyml-2.0.2/models/timm/resnet101.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet101d.py` & `turnkeyml-2.0.2/models/timm/resnet101d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet10t.py` & `turnkeyml-2.0.2/models/timm/resnet10t.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet14t.py` & `turnkeyml-2.0.2/models/timm/resnet14t.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet152.py` & `turnkeyml-2.0.2/models/timm/resnet152.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet152d.py` & `turnkeyml-2.0.2/models/timm/resnet152d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet18.py` & `turnkeyml-2.0.2/models/timm/resnet18.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet18d.py` & `turnkeyml-2.0.2/models/timm/resnet18d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet200.py` & `turnkeyml-2.0.2/models/timm/resnet200.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet200d.py` & `turnkeyml-2.0.2/models/timm/resnet200d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet26.py` & `turnkeyml-2.0.2/models/timm/resnet26.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet26d.py` & `turnkeyml-2.0.2/models/timm/resnet26d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet26t.py` & `turnkeyml-2.0.2/models/timm/resnet26t.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet32ts.py` & `turnkeyml-2.0.2/models/timm/resnet32ts.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet33ts.py` & `turnkeyml-2.0.2/models/timm/resnet33ts.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet34.py` & `turnkeyml-2.0.2/models/timm/resnet34.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet34d.py` & `turnkeyml-2.0.2/models/timm/resnet34d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet50.py` & `turnkeyml-2.0.2/models/timm/resnet50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet50_gn.py` & `turnkeyml-2.0.2/models/timm/resnet50_gn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet50d.py` & `turnkeyml-2.0.2/models/timm/resnet50d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet50t.py` & `turnkeyml-2.0.2/models/timm/resnet50t.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet51q.py` & `turnkeyml-2.0.2/models/timm/resnet51q.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnet61q.py` & `turnkeyml-2.0.2/models/timm/resnet61q.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetaa101d.py` & `turnkeyml-2.0.2/models/timm/resnetaa101d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetaa50.py` & `turnkeyml-2.0.2/models/timm/resnetaa50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetaa50d.py` & `turnkeyml-2.0.2/models/timm/resnetaa50d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetblur101d.py` & `turnkeyml-2.0.2/models/timm/resnetblur101d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetblur18.py` & `turnkeyml-2.0.2/models/timm/resnetblur18.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetblur50.py` & `turnkeyml-2.0.2/models/timm/resnetblur50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetblur50d.py` & `turnkeyml-2.0.2/models/timm/resnetblur50d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetrs101.py` & `turnkeyml-2.0.2/models/timm/resnetrs101.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetrs152.py` & `turnkeyml-2.0.2/models/timm/resnetrs152.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetrs200.py` & `turnkeyml-2.0.2/models/timm/resnetrs200.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetrs270.py` & `turnkeyml-2.0.2/models/timm/resnetrs270.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetrs350.py` & `turnkeyml-2.0.2/models/timm/resnetrs350.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetrs420.py` & `turnkeyml-2.0.2/models/timm/resnetrs420.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetrs50.py` & `turnkeyml-2.0.2/models/timm/resnetrs50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_101.py` & `turnkeyml-2.0.2/models/timm/resnetv2_101.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_101d.py` & `turnkeyml-2.0.2/models/timm/resnetv2_101d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_101x1_bitm.py` & `turnkeyml-2.0.2/models/timm/resnetv2_101x1_bitm.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_101x1_bitm_in21k.py` & `turnkeyml-2.0.2/models/timm/resnetv2_101x1_bitm_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_101x3_bitm.py` & `turnkeyml-2.0.2/models/timm/resnetv2_101x3_bitm.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_101x3_bitm_in21k.py` & `turnkeyml-2.0.2/models/timm/resnetv2_101x3_bitm_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_152.py` & `turnkeyml-2.0.2/models/timm/resnetv2_152.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_152d.py` & `turnkeyml-2.0.2/models/timm/resnetv2_152d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_152x2_bit_teacher.py` & `turnkeyml-2.0.2/models/timm/resnetv2_152x2_bit_teacher.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_152x2_bit_teacher_384.py` & `turnkeyml-2.0.2/models/timm/resnetv2_152x2_bit_teacher_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_152x2_bitm.py` & `turnkeyml-2.0.2/models/timm/resnetv2_152x2_bitm.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_152x2_bitm_in21k.py` & `turnkeyml-2.0.2/models/timm/resnetv2_152x2_bitm_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_152x4_bitm.py` & `turnkeyml-2.0.2/models/timm/resnetv2_152x4_bitm.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_152x4_bitm_in21k.py` & `turnkeyml-2.0.2/models/timm/resnetv2_152x4_bitm_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_50.py` & `turnkeyml-2.0.2/models/timm/resnetv2_50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_50d.py` & `turnkeyml-2.0.2/models/timm/resnetv2_50d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_50d_evos.py` & `turnkeyml-2.0.2/models/timm/resnetv2_50d_evos.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_50d_frn.py` & `turnkeyml-2.0.2/models/timm/resnetv2_50d_frn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_50d_gn.py` & `turnkeyml-2.0.2/models/timm/resnetv2_50d_gn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_50t.py` & `turnkeyml-2.0.2/models/timm/resnetv2_50t.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_50x1_bit_distilled.py` & `turnkeyml-2.0.2/models/timm/resnetv2_50x1_bit_distilled.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_50x1_bitm.py` & `turnkeyml-2.0.2/models/timm/resnetv2_50x1_bitm.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_50x1_bitm_in21k.py` & `turnkeyml-2.0.2/models/timm/resnetv2_50x1_bitm_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_50x3_bitm.py` & `turnkeyml-2.0.2/models/timm/resnetv2_50x3_bitm.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnetv2_50x3_bitm_in21k.py` & `turnkeyml-2.0.2/models/timm/resnetv2_50x3_bitm_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnext101_32x4d.py` & `turnkeyml-2.0.2/models/timm/resnext101_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnext101_32x8d.py` & `turnkeyml-2.0.2/models/timm/resnext101_32x8d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnext101_64x4d.py` & `turnkeyml-2.0.2/models/timm/resnext101_64x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnext26ts.py` & `turnkeyml-2.0.2/models/timm/resnext26ts.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnext50_32x4d.py` & `turnkeyml-2.0.2/models/timm/resnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/resnext50d_32x4d.py` & `turnkeyml-2.0.2/models/timm/resnext50d_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/rexnet_100.py` & `turnkeyml-2.0.2/models/timm/rexnet_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/rexnet_130.py` & `turnkeyml-2.0.2/models/timm/rexnet_130.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/rexnet_150.py` & `turnkeyml-2.0.2/models/timm/rexnet_150.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/rexnet_200.py` & `turnkeyml-2.0.2/models/timm/rexnet_200.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/rexnetr_100.py` & `turnkeyml-2.0.2/models/timm/rexnetr_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/rexnetr_130.py` & `turnkeyml-2.0.2/models/timm/rexnetr_130.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/rexnetr_150.py` & `turnkeyml-2.0.2/models/timm/rexnetr_150.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/rexnetr_200.py` & `turnkeyml-2.0.2/models/timm/rexnetr_200.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/sebotnet33ts_256.py` & `turnkeyml-2.0.2/models/timm/sebotnet33ts_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/sedarknet21.py` & `turnkeyml-2.0.2/models/timm/sedarknet21.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/sehalonet33ts.py` & `turnkeyml-2.0.2/models/timm/sehalonet33ts.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/selecsls42.py` & `turnkeyml-2.0.2/models/timm/selecsls42.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/selecsls42b.py` & `turnkeyml-2.0.2/models/timm/selecsls42b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/selecsls60.py` & `turnkeyml-2.0.2/models/timm/selecsls60.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/selecsls60b.py` & `turnkeyml-2.0.2/models/timm/selecsls60b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/selecsls84.py` & `turnkeyml-2.0.2/models/timm/selecsls84.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/semnasnet_050.py` & `turnkeyml-2.0.2/models/timm/semnasnet_050.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/semnasnet_075.py` & `turnkeyml-2.0.2/models/timm/semnasnet_075.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/semnasnet_100.py` & `turnkeyml-2.0.2/models/timm/semnasnet_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/semnasnet_140.py` & `turnkeyml-2.0.2/models/timm/semnasnet_140.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/senet154.py` & `turnkeyml-2.0.2/models/timm/senet154.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/sequencer2d_l.py` & `turnkeyml-2.0.2/models/timm/sequencer2d_l.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/sequencer2d_m.py` & `turnkeyml-2.0.2/models/timm/sequencer2d_m.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/sequencer2d_s.py` & `turnkeyml-2.0.2/models/timm/sequencer2d_s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnet101.py` & `turnkeyml-2.0.2/models/timm/seresnet101.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnet152.py` & `turnkeyml-2.0.2/models/timm/seresnet152.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnet152d.py` & `turnkeyml-2.0.2/models/timm/seresnet152d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnet18.py` & `turnkeyml-2.0.2/models/timm/seresnet18.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnet200d.py` & `turnkeyml-2.0.2/models/timm/seresnet200d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnet269d.py` & `turnkeyml-2.0.2/models/timm/seresnet269d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnet33ts.py` & `turnkeyml-2.0.2/models/timm/seresnet33ts.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnet34.py` & `turnkeyml-2.0.2/models/timm/seresnet34.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnet50.py` & `turnkeyml-2.0.2/models/timm/seresnet50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnet50t.py` & `turnkeyml-2.0.2/models/timm/seresnet50t.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnetaa50d.py` & `turnkeyml-2.0.2/models/timm/seresnetaa50d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnext101_32x4d.py` & `turnkeyml-2.0.2/models/timm/seresnext101_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnext101_32x8d.py` & `turnkeyml-2.0.2/models/timm/seresnext101_32x8d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnext101d_32x8d.py` & `turnkeyml-2.0.2/models/timm/seresnext101d_32x8d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnext26d_32x4d.py` & `turnkeyml-2.0.2/models/timm/seresnext26d_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnext26t_32x4d.py` & `turnkeyml-2.0.2/models/timm/seresnext26t_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnext26tn_32x4d.py` & `turnkeyml-2.0.2/models/timm/seresnext26tn_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnext26ts.py` & `turnkeyml-2.0.2/models/timm/seresnext26ts.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnext50_32x4d.py` & `turnkeyml-2.0.2/models/timm/seresnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/seresnextaa101d_32x8d.py` & `turnkeyml-2.0.2/models/timm/seresnextaa101d_32x8d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/skresnet18.py` & `turnkeyml-2.0.2/models/timm/skresnet18.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/skresnet34.py` & `turnkeyml-2.0.2/models/timm/skresnet34.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/skresnet50.py` & `turnkeyml-2.0.2/models/timm/skresnet50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/skresnet50d.py` & `turnkeyml-2.0.2/models/timm/skresnet50d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/skresnext50_32x4d.py` & `turnkeyml-2.0.2/models/timm/skresnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/spnasnet_100.py` & `turnkeyml-2.0.2/models/timm/spnasnet_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ssl_resnet18.py` & `turnkeyml-2.0.2/models/timm/ssl_resnet18.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ssl_resnet50.py` & `turnkeyml-2.0.2/models/timm/ssl_resnet50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ssl_resnext101_32x16d.py` & `turnkeyml-2.0.2/models/timm/ssl_resnext101_32x16d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ssl_resnext101_32x4d.py` & `turnkeyml-2.0.2/models/timm/ssl_resnext101_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ssl_resnext101_32x8d.py` & `turnkeyml-2.0.2/models/timm/ssl_resnext101_32x8d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/ssl_resnext50_32x4d.py` & `turnkeyml-2.0.2/models/timm/ssl_resnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swin_base_patch4_window12_384.py` & `turnkeyml-2.0.2/models/timm/swin_base_patch4_window12_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swin_base_patch4_window12_384_in22k.py` & `turnkeyml-2.0.2/models/timm/swin_base_patch4_window12_384_in22k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swin_base_patch4_window7_224.py` & `turnkeyml-2.0.2/models/timm/swin_base_patch4_window7_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swin_base_patch4_window7_224_in22k.py` & `turnkeyml-2.0.2/models/timm/swin_base_patch4_window7_224_in22k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swin_large_patch4_window12_384.py` & `turnkeyml-2.0.2/models/timm/swin_large_patch4_window12_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swin_large_patch4_window12_384_in22k.py` & `turnkeyml-2.0.2/models/timm/swin_large_patch4_window12_384_in22k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swin_large_patch4_window7_224.py` & `turnkeyml-2.0.2/models/timm/swin_large_patch4_window7_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swin_large_patch4_window7_224_in22k.py` & `turnkeyml-2.0.2/models/timm/swin_large_patch4_window7_224_in22k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swin_s3_base_224.py` & `turnkeyml-2.0.2/models/timm/swin_s3_base_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swin_s3_small_224.py` & `turnkeyml-2.0.2/models/timm/swin_s3_small_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swin_s3_tiny_224.py` & `turnkeyml-2.0.2/models/timm/swin_s3_tiny_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swin_small_patch4_window7_224.py` & `turnkeyml-2.0.2/models/timm/swin_small_patch4_window7_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swin_tiny_patch4_window7_224.py` & `turnkeyml-2.0.2/models/timm/swin_tiny_patch4_window7_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_base_window12_192_22k.py` & `turnkeyml-2.0.2/models/timm/swinv2_base_window12_192_22k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_base_window12to16_192to256_22kft1k.py` & `turnkeyml-2.0.2/models/timm/swinv2_base_window12to16_192to256_22kft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_base_window12to24_192to384_22kft1k.py` & `turnkeyml-2.0.2/models/timm/swinv2_base_window12to24_192to384_22kft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_base_window16_256.py` & `turnkeyml-2.0.2/models/timm/swinv2_base_window16_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_base_window8_256.py` & `turnkeyml-2.0.2/models/timm/swinv2_base_window8_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_cr_base_224.py` & `turnkeyml-2.0.2/models/timm/swinv2_cr_base_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_cr_base_384.py` & `turnkeyml-2.0.2/models/timm/swinv2_cr_base_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_cr_base_ns_224.py` & `turnkeyml-2.0.2/models/timm/swinv2_cr_base_ns_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_cr_giant_224.py` & `turnkeyml-2.0.2/models/timm/swinv2_cr_giant_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_cr_giant_384.py` & `turnkeyml-2.0.2/models/timm/swinv2_cr_giant_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_cr_huge_224.py` & `turnkeyml-2.0.2/models/timm/swinv2_cr_huge_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_cr_huge_384.py` & `turnkeyml-2.0.2/models/timm/swinv2_cr_huge_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_cr_large_224.py` & `turnkeyml-2.0.2/models/timm/swinv2_cr_large_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_cr_large_384.py` & `turnkeyml-2.0.2/models/timm/swinv2_cr_large_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_cr_small_224.py` & `turnkeyml-2.0.2/models/timm/swinv2_cr_small_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_cr_small_384.py` & `turnkeyml-2.0.2/models/timm/swinv2_cr_small_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_cr_small_ns_224.py` & `turnkeyml-2.0.2/models/timm/swinv2_cr_small_ns_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_cr_tiny_224.py` & `turnkeyml-2.0.2/models/timm/swinv2_cr_tiny_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_cr_tiny_384.py` & `turnkeyml-2.0.2/models/timm/swinv2_cr_tiny_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_cr_tiny_ns_224.py` & `turnkeyml-2.0.2/models/timm/swinv2_cr_tiny_ns_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_large_window12_192_22k.py` & `turnkeyml-2.0.2/models/timm/swinv2_large_window12_192_22k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_large_window12to16_192to256_22kft1k.py` & `turnkeyml-2.0.2/models/timm/swinv2_large_window12to16_192to256_22kft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_large_window12to24_192to384_22kft1k.py` & `turnkeyml-2.0.2/models/timm/swinv2_large_window12to24_192to384_22kft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_small_window16_256.py` & `turnkeyml-2.0.2/models/timm/swinv2_small_window16_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_small_window8_256.py` & `turnkeyml-2.0.2/models/timm/swinv2_small_window8_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_tiny_window16_256.py` & `turnkeyml-2.0.2/models/timm/swinv2_tiny_window16_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swinv2_tiny_window8_256.py` & `turnkeyml-2.0.2/models/timm/swinv2_tiny_window8_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swsl_resnet18.py` & `turnkeyml-2.0.2/models/timm/swsl_resnet18.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swsl_resnet50.py` & `turnkeyml-2.0.2/models/timm/swsl_resnet50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swsl_resnext101_32x16d.py` & `turnkeyml-2.0.2/models/timm/swsl_resnext101_32x16d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swsl_resnext101_32x4d.py` & `turnkeyml-2.0.2/models/timm/swsl_resnext101_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swsl_resnext101_32x8d.py` & `turnkeyml-2.0.2/models/timm/swsl_resnext101_32x8d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/swsl_resnext50_32x4d.py` & `turnkeyml-2.0.2/models/timm/swsl_resnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b0.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b0_ap.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b0_ap.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b0_ns.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b0_ns.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b1.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b1_ap.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b1_ap.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b1_ns.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b1_ns.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b2.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b2_ap.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b2_ap.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b2_ns.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b2_ns.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b3.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b3_ap.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b3_ap.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b3_ns.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b3_ns.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b4.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b4.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b4_ap.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b4_ap.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b4_ns.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b4_ns.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b5.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b5.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b5_ap.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b5_ap.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b5_ns.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b5_ns.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b6.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b6.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b6_ap.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b6_ap.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b6_ns.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b6_ns.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b7.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b7.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b7_ap.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b7_ap.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b7_ns.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b7_ns.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b8.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b8.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_b8_ap.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_b8_ap.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_cc_b0_4e.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_cc_b0_4e.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_cc_b0_8e.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_cc_b0_8e.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_cc_b1_8e.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_cc_b1_8e.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_el.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_el.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_em.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_em.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_es.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_es.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_l2_ns.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_l2_ns.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_l2_ns_475.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_l2_ns_475.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_lite0.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_lite0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_lite1.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_lite1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_lite2.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_lite2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_lite3.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_lite3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnet_lite4.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnet_lite4.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnetv2_b0.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnetv2_b0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnetv2_b1.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnetv2_b1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnetv2_b2.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnetv2_b2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnetv2_b3.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnetv2_b3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnetv2_l.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnetv2_l.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnetv2_l_in21ft1k.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnetv2_l_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnetv2_l_in21k.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnetv2_l_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnetv2_m.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnetv2_m.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnetv2_m_in21ft1k.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnetv2_m_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnetv2_m_in21k.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnetv2_m_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnetv2_s.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnetv2_s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnetv2_s_in21ft1k.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnetv2_s_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnetv2_s_in21k.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnetv2_s_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnetv2_xl_in21ft1k.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnetv2_xl_in21ft1k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_efficientnetv2_xl_in21k.py` & `turnkeyml-2.0.2/models/timm/tf_efficientnetv2_xl_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_inception_v3.py` & `turnkeyml-2.0.2/models/timm/tf_inception_v3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_mixnet_l.py` & `turnkeyml-2.0.2/models/timm/tf_mixnet_l.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_mixnet_m.py` & `turnkeyml-2.0.2/models/timm/tf_mixnet_m.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_mixnet_s.py` & `turnkeyml-2.0.2/models/timm/tf_mixnet_s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_mobilenetv3_large_075.py` & `turnkeyml-2.0.2/models/timm/tf_mobilenetv3_large_075.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_mobilenetv3_large_100.py` & `turnkeyml-2.0.2/models/timm/tf_mobilenetv3_large_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_mobilenetv3_large_minimal_100.py` & `turnkeyml-2.0.2/models/timm/tf_mobilenetv3_large_minimal_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_mobilenetv3_small_075.py` & `turnkeyml-2.0.2/models/timm/tf_mobilenetv3_small_075.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_mobilenetv3_small_100.py` & `turnkeyml-2.0.2/models/timm/tf_mobilenetv3_small_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tf_mobilenetv3_small_minimal_100.py` & `turnkeyml-2.0.2/models/timm/tf_mobilenetv3_small_minimal_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tinynet_a.py` & `turnkeyml-2.0.2/models/timm/tinynet_a.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tinynet_b.py` & `turnkeyml-2.0.2/models/timm/tinynet_b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tinynet_c.py` & `turnkeyml-2.0.2/models/timm/tinynet_c.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tinynet_d.py` & `turnkeyml-2.0.2/models/timm/tinynet_d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tinynet_e.py` & `turnkeyml-2.0.2/models/timm/tinynet_e.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tnt_b_patch16_224.py` & `turnkeyml-2.0.2/models/timm/tnt_b_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tnt_s_patch16_224.py` & `turnkeyml-2.0.2/models/timm/tnt_s_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tv_resnet101.py` & `turnkeyml-2.0.2/models/timm/tv_resnet101.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tv_resnet152.py` & `turnkeyml-2.0.2/models/timm/tv_resnet152.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tv_resnet34.py` & `turnkeyml-2.0.2/models/timm/tv_resnet34.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tv_resnet50.py` & `turnkeyml-2.0.2/models/timm/tv_resnet50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/tv_resnext50_32x4d.py` & `turnkeyml-2.0.2/models/timm/tv_resnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/twins_pcpvt_base.py` & `turnkeyml-2.0.2/models/timm/twins_pcpvt_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/twins_pcpvt_large.py` & `turnkeyml-2.0.2/models/timm/twins_pcpvt_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/twins_pcpvt_small.py` & `turnkeyml-2.0.2/models/timm/twins_pcpvt_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/twins_svt_base.py` & `turnkeyml-2.0.2/models/timm/twins_svt_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/twins_svt_large.py` & `turnkeyml-2.0.2/models/timm/twins_svt_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/twins_svt_small.py` & `turnkeyml-2.0.2/models/timm/twins_svt_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vgg11.py` & `turnkeyml-2.0.2/models/timm/vgg11.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vgg11_bn.py` & `turnkeyml-2.0.2/models/timm/vgg11_bn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vgg13.py` & `turnkeyml-2.0.2/models/timm/vgg13.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vgg13_bn.py` & `turnkeyml-2.0.2/models/timm/vgg13_bn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vgg16.py` & `turnkeyml-2.0.2/models/timm/vgg16.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vgg16_bn.py` & `turnkeyml-2.0.2/models/timm/vgg16_bn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vgg19.py` & `turnkeyml-2.0.2/models/timm/vgg19.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vgg19_bn.py` & `turnkeyml-2.0.2/models/timm/vgg19_bn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/visformer_small.py` & `turnkeyml-2.0.2/models/timm/visformer_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/visformer_tiny.py` & `turnkeyml-2.0.2/models/timm/visformer_tiny.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch16_18x2_224.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch16_18x2_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch16_224.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch16_224_dino.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch16_224_dino.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch16_224_in21k.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch16_224_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch16_224_miil.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch16_224_miil.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch16_224_miil_in21k.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch16_224_miil_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch16_384.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch16_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch16_plus_240.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch16_plus_240.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch16_rpn_224.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch16_rpn_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch32_224.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch32_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch32_224_in21k.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch32_224_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch32_384.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch32_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch32_plus_256.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch32_plus_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch8_224.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch8_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch8_224_dino.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch8_224_dino.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_base_patch8_224_in21k.py` & `turnkeyml-2.0.2/models/timm/vit_base_patch8_224_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_giant_patch14_224.py` & `turnkeyml-2.0.2/models/timm/vit_giant_patch14_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_gigantic_patch14_224.py` & `turnkeyml-2.0.2/models/timm/vit_gigantic_patch14_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_huge_patch14_224.py` & `turnkeyml-2.0.2/models/timm/vit_huge_patch14_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_huge_patch14_224_in21k.py` & `turnkeyml-2.0.2/models/timm/vit_huge_patch14_224_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_large_patch14_224.py` & `turnkeyml-2.0.2/models/timm/vit_large_patch14_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_large_patch16_224.py` & `turnkeyml-2.0.2/models/timm/vit_large_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_large_patch16_224_in21k.py` & `turnkeyml-2.0.2/models/timm/vit_large_patch16_224_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_large_patch16_384.py` & `turnkeyml-2.0.2/models/timm/vit_large_patch16_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_large_patch32_224.py` & `turnkeyml-2.0.2/models/timm/vit_large_patch32_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_large_patch32_224_in21k.py` & `turnkeyml-2.0.2/models/timm/vit_large_patch32_224_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_large_patch32_384.py` & `turnkeyml-2.0.2/models/timm/vit_large_patch32_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_relpos_base_patch16_224.py` & `turnkeyml-2.0.2/models/timm/vit_relpos_base_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_relpos_base_patch16_cls_224.py` & `turnkeyml-2.0.2/models/timm/vit_relpos_base_patch16_cls_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_relpos_base_patch16_clsgap_224.py` & `turnkeyml-2.0.2/models/timm/vit_relpos_base_patch16_clsgap_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_relpos_base_patch16_plus_240.py` & `turnkeyml-2.0.2/models/timm/vit_relpos_base_patch16_plus_240.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_relpos_base_patch16_rpn_224.py` & `turnkeyml-2.0.2/models/timm/vit_relpos_base_patch16_rpn_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_relpos_base_patch32_plus_rpn_256.py` & `turnkeyml-2.0.2/models/timm/vit_relpos_base_patch32_plus_rpn_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_relpos_medium_patch16_224.py` & `turnkeyml-2.0.2/models/timm/vit_relpos_medium_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_relpos_medium_patch16_cls_224.py` & `turnkeyml-2.0.2/models/timm/vit_relpos_medium_patch16_cls_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_relpos_medium_patch16_rpn_224.py` & `turnkeyml-2.0.2/models/timm/vit_relpos_medium_patch16_rpn_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_relpos_small_patch16_224.py` & `turnkeyml-2.0.2/models/timm/vit_relpos_small_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_relpos_small_patch16_rpn_224.py` & `turnkeyml-2.0.2/models/timm/vit_relpos_small_patch16_rpn_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_small_patch16_18x2_224.py` & `turnkeyml-2.0.2/models/timm/vit_small_patch16_18x2_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_small_patch16_224.py` & `turnkeyml-2.0.2/models/timm/vit_small_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_small_patch16_224_dino.py` & `turnkeyml-2.0.2/models/timm/vit_small_patch16_224_dino.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_small_patch16_224_in21k.py` & `turnkeyml-2.0.2/models/timm/vit_small_patch16_224_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_small_patch16_36x1_224.py` & `turnkeyml-2.0.2/models/timm/vit_small_patch16_36x1_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_small_patch16_384.py` & `turnkeyml-2.0.2/models/timm/vit_small_patch16_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_small_patch32_224.py` & `turnkeyml-2.0.2/models/timm/vit_small_patch32_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_small_patch32_224_in21k.py` & `turnkeyml-2.0.2/models/timm/vit_small_patch32_224_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_small_patch32_384.py` & `turnkeyml-2.0.2/models/timm/vit_small_patch32_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_small_patch8_224_dino.py` & `turnkeyml-2.0.2/models/timm/vit_small_patch8_224_dino.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_srelpos_medium_patch16_224.py` & `turnkeyml-2.0.2/models/timm/vit_srelpos_medium_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_srelpos_small_patch16_224.py` & `turnkeyml-2.0.2/models/timm/vit_srelpos_small_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_tiny_patch16_224.py` & `turnkeyml-2.0.2/models/timm/vit_tiny_patch16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_tiny_patch16_224_in21k.py` & `turnkeyml-2.0.2/models/timm/vit_tiny_patch16_224_in21k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vit_tiny_patch16_384.py` & `turnkeyml-2.0.2/models/timm/vit_tiny_patch16_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/volo_d1_224.py` & `turnkeyml-2.0.2/models/timm/volo_d1_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/volo_d1_384.py` & `turnkeyml-2.0.2/models/timm/volo_d1_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/volo_d2_224.py` & `turnkeyml-2.0.2/models/timm/volo_d2_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/volo_d2_384.py` & `turnkeyml-2.0.2/models/timm/volo_d2_384.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/volo_d3_224.py` & `turnkeyml-2.0.2/models/timm/volo_d3_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/volo_d3_448.py` & `turnkeyml-2.0.2/models/timm/volo_d3_448.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/volo_d4_224.py` & `turnkeyml-2.0.2/models/timm/volo_d4_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/volo_d4_448.py` & `turnkeyml-2.0.2/models/timm/volo_d4_448.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/volo_d5_224.py` & `turnkeyml-2.0.2/models/timm/volo_d5_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/volo_d5_448.py` & `turnkeyml-2.0.2/models/timm/volo_d5_448.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/volo_d5_512.py` & `turnkeyml-2.0.2/models/timm/volo_d5_512.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vovnet39a.py` & `turnkeyml-2.0.2/models/timm/vovnet39a.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/vovnet57a.py` & `turnkeyml-2.0.2/models/timm/vovnet57a.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/wide_resnet101_2.py` & `turnkeyml-2.0.2/models/timm/wide_resnet101_2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/wide_resnet50_2.py` & `turnkeyml-2.0.2/models/timm/wide_resnet50_2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xception.py` & `turnkeyml-2.0.2/models/timm/xception.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xception41.py` & `turnkeyml-2.0.2/models/timm/xception41.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xception41p.py` & `turnkeyml-2.0.2/models/timm/xception41p.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xception65.py` & `turnkeyml-2.0.2/models/timm/xception65.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xception65p.py` & `turnkeyml-2.0.2/models/timm/xception65p.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xception71.py` & `turnkeyml-2.0.2/models/timm/xception71.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_large_24_p16_224.py` & `turnkeyml-2.0.2/models/timm/xcit_large_24_p16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_large_24_p16_224_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_large_24_p16_224_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_large_24_p16_384_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_large_24_p16_384_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_large_24_p8_224.py` & `turnkeyml-2.0.2/models/timm/xcit_large_24_p8_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_large_24_p8_224_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_large_24_p8_224_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_large_24_p8_384_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_large_24_p8_384_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_medium_24_p16_224.py` & `turnkeyml-2.0.2/models/timm/xcit_medium_24_p16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_medium_24_p16_224_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_medium_24_p16_224_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_medium_24_p16_384_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_medium_24_p16_384_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_medium_24_p8_224.py` & `turnkeyml-2.0.2/models/timm/xcit_medium_24_p8_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_medium_24_p8_224_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_medium_24_p8_224_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_medium_24_p8_384_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_medium_24_p8_384_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_nano_12_p16_224.py` & `turnkeyml-2.0.2/models/timm/xcit_nano_12_p16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_nano_12_p16_224_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_nano_12_p16_224_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_nano_12_p16_384_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_nano_12_p16_384_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_nano_12_p8_224.py` & `turnkeyml-2.0.2/models/timm/xcit_nano_12_p8_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_nano_12_p8_224_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_nano_12_p8_224_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_nano_12_p8_384_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_nano_12_p8_384_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_small_12_p16_224.py` & `turnkeyml-2.0.2/models/timm/xcit_small_12_p16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_small_12_p16_224_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_small_12_p16_224_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_small_12_p16_384_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_small_12_p16_384_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_small_12_p8_224.py` & `turnkeyml-2.0.2/models/timm/xcit_small_12_p8_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_small_12_p8_224_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_small_12_p8_224_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_small_12_p8_384_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_small_12_p8_384_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_small_24_p16_224.py` & `turnkeyml-2.0.2/models/timm/xcit_small_24_p16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_small_24_p16_224_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_small_24_p16_224_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_small_24_p8_224.py` & `turnkeyml-2.0.2/models/timm/xcit_small_24_p8_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_small_24_p8_224_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_small_24_p8_224_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_small_24_p8_384_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_small_24_p8_384_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_tiny_12_p16_224.py` & `turnkeyml-2.0.2/models/timm/xcit_tiny_12_p16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_tiny_12_p16_224_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_tiny_12_p16_224_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_tiny_12_p16_384_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_tiny_12_p16_384_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_tiny_12_p8_224.py` & `turnkeyml-2.0.2/models/timm/xcit_tiny_12_p8_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_tiny_12_p8_224_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_tiny_12_p8_224_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_tiny_12_p8_384_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_tiny_12_p8_384_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_tiny_24_p16_224.py` & `turnkeyml-2.0.2/models/timm/xcit_tiny_24_p16_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_tiny_24_p16_224_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_tiny_24_p16_224_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_tiny_24_p16_384_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_tiny_24_p16_384_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_tiny_24_p8_224.py` & `turnkeyml-2.0.2/models/timm/xcit_tiny_24_p8_224.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_tiny_24_p8_224_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_tiny_24_p8_224_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/timm/xcit_tiny_24_p8_384_dist.py` & `turnkeyml-2.0.2/models/timm/xcit_tiny_24_p8_384_dist.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/alexnet.py` & `turnkeyml-2.0.2/models/torch_hub/alexnet.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/convnext_base.py` & `turnkeyml-2.0.2/models/torch_hub/convnext_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/convnext_large.py` & `turnkeyml-2.0.2/models/torch_hub/convnext_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/convnext_small.py` & `turnkeyml-2.0.2/models/torch_hub/convnext_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/convnext_tiny.py` & `turnkeyml-2.0.2/models/torch_hub/convnext_tiny.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/densenet121.py` & `turnkeyml-2.0.2/models/torch_hub/densenet121.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/densenet161.py` & `turnkeyml-2.0.2/models/torch_hub/densenet161.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/densenet169.py` & `turnkeyml-2.0.2/models/torch_hub/densenet169.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/densenet201.py` & `turnkeyml-2.0.2/models/torch_hub/densenet201.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/efficientnet_b1.py` & `turnkeyml-2.0.2/models/torch_hub/efficientnet_b1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/efficientnet_v2_l.py` & `turnkeyml-2.0.2/models/torch_hub/efficientnet_v2_l.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/efficientnet_v2_m.py` & `turnkeyml-2.0.2/models/torch_hub/efficientnet_v2_m.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/efficientnet_v2_s.py` & `turnkeyml-2.0.2/models/torch_hub/efficientnet_v2_s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/googlenet.py` & `turnkeyml-2.0.2/models/torch_hub/googlenet.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/hardnet39ds.py` & `turnkeyml-2.0.2/models/torch_hub/hardnet39ds.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/hardnet68.py` & `turnkeyml-2.0.2/models/torch_hub/hardnet68.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/hardnet68ds.py` & `turnkeyml-2.0.2/models/torch_hub/hardnet68ds.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/hardnet85.py` & `turnkeyml-2.0.2/models/torch_hub/hardnet85.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/inception_v3.py` & `turnkeyml-2.0.2/models/torch_hub/inception_v3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/mealv1_resnest50.py` & `turnkeyml-2.0.2/models/torch_hub/mealv1_resnest50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/mealv2_efficientnet_b0.py` & `turnkeyml-2.0.2/models/torch_hub/mealv2_efficientnet_b0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/mealv2_mobilenet_v3_large_100.py` & `turnkeyml-2.0.2/models/torch_hub/mealv2_mobilenet_v3_large_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/mealv2_mobilenetv3_small_075.py` & `turnkeyml-2.0.2/models/torch_hub/mealv2_mobilenetv3_small_075.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/mealv2_mobilenetv3_small_100.py` & `turnkeyml-2.0.2/models/torch_hub/mealv2_mobilenetv3_small_100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/mealv2_resnest50.py` & `turnkeyml-2.0.2/models/torch_hub/mealv2_resnest50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/mealv2_resnest50_380x380.py` & `turnkeyml-2.0.2/models/torch_hub/mealv2_resnest50_380x380.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/mealv2_resnest50_cutmix.py` & `turnkeyml-2.0.2/models/torch_hub/mealv2_resnest50_cutmix.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/midas_v2.1_small.py` & `turnkeyml-2.0.2/models/torch_hub/midas_v2.1_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/midas_v3_large.py` & `turnkeyml-2.0.2/models/torch_hub/midas_v3_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/mnasnet0_5.py` & `turnkeyml-2.0.2/models/torch_hub/mnasnet0_5.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/mnasnet0_75.py` & `turnkeyml-2.0.2/models/torch_hub/mnasnet0_75.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/mnasnet1_0.py` & `turnkeyml-2.0.2/models/torch_hub/mnasnet1_0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/mnasnet1_3.py` & `turnkeyml-2.0.2/models/torch_hub/mnasnet1_3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/mobilenet_v2.py` & `turnkeyml-2.0.2/models/torch_hub/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/mobilenet_v3_large.py` & `turnkeyml-2.0.2/models/torch_hub/mobilenet_v3_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/mobilenet_v3_small.py` & `turnkeyml-2.0.2/models/torch_hub/mobilenet_v3_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/proxyless_cpu.py` & `turnkeyml-2.0.2/models/torch_hub/proxyless_cpu.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/proxyless_gpu.py` & `turnkeyml-2.0.2/models/torch_hub/proxyless_gpu.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/proxyless_mobile.py` & `turnkeyml-2.0.2/models/torch_hub/proxyless_mobile.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/proxyless_mobile_14.py` & `turnkeyml-2.0.2/models/torch_hub/proxyless_mobile_14.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/regnet_x_16gf.py` & `turnkeyml-2.0.2/models/torch_hub/regnet_x_16gf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/regnet_x_1_6gf.py` & `turnkeyml-2.0.2/models/torch_hub/regnet_x_1_6gf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/regnet_x_32gf.py` & `turnkeyml-2.0.2/models/torch_hub/regnet_x_32gf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/regnet_x_3_2gf.py` & `turnkeyml-2.0.2/models/torch_hub/regnet_x_3_2gf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/regnet_x_400mf.py` & `turnkeyml-2.0.2/models/torch_hub/regnet_x_400mf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/regnet_x_800mf.py` & `turnkeyml-2.0.2/models/torch_hub/regnet_x_800mf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/regnet_x_8gf.py` & `turnkeyml-2.0.2/models/torch_hub/regnet_x_8gf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/regnet_y_128gf.py` & `turnkeyml-2.0.2/models/torch_hub/regnet_y_128gf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/regnet_y_16gf.py` & `turnkeyml-2.0.2/models/torch_hub/regnet_y_16gf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/regnet_y_1_6gf.py` & `turnkeyml-2.0.2/models/torch_hub/regnet_y_1_6gf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/regnet_y_32gf.py` & `turnkeyml-2.0.2/models/torch_hub/regnet_y_32gf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/regnet_y_3_2gf.py` & `turnkeyml-2.0.2/models/torch_hub/regnet_y_3_2gf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/regnet_y_400mf.py` & `turnkeyml-2.0.2/models/torch_hub/regnet_y_400mf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/regnet_y_800mf.py` & `turnkeyml-2.0.2/models/torch_hub/regnet_y_800mf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/regnet_y_8gf.py` & `turnkeyml-2.0.2/models/torch_hub/regnet_y_8gf.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnest101.py` & `turnkeyml-2.0.2/models/torch_hub/resnest101.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnest200.py` & `turnkeyml-2.0.2/models/torch_hub/resnest200.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnest269.py` & `turnkeyml-2.0.2/models/torch_hub/resnest269.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnest50.py` & `turnkeyml-2.0.2/models/torch_hub/resnest50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnest50_fast_1s1x64d.py` & `turnkeyml-2.0.2/models/torch_hub/resnest50_fast_1s1x64d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnest50_fast_1s2x40d.py` & `turnkeyml-2.0.2/models/torch_hub/resnest50_fast_1s2x40d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnest50_fast_1s4x24d.py` & `turnkeyml-2.0.2/models/torch_hub/resnest50_fast_1s4x24d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnest50_fast_2s1x64d.py` & `turnkeyml-2.0.2/models/torch_hub/resnest50_fast_2s1x64d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnest50_fast_2s2x40d.py` & `turnkeyml-2.0.2/models/torch_hub/resnest50_fast_2s2x40d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnest50_fast_4s1x64d.py` & `turnkeyml-2.0.2/models/torch_hub/resnest50_fast_4s1x64d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnest50_fast_4s2x40d.py` & `turnkeyml-2.0.2/models/torch_hub/resnest50_fast_4s2x40d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnet101.py` & `turnkeyml-2.0.2/models/torch_hub/resnet101.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnet101_ibn_a.py` & `turnkeyml-2.0.2/models/torch_hub/resnet101_ibn_a.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnet101_ibn_b.py` & `turnkeyml-2.0.2/models/torch_hub/resnet101_ibn_b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnet152.py` & `turnkeyml-2.0.2/models/torch_hub/resnet152.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnet18.py` & `turnkeyml-2.0.2/models/torch_hub/resnet18.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnet18_ibn_a.py` & `turnkeyml-2.0.2/models/torch_hub/resnet18_ibn_a.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnet18_ibn_b.py` & `turnkeyml-2.0.2/models/torch_hub/resnet18_ibn_b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnet34.py` & `turnkeyml-2.0.2/models/torch_hub/resnet34.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnet34_ibn_a.py` & `turnkeyml-2.0.2/models/torch_hub/resnet34_ibn_a.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnet34_ibn_b.py` & `turnkeyml-2.0.2/models/torch_hub/resnet34_ibn_b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnet50.py` & `turnkeyml-2.0.2/models/torch_hub/resnet50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnet50_ibn_a.py` & `turnkeyml-2.0.2/models/torch_hub/resnet50_ibn_a.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnet50_ibn_b.py` & `turnkeyml-2.0.2/models/torch_hub/resnet50_ibn_b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnext101_32x8d.py` & `turnkeyml-2.0.2/models/torch_hub/resnext101_32x8d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnext101_ibn_a.py` & `turnkeyml-2.0.2/models/torch_hub/resnext101_ibn_a.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/resnext50_32x4d.py` & `turnkeyml-2.0.2/models/torch_hub/resnext50_32x4d.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/se_resnet101_ibn_a.py` & `turnkeyml-2.0.2/models/torch_hub/se_resnet101_ibn_a.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/shufflenet_v2_x0_5.py` & `turnkeyml-2.0.2/models/torch_hub/shufflenet_v2_x0_5.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/shufflenet_v2_x1_0.py` & `turnkeyml-2.0.2/models/torch_hub/shufflenet_v2_x1_0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/shufflenet_v2_x1_5.py` & `turnkeyml-2.0.2/models/torch_hub/shufflenet_v2_x1_5.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/shufflenet_v2_x2_0.py` & `turnkeyml-2.0.2/models/torch_hub/shufflenet_v2_x2_0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/squeezenet1_0.py` & `turnkeyml-2.0.2/models/torch_hub/squeezenet1_0.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/squeezenet1_1.py` & `turnkeyml-2.0.2/models/torch_hub/squeezenet1_1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/swin_b.py` & `turnkeyml-2.0.2/models/torch_hub/swin_b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/swin_s.py` & `turnkeyml-2.0.2/models/torch_hub/swin_s.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/swin_t.py` & `turnkeyml-2.0.2/models/torch_hub/swin_t.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/unet.py` & `turnkeyml-2.0.2/models/torch_hub/unet.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/vgg11.py` & `turnkeyml-2.0.2/models/torch_hub/vgg11.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/vgg11_bn.py` & `turnkeyml-2.0.2/models/torch_hub/vgg11_bn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/vgg13.py` & `turnkeyml-2.0.2/models/torch_hub/vgg13.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/vgg13_bn.py` & `turnkeyml-2.0.2/models/torch_hub/vgg13_bn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/vgg16.py` & `turnkeyml-2.0.2/models/torch_hub/vgg16.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/vgg16_bn.py` & `turnkeyml-2.0.2/models/torch_hub/vgg16_bn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/vgg19.py` & `turnkeyml-2.0.2/models/torch_hub/vgg19.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/vgg19_bn.py` & `turnkeyml-2.0.2/models/torch_hub/vgg19_bn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/vit_b_16.py` & `turnkeyml-2.0.2/models/torch_hub/vit_b_16.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/vit_b_32.py` & `turnkeyml-2.0.2/models/torch_hub/vit_b_32.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/vit_l_16.py` & `turnkeyml-2.0.2/models/torch_hub/vit_l_16.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/vit_l_32.py` & `turnkeyml-2.0.2/models/torch_hub/vit_l_32.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/wide_resnet101_2.py` & `turnkeyml-2.0.2/models/torch_hub/wide_resnet101_2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torch_hub/wide_resnet50_2.py` & `turnkeyml-2.0.2/models/torch_hub/wide_resnet50_2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torchvision/fasterrcnn_mobilenet_v3_large_320_fpn.py` & `turnkeyml-2.0.2/models/torchvision/fasterrcnn_mobilenet_v3_large_320_fpn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torchvision/fasterrcnn_mobilenet_v3_large_fpn.py` & `turnkeyml-2.0.2/models/torchvision/fasterrcnn_mobilenet_v3_large_fpn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torchvision/fasterrcnn_resnet50_fpn_v2.py` & `turnkeyml-2.0.2/models/torchvision/fasterrcnn_resnet50_fpn_v2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torchvision/fcos_resnet50_fpn.py` & `turnkeyml-2.0.2/models/torchvision/fcos_resnet50_fpn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torchvision/maskrcnn_resnet50_fpn_v2.py` & `turnkeyml-2.0.2/models/torchvision/maskrcnn_resnet50_fpn_v2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/torchvision/retinanet_resnet50_fpn_v2.py` & `turnkeyml-2.0.2/models/torchvision/retinanet_resnet50_fpn_v2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/albert.py` & `turnkeyml-2.0.2/models/transformers/albert.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/albert_base_v1.py` & `turnkeyml-2.0.2/models/transformers/albert_base_v1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/albert_large_v1.py` & `turnkeyml-2.0.2/models/transformers/albert_large_v1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/albert_large_v2.py` & `turnkeyml-2.0.2/models/transformers/albert_large_v2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/albert_xlarge_v1.py` & `turnkeyml-2.0.2/models/transformers/albert_xlarge_v1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/albert_xlarge_v2.py` & `turnkeyml-2.0.2/models/transformers/albert_xlarge_v2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/albert_xxlarge_v1.py` & `turnkeyml-2.0.2/models/transformers/albert_xxlarge_v1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/albert_xxlarge_v2.py` & `turnkeyml-2.0.2/models/transformers/albert_xxlarge_v2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/auto.py` & `turnkeyml-2.0.2/models/transformers/auto.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bart.py` & `turnkeyml-2.0.2/models/transformers/bart.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bart_large.py` & `turnkeyml-2.0.2/models/transformers/bart_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/barthez.py` & `turnkeyml-2.0.2/models/transformers/barthez.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/barthez_classification.py` & `turnkeyml-2.0.2/models/transformers/barthez_classification.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/barthez_summarization.py` & `turnkeyml-2.0.2/models/transformers/barthez_summarization.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bartpho_syllable.py` & `turnkeyml-2.0.2/models/transformers/bartpho_syllable.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bartpho_syllable_base.py` & `turnkeyml-2.0.2/models/transformers/bartpho_syllable_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bartpho_word.py` & `turnkeyml-2.0.2/models/transformers/bartpho_word.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bartpho_word_base.py` & `turnkeyml-2.0.2/models/transformers/bartpho_word_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bert.py` & `turnkeyml-2.0.2/models/transformers/bert.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bert_large.py` & `turnkeyml-2.0.2/models/transformers/bert_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bertjapanese.py` & `turnkeyml-2.0.2/models/transformers/bertjapanese.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bertjapanese_large.py` & `turnkeyml-2.0.2/models/transformers/bertjapanese_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bertlmhead.py` & `turnkeyml-2.0.2/models/transformers/bertlmhead.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bertweet.py` & `turnkeyml-2.0.2/models/transformers/bertweet.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bertweet_large.py` & `turnkeyml-2.0.2/models/transformers/bertweet_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bigbird.py` & `turnkeyml-2.0.2/models/transformers/bigbird.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bigbirdpegasus.py` & `turnkeyml-2.0.2/models/transformers/bigbirdpegasus.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/biogpt.py` & `turnkeyml-2.0.2/models/transformers/biogpt.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/biogpt_large.py` & `turnkeyml-2.0.2/models/transformers/biogpt_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/blenderbot.py` & `turnkeyml-2.0.2/models/transformers/blenderbot.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/blenderbotsmall.py` & `turnkeyml-2.0.2/models/transformers/blenderbotsmall.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bloom.py` & `turnkeyml-2.0.2/models/transformers/bloom.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bloom_1b1.py` & `turnkeyml-2.0.2/models/transformers/bloom_1b1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bloom_1b7.py` & `turnkeyml-2.0.2/models/transformers/bloom_1b7.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bloom_3b.py` & `turnkeyml-2.0.2/models/transformers/bloom_3b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/bloom_7b1.py` & `turnkeyml-2.0.2/models/transformers/bloom_7b1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/camembert.py` & `turnkeyml-2.0.2/models/transformers/camembert.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/camembert_large.py` & `turnkeyml-2.0.2/models/transformers/camembert_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/canine.py` & `turnkeyml-2.0.2/models/transformers/canine.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/codegen.py` & `turnkeyml-2.0.2/models/transformers/codegen.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/codegen_350m.py` & `turnkeyml-2.0.2/models/transformers/codegen_350m.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/codegen_6b.py` & `turnkeyml-2.0.2/models/transformers/codegen_6b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/convbert.py` & `turnkeyml-2.0.2/models/transformers/convbert.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/convbert_medium_small.py` & `turnkeyml-2.0.2/models/transformers/convbert_medium_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/convbert_small.py` & `turnkeyml-2.0.2/models/transformers/convbert_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/ctrl.py` & `turnkeyml-2.0.2/models/transformers/ctrl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/ctrllmhead.py` & `turnkeyml-2.0.2/models/transformers/ctrllmhead.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/deberta.py` & `turnkeyml-2.0.2/models/transformers/deberta.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/deberta_large.py` & `turnkeyml-2.0.2/models/transformers/deberta_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/deberta_xlarge.py` & `turnkeyml-2.0.2/models/transformers/deberta_xlarge.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/debertav2.py` & `turnkeyml-2.0.2/models/transformers/debertav2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/debertav2_xxlarge.py` & `turnkeyml-2.0.2/models/transformers/debertav2_xxlarge.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/debertav3_base.py` & `turnkeyml-2.0.2/models/transformers/debertav3_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/debertav3_large.py` & `turnkeyml-2.0.2/models/transformers/debertav3_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/debertav3_small.py` & `turnkeyml-2.0.2/models/transformers/debertav3_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/debertav3_xsmall.py` & `turnkeyml-2.0.2/models/transformers/debertav3_xsmall.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/distilbert.py` & `turnkeyml-2.0.2/models/transformers/distilbert.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/dpr_context_encoder.py` & `turnkeyml-2.0.2/models/transformers/dpr_context_encoder.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/dpr_question_encoder.py` & `turnkeyml-2.0.2/models/transformers/dpr_question_encoder.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/dpr_reader.py` & `turnkeyml-2.0.2/models/transformers/dpr_reader.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/electra.py` & `turnkeyml-2.0.2/models/transformers/electra.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/electra_base.py` & `turnkeyml-2.0.2/models/transformers/electra_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/electra_generator_base.py` & `turnkeyml-2.0.2/models/transformers/electra_generator_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/electra_generator_large.py` & `turnkeyml-2.0.2/models/transformers/electra_generator_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/electra_generator_small.py` & `turnkeyml-2.0.2/models/transformers/electra_generator_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/electra_large.py` & `turnkeyml-2.0.2/models/transformers/electra_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/encoderdecoder.py` & `turnkeyml-2.0.2/models/transformers/encoderdecoder.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/ernie.py` & `turnkeyml-2.0.2/models/transformers/ernie.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/ernie2_base.py` & `turnkeyml-2.0.2/models/transformers/ernie2_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/ernie2_large.py` & `turnkeyml-2.0.2/models/transformers/ernie2_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/ernie3_base.py` & `turnkeyml-2.0.2/models/transformers/ernie3_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/ernie3_medium.py` & `turnkeyml-2.0.2/models/transformers/ernie3_medium.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/ernie3_micro.py` & `turnkeyml-2.0.2/models/transformers/ernie3_micro.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/ernie3_mini.py` & `turnkeyml-2.0.2/models/transformers/ernie3_mini.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/ernie3_nano.py` & `turnkeyml-2.0.2/models/transformers/ernie3_nano.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/ernie_health.py` & `turnkeyml-2.0.2/models/transformers/ernie_health.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/erniem.py` & `turnkeyml-2.0.2/models/transformers/erniem.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/erniem_large.py` & `turnkeyml-2.0.2/models/transformers/erniem_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/esm.py` & `turnkeyml-2.0.2/models/transformers/esm.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/esm2_150M.py` & `turnkeyml-2.0.2/models/transformers/esm2_150M.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/esm2_15B.py` & `turnkeyml-2.0.2/models/transformers/esm2_15B.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/esm2_35M.py` & `turnkeyml-2.0.2/models/transformers/esm2_35M.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/esm2_3B.py` & `turnkeyml-2.0.2/models/transformers/esm2_3B.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/esm2_650M.py` & `turnkeyml-2.0.2/models/transformers/esm2_650M.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/falcon.py` & `turnkeyml-2.0.2/models/transformers/falcon.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/falcon_40b.py` & `turnkeyml-2.0.2/models/transformers/falcon_40b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/falcon_7b.py` & `turnkeyml-2.0.2/models/transformers/falcon_7b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/flaubert.py` & `turnkeyml-2.0.2/models/transformers/flaubert.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/flaubert_large.py` & `turnkeyml-2.0.2/models/transformers/flaubert_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/flaubert_small.py` & `turnkeyml-2.0.2/models/transformers/flaubert_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/flaubertwithlmhead.py` & `turnkeyml-2.0.2/models/transformers/flaubertwithlmhead.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/flaubertwithlmhead_large.py` & `turnkeyml-2.0.2/models/transformers/flaubertwithlmhead_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/flaubertwithlmhead_small.py` & `turnkeyml-2.0.2/models/transformers/flaubertwithlmhead_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/fnet.py` & `turnkeyml-2.0.2/models/transformers/fnet.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/fnet_large.py` & `turnkeyml-2.0.2/models/transformers/fnet_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/fsmt.py` & `turnkeyml-2.0.2/models/transformers/fsmt.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/fsmt_de_en.py` & `turnkeyml-2.0.2/models/transformers/fsmt_de_en.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/fsmt_en_de.py` & `turnkeyml-2.0.2/models/transformers/fsmt_en_de.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/fsmt_en_ru.py` & `turnkeyml-2.0.2/models/transformers/fsmt_en_ru.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/funnel.py` & `turnkeyml-2.0.2/models/transformers/funnel.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/funnel_intermediate.py` & `turnkeyml-2.0.2/models/transformers/funnel_intermediate.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/funnel_intermediate_base.py` & `turnkeyml-2.0.2/models/transformers/funnel_intermediate_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/funnel_large.py` & `turnkeyml-2.0.2/models/transformers/funnel_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/funnel_large_base.py` & `turnkeyml-2.0.2/models/transformers/funnel_large_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/funnel_medium.py` & `turnkeyml-2.0.2/models/transformers/funnel_medium.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/funnel_medium_base.py` & `turnkeyml-2.0.2/models/transformers/funnel_medium_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/funnel_small_base.py` & `turnkeyml-2.0.2/models/transformers/funnel_small_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/funnel_xlarge.py` & `turnkeyml-2.0.2/models/transformers/funnel_xlarge.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/funnel_xlarge_base.py` & `turnkeyml-2.0.2/models/transformers/funnel_xlarge_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/gpt2.py` & `turnkeyml-2.0.2/models/transformers/gpt2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/gpt2doubleheads.py` & `turnkeyml-2.0.2/models/transformers/gpt2doubleheads.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/gpt2lmhead.py` & `turnkeyml-2.0.2/models/transformers/gpt2lmhead.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/gptbigcode.py` & `turnkeyml-2.0.2/models/transformers/gptbigcode.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/gptj.py` & `turnkeyml-2.0.2/models/transformers/gptj.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/gptj_tiny.py` & `turnkeyml-2.0.2/models/transformers/gptj_tiny.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/gptneo.py` & `turnkeyml-2.0.2/models/transformers/gptneo.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/gptneo_125M.py` & `turnkeyml-2.0.2/models/transformers/gptneo_125M.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/gptneo_2B7.py` & `turnkeyml-2.0.2/models/transformers/gptneo_2B7.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/gptneox.py` & `turnkeyml-2.0.2/models/transformers/gptneox.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/gptneoxjapanese.py` & `turnkeyml-2.0.2/models/transformers/gptneoxjapanese.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/ibert.py` & `turnkeyml-2.0.2/models/transformers/ibert.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/ibert_large.py` & `turnkeyml-2.0.2/models/transformers/ibert_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/led.py` & `turnkeyml-2.0.2/models/transformers/led.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/led_large.py` & `turnkeyml-2.0.2/models/transformers/led_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/llama2_13b.py` & `turnkeyml-2.0.2/models/transformers/llama2_13b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/llama2_34b.py` & `turnkeyml-2.0.2/models/transformers/llama2_34b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/llama2_70b.py` & `turnkeyml-2.0.2/models/transformers/llama2_70b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/llama2_7b.py` & `turnkeyml-2.0.2/models/transformers/llama2_7b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/longformer.py` & `turnkeyml-2.0.2/models/transformers/longformer.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/longformer_large.py` & `turnkeyml-2.0.2/models/transformers/longformer_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/longt5.py` & `turnkeyml-2.0.2/models/transformers/longt5.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/longt5_large.py` & `turnkeyml-2.0.2/models/transformers/longt5_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/longt5_tglobal_base.py` & `turnkeyml-2.0.2/models/transformers/longt5_tglobal_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/longt5_tglobal_large.py` & `turnkeyml-2.0.2/models/transformers/longt5_tglobal_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/longt5_tglobal_xl.py` & `turnkeyml-2.0.2/models/transformers/longt5_tglobal_xl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/longt5encoder.py` & `turnkeyml-2.0.2/models/transformers/longt5encoder.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/luke.py` & `turnkeyml-2.0.2/models/transformers/luke.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/luke_base_lite.py` & `turnkeyml-2.0.2/models/transformers/luke_base_lite.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/luke_japanese_base.py` & `turnkeyml-2.0.2/models/transformers/luke_japanese_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/luke_japanese_base_lite.py` & `turnkeyml-2.0.2/models/transformers/luke_japanese_base_lite.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/luke_japanese_large.py` & `turnkeyml-2.0.2/models/transformers/luke_japanese_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/luke_japanese_large_lite.py` & `turnkeyml-2.0.2/models/transformers/luke_japanese_large_lite.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/luke_large.py` & `turnkeyml-2.0.2/models/transformers/luke_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/luke_large_lite.py` & `turnkeyml-2.0.2/models/transformers/luke_large_lite.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/m2m100.py` & `turnkeyml-2.0.2/models/transformers/m2m100.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/m2m100_12B.py` & `turnkeyml-2.0.2/models/transformers/m2m100_12B.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/m2m100_1B2.py` & `turnkeyml-2.0.2/models/transformers/m2m100_1B2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/madlad400_10b.py` & `turnkeyml-2.0.2/models/transformers/madlad400_10b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/madlad400_3b.py` & `turnkeyml-2.0.2/models/transformers/madlad400_3b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/madlad400_7b.py` & `turnkeyml-2.0.2/models/transformers/madlad400_7b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/marian.py` & `turnkeyml-2.0.2/models/transformers/marian.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/markuplm.py` & `turnkeyml-2.0.2/models/transformers/markuplm.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/markuplm_large.py` & `turnkeyml-2.0.2/models/transformers/markuplm_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mbart.py` & `turnkeyml-2.0.2/models/transformers/mbart.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mbart_50.py` & `turnkeyml-2.0.2/models/transformers/mbart_50.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mbarthez.py` & `turnkeyml-2.0.2/models/transformers/mbarthez.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mega.py` & `turnkeyml-2.0.2/models/transformers/mega.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mistral_7b.py` & `turnkeyml-2.0.2/models/transformers/mistral_7b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mixtral_7bx8.py` & `turnkeyml-2.0.2/models/transformers/mixtral_7bx8.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mluke_base.py` & `turnkeyml-2.0.2/models/transformers/mluke_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mluke_base_lite.py` & `turnkeyml-2.0.2/models/transformers/mluke_base_lite.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mluke_large.py` & `turnkeyml-2.0.2/models/transformers/mluke_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mluke_large_lite.py` & `turnkeyml-2.0.2/models/transformers/mluke_large_lite.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mobilebert.py` & `turnkeyml-2.0.2/models/transformers/mobilebert.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mpnet.py` & `turnkeyml-2.0.2/models/transformers/mpnet.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mpt.py` & `turnkeyml-2.0.2/models/transformers/mpt.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mpt_30b.py` & `turnkeyml-2.0.2/models/transformers/mpt_30b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mpt_7b_8k.py` & `turnkeyml-2.0.2/models/transformers/mpt_7b_8k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mra.py` & `turnkeyml-2.0.2/models/transformers/mra.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mra_4096.py` & `turnkeyml-2.0.2/models/transformers/mra_4096.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mt5.py` & `turnkeyml-2.0.2/models/transformers/mt5.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mt5_base.py` & `turnkeyml-2.0.2/models/transformers/mt5_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mt5_large.py` & `turnkeyml-2.0.2/models/transformers/mt5_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mt5_xl.py` & `turnkeyml-2.0.2/models/transformers/mt5_xl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mt5_xxl.py` & `turnkeyml-2.0.2/models/transformers/mt5_xxl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mt5encoder.py` & `turnkeyml-2.0.2/models/transformers/mt5encoder.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mt5encoder_base.py` & `turnkeyml-2.0.2/models/transformers/mt5encoder_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mt5encoder_large.py` & `turnkeyml-2.0.2/models/transformers/mt5encoder_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mt5encoder_xl.py` & `turnkeyml-2.0.2/models/transformers/mt5encoder_xl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mt5encoder_xxl.py` & `turnkeyml-2.0.2/models/transformers/mt5encoder_xxl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/mvp.py` & `turnkeyml-2.0.2/models/transformers/mvp.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/nezha.py` & `turnkeyml-2.0.2/models/transformers/nezha.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/nezha_large.py` & `turnkeyml-2.0.2/models/transformers/nezha_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/nystromformer.py` & `turnkeyml-2.0.2/models/transformers/nystromformer.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/nystromformer_1024.py` & `turnkeyml-2.0.2/models/transformers/nystromformer_1024.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/nystromformer_2048.py` & `turnkeyml-2.0.2/models/transformers/nystromformer_2048.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/nystromformer_4096.py` & `turnkeyml-2.0.2/models/transformers/nystromformer_4096.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/openaigpt.py` & `turnkeyml-2.0.2/models/transformers/openaigpt.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/openaigptdoubleheads.py` & `turnkeyml-2.0.2/models/transformers/openaigptdoubleheads.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/openaigptlmhead.py` & `turnkeyml-2.0.2/models/transformers/openaigptlmhead.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/opt.py` & `turnkeyml-2.0.2/models/transformers/opt.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/opt_125m.py` & `turnkeyml-2.0.2/models/transformers/opt_125m.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/opt_13B.py` & `turnkeyml-2.0.2/models/transformers/opt_13B.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/opt_1B3.py` & `turnkeyml-2.0.2/models/transformers/opt_1B3.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/opt_2B7.py` & `turnkeyml-2.0.2/models/transformers/opt_2B7.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/opt_30B.py` & `turnkeyml-2.0.2/models/transformers/opt_30B.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/opt_66B.py` & `turnkeyml-2.0.2/models/transformers/opt_66B.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/opt_6B7.py` & `turnkeyml-2.0.2/models/transformers/opt_6B7.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/pegasus_base.py` & `turnkeyml-2.0.2/models/transformers/pegasus_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/pegasus_large.py` & `turnkeyml-2.0.2/models/transformers/pegasus_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/pegasus_x_base.py` & `turnkeyml-2.0.2/models/transformers/pegasus_x_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/pegasus_x_large.py` & `turnkeyml-2.0.2/models/transformers/pegasus_x_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/persimmon_8b.py` & `turnkeyml-2.0.2/models/transformers/persimmon_8b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/phi1.py` & `turnkeyml-2.0.2/models/transformers/phi1.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/phi1point5.py` & `turnkeyml-2.0.2/models/transformers/phi1point5.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/phi2.py` & `turnkeyml-2.0.2/models/transformers/phi2.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/phobert_base.py` & `turnkeyml-2.0.2/models/transformers/phobert_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/phobert_large.py` & `turnkeyml-2.0.2/models/transformers/phobert_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/plbart.py` & `turnkeyml-2.0.2/models/transformers/plbart.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/plbart_large.py` & `turnkeyml-2.0.2/models/transformers/plbart_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/prophetnet.py` & `turnkeyml-2.0.2/models/transformers/prophetnet.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/reformer.py` & `turnkeyml-2.0.2/models/transformers/reformer.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/rembert.py` & `turnkeyml-2.0.2/models/transformers/rembert.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/roberta.py` & `turnkeyml-2.0.2/models/transformers/roberta.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/roberta_large.py` & `turnkeyml-2.0.2/models/transformers/roberta_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/robertaprelayernorm.py` & `turnkeyml-2.0.2/models/transformers/robertaprelayernorm.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/rocbert.py` & `turnkeyml-2.0.2/models/transformers/rocbert.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/roformer.py` & `turnkeyml-2.0.2/models/transformers/roformer.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/roformer_small.py` & `turnkeyml-2.0.2/models/transformers/roformer_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/splinter.py` & `turnkeyml-2.0.2/models/transformers/splinter.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/splinter_large.py` & `turnkeyml-2.0.2/models/transformers/splinter_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/squeezebert.py` & `turnkeyml-2.0.2/models/transformers/squeezebert.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformers.py` & `turnkeyml-2.0.2/models/transformers/switchtransformers.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformers_base_128.py` & `turnkeyml-2.0.2/models/transformers/switchtransformers_base_128.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformers_base_16.py` & `turnkeyml-2.0.2/models/transformers/switchtransformers_base_16.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformers_base_256.py` & `turnkeyml-2.0.2/models/transformers/switchtransformers_base_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformers_base_32.py` & `turnkeyml-2.0.2/models/transformers/switchtransformers_base_32.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformers_base_64.py` & `turnkeyml-2.0.2/models/transformers/switchtransformers_base_64.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformers_large.py` & `turnkeyml-2.0.2/models/transformers/switchtransformers_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformers_xxl.py` & `turnkeyml-2.0.2/models/transformers/switchtransformers_xxl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformersencoder.py` & `turnkeyml-2.0.2/models/transformers/switchtransformersencoder.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformersencoder_base_128.py` & `turnkeyml-2.0.2/models/transformers/switchtransformersencoder_base_128.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformersencoder_base_16.py` & `turnkeyml-2.0.2/models/transformers/switchtransformersencoder_base_16.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformersencoder_base_256.py` & `turnkeyml-2.0.2/models/transformers/switchtransformersencoder_base_256.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformersencoder_base_32.py` & `turnkeyml-2.0.2/models/transformers/switchtransformersencoder_base_32.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformersencoder_base_64.py` & `turnkeyml-2.0.2/models/transformers/switchtransformersencoder_base_64.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformersencoder_large.py` & `turnkeyml-2.0.2/models/transformers/switchtransformersencoder_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/switchtransformersencoder_xxl.py` & `turnkeyml-2.0.2/models/transformers/switchtransformersencoder_xxl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/t5.py` & `turnkeyml-2.0.2/models/transformers/t5.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/t5_11b.py` & `turnkeyml-2.0.2/models/transformers/t5_11b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/t5_3b.py` & `turnkeyml-2.0.2/models/transformers/t5_3b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/t5_base.py` & `turnkeyml-2.0.2/models/transformers/t5_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/t5_large.py` & `turnkeyml-2.0.2/models/transformers/t5_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/t5encoder.py` & `turnkeyml-2.0.2/models/transformers/t5encoder.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/t5encoder_11b.py` & `turnkeyml-2.0.2/models/transformers/t5encoder_11b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/t5encoder_3b.py` & `turnkeyml-2.0.2/models/transformers/t5encoder_3b.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/t5encoder_base.py` & `turnkeyml-2.0.2/models/transformers/t5encoder_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/t5encoder_large.py` & `turnkeyml-2.0.2/models/transformers/t5encoder_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/t5v1dot1_base.py` & `turnkeyml-2.0.2/models/transformers/t5v1dot1_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/t5v1dot1_large.py` & `turnkeyml-2.0.2/models/transformers/t5v1dot1_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/t5v1dot1_small.py` & `turnkeyml-2.0.2/models/transformers/t5v1dot1_small.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/t5v1dot1_xl.py` & `turnkeyml-2.0.2/models/transformers/t5v1dot1_xl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/t5v1dot1_xxl.py` & `turnkeyml-2.0.2/models/transformers/t5v1dot1_xxl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/transfoxl.py` & `turnkeyml-2.0.2/models/transformers/transfoxl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/transfoxllmhead.py` & `turnkeyml-2.0.2/models/transformers/transfoxllmhead.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/umt5.py` & `turnkeyml-2.0.2/models/transformers/umt5.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/umt5_base.py` & `turnkeyml-2.0.2/models/transformers/umt5_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/umt5_xl.py` & `turnkeyml-2.0.2/models/transformers/umt5_xl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/umt5_xxl.py` & `turnkeyml-2.0.2/models/transformers/umt5_xxl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/umt5encoder.py` & `turnkeyml-2.0.2/models/transformers/umt5encoder.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/umt5encoder_base.py` & `turnkeyml-2.0.2/models/transformers/umt5encoder_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/umt5encoder_xl.py` & `turnkeyml-2.0.2/models/transformers/umt5encoder_xl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/umt5encoder_xxl.py` & `turnkeyml-2.0.2/models/transformers/umt5encoder_xxl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xglm.py` & `turnkeyml-2.0.2/models/transformers/xglm.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xglm_1B7.py` & `turnkeyml-2.0.2/models/transformers/xglm_1B7.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xglm_2B9.py` & `turnkeyml-2.0.2/models/transformers/xglm_2B9.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xglm_4B5.py` & `turnkeyml-2.0.2/models/transformers/xglm_4B5.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xglm_7B5.py` & `turnkeyml-2.0.2/models/transformers/xglm_7B5.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xlm.py` & `turnkeyml-2.0.2/models/transformers/xlm.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xlm_1024.py` & `turnkeyml-2.0.2/models/transformers/xlm_1024.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xlm_1280.py` & `turnkeyml-2.0.2/models/transformers/xlm_1280.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xlmroberta.py` & `turnkeyml-2.0.2/models/transformers/xlmroberta.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xlmroberta_large.py` & `turnkeyml-2.0.2/models/transformers/xlmroberta_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xlmrobertaxl.py` & `turnkeyml-2.0.2/models/transformers/xlmrobertaxl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xlmrobertaxl_xxl.py` & `turnkeyml-2.0.2/models/transformers/xlmrobertaxl_xxl.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xlmv.py` & `turnkeyml-2.0.2/models/transformers/xlmv.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xlmwithlmhead.py` & `turnkeyml-2.0.2/models/transformers/xlmwithlmhead.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xlmwithlmhead_1024.py` & `turnkeyml-2.0.2/models/transformers/xlmwithlmhead_1024.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xlmwithlmhead_1280.py` & `turnkeyml-2.0.2/models/transformers/xlmwithlmhead_1280.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xlnet.py` & `turnkeyml-2.0.2/models/transformers/xlnet.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xlnet_large.py` & `turnkeyml-2.0.2/models/transformers/xlnet_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xlnetlmhead.py` & `turnkeyml-2.0.2/models/transformers/xlnetlmhead.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xlnetlmhead_base.py` & `turnkeyml-2.0.2/models/transformers/xlnetlmhead_base.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xmod.py` & `turnkeyml-2.0.2/models/transformers/xmod.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xmod_base_13_125k.py` & `turnkeyml-2.0.2/models/transformers/xmod_base_13_125k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xmod_base_30_125k.py` & `turnkeyml-2.0.2/models/transformers/xmod_base_30_125k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xmod_base_30_195k.py` & `turnkeyml-2.0.2/models/transformers/xmod_base_30_195k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xmod_base_60_125k.py` & `turnkeyml-2.0.2/models/transformers/xmod_base_60_125k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xmod_base_60_265k.py` & `turnkeyml-2.0.2/models/transformers/xmod_base_60_265k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xmod_base_75_125k.py` & `turnkeyml-2.0.2/models/transformers/xmod_base_75_125k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xmod_base_75_269k.py` & `turnkeyml-2.0.2/models/transformers/xmod_base_75_269k.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/xmod_large.py` & `turnkeyml-2.0.2/models/transformers/xmod_large.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/models/transformers/yoso.py` & `turnkeyml-2.0.2/models/transformers/yoso.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/setup.py` & `turnkeyml-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         "invoke>=2.0.0",
         "onnx>=1.11.0",
         "onnxmltools==1.10.0",
         "hummingbird-ml==0.4.4",
         "scikit-learn==1.1.1",
         "xgboost==1.6.1",
         "lightgbm==3.3.5",
-        "onnxruntime >=1.10.1, <1.16.0",
+        "onnxruntime >=1.10.1",
         "torch>=1.12.1",
         "protobuf>=3.17.3,<3.21",
         "pyyaml>=5.4",
         "typeguard>=2.3.13",
         "packaging>=20.9",
         "pandas>=1.5.3",
         "fasteners",
```

### Comparing `turnkeyml-2.0.1/src/turnkeyml/analyze/model.py` & `turnkeyml-2.0.2/src/turnkeyml/analyze/model.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/analyze/script.py` & `turnkeyml-2.0.2/src/turnkeyml/analyze/script.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/analyze/status.py` & `turnkeyml-2.0.2/src/turnkeyml/analyze/status.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/build/export.py` & `turnkeyml-2.0.2/src/turnkeyml/build/export.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/build/hummingbird.py` & `turnkeyml-2.0.2/src/turnkeyml/build/hummingbird.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/build/ignition.py` & `turnkeyml-2.0.2/src/turnkeyml/build/ignition.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/build/onnx_helpers.py` & `turnkeyml-2.0.2/src/turnkeyml/build/onnx_helpers.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/build/sequences.py` & `turnkeyml-2.0.2/src/turnkeyml/build/sequences.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/build/stage.py` & `turnkeyml-2.0.2/src/turnkeyml/build/stage.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/build/tensor_helpers.py` & `turnkeyml-2.0.2/src/turnkeyml/build/tensor_helpers.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/build_api.py` & `turnkeyml-2.0.2/src/turnkeyml/build_api.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/cli/cli.py` & `turnkeyml-2.0.2/src/turnkeyml/cli/cli.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/cli/login.py` & `turnkeyml-2.0.2/src/turnkeyml/cli/login.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/cli/parser_helpers.py` & `turnkeyml-2.0.2/src/turnkeyml/cli/parser_helpers.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/cli/report.py` & `turnkeyml-2.0.2/src/turnkeyml/cli/report.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/cli/spawn.py` & `turnkeyml-2.0.2/src/turnkeyml/cli/spawn.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/common/build.py` & `turnkeyml-2.0.2/src/turnkeyml/common/build.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/common/exceptions.py` & `turnkeyml-2.0.2/src/turnkeyml/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/common/filesystem.py` & `turnkeyml-2.0.2/src/turnkeyml/common/filesystem.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/common/labels.py` & `turnkeyml-2.0.2/src/turnkeyml/common/labels.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/common/performance.py` & `turnkeyml-2.0.2/src/turnkeyml/common/performance.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/common/printing.py` & `turnkeyml-2.0.2/src/turnkeyml/common/printing.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/common/tf_helpers.py` & `turnkeyml-2.0.2/src/turnkeyml/common/tf_helpers.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/files_api.py` & `turnkeyml-2.0.2/src/turnkeyml/files_api.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/parser.py` & `turnkeyml-2.0.2/src/turnkeyml/parser.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/run/basert.py` & `turnkeyml-2.0.2/src/turnkeyml/run/basert.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/run/benchmark_build.py` & `turnkeyml-2.0.2/src/turnkeyml/run/benchmark_build.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,20 @@
     from tqdm import tqdm
 except ImportError:
 
     def tqdm(iterable, **kwargs):  # pylint: disable=unused-argument
         return iterable
 
 
+class SkippedBenchmark(Exception):
+    """
+    Indicates that a benchmark was skipped
+    """
+
+
 class Process(multiprocessing.Process):
     """
     Standardized way to make it possible to catch exceptions from a
     multiprocessing.Process.
     """
 
     def __init__(self, *args, **kwargs):
@@ -77,15 +83,15 @@
         iterations: same as turnkey
         rt_args: same as turnkey
     """
 
     state = build.load_state(cache_dir, build_name)
 
     if state.build_status != build.FunctionStatus.SUCCESSFUL:
-        raise exp.BenchmarkException(
+        raise SkippedBenchmark(
             "Only successful builds can be benchmarked with this "
             f"function, however selected build at {build_name} "
             f"has state: {state.build_status}"
         )
 
     selected_runtime = apply_default_runtime(state.config.device, runtime)
 
@@ -95,15 +101,15 @@
         rt_args_to_use = rt_args
 
     try:
         runtime_info = SUPPORTED_RUNTIMES[selected_runtime]
     except KeyError as e:
         # User should never get this far without hitting an actionable error message,
         # but let's raise an exception just in case.
-        raise exp.BenchmarkException(
+        raise SkippedBenchmark(
             f"Selected runtime is not supported: {selected_runtime}"
         ) from e
 
     # Check whether the device and runtime are ready for use prior to
     # running the first benchmark in the job
     # NOTE: we perform this check here, instead of in the outer loop,
     # because this is where we know `runtime_info`
@@ -291,17 +297,23 @@
         elif p.exception:
             # Handle any exception raised by the child process. In most cases, we should
             # move on to the next benchmark. However, if the exception was a
             # HardwareError that means the underlying runtime or device
             # is not able to conduct any more benchmarking. In this case the program
             # should exit and the user should follow the suggestion in the exception
             # message (e.g., restart their computer).
-            stats.save_model_eval_stat(
-                fs.Keys.BENCHMARK_STATUS, build.FunctionStatus.ERROR.value
-            )
+
+            if isinstance(p.exception[0], SkippedBenchmark):
+                stats.save_model_eval_stat(
+                    fs.Keys.BENCHMARK_STATUS, build.FunctionStatus.NOT_STARTED.value
+                )
+            else:
+                stats.save_model_eval_stat(
+                    fs.Keys.BENCHMARK_STATUS, build.FunctionStatus.ERROR.value
+                )
 
             if isinstance(p.exception[0], exp.HardwareError):
                 stats.save_model_eval_stat(fs.Keys.ERROR_LOG, p.exception[1])
                 raise p.exception[0]
             else:
                 printing.log_warning("Benchmarking failed with exception:")
                 print(p.exception[1])
```

### Comparing `turnkeyml-2.0.1/src/turnkeyml/run/devices.py` & `turnkeyml-2.0.2/src/turnkeyml/run/devices.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/run/onnxrt/execute.py` & `turnkeyml-2.0.2/src/turnkeyml/run/onnxrt/execute.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 # pylint: disable = no-name-in-module
 # pylint: disable = import-error
 import os
 import subprocess
 import json
 from statistics import mean
 import platform
+import onnxruntime
 import turnkeyml.run.plugin_helpers as plugin_helpers
 
-ORT_VERSION = "1.15.1"
+# Use the same ORT version of the base environment in the new conda env
+ORT_VERSION = onnxruntime.__version__
 
 BATCHSIZE = 1
 
 
 def create_conda_env(conda_env_name: str):
     """Create a Conda environment with the given name and install requirements."""
     conda_path = os.getenv("CONDA_EXE")
```

### Comparing `turnkeyml-2.0.1/src/turnkeyml/run/onnxrt/runtime.py` & `turnkeyml-2.0.2/src/turnkeyml/run/onnxrt/runtime.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/run/onnxrt/within_conda.py` & `turnkeyml-2.0.2/src/turnkeyml/run/onnxrt/within_conda.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/run/plugin_helpers.py` & `turnkeyml-2.0.2/src/turnkeyml/run/plugin_helpers.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/run/tensorrt/execute.py` & `turnkeyml-2.0.2/src/turnkeyml/run/tensorrt/execute.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/run/tensorrt/runtime.py` & `turnkeyml-2.0.2/src/turnkeyml/run/tensorrt/runtime.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml/run/torchrt/runtime.py` & `turnkeyml-2.0.2/src/turnkeyml/run/torchrt/runtime.py`

 * *Files identical despite different names*

### Comparing `turnkeyml-2.0.1/src/turnkeyml.egg-info/PKG-INFO` & `turnkeyml-2.0.2/src/turnkeyml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: turnkeyml
-Version: 2.0.1
+Version: 2.0.2
 Summary: TurnkeyML Tools and Models
 Author: Jeremy Fowers, Daniel Holanda, Ramakrishnan Sivakumar, Victoria Godsoe
 Author-email: jeremy.fowers@amd.com, daniel.holandanoronha@amd.com, krishna.sivakumar@amd.com, victoria.godsoe@amd.com
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE.md
 Requires-Dist: invoke>=2.0.0
 Requires-Dist: onnx>=1.11.0
 Requires-Dist: onnxmltools==1.10.0
 Requires-Dist: hummingbird-ml==0.4.4
 Requires-Dist: scikit-learn==1.1.1
 Requires-Dist: xgboost==1.6.1
 Requires-Dist: lightgbm==3.3.5
-Requires-Dist: onnxruntime<1.16.0,>=1.10.1
+Requires-Dist: onnxruntime>=1.10.1
 Requires-Dist: torch>=1.12.1
 Requires-Dist: protobuf<3.21,>=3.17.3
 Requires-Dist: pyyaml>=5.4
 Requires-Dist: typeguard>=2.3.13
 Requires-Dist: packaging>=20.9
 Requires-Dist: pandas>=1.5.3
 Requires-Dist: fasteners
```

### Comparing `turnkeyml-2.0.1/src/turnkeyml.egg-info/SOURCES.txt` & `turnkeyml-2.0.2/src/turnkeyml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

