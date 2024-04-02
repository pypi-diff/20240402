# Comparing `tmp/assonant-1.1.0.tar.gz` & `tmp/assonant-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assonant-1.1.0.tar", last modified: Wed Mar  6 12:52:11 2024, max compression
+gzip compressed data, was "assonant-1.2.0.tar", last modified: Tue Apr  2 11:54:38 2024, max compression
```

## Comparing `assonant-1.1.0.tar` & `assonant-1.2.0.tar`

### file list

```diff
@@ -1,69 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:52:11.674893 assonant-1.1.0/
--rw-r--r--   0 root         (0) root         (0)     6318 2024-03-06 12:52:11.674893 assonant-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5601 2024-03-06 12:42:03.000000 assonant-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:52:11.670893 assonant-1.1.0/assonant/
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:52:11.670893 assonant-1.1.0/assonant/_kafka/
--rw-rw-rw-   0 root         (0) root         (0)       82 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/_kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5920 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/_kafka/producer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:52:11.670893 assonant-1.1.0/assonant/_nexus/
--rw-rw-rw-   0 root         (0) root         (0)      235 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/_nexus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/_nexus/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    16420 2024-03-05 21:26:30.000000 assonant-1.1.0/assonant/_nexus/nexus_object_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:52:11.670893 assonant-1.1.0/assonant/data_classes/
--rw-rw-rw-   0 root         (0) root         (0)      834 2024-03-04 19:23:45.000000 assonant-1.1.0/assonant/data_classes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_classes/assonant_data_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:52:11.670893 assonant-1.1.0/assonant/data_classes/components/
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-02-22 21:00:18.000000 assonant-1.1.0/assonant/data_classes/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2024-02-22 21:00:18.000000 assonant-1.1.0/assonant/data_classes/components/bvs.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-02-22 21:00:18.000000 assonant-1.1.0/assonant/data_classes/components/component.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-02-22 21:00:18.000000 assonant-1.1.0/assonant/data_classes/components/detector.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-02-22 21:00:18.000000 assonant-1.1.0/assonant/data_classes/components/mirror.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-02-22 21:00:18.000000 assonant-1.1.0/assonant/data_classes/components/monochromator.py
--rw-rw-rw-   0 root         (0) root         (0)      174 2024-02-22 21:00:18.000000 assonant-1.1.0/assonant/data_classes/components/sample.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2024-02-22 21:00:18.000000 assonant-1.1.0/assonant/data_classes/components/slit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:52:11.670893 assonant-1.1.0/assonant/data_classes/data_handlers/
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_classes/data_handlers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_classes/data_handlers/axis.py
--rw-rw-rw-   0 root         (0) root         (0)      463 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_classes/data_handlers/data_field.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_classes/data_handlers/data_handler.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_classes/data_handlers/external_link.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_classes/data_handlers/time_series.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2024-02-22 21:00:18.000000 assonant-1.1.0/assonant/data_classes/entry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:52:11.670893 assonant-1.1.0/assonant/data_classes/events/
--rw-rw-rw-   0 root         (0) root         (0)      278 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_classes/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_classes/events/assonant_event.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_classes/events/experiment_done.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:52:11.674893 assonant-1.1.0/assonant/data_classes/subcomponents/
--rw-rw-rw-   0 root         (0) root         (0)      500 2024-03-04 19:23:45.000000 assonant-1.1.0/assonant/data_classes/subcomponents/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2024-03-04 19:23:45.000000 assonant-1.1.0/assonant/data_classes/subcomponents/detector_module.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2024-02-22 21:00:18.000000 assonant-1.1.0/assonant/data_classes/subcomponents/detector_roi.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-02-22 21:00:18.000000 assonant-1.1.0/assonant/data_classes/subcomponents/monochromator_crystal.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-02-22 21:00:18.000000 assonant-1.1.0/assonant/data_classes/subcomponents/monochromator_velocity_selector.py
--rw-rw-rw-   0 root         (0) root         (0)      651 2024-02-22 21:00:18.000000 assonant-1.1.0/assonant/data_classes/subcomponents/subcomponent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:52:11.674893 assonant-1.1.0/assonant/data_classes/types/
--rw-rw-rw-   0 root         (0) root         (0)      287 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_classes/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      243 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_classes/types/scope_type.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_classes/types/transformation_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:52:11.674893 assonant-1.1.0/assonant/data_sender/
--rw-rw-rw-   0 root         (0) root         (0)      341 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_sender/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      599 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_sender/_assonant_data_sender_interface.py
--rw-rw-rw-   0 root         (0) root         (0)     2693 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_sender/_data_sender_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2648 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_sender/_kafka_data_sender.py
--rw-rw-rw-   0 root         (0) root         (0)     1527 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_sender/assonant_data_sender.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/data_sender/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:52:11.674893 assonant-1.1.0/assonant/file_writer/
--rw-rw-rw-   0 root         (0) root         (0)      338 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/file_writer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      727 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/file_writer/_assonant_file_writer_interface.py
--rw-rw-rw-   0 root         (0) root         (0)     2346 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/file_writer/_file_writer_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/file_writer/_nexus_file_writer.py
--rw-rw-rw-   0 root         (0) root         (0)     2436 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/file_writer/assonant_file_writer.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-02-20 12:39:57.000000 assonant-1.1.0/assonant/file_writer/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 12:52:11.674893 assonant-1.1.0/assonant.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6318 2024-03-06 12:52:11.000000 assonant-1.1.0/assonant.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2241 2024-03-06 12:52:11.000000 assonant-1.1.0/assonant.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-06 12:52:11.000000 assonant-1.1.0/assonant.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      147 2024-03-06 12:52:11.000000 assonant-1.1.0/assonant.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-06 12:52:11.000000 assonant-1.1.0/assonant.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      840 2024-03-06 12:42:03.000000 assonant-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-06 12:52:11.674893 assonant-1.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.233060 assonant-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     6513 2024-04-02 11:54:38.233060 assonant-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5645 2024-04-01 19:04:21.000000 assonant-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.225060 assonant-1.2.0/assonant/
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.229060 assonant-1.2.0/assonant/_kafka/
+-rw-rw-rw-   0 root         (0) root         (0)       82 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/_kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5920 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/_kafka/producer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.229060 assonant-1.2.0/assonant/_nexus/
+-rw-rw-rw-   0 root         (0) root         (0)      235 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/_nexus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/_nexus/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    22987 2024-04-01 17:43:16.000000 assonant-1.2.0/assonant/_nexus/nexus_object_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.229060 assonant-1.2.0/assonant/data_classes/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2024-03-27 18:55:31.000000 assonant-1.2.0/assonant/data_classes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/assonant_data_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.229060 assonant-1.2.0/assonant/data_classes/components/
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2024-04-01 17:43:16.000000 assonant-1.2.0/assonant/data_classes/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-03-28 14:10:38.000000 assonant-1.2.0/assonant/data_classes/components/attenuator.py
+-rw-rw-rw-   0 root         (0) root         (0)      170 2024-03-28 13:44:08.000000 assonant-1.2.0/assonant/data_classes/components/beam.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-03-28 13:44:08.000000 assonant-1.2.0/assonant/data_classes/components/beam_stopper.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-03-28 13:28:11.000000 assonant-1.2.0/assonant/data_classes/components/bending_magnet.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/components/bvs.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-03-28 14:06:26.000000 assonant-1.2.0/assonant/data_classes/components/collimator.py
+-rw-rw-rw-   0 root         (0) root         (0)     9495 2024-03-27 19:22:57.000000 assonant-1.2.0/assonant/data_classes/components/component.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-03-26 18:27:23.000000 assonant-1.2.0/assonant/data_classes/components/detector.py
+-rw-rw-rw-   0 root         (0) root         (0)      208 2024-04-01 17:43:16.000000 assonant-1.2.0/assonant/data_classes/components/fresnel_zone_plate.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/components/mirror.py
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-03-26 18:27:23.000000 assonant-1.2.0/assonant/data_classes/components/monochromator.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-01 17:43:16.000000 assonant-1.2.0/assonant/data_classes/components/pinhole.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/components/sample.py
+-rw-rw-rw-   0 root         (0) root         (0)      572 2024-04-01 17:43:16.000000 assonant-1.2.0/assonant/data_classes/components/sensor.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2024-03-28 14:01:19.000000 assonant-1.2.0/assonant/data_classes/components/shutter.py
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/components/slit.py
+-rw-rw-rw-   0 root         (0) root         (0)      212 2024-03-28 13:28:11.000000 assonant-1.2.0/assonant/data_classes/components/storage_ring.py
+-rw-rw-rw-   0 root         (0) root         (0)      200 2024-03-28 13:28:11.000000 assonant-1.2.0/assonant/data_classes/components/undulator.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2024-03-28 13:28:11.000000 assonant-1.2.0/assonant/data_classes/components/wiggler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.229060 assonant-1.2.0/assonant/data_classes/data_handlers/
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/data_handlers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/data_handlers/axis.py
+-rw-rw-rw-   0 root         (0) root         (0)      463 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/data_handlers/data_field.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/data_handlers/data_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/data_handlers/external_link.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/data_handlers/time_series.py
+-rw-rw-rw-   0 root         (0) root         (0)      688 2024-03-26 18:27:23.000000 assonant-1.2.0/assonant/data_classes/entry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.229060 assonant-1.2.0/assonant/data_classes/events/
+-rw-rw-rw-   0 root         (0) root         (0)      278 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/events/assonant_event.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/events/experiment_done.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-03-27 18:55:31.000000 assonant-1.2.0/assonant/data_classes/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.233060 assonant-1.2.0/assonant/data_classes/types/
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-04-01 17:43:16.000000 assonant-1.2.0/assonant/data_classes/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-01 17:43:16.000000 assonant-1.2.0/assonant/data_classes/types/measurement_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/types/scope_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_classes/types/transformation_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.233060 assonant-1.2.0/assonant/data_sender/
+-rw-rw-rw-   0 root         (0) root         (0)      341 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_sender/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      599 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_sender/_assonant_data_sender_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     2693 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_sender/_data_sender_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2648 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_sender/_kafka_data_sender.py
+-rw-rw-rw-   0 root         (0) root         (0)     1527 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_sender/assonant_data_sender.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/data_sender/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.233060 assonant-1.2.0/assonant/file_writer/
+-rw-rw-rw-   0 root         (0) root         (0)      338 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/file_writer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      727 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/file_writer/_assonant_file_writer_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     2346 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/file_writer/_file_writer_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/file_writer/_nexus_file_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2436 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/file_writer/assonant_file_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-03-20 19:48:00.000000 assonant-1.2.0/assonant/file_writer/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 11:54:38.233060 assonant-1.2.0/assonant.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6513 2024-04-02 11:54:38.000000 assonant-1.2.0/assonant.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2546 2024-04-02 11:54:38.000000 assonant-1.2.0/assonant.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 11:54:38.000000 assonant-1.2.0/assonant.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      147 2024-04-02 11:54:38.000000 assonant-1.2.0/assonant.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-02 11:54:38.000000 assonant-1.2.0/assonant.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      976 2024-04-01 19:04:21.000000 assonant-1.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 11:54:38.233060 assonant-1.2.0/setup.cfg
```

### Comparing `assonant-1.1.0/PKG-INFO` & `assonant-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: assonant
-Version: 1.1.0
+Version: 1.2.0
 Summary: (Meta)Data standardization package for Sirius, the 4th generation brazillian synchrotron light source
 Author: Data Science and Management Group @ GCD
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: annotated-types>=0.5
 Requires-Dist: confluent-kafka>=2
 Requires-Dist: h5py>=3
 Requires-Dist: hdf5plugin>=4
 Requires-Dist: nexusformat>=1
@@ -22,15 +25,15 @@
     Welcome to Assonant 🎶 𝄇
 </h1>
 <p align="center">
     <em>A beamline-agnostic event processing engine for data collection and organization</em>
 </p>
 <p align="center">
 <a href="https://gitlab.cnpem.br/GCD/data-management/assonant#readme" target="_blank">
-    <img alt="Version" src="https://img.shields.io/badge/version-1.1.0-blue.svg?cacheSeconds=2592000"/>
+    <img alt="Version" src="https://img.shields.io/badge/version-1.2.0-blue.svg?cacheSeconds=2592000"/>
 </a>
 <a href="https://gitlab.cnpem.br/GCD/data-science/data-management/assonant/commits/dev" target="_blank">
     <img alt="Maintenance" src="https://img.shields.io/badge/Developing%3F-yes-green.svg"/>
 </a>
 <a href="https://pypi.org/project/fastapi" target="_blank">
     <img src="https://img.shields.io/badge/pyversions-3.7|3.8|3.9|3.10-orange" alt="Supported Python versions">
 </a>
@@ -99,15 +102,15 @@
 python -m pip install -e .
 ```
 
 3. After that install manually the requirements listed in the requirements-dev.txt file and install the pre-commit.
 
 ```bash
 python -m pip install -r requirements-dev.txt
-pre-commit install
+pre-commit install --install-hooks -t pre-commit -t commit-msg
 ```
 
 ## Deploy
 
 1. Firstly, remember to update the version value in this README file badge, and on the pyproject.toml file.
 
 2. Secondly, you will need to build your package:
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 2.1 Name: assonant Version: 1.1.0 Summary: (Meta)Data
+Metadata-Version: 2.1 Name: assonant Version: 1.2.0 Summary: (Meta)Data
 standardization package for Sirius, the 4th generation brazillian synchrotron
 light source Author: Data Science and Management Group @ GCD Classifier:
 License :: OSI Approved :: GNU Lesser General Public License v3 or later
-(LGPLv3+) Classifier: Programming Language :: Python :: 3.7 Requires-Python:
->=3.7 Description-Content-Type: text/markdown Requires-Dist: annotated-
+(LGPLv3+) Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
+Python: >=3.7 Description-Content-Type: text/markdown Requires-Dist: annotated-
 types>=0.5 Requires-Dist: confluent-kafka>=2 Requires-Dist: h5py>=3 Requires-
 Dist: hdf5plugin>=4 Requires-Dist: nexusformat>=1 Requires-Dist: numpy>=1
 Requires-Dist: pydantic>=2.5 Requires-Dist: pydantic_core>=2 Requires-Dist:
 scipy>=1 Requires-Dist: typing_extensions>=4
                   ************ WWeellccoommee ttoo AAssssoonnaanntt ?ð???¶ ?ð??? ************
       AA bbeeaammlliinnee--aaggnnoossttiicc eevveenntt pprroocceessssiinngg eennggiinnee ffoorr ddaattaa ccoolllleeccttiioonn aanndd
                                  oorrggaanniizzaattiioonn
@@ -45,25 +47,25 @@
 Users Assonant package can be directly installed from Pypi server by simply
 executing the following command line: ```bash python -m pip install assonant
 ``` ### Developers 1. First of all, If you want to prepare a development
 environment, clone the repository into your local machine: 2. Secondly install
 assonant by executing pip install . inside the cloned repository ```bash python
 -m pip install -e . ``` 3. After that install manually the requirements listed
 in the requirements-dev.txt file and install the pre-commit. ```bash python -
-m pip install -r requirements-dev.txt pre-commit install ``` ## Deploy 1.
-Firstly, remember to update the version value in this README file badge, and on
-the pyproject.toml file. 2. Secondly, you will need to build your package:
-```bash python -m build ``` 3. After that you need to send the new version to
-the Global PyPi version by executing the following command line. Exchange the
-place holder by the current version that will be deployed: ```bash twine upload
---repository pypi dist/assonant-* --verbose ``` **Note**: *To deploy a new
-version you will need a PyPi token which only the project maintainers have.
-That said, if you are a project maintainer and don't have access to it, ask
-your leader for it.* --- ## Mantainers - ð¤ **Allan Pinto** - ð¤ **Paulo B.
-Mausbach** --- ## Credits - **[Apache Kafka](https://github.com/apache/kafka)**
-- **[Confluent's Kafka Python Client](https://github.com/confluentinc/
-confluent-kafka-python)** - **[Dockerfile for Apache Kafka](https://github.com/
-wurstmeister/kafka-docker)** - **[JSON schema for NeXus files](https://
-github.com/ess-dmsc/nexus-json)** - **[NeXus Data Format](https://
-www.nexusformat.org/)** - **[Nexusformat (python package)](https://github.com/
-nexpy/nexusformat)** - **[Pydantic](https://github.com/pydantic/pydantic)** --
-- ## License _TODO: Define a License_ ---
+m pip install -r requirements-dev.txt pre-commit install --install-hooks -
+t pre-commit -t commit-msg ``` ## Deploy 1. Firstly, remember to update the
+version value in this README file badge, and on the pyproject.toml file. 2.
+Secondly, you will need to build your package: ```bash python -m build ``` 3.
+After that you need to send the new version to the Global PyPi version by
+executing the following command line. Exchange the place holder by the current
+version that will be deployed: ```bash twine upload --repository pypi dist/
+assonant-* --verbose ``` **Note**: *To deploy a new version you will need a
+PyPi token which only the project maintainers have. That said, if you are a
+project maintainer and don't have access to it, ask your leader for it.* --- ##
+Mantainers - ð¤ **Allan Pinto** - ð¤ **Paulo B. Mausbach** --- ## Credits -
+**[Apache Kafka](https://github.com/apache/kafka)** - **[Confluent's Kafka
+Python Client](https://github.com/confluentinc/confluent-kafka-python)** - **
+[Dockerfile for Apache Kafka](https://github.com/wurstmeister/kafka-docker)** -
+**[JSON schema for NeXus files](https://github.com/ess-dmsc/nexus-json)** - **
+[NeXus Data Format](https://www.nexusformat.org/)** - **[Nexusformat (python
+package)](https://github.com/nexpy/nexusformat)** - **[Pydantic](https://
+github.com/pydantic/pydantic)** --- ## License _TODO: Define a License_ ---
```

### Comparing `assonant-1.1.0/README.md` & `assonant-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     Welcome to Assonant 🎶 𝄇
 </h1>
 <p align="center">
     <em>A beamline-agnostic event processing engine for data collection and organization</em>
 </p>
 <p align="center">
 <a href="https://gitlab.cnpem.br/GCD/data-management/assonant#readme" target="_blank">
-    <img alt="Version" src="https://img.shields.io/badge/version-1.1.0-blue.svg?cacheSeconds=2592000"/>
+    <img alt="Version" src="https://img.shields.io/badge/version-1.2.0-blue.svg?cacheSeconds=2592000"/>
 </a>
 <a href="https://gitlab.cnpem.br/GCD/data-science/data-management/assonant/commits/dev" target="_blank">
     <img alt="Maintenance" src="https://img.shields.io/badge/Developing%3F-yes-green.svg"/>
 </a>
 <a href="https://pypi.org/project/fastapi" target="_blank">
     <img src="https://img.shields.io/badge/pyversions-3.7|3.8|3.9|3.10-orange" alt="Supported Python versions">
 </a>
@@ -79,15 +79,15 @@
 python -m pip install -e .
 ```
 
 3. After that install manually the requirements listed in the requirements-dev.txt file and install the pre-commit.
 
 ```bash
 python -m pip install -r requirements-dev.txt
-pre-commit install
+pre-commit install --install-hooks -t pre-commit -t commit-msg
 ```
 
 ## Deploy
 
 1. Firstly, remember to update the version value in this README file badge, and on the pyproject.toml file.
 
 2. Secondly, you will need to build your package:
```

#### html2text {}

```diff
@@ -35,25 +35,25 @@
 Users Assonant package can be directly installed from Pypi server by simply
 executing the following command line: ```bash python -m pip install assonant
 ``` ### Developers 1. First of all, If you want to prepare a development
 environment, clone the repository into your local machine: 2. Secondly install
 assonant by executing pip install . inside the cloned repository ```bash python
 -m pip install -e . ``` 3. After that install manually the requirements listed
 in the requirements-dev.txt file and install the pre-commit. ```bash python -
-m pip install -r requirements-dev.txt pre-commit install ``` ## Deploy 1.
-Firstly, remember to update the version value in this README file badge, and on
-the pyproject.toml file. 2. Secondly, you will need to build your package:
-```bash python -m build ``` 3. After that you need to send the new version to
-the Global PyPi version by executing the following command line. Exchange the
-place holder by the current version that will be deployed: ```bash twine upload
---repository pypi dist/assonant-* --verbose ``` **Note**: *To deploy a new
-version you will need a PyPi token which only the project maintainers have.
-That said, if you are a project maintainer and don't have access to it, ask
-your leader for it.* --- ## Mantainers - ð¤ **Allan Pinto** - ð¤ **Paulo B.
-Mausbach** --- ## Credits - **[Apache Kafka](https://github.com/apache/kafka)**
-- **[Confluent's Kafka Python Client](https://github.com/confluentinc/
-confluent-kafka-python)** - **[Dockerfile for Apache Kafka](https://github.com/
-wurstmeister/kafka-docker)** - **[JSON schema for NeXus files](https://
-github.com/ess-dmsc/nexus-json)** - **[NeXus Data Format](https://
-www.nexusformat.org/)** - **[Nexusformat (python package)](https://github.com/
-nexpy/nexusformat)** - **[Pydantic](https://github.com/pydantic/pydantic)** --
-- ## License _TODO: Define a License_ ---
+m pip install -r requirements-dev.txt pre-commit install --install-hooks -
+t pre-commit -t commit-msg ``` ## Deploy 1. Firstly, remember to update the
+version value in this README file badge, and on the pyproject.toml file. 2.
+Secondly, you will need to build your package: ```bash python -m build ``` 3.
+After that you need to send the new version to the Global PyPi version by
+executing the following command line. Exchange the place holder by the current
+version that will be deployed: ```bash twine upload --repository pypi dist/
+assonant-* --verbose ``` **Note**: *To deploy a new version you will need a
+PyPi token which only the project maintainers have. That said, if you are a
+project maintainer and don't have access to it, ask your leader for it.* --- ##
+Mantainers - ð¤ **Allan Pinto** - ð¤ **Paulo B. Mausbach** --- ## Credits -
+**[Apache Kafka](https://github.com/apache/kafka)** - **[Confluent's Kafka
+Python Client](https://github.com/confluentinc/confluent-kafka-python)** - **
+[Dockerfile for Apache Kafka](https://github.com/wurstmeister/kafka-docker)** -
+**[JSON schema for NeXus files](https://github.com/ess-dmsc/nexus-json)** - **
+[NeXus Data Format](https://www.nexusformat.org/)** - **[Nexusformat (python
+package)](https://github.com/nexpy/nexusformat)** - **[Pydantic](https://
+github.com/pydantic/pydantic)** --- ## License _TODO: Define a License_ ---
```

### Comparing `assonant-1.1.0/assonant/_kafka/producer.py` & `assonant-1.2.0/assonant/_kafka/producer.py`

 * *Files identical despite different names*

### Comparing `assonant-1.1.0/assonant/data_classes/__init__.py` & `assonant-1.2.0/assonant/data_classes/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,12 +13,14 @@
 To import and uses data classes from each type, refer to its specific submodule as shown below:
 
 from .assonant_data_class.<sub_module_name> import <data_class_name>, ...
 """
 
 from .assonant_data_class import AssonantDataClass
 from .entry import Entry
+from .exceptions import AssonantDataClassesError
 
 __all__ = [
     "AssonantDataClass",
+    "AssonantDataClassesError",
     "Entry",
 ]
```

### Comparing `assonant-1.1.0/assonant/data_classes/assonant_data_class.py` & `assonant-1.2.0/assonant/data_classes/assonant_data_class.py`

 * *Files identical despite different names*

### Comparing `assonant-1.1.0/assonant/data_classes/data_handlers/axis.py` & `assonant-1.2.0/assonant/data_classes/data_handlers/axis.py`

 * *Files identical despite different names*

### Comparing `assonant-1.1.0/assonant/data_classes/entry.py` & `assonant-1.2.0/assonant/data_classes/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 
     Entries are used to group and represent data in a defined temporal/logical scope of the
     experiment, which is directly define by the field "scope_type". e.g: calibration,
     pre-exposition.
     """
 
     scope_type: ScopeType
-    components: Optional[List[Component]] = []
+    subcomponents: Optional[List[Component]] = []
     fields: Optional[Dict[str, DataHandler]] = {}
```

### Comparing `assonant-1.1.0/assonant/data_classes/events/assonant_event.py` & `assonant-1.2.0/assonant/data_classes/events/assonant_event.py`

 * *Files identical despite different names*

### Comparing `assonant-1.1.0/assonant/data_sender/_assonant_data_sender_interface.py` & `assonant-1.2.0/assonant/data_sender/_assonant_data_sender_interface.py`

 * *Files identical despite different names*

### Comparing `assonant-1.1.0/assonant/data_sender/_data_sender_factory.py` & `assonant-1.2.0/assonant/data_sender/_data_sender_factory.py`

 * *Files identical despite different names*

### Comparing `assonant-1.1.0/assonant/data_sender/_kafka_data_sender.py` & `assonant-1.2.0/assonant/data_sender/_kafka_data_sender.py`

 * *Files identical despite different names*

### Comparing `assonant-1.1.0/assonant/data_sender/assonant_data_sender.py` & `assonant-1.2.0/assonant/data_sender/assonant_data_sender.py`

 * *Files identical despite different names*

### Comparing `assonant-1.1.0/assonant/file_writer/_assonant_file_writer_interface.py` & `assonant-1.2.0/assonant/file_writer/_assonant_file_writer_interface.py`

 * *Files identical despite different names*

### Comparing `assonant-1.1.0/assonant/file_writer/_file_writer_factory.py` & `assonant-1.2.0/assonant/file_writer/_file_writer_factory.py`

 * *Files identical despite different names*

### Comparing `assonant-1.1.0/assonant/file_writer/_nexus_file_writer.py` & `assonant-1.2.0/assonant/file_writer/_nexus_file_writer.py`

 * *Files identical despite different names*

### Comparing `assonant-1.1.0/assonant/file_writer/assonant_file_writer.py` & `assonant-1.2.0/assonant/file_writer/assonant_file_writer.py`

 * *Files identical despite different names*

### Comparing `assonant-1.1.0/assonant.egg-info/PKG-INFO` & `assonant-1.2.0/assonant.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: assonant
-Version: 1.1.0
+Version: 1.2.0
 Summary: (Meta)Data standardization package for Sirius, the 4th generation brazillian synchrotron light source
 Author: Data Science and Management Group @ GCD
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: annotated-types>=0.5
 Requires-Dist: confluent-kafka>=2
 Requires-Dist: h5py>=3
 Requires-Dist: hdf5plugin>=4
 Requires-Dist: nexusformat>=1
@@ -22,15 +25,15 @@
     Welcome to Assonant 🎶 𝄇
 </h1>
 <p align="center">
     <em>A beamline-agnostic event processing engine for data collection and organization</em>
 </p>
 <p align="center">
 <a href="https://gitlab.cnpem.br/GCD/data-management/assonant#readme" target="_blank">
-    <img alt="Version" src="https://img.shields.io/badge/version-1.1.0-blue.svg?cacheSeconds=2592000"/>
+    <img alt="Version" src="https://img.shields.io/badge/version-1.2.0-blue.svg?cacheSeconds=2592000"/>
 </a>
 <a href="https://gitlab.cnpem.br/GCD/data-science/data-management/assonant/commits/dev" target="_blank">
     <img alt="Maintenance" src="https://img.shields.io/badge/Developing%3F-yes-green.svg"/>
 </a>
 <a href="https://pypi.org/project/fastapi" target="_blank">
     <img src="https://img.shields.io/badge/pyversions-3.7|3.8|3.9|3.10-orange" alt="Supported Python versions">
 </a>
@@ -99,15 +102,15 @@
 python -m pip install -e .
 ```
 
 3. After that install manually the requirements listed in the requirements-dev.txt file and install the pre-commit.
 
 ```bash
 python -m pip install -r requirements-dev.txt
-pre-commit install
+pre-commit install --install-hooks -t pre-commit -t commit-msg
 ```
 
 ## Deploy
 
 1. Firstly, remember to update the version value in this README file badge, and on the pyproject.toml file.
 
 2. Secondly, you will need to build your package:
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 2.1 Name: assonant Version: 1.1.0 Summary: (Meta)Data
+Metadata-Version: 2.1 Name: assonant Version: 1.2.0 Summary: (Meta)Data
 standardization package for Sirius, the 4th generation brazillian synchrotron
 light source Author: Data Science and Management Group @ GCD Classifier:
 License :: OSI Approved :: GNU Lesser General Public License v3 or later
-(LGPLv3+) Classifier: Programming Language :: Python :: 3.7 Requires-Python:
->=3.7 Description-Content-Type: text/markdown Requires-Dist: annotated-
+(LGPLv3+) Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Requires-
+Python: >=3.7 Description-Content-Type: text/markdown Requires-Dist: annotated-
 types>=0.5 Requires-Dist: confluent-kafka>=2 Requires-Dist: h5py>=3 Requires-
 Dist: hdf5plugin>=4 Requires-Dist: nexusformat>=1 Requires-Dist: numpy>=1
 Requires-Dist: pydantic>=2.5 Requires-Dist: pydantic_core>=2 Requires-Dist:
 scipy>=1 Requires-Dist: typing_extensions>=4
                   ************ WWeellccoommee ttoo AAssssoonnaanntt ?ð???¶ ?ð??? ************
       AA bbeeaammlliinnee--aaggnnoossttiicc eevveenntt pprroocceessssiinngg eennggiinnee ffoorr ddaattaa ccoolllleeccttiioonn aanndd
                                  oorrggaanniizzaattiioonn
@@ -45,25 +47,25 @@
 Users Assonant package can be directly installed from Pypi server by simply
 executing the following command line: ```bash python -m pip install assonant
 ``` ### Developers 1. First of all, If you want to prepare a development
 environment, clone the repository into your local machine: 2. Secondly install
 assonant by executing pip install . inside the cloned repository ```bash python
 -m pip install -e . ``` 3. After that install manually the requirements listed
 in the requirements-dev.txt file and install the pre-commit. ```bash python -
-m pip install -r requirements-dev.txt pre-commit install ``` ## Deploy 1.
-Firstly, remember to update the version value in this README file badge, and on
-the pyproject.toml file. 2. Secondly, you will need to build your package:
-```bash python -m build ``` 3. After that you need to send the new version to
-the Global PyPi version by executing the following command line. Exchange the
-place holder by the current version that will be deployed: ```bash twine upload
---repository pypi dist/assonant-* --verbose ``` **Note**: *To deploy a new
-version you will need a PyPi token which only the project maintainers have.
-That said, if you are a project maintainer and don't have access to it, ask
-your leader for it.* --- ## Mantainers - ð¤ **Allan Pinto** - ð¤ **Paulo B.
-Mausbach** --- ## Credits - **[Apache Kafka](https://github.com/apache/kafka)**
-- **[Confluent's Kafka Python Client](https://github.com/confluentinc/
-confluent-kafka-python)** - **[Dockerfile for Apache Kafka](https://github.com/
-wurstmeister/kafka-docker)** - **[JSON schema for NeXus files](https://
-github.com/ess-dmsc/nexus-json)** - **[NeXus Data Format](https://
-www.nexusformat.org/)** - **[Nexusformat (python package)](https://github.com/
-nexpy/nexusformat)** - **[Pydantic](https://github.com/pydantic/pydantic)** --
-- ## License _TODO: Define a License_ ---
+m pip install -r requirements-dev.txt pre-commit install --install-hooks -
+t pre-commit -t commit-msg ``` ## Deploy 1. Firstly, remember to update the
+version value in this README file badge, and on the pyproject.toml file. 2.
+Secondly, you will need to build your package: ```bash python -m build ``` 3.
+After that you need to send the new version to the Global PyPi version by
+executing the following command line. Exchange the place holder by the current
+version that will be deployed: ```bash twine upload --repository pypi dist/
+assonant-* --verbose ``` **Note**: *To deploy a new version you will need a
+PyPi token which only the project maintainers have. That said, if you are a
+project maintainer and don't have access to it, ask your leader for it.* --- ##
+Mantainers - ð¤ **Allan Pinto** - ð¤ **Paulo B. Mausbach** --- ## Credits -
+**[Apache Kafka](https://github.com/apache/kafka)** - **[Confluent's Kafka
+Python Client](https://github.com/confluentinc/confluent-kafka-python)** - **
+[Dockerfile for Apache Kafka](https://github.com/wurstmeister/kafka-docker)** -
+**[JSON schema for NeXus files](https://github.com/ess-dmsc/nexus-json)** - **
+[NeXus Data Format](https://www.nexusformat.org/)** - **[Nexusformat (python
+package)](https://github.com/nexpy/nexusformat)** - **[Pydantic](https://
+github.com/pydantic/pydantic)** --- ## License _TODO: Define a License_ ---
```

### Comparing `assonant-1.1.0/assonant.egg-info/SOURCES.txt` & `assonant-1.2.0/assonant.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,38 +10,46 @@
 assonant/_kafka/producer.py
 assonant/_nexus/__init__.py
 assonant/_nexus/exceptions.py
 assonant/_nexus/nexus_object_factory.py
 assonant/data_classes/__init__.py
 assonant/data_classes/assonant_data_class.py
 assonant/data_classes/entry.py
+assonant/data_classes/exceptions.py
 assonant/data_classes/components/__init__.py
+assonant/data_classes/components/attenuator.py
+assonant/data_classes/components/beam.py
+assonant/data_classes/components/beam_stopper.py
+assonant/data_classes/components/bending_magnet.py
 assonant/data_classes/components/bvs.py
+assonant/data_classes/components/collimator.py
 assonant/data_classes/components/component.py
 assonant/data_classes/components/detector.py
+assonant/data_classes/components/fresnel_zone_plate.py
 assonant/data_classes/components/mirror.py
 assonant/data_classes/components/monochromator.py
+assonant/data_classes/components/pinhole.py
 assonant/data_classes/components/sample.py
+assonant/data_classes/components/sensor.py
+assonant/data_classes/components/shutter.py
 assonant/data_classes/components/slit.py
+assonant/data_classes/components/storage_ring.py
+assonant/data_classes/components/undulator.py
+assonant/data_classes/components/wiggler.py
 assonant/data_classes/data_handlers/__init__.py
 assonant/data_classes/data_handlers/axis.py
 assonant/data_classes/data_handlers/data_field.py
 assonant/data_classes/data_handlers/data_handler.py
 assonant/data_classes/data_handlers/external_link.py
 assonant/data_classes/data_handlers/time_series.py
 assonant/data_classes/events/__init__.py
 assonant/data_classes/events/assonant_event.py
 assonant/data_classes/events/experiment_done.py
-assonant/data_classes/subcomponents/__init__.py
-assonant/data_classes/subcomponents/detector_module.py
-assonant/data_classes/subcomponents/detector_roi.py
-assonant/data_classes/subcomponents/monochromator_crystal.py
-assonant/data_classes/subcomponents/monochromator_velocity_selector.py
-assonant/data_classes/subcomponents/subcomponent.py
 assonant/data_classes/types/__init__.py
+assonant/data_classes/types/measurement_type.py
 assonant/data_classes/types/scope_type.py
 assonant/data_classes/types/transformation_type.py
 assonant/data_sender/__init__.py
 assonant/data_sender/_assonant_data_sender_interface.py
 assonant/data_sender/_data_sender_factory.py
 assonant/data_sender/_kafka_data_sender.py
 assonant/data_sender/assonant_data_sender.py
```

### Comparing `assonant-1.1.0/pyproject.toml` & `assonant-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "assonant"
-version="1.1.0"
+version="1.2.0"
 description = "(Meta)Data standardization package for Sirius, the 4th generation brazillian synchrotron light source"
 authors = [
     {name = "Data Science and Management Group @ GCD"}
 ]
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 requires-python = ">=3.7"
@@ -22,12 +22,15 @@
     "pydantic>=2.5",
     "pydantic_core>=2",
     "scipy>=1",
     "typing_extensions>=4",
 ]
 classifiers = [
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
-    "Programming Language :: Python :: 3.7"
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10"
 ]
 
 [tool.setuptools]
 package-dir = {"assonant" = "assonant"}
```

