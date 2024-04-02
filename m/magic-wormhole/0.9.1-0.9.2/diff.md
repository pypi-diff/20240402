# Comparing `tmp/magic-wormhole-0.9.1.tar.gz` & `tmp/magic-wormhole-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/magic-wormhole-0.9.1.tar", last modified: Sun Jan  1 18:18:25 2017, max compression
+gzip compressed data, was "dist/magic-wormhole-0.9.2.tar", last modified: Mon Jan 16 23:23:48 2017, max compression
```

## Comparing `magic-wormhole-0.9.1.tar` & `magic-wormhole-0.9.2.tar`

### file list

```diff
@@ -1,91 +1,95 @@
-drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/
--rw-r--r--   0 warner     (502) staff       (20)      697 2016-05-24 23:05:34.000000 magic-wormhole-0.9.1/.coveragerc
-drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/docs/
--rw-r--r--   0 warner     (502) staff       (20)     9226 2016-05-27 06:20:37.000000 magic-wormhole-0.9.1/docs/api.md
--rw-r--r--   0 warner     (502) staff       (20)    10037 2016-02-18 16:26:14.000000 magic-wormhole-0.9.1/docs/transit.md
--rw-r--r--   0 warner     (502) staff       (20)      832 2016-12-22 21:13:32.000000 magic-wormhole-0.9.1/docs/wormhole-server.8
--rw-r--r--   0 warner     (502) staff       (20)     1089 2016-12-22 21:13:32.000000 magic-wormhole-0.9.1/docs/wormhole.1
--rw-r--r--   0 warner     (502) staff       (20)     1080 2015-02-11 22:28:13.000000 magic-wormhole-0.9.1/LICENSE
--rw-r--r--   0 warner     (502) staff       (20)      559 2016-12-30 18:57:39.000000 magic-wormhole-0.9.1/MANIFEST.in
-drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/misc/
--rwxr-xr-x   0 warner     (502) staff       (20)      421 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/misc/dump-stats.py
--rw-r--r--   0 warner     (502) staff       (20)     2016 2016-05-09 22:14:32.000000 magic-wormhole-0.9.1/misc/dump-timing.py
-drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/misc/munin/
--rwxr-xr-x   0 warner     (502) staff       (20)     1260 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/misc/munin/wormhole_active
--rwxr-xr-x   0 warner     (502) staff       (20)     1322 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/misc/munin/wormhole_errors
--rwxr-xr-x   0 warner     (502) staff       (20)     1115 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/misc/munin/wormhole_event_rate
--rwxr-xr-x   0 warner     (502) staff       (20)     1280 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/misc/munin/wormhole_events
--rw-r--r--   0 warner     (502) staff       (20)     1277 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/misc/munin/wormhole_events_alltime
--rwxr-xr-x   0 warner     (502) staff       (20)      715 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/misc/munin/wormhole_transit
--rw-r--r--   0 warner     (502) staff       (20)      712 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/misc/munin/wormhole_transit_alltime
-drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/misc/web/
--rw-r--r--   0 warner     (502) staff       (20)     1229 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/misc/web/timeline.css
--rw-r--r--   0 warner     (502) staff       (20)      473 2016-05-02 17:34:07.000000 magic-wormhole-0.9.1/misc/web/timeline.html
--rw-r--r--   0 warner     (502) staff       (20)    38820 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/misc/web/timeline.js
--rw-r--r--   0 warner     (502) staff       (20)      838 2016-02-28 18:02:04.000000 magic-wormhole-0.9.1/misc/windows-build.cmd
--rw-r--r--   0 warner     (502) staff       (20)    14755 2017-01-01 18:14:22.000000 magic-wormhole-0.9.1/NEWS.md
--rw-r--r--   0 warner     (502) staff       (20)      280 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/PKG-INFO
--rw-r--r--   0 warner     (502) staff       (20)     8650 2016-12-30 18:59:29.000000 magic-wormhole-0.9.1/README.md
--rw-r--r--   0 warner     (502) staff       (20)      241 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/setup.cfg
--rw-r--r--   0 warner     (502) staff       (20)     1332 2016-12-30 18:59:46.000000 magic-wormhole-0.9.1/setup.py
-drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/src/
-drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/src/magic_wormhole.egg-info/
--rw-r--r--   0 warner     (502) staff       (20)        1 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/src/magic_wormhole.egg-info/dependency_links.txt
--rw-r--r--   0 warner     (502) staff       (20)      101 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/src/magic_wormhole.egg-info/entry_points.txt
--rw-r--r--   0 warner     (502) staff       (20)      280 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/src/magic_wormhole.egg-info/PKG-INFO
--rw-r--r--   0 warner     (502) staff       (20)      176 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/src/magic_wormhole.egg-info/requires.txt
--rw-r--r--   0 warner     (502) staff       (20)     2167 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/src/magic_wormhole.egg-info/SOURCES.txt
--rw-r--r--   0 warner     (502) staff       (20)        9 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/src/magic_wormhole.egg-info/top_level.txt
-drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/src/wormhole/
--rw-r--r--   0 warner     (502) staff       (20)       93 2016-04-15 23:01:07.000000 magic-wormhole-0.9.1/src/wormhole/__init__.py
--rw-r--r--   0 warner     (502) staff       (20)      497 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/src/wormhole/_version.py
--rw-r--r--   0 warner     (502) staff       (20)      473 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/channel_monitor.py
-drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/src/wormhole/cli/
--rw-r--r--   0 warner     (502) staff       (20)        0 2016-04-21 02:20:39.000000 magic-wormhole-0.9.1/src/wormhole/cli/__init__.py
--rw-r--r--   0 warner     (502) staff       (20)     8446 2016-12-24 03:35:14.000000 magic-wormhole-0.9.1/src/wormhole/cli/cli.py
--rw-r--r--   0 warner     (502) staff       (20)    13924 2016-12-24 05:18:53.000000 magic-wormhole-0.9.1/src/wormhole/cli/cmd_receive.py
--rw-r--r--   0 warner     (502) staff       (20)    12135 2016-12-24 05:18:53.000000 magic-wormhole-0.9.1/src/wormhole/cli/cmd_send.py
--rw-r--r--   0 warner     (502) staff       (20)     3719 2016-12-24 03:35:14.000000 magic-wormhole-0.9.1/src/wormhole/cli/cmd_ssh.py
--rw-r--r--   0 warner     (502) staff       (20)      218 2016-05-29 02:03:56.000000 magic-wormhole-0.9.1/src/wormhole/cli/public_relay.py
--rw-r--r--   0 warner     (502) staff       (20)     4124 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/codes.py
--rw-r--r--   0 warner     (502) staff       (20)     1725 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/errors.py
--rw-r--r--   0 warner     (502) staff       (20)     3011 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/ipaddrs.py
-drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/src/wormhole/server/
--rw-r--r--   0 warner     (502) staff       (20)        0 2016-04-21 02:20:39.000000 magic-wormhole-0.9.1/src/wormhole/server/__init__.py
--rw-r--r--   0 warner     (502) staff       (20)     4022 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/server/cli.py
--rw-r--r--   0 warner     (502) staff       (20)     2116 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/server/cmd_server.py
--rw-r--r--   0 warner     (502) staff       (20)     9166 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/server/cmd_usage.py
--rw-r--r--   0 warner     (502) staff       (20)     2970 2016-12-24 03:34:56.000000 magic-wormhole-0.9.1/src/wormhole/server/database.py
-drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/src/wormhole/server/db-schemas/
--rw-r--r--   0 warner     (502) staff       (20)     2215 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/server/db-schemas/upgrade-to-v3.sql
--rw-r--r--   0 warner     (502) staff       (20)     4090 2016-06-21 00:26:52.000000 magic-wormhole-0.9.1/src/wormhole/server/db-schemas/v2.sql
--rw-r--r--   0 warner     (502) staff       (20)     4308 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/server/db-schemas/v3.sql
--rw-r--r--   0 warner     (502) staff       (20)    28376 2016-12-30 18:57:39.000000 magic-wormhole-0.9.1/src/wormhole/server/rendezvous.py
--rw-r--r--   0 warner     (502) staff       (20)    12161 2016-12-30 18:57:39.000000 magic-wormhole-0.9.1/src/wormhole/server/rendezvous_websocket.py
--rw-r--r--   0 warner     (502) staff       (20)     2071 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/server/runner.py
--rw-r--r--   0 warner     (502) staff       (20)     5311 2017-01-01 17:58:43.000000 magic-wormhole-0.9.1/src/wormhole/server/server.py
--rw-r--r--   0 warner     (502) staff       (20)    13594 2017-01-01 17:54:04.000000 magic-wormhole-0.9.1/src/wormhole/server/transit_server.py
-drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-01 18:18:25.000000 magic-wormhole-0.9.1/src/wormhole/test/
--rw-r--r--   0 warner     (502) staff       (20)        0 2016-04-21 02:20:39.000000 magic-wormhole-0.9.1/src/wormhole/test/__init__.py
--rw-r--r--   0 warner     (502) staff       (20)     3507 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/test/common.py
--rw-r--r--   0 warner     (502) staff       (20)      623 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/test/run_trial.py
--rw-r--r--   0 warner     (502) staff       (20)     5065 2016-12-24 03:35:14.000000 magic-wormhole-0.9.1/src/wormhole/test/test_args.py
--rw-r--r--   0 warner     (502) staff       (20)     2077 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/test/test_database.py
--rw-r--r--   0 warner     (502) staff       (20)     1798 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/test/test_hkdf.py
--rw-r--r--   0 warner     (502) staff       (20)    31005 2016-12-24 05:18:53.000000 magic-wormhole-0.9.1/src/wormhole/test/test_scripts.py
--rw-r--r--   0 warner     (502) staff       (20)    49049 2016-12-30 18:57:39.000000 magic-wormhole-0.9.1/src/wormhole/test/test_server.py
--rw-r--r--   0 warner     (502) staff       (20)     2721 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/test/test_ssh.py
--rw-r--r--   0 warner     (502) staff       (20)    58807 2016-12-31 05:59:20.000000 magic-wormhole-0.9.1/src/wormhole/test/test_transit.py
--rw-r--r--   0 warner     (502) staff       (20)    10814 2016-12-30 18:57:39.000000 magic-wormhole-0.9.1/src/wormhole/test/test_transit_server.py
--rw-r--r--   0 warner     (502) staff       (20)     1693 2016-12-22 21:13:32.000000 magic-wormhole-0.9.1/src/wormhole/test/test_util.py
--rw-r--r--   0 warner     (502) staff       (20)    36691 2016-12-30 18:59:29.000000 magic-wormhole-0.9.1/src/wormhole/test/test_wormhole.py
--rw-r--r--   0 warner     (502) staff       (20)     1780 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/test/test_xfer_util.py
--rw-r--r--   0 warner     (502) staff       (20)     1993 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/timing.py
--rw-r--r--   0 warner     (502) staff       (20)     5975 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/tor_manager.py
--rw-r--r--   0 warner     (502) staff       (20)    37682 2016-12-31 05:59:20.000000 magic-wormhole-0.9.1/src/wormhole/transit.py
--rw-r--r--   0 warner     (502) staff       (20)     1291 2016-12-22 21:13:32.000000 magic-wormhole-0.9.1/src/wormhole/util.py
--rw-r--r--   0 warner     (502) staff       (20)     9220 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/wordlist.py
--rw-r--r--   0 warner     (502) staff       (20)    38248 2016-12-30 18:59:46.000000 magic-wormhole-0.9.1/src/wormhole/wormhole.py
--rw-r--r--   0 warner     (502) staff       (20)     3131 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/src/wormhole/xfer_util.py
--rw-r--r--   0 warner     (502) staff       (20)     1715 2016-12-30 18:59:29.000000 magic-wormhole-0.9.1/tox.ini
--rw-r--r--   0 warner     (502) staff       (20)    68587 2016-12-15 15:20:20.000000 magic-wormhole-0.9.1/versioneer.py
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/
+-rw-r--r--   0 warner     (502) staff       (20)      697 2016-05-24 23:05:34.000000 magic-wormhole-0.9.2/.coveragerc
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/docs/
+-rw-r--r--   0 warner     (502) staff       (20)     9226 2016-05-27 06:20:37.000000 magic-wormhole-0.9.2/docs/api.md
+-rw-r--r--   0 warner     (502) staff       (20)     4714 2017-01-12 22:35:51.000000 magic-wormhole-0.9.2/docs/attacks.md
+-rw-r--r--   0 warner     (502) staff       (20)     3895 2017-01-16 23:21:42.000000 magic-wormhole-0.9.2/docs/tor.md
+-rw-r--r--   0 warner     (502) staff       (20)    10037 2016-02-18 16:26:14.000000 magic-wormhole-0.9.2/docs/transit.md
+-rw-r--r--   0 warner     (502) staff       (20)      832 2016-12-22 21:13:32.000000 magic-wormhole-0.9.2/docs/wormhole-server.8
+-rw-r--r--   0 warner     (502) staff       (20)     1089 2016-12-22 21:13:32.000000 magic-wormhole-0.9.2/docs/wormhole.1
+-rw-r--r--   0 warner     (502) staff       (20)     1080 2015-02-11 22:28:13.000000 magic-wormhole-0.9.2/LICENSE
+-rw-r--r--   0 warner     (502) staff       (20)      574 2017-01-16 23:10:01.000000 magic-wormhole-0.9.2/MANIFEST.in
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/misc/
+-rwxr-xr-x   0 warner     (502) staff       (20)      421 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/misc/dump-stats.py
+-rw-r--r--   0 warner     (502) staff       (20)     2016 2016-05-09 22:14:32.000000 magic-wormhole-0.9.2/misc/dump-timing.py
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/misc/munin/
+-rwxr-xr-x   0 warner     (502) staff       (20)     1260 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/misc/munin/wormhole_active
+-rwxr-xr-x   0 warner     (502) staff       (20)     1322 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/misc/munin/wormhole_errors
+-rwxr-xr-x   0 warner     (502) staff       (20)     1115 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/misc/munin/wormhole_event_rate
+-rwxr-xr-x   0 warner     (502) staff       (20)     1280 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/misc/munin/wormhole_events
+-rw-r--r--   0 warner     (502) staff       (20)     1277 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/misc/munin/wormhole_events_alltime
+-rwxr-xr-x   0 warner     (502) staff       (20)      715 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/misc/munin/wormhole_transit
+-rw-r--r--   0 warner     (502) staff       (20)      712 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/misc/munin/wormhole_transit_alltime
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/misc/web/
+-rw-r--r--   0 warner     (502) staff       (20)     1229 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/misc/web/timeline.css
+-rw-r--r--   0 warner     (502) staff       (20)      473 2016-05-02 17:34:07.000000 magic-wormhole-0.9.2/misc/web/timeline.html
+-rw-r--r--   0 warner     (502) staff       (20)    38820 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/misc/web/timeline.js
+-rw-r--r--   0 warner     (502) staff       (20)      838 2016-02-28 18:02:04.000000 magic-wormhole-0.9.2/misc/windows-build.cmd
+-rw-r--r--   0 warner     (502) staff       (20)    16451 2017-01-16 23:21:42.000000 magic-wormhole-0.9.2/NEWS.md
+-rw-r--r--   0 warner     (502) staff       (20)      280 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/PKG-INFO
+-rw-r--r--   0 warner     (502) staff       (20)     8654 2017-01-13 00:34:57.000000 magic-wormhole-0.9.2/README.md
+-rw-r--r--   0 warner     (502) staff       (20)      241 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/setup.cfg
+-rw-r--r--   0 warner     (502) staff       (20)     1875 2017-01-16 16:37:44.000000 magic-wormhole-0.9.2/setup.py
+-rw-r--r--   0 warner     (502) staff       (20)     1076 2017-01-13 00:34:57.000000 magic-wormhole-0.9.2/snapcraft.yaml
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/src/
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/src/magic_wormhole.egg-info/
+-rw-r--r--   0 warner     (502) staff       (20)        1 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/src/magic_wormhole.egg-info/dependency_links.txt
+-rw-r--r--   0 warner     (502) staff       (20)      101 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/src/magic_wormhole.egg-info/entry_points.txt
+-rw-r--r--   0 warner     (502) staff       (20)      280 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/src/magic_wormhole.egg-info/PKG-INFO
+-rw-r--r--   0 warner     (502) staff       (20)      185 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/src/magic_wormhole.egg-info/requires.txt
+-rw-r--r--   0 warner     (502) staff       (20)     2248 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/src/magic_wormhole.egg-info/SOURCES.txt
+-rw-r--r--   0 warner     (502) staff       (20)        9 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/src/magic_wormhole.egg-info/top_level.txt
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/src/wormhole/
+-rw-r--r--   0 warner     (502) staff       (20)       93 2016-04-15 23:01:07.000000 magic-wormhole-0.9.2/src/wormhole/__init__.py
+-rw-r--r--   0 warner     (502) staff       (20)      497 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/src/wormhole/_version.py
+-rw-r--r--   0 warner     (502) staff       (20)      473 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/channel_monitor.py
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/src/wormhole/cli/
+-rw-r--r--   0 warner     (502) staff       (20)        0 2016-04-21 02:20:39.000000 magic-wormhole-0.9.2/src/wormhole/cli/__init__.py
+-rw-r--r--   0 warner     (502) staff       (20)     9021 2017-01-16 16:37:44.000000 magic-wormhole-0.9.2/src/wormhole/cli/cli.py
+-rw-r--r--   0 warner     (502) staff       (20)    14161 2017-01-16 22:23:31.000000 magic-wormhole-0.9.2/src/wormhole/cli/cmd_receive.py
+-rw-r--r--   0 warner     (502) staff       (20)    12505 2017-01-16 22:44:44.000000 magic-wormhole-0.9.2/src/wormhole/cli/cmd_send.py
+-rw-r--r--   0 warner     (502) staff       (20)     3883 2017-01-16 16:37:44.000000 magic-wormhole-0.9.2/src/wormhole/cli/cmd_ssh.py
+-rw-r--r--   0 warner     (502) staff       (20)      214 2017-01-13 00:34:57.000000 magic-wormhole-0.9.2/src/wormhole/cli/public_relay.py
+-rw-r--r--   0 warner     (502) staff       (20)     4427 2017-01-15 21:10:55.000000 magic-wormhole-0.9.2/src/wormhole/codes.py
+-rw-r--r--   0 warner     (502) staff       (20)     1819 2017-01-16 16:37:44.000000 magic-wormhole-0.9.2/src/wormhole/errors.py
+-rw-r--r--   0 warner     (502) staff       (20)     3011 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/ipaddrs.py
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/src/wormhole/server/
+-rw-r--r--   0 warner     (502) staff       (20)        0 2016-04-21 02:20:39.000000 magic-wormhole-0.9.2/src/wormhole/server/__init__.py
+-rw-r--r--   0 warner     (502) staff       (20)     4022 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/server/cli.py
+-rw-r--r--   0 warner     (502) staff       (20)     2116 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/server/cmd_server.py
+-rw-r--r--   0 warner     (502) staff       (20)     9166 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/server/cmd_usage.py
+-rw-r--r--   0 warner     (502) staff       (20)     2970 2016-12-24 03:34:56.000000 magic-wormhole-0.9.2/src/wormhole/server/database.py
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/src/wormhole/server/db-schemas/
+-rw-r--r--   0 warner     (502) staff       (20)     2215 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/server/db-schemas/upgrade-to-v3.sql
+-rw-r--r--   0 warner     (502) staff       (20)     4090 2016-06-21 00:26:52.000000 magic-wormhole-0.9.2/src/wormhole/server/db-schemas/v2.sql
+-rw-r--r--   0 warner     (502) staff       (20)     4308 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/server/db-schemas/v3.sql
+-rw-r--r--   0 warner     (502) staff       (20)    28376 2016-12-30 18:57:39.000000 magic-wormhole-0.9.2/src/wormhole/server/rendezvous.py
+-rw-r--r--   0 warner     (502) staff       (20)    12161 2016-12-30 18:57:39.000000 magic-wormhole-0.9.2/src/wormhole/server/rendezvous_websocket.py
+-rw-r--r--   0 warner     (502) staff       (20)     2071 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/server/runner.py
+-rw-r--r--   0 warner     (502) staff       (20)     5311 2017-01-12 22:35:51.000000 magic-wormhole-0.9.2/src/wormhole/server/server.py
+-rw-r--r--   0 warner     (502) staff       (20)    13594 2017-01-12 22:35:51.000000 magic-wormhole-0.9.2/src/wormhole/server/transit_server.py
+drwxr-xr-x   0 warner     (502) staff       (20)        0 2017-01-16 23:23:48.000000 magic-wormhole-0.9.2/src/wormhole/test/
+-rw-r--r--   0 warner     (502) staff       (20)        0 2016-04-21 02:20:39.000000 magic-wormhole-0.9.2/src/wormhole/test/__init__.py
+-rw-r--r--   0 warner     (502) staff       (20)     3507 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/test/common.py
+-rw-r--r--   0 warner     (502) staff       (20)      623 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/test/run_trial.py
+-rw-r--r--   0 warner     (502) staff       (20)     5065 2016-12-24 03:35:14.000000 magic-wormhole-0.9.2/src/wormhole/test/test_args.py
+-rw-r--r--   0 warner     (502) staff       (20)     2077 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/test/test_database.py
+-rw-r--r--   0 warner     (502) staff       (20)     1798 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/test/test_hkdf.py
+-rw-r--r--   0 warner     (502) staff       (20)    33477 2017-01-16 22:44:44.000000 magic-wormhole-0.9.2/src/wormhole/test/test_scripts.py
+-rw-r--r--   0 warner     (502) staff       (20)    49049 2016-12-30 18:57:39.000000 magic-wormhole-0.9.2/src/wormhole/test/test_server.py
+-rw-r--r--   0 warner     (502) staff       (20)     2721 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/test/test_ssh.py
+-rw-r--r--   0 warner     (502) staff       (20)    15415 2017-01-16 16:37:44.000000 magic-wormhole-0.9.2/src/wormhole/test/test_tor_manager.py
+-rw-r--r--   0 warner     (502) staff       (20)    58807 2017-01-12 22:35:51.000000 magic-wormhole-0.9.2/src/wormhole/test/test_transit.py
+-rw-r--r--   0 warner     (502) staff       (20)    10814 2016-12-30 18:57:39.000000 magic-wormhole-0.9.2/src/wormhole/test/test_transit_server.py
+-rw-r--r--   0 warner     (502) staff       (20)     1693 2016-12-22 21:13:32.000000 magic-wormhole-0.9.2/src/wormhole/test/test_util.py
+-rw-r--r--   0 warner     (502) staff       (20)    36908 2017-01-13 00:34:57.000000 magic-wormhole-0.9.2/src/wormhole/test/test_wormhole.py
+-rw-r--r--   0 warner     (502) staff       (20)     1780 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/test/test_xfer_util.py
+-rw-r--r--   0 warner     (502) staff       (20)     1993 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/timing.py
+-rw-r--r--   0 warner     (502) staff       (20)     7407 2017-01-16 16:37:44.000000 magic-wormhole-0.9.2/src/wormhole/tor_manager.py
+-rw-r--r--   0 warner     (502) staff       (20)    38063 2017-01-16 22:56:00.000000 magic-wormhole-0.9.2/src/wormhole/transit.py
+-rw-r--r--   0 warner     (502) staff       (20)     1291 2016-12-22 21:13:32.000000 magic-wormhole-0.9.2/src/wormhole/util.py
+-rw-r--r--   0 warner     (502) staff       (20)     9220 2016-12-15 15:20:20.000000 magic-wormhole-0.9.2/src/wormhole/wordlist.py
+-rw-r--r--   0 warner     (502) staff       (20)    38624 2017-01-13 00:34:57.000000 magic-wormhole-0.9.2/src/wormhole/wormhole.py
+-rw-r--r--   0 warner     (502) staff       (20)     4248 2017-01-16 16:37:44.000000 magic-wormhole-0.9.2/src/wormhole/xfer_util.py
+-rw-r--r--   0 warner     (502) staff       (20)     1250 2017-01-16 16:37:44.000000 magic-wormhole-0.9.2/tox.ini
+-rw-r--r--   0 warner     (502) staff       (20)    68611 2017-01-12 22:35:51.000000 magic-wormhole-0.9.2/versioneer.py
```

### Comparing `magic-wormhole-0.9.1/.coveragerc` & `magic-wormhole-0.9.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/docs/api.md` & `magic-wormhole-0.9.2/docs/api.md`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/docs/transit.md` & `magic-wormhole-0.9.2/docs/transit.md`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/docs/wormhole-server.8` & `magic-wormhole-0.9.2/docs/wormhole-server.8`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/docs/wormhole.1` & `magic-wormhole-0.9.2/docs/wormhole.1`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/LICENSE` & `magic-wormhole-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/MANIFEST.in` & `magic-wormhole-0.9.2/MANIFEST.in`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 include versioneer.py
 include src/wormhole/_version.py
 include LICENSE README.md NEWS.md
 recursive-include docs *.md *.rst
 include docs/wormhole.1 docs/wormhole-server.8
-include .coveragerc tox.ini
+include .coveragerc tox.ini snapcraft.yaml
 include misc/windows-build.cmd
 include misc/*.py misc/web/*.html misc/web/*.js misc/web/*.css
 include misc/munin/wormhole_active
 include misc/munin/wormhole_errors
 include misc/munin/wormhole_event_rate
 include misc/munin/wormhole_events
 include misc/munin/wormhole_events_alltime
```

### Comparing `magic-wormhole-0.9.1/misc/dump-timing.py` & `magic-wormhole-0.9.2/misc/dump-timing.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/misc/munin/wormhole_active` & `magic-wormhole-0.9.2/misc/munin/wormhole_active`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/misc/munin/wormhole_errors` & `magic-wormhole-0.9.2/misc/munin/wormhole_errors`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/misc/munin/wormhole_event_rate` & `magic-wormhole-0.9.2/misc/munin/wormhole_event_rate`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/misc/munin/wormhole_events` & `magic-wormhole-0.9.2/misc/munin/wormhole_events`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/misc/munin/wormhole_events_alltime` & `magic-wormhole-0.9.2/misc/munin/wormhole_events_alltime`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/misc/munin/wormhole_transit` & `magic-wormhole-0.9.2/misc/munin/wormhole_transit`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/misc/munin/wormhole_transit_alltime` & `magic-wormhole-0.9.2/misc/munin/wormhole_transit_alltime`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/misc/web/timeline.css` & `magic-wormhole-0.9.2/misc/web/timeline.css`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/misc/web/timeline.js` & `magic-wormhole-0.9.2/misc/web/timeline.js`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/misc/windows-build.cmd` & `magic-wormhole-0.9.2/misc/windows-build.cmd`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/NEWS.md` & `magic-wormhole-0.9.2/NEWS.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,51 @@
 
 User-visible changes in "magic-wormhole":
 
+## Release 0.9.2 (16-Jan-2017)
+
+Tor support was rewritten. `wormhole send`, `wormhole receive`,
+`wormhole ssh invite`, and `wormhole ssh accept` all now accept three
+Tor-related arguments:
+
+* `--tor`: use Tor for all connections, and hide all IP addresses
+* `--launch-tor`: launch a new Tor process instead of using an existing
+  one
+* `--tor-control-port=`: use a specific control port, instead of using
+  the default
+
+If Tor is already running on your system (either as an OS-installed
+package, or because the
+[TorBrowser](https://www.torproject.org/projects/torbrowser.html)
+application is running), simply adding `--tor` should be sufficient. If
+Tor is installed but not running, you may need to use both, e.g.
+`wormhole send --tor --launch-tor`. See docs/tor.md for more details.
+Note that Tor support must be requested at install time (with `pip
+install magic-wormhole[tor]`), and only works on python2.7 (not py3).
+(#64, #97)
+
+The relay and transit URLs were changed to point at the project's
+official domain name (magic-wormhole.io). The servers themselves are
+identical (only the domain name changed, not the IP address), so this
+release is fully compatible with previous releases.
+
+A packaging file for "snapcraft.io" is now included. (#131)
+
+`wormhole receive` now reminds you that tab-completion is available, if
+you didn't use the Tab key while entering the code. (#15)
+
+`wormhole receive` should work on cygwin now (a problem with the
+readline-completion library caused a failure on previous releases).
+(#111)
+
+Thanks to Atul Varma, Leo Arias, Daniel Kahn Gillmor, Christopher Wood,
+Kostin Anagnostopoulos, Martin Falatic, and Joey Hess for patches and
+bug reports in this cycle.
+
+
 ## Release 0.9.1 (01-Jan-2017)
 
 The `wormhole` client's `--transit-helper=` argument can now include a
 "relay priority" via a numerical `priority=` field, e.g.
 `--transit-helper tcp:example.org:12345:priority=2.5`. Clients exchange
 transit relay suggestions, then try to use the highest-priority relay
 first, falling back to others after a few seconds if necessary. Direct
```

### Comparing `magic-wormhole-0.9.1/README.md` & `magic-wormhole-0.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -181,10 +181,10 @@
 This library is released under the MIT license, see LICENSE for details.
 
 This library is compatible with python2.7, 3.3, 3.4, 3.5, and 3.6 . It
 is probably compatible with py2.6, but the latest Twisted (>=15.5.0) is
 not.
 
 
-#### footnotes
+<!-- footnotes -->
 
 [1]: http://www.di.ens.fr/~pointche/Documents/Papers/2005_rsa.pdf "RSA 2005"
```

### Comparing `magic-wormhole-0.9.1/src/magic_wormhole.egg-info/SOURCES.txt` & `magic-wormhole-0.9.2/src/magic_wormhole.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 .coveragerc
 LICENSE
 MANIFEST.in
 NEWS.md
 README.md
 setup.cfg
 setup.py
+snapcraft.yaml
 tox.ini
 versioneer.py
 docs/api.md
+docs/attacks.md
+docs/tor.md
 docs/transit.md
 docs/wormhole-server.8
 docs/wormhole.1
 misc/dump-stats.py
 misc/dump-timing.py
 misc/windows-build.cmd
 misc/munin/wormhole_active
@@ -67,12 +70,13 @@
 src/wormhole/test/run_trial.py
 src/wormhole/test/test_args.py
 src/wormhole/test/test_database.py
 src/wormhole/test/test_hkdf.py
 src/wormhole/test/test_scripts.py
 src/wormhole/test/test_server.py
 src/wormhole/test/test_ssh.py
+src/wormhole/test/test_tor_manager.py
 src/wormhole/test/test_transit.py
 src/wormhole/test/test_transit_server.py
 src/wormhole/test/test_util.py
 src/wormhole/test/test_wormhole.py
 src/wormhole/test/test_xfer_util.py
```

### Comparing `magic-wormhole-0.9.1/src/wormhole/cli/cli.py` & `magic-wormhole-0.9.2/src/wormhole/cli/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 start = time.time()
 from textwrap import fill, dedent
 from sys import stdout, stderr
 from . import public_relay
 from .. import __version__
 from ..timing import DebugTiming
 from ..errors import (WrongPasswordError, WelcomeError, KeyFormatError,
-                      TransferError)
+                      TransferError, NoTorError)
 from twisted.internet.defer import inlineCallbacks, maybeDeferred
 from twisted.python.failure import Failure
 from twisted.internet.task import react
 
 import click
 top_import_finish = time.time()
 
@@ -100,15 +100,15 @@
     errors for the user.
     """
     cfg.timing.add("command dispatch")
     cfg.timing.add("import", when=start, which="top").finish(when=top_import_finish)
 
     try:
         yield maybeDeferred(command)
-    except (WrongPasswordError, KeyFormatError) as e:
+    except (WrongPasswordError, KeyFormatError, NoTorError) as e:
         msg = fill("ERROR: " + dedent(e.__doc__))
         print(msg, file=stderr)
         raise SystemExit(1)
     except WelcomeError as e:
         msg = fill("ERROR: " + dedent(e.__doc__))
         print(msg, file=stderr)
         print(file=stderr)
@@ -142,22 +142,32 @@
                  ),
     click.option("--hide-progress", is_flag=True, default=False,
                  help="supress progress-bar display",
                  ),
     click.option("--listen/--no-listen", default=True,
                  help="(debug) don't open a listening socket for Transit",
                  ),
+)
+
+TorArgs = _compose(
     click.option("--tor", is_flag=True, default=False,
                  help="use Tor when connecting",
                  ),
+    click.option("--launch-tor", is_flag=True, default=False,
+                 help="launch Tor, rather than use existing control/socks port",
+                 ),
+    click.option("--tor-control-port", default=None, metavar="ENDPOINT",
+                 help="endpoint descriptor for Tor control port",
+                 ),
 )
 
 # wormhole send (or "wormhole tx")
 @wormhole.command()
 @CommonArgs
+@TorArgs
 @click.option(
     "--code", metavar="CODE",
     help="human-generated code phrase",
 )
 @click.option(
     "--text", default=None, metavar="MESSAGE",
     help="text message to send, instead of a file. Use '-' to read from stdin.",
@@ -179,14 +189,15 @@
     # note: react() does not return
     return react(_dispatch_command, (cfg, lambda: f(cfg)))
 
 
 # wormhole receive (or "wormhole rx")
 @wormhole.command()
 @CommonArgs
+@TorArgs
 @click.option(
     "--only-text", "-t", is_flag=True,
     help="refuse file transfers, only accept text transfers",
 )
 @click.option(
     "--accept-file", is_flag=True,
     help="accept file transfer without asking for confirmation",
@@ -241,19 +252,22 @@
 )
 @click.option(
     "--user", "-u",
     default=None,
     metavar="USER",
     help="Add to USER's ~/.ssh/authorized_keys",
 )
+@TorArgs
 @click.pass_context
-def ssh_invite(ctx, code_length, user):
+def ssh_invite(ctx, code_length, user, **kwargs):
     """
     Add a public-key to a ~/.ssh/authorized_keys file
     """
+    for name, value in kwargs.items():
+        setattr(ctx.obj, name, value)
     from . import cmd_ssh
     ctx.obj.code_length = code_length
     ctx.obj.ssh_user = user
     return go(cmd_ssh.invite, ctx.obj)
 
 
 @ssh.command(name="accept")
@@ -265,23 +279,26 @@
     default=None,
     type=click.Path(exists=True),
 )
 @click.option(
     "--yes", "-y", is_flag=True,
     help="Skip confirmation prompt to send key",
 )
+@TorArgs
 @click.pass_obj
-def ssh_accept(cfg, code, key_file, yes):
+def ssh_accept(cfg, code, key_file, yes, **kwargs):
     """
     Send your SSH public-key
 
     In response to a 'wormhole ssh invite' this will send public-key
     you specify (if there's only one in ~/.ssh/* that will be sent).
     """
 
+    for name, value in kwargs.items():
+        setattr(cfg, name, value)
     from . import cmd_ssh
     kind, keyid, pubkey = cmd_ssh.find_public_key(key_file)
     print("Sending public key type='{}' keyid='{}'".format(kind, keyid))
     if yes is not True:
         click.confirm("Really send public key '{}' ?".format(keyid), abort=True)
     cfg.public_key = (kind, keyid, pubkey)
     cfg.code = code
```

### Comparing `magic-wormhole-0.9.1/src/wormhole/cli/cmd_receive.py` & `magic-wormhole-0.9.2/src/wormhole/cli/cmd_receive.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from tqdm import tqdm
 from humanize import naturalsize
 from twisted.internet import reactor
 from twisted.internet.defer import inlineCallbacks, returnValue
 from twisted.python import log
 from ..wormhole import wormhole
 from ..transit import TransitReceiver
-from ..errors import TransferError, WormholeClosedError
+from ..errors import TransferError, WormholeClosedError, NoTorError
 from ..util import (dict_to_bytes, bytes_to_dict, bytes_to_hexstr,
                     estimate_free_space)
 
 APPID = u"lothar.com/wormhole/text-or-file-xfer"
 VERIFY_TIMER = 1
 
 class RespondError(Exception):
@@ -46,15 +46,19 @@
 
     @inlineCallbacks
     def go(self):
         if self.args.tor:
             with self.args.timing.add("import", which="tor_manager"):
                 from ..tor_manager import TorManager
             self._tor_manager = TorManager(self._reactor,
+                                           self.args.launch_tor,
+                                           self.args.tor_control_port,
                                            timing=self.args.timing)
+            if not self._tor_manager.tor_available():
+                raise NoTorError()
             # For now, block everything until Tor has started. Soon: launch
             # tor in parallel with everything else, make sure the TorManager
             # can lazy-provide an endpoint, and overlap the startup process
             # with the user handing off the wormhole code
             yield self._tor_manager.start()
 
         w = wormhole(self.args.appid or APPID, self.args.relay_url,
```

### Comparing `magic-wormhole-0.9.1/src/wormhole/cli/cmd_send.py` & `magic-wormhole-0.9.2/src/wormhole/cli/cmd_send.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os, sys, six, tempfile, zipfile, hashlib
 from tqdm import tqdm
 from humanize import naturalsize
 from twisted.python import log
 from twisted.protocols import basic
 from twisted.internet import reactor
 from twisted.internet.defer import inlineCallbacks, returnValue
-from ..errors import TransferError, WormholeClosedError
+from ..errors import TransferError, WormholeClosedError, NoTorError
 from ..wormhole import wormhole
 from ..transit import TransitSender
 from ..util import dict_to_bytes, bytes_to_dict, bytes_to_hexstr
 
 APPID = u"lothar.com/wormhole/text-or-file-xfer"
 VERIFY_TIMER = 1
 
@@ -36,15 +36,20 @@
 
     @inlineCallbacks
     def go(self):
         assert isinstance(self._args.relay_url, type(u""))
         if self._args.tor:
             with self._timing.add("import", which="tor_manager"):
                 from ..tor_manager import TorManager
-            self._tor_manager = TorManager(reactor, timing=self._timing)
+            self._tor_manager = TorManager(reactor,
+                                           self._args.launch_tor,
+                                           self._args.tor_control_port,
+                                           timing=self._timing)
+            if not self._tor_manager.tor_available():
+                raise NoTorError()
             # For now, block everything until Tor has started. Soon: launch
             # tor in parallel with everything else, make sure the TorManager
             # can lazy-provide an endpoint, and overlap the startup process
             # with the user handing off the wormhole code
             yield self._tor_manager.start()
 
         w = wormhole(self._args.appid or APPID, self._args.relay_url,
@@ -281,16 +286,18 @@
             hasher.update(data)
             progress.update(len(data))
             return data
         fs = basic.FileSender()
 
         with self._timing.add("tx file"):
             with progress:
-                yield fs.beginFileTransfer(self._fd_to_send, record_pipe,
-                                           transform=_count_and_hash)
+                if filesize:
+                    # don't send zero-length files
+                    yield fs.beginFileTransfer(self._fd_to_send, record_pipe,
+                                               transform=_count_and_hash)
 
         expected_hash = hasher.digest()
         expected_hex = bytes_to_hexstr(expected_hash)
         print(u"File sent.. waiting for confirmation", file=stderr)
         with self._timing.add("get ack") as t:
             ack_bytes = yield record_pipe.receive_record()
             record_pipe.close()
```

### Comparing `magic-wormhole-0.9.1/src/wormhole/cli/cmd_ssh.py` & `magic-wormhole-0.9.2/src/wormhole/cli/cmd_ssh.py`

 * *Files 15% similar despite different names*

```diff
@@ -64,14 +64,16 @@
     yield xfer_util.send(
         reactor,
         cfg.appid or u"lothar.com/wormhole/ssh-add",
         cfg.relay_url,
         data=cfg.public_key[2],
         code=cfg.code,
         use_tor=cfg.tor,
+        launch_tor=cfg.launch_tor,
+        tor_control_port=cfg.tor_control_port,
     )
     print("Key sent.")
 
 
 @inlineCallbacks
 def invite(cfg, reactor=reactor):
 
@@ -104,14 +106,16 @@
 
     pubkey = yield xfer_util.receive(
         reactor,
         cfg.appid or u"lothar.com/wormhole/ssh-add",
         cfg.relay_url,
         None,  # allocate a code for us
         use_tor=cfg.tor,
+        launch_tor=cfg.launch_tor,
+        tor_control_port=cfg.tor_control_port,
         on_code=on_code_created,
     )
 
     parts = pubkey.split()
     kind = parts[0]
     keyid = 'unknown' if len(parts) <= 2 else parts[2]
```

### Comparing `magic-wormhole-0.9.1/src/wormhole/codes.py` & `magic-wormhole-0.9.2/src/wormhole/codes.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,20 +15,22 @@
     return "%s-%s" % (channel_id, "-".join(words))
 
 def extract_channel_id(code):
     channel_id = int(code.split("-")[0])
     return channel_id
 
 class CodeInputter:
-    def __init__(self, initial_channelids, get_channel_ids, code_length):
+    def __init__(self, initial_channelids, get_channel_ids, code_length,
+                 used_completion_f):
         self._initial_channelids = initial_channelids
         self._get_channel_ids = get_channel_ids
         self.code_length = code_length
         self.last_text = None # memoize for a speedup
         self.last_matches = None
+        self._used_completion_f = used_completion_f
 
     def get_current_channel_ids(self):
         if self._initial_channelids is not None:
             channelids = self._initial_channelids
             self._initial_channelids = None
             return channelids
         return self._get_channel_ids()
@@ -39,14 +41,15 @@
         except Exception as e:
             # completer exceptions are normally silently discarded, which
             # makes debugging challenging
             print("completer exception: %s" % e)
             raise e
 
     def completer(self, text, state):
+        self._used_completion_f()
         #if state == 0:
         #    print("", file=sys.stderr)
         #print("completer: '%s' %d '%d'" % (text, state,
         #                                   readline.get_completion_type()),
         #      file=sys.stderr)
         #sys.stderr.flush()
         pieces = text.split("-")
@@ -80,28 +83,32 @@
         #print(" match: '%s'" % match, file=sys.stderr)
         #sys.stderr.flush()
         return match
 
 
 def input_code_with_completion(prompt, initial_channelids, get_channel_ids,
                                code_length):
+    used_completion = []
+    def used_completion_f():
+        used_completion.append(True)
     try:
         import readline
-        c = CodeInputter(initial_channelids, get_channel_ids, code_length)
-        if "libedit" in readline.__doc__:
+        c = CodeInputter(initial_channelids, get_channel_ids, code_length,
+                         used_completion_f)
+        if readline.__doc__ and "libedit" in readline.__doc__:
             readline.parse_and_bind("bind ^I rl_complete")
         else:
             readline.parse_and_bind("tab: complete")
         readline.set_completer(c.wrap_completer)
         readline.set_completer_delims("")
     except ImportError:
         pass
     code = six.moves.input(prompt)
     # Code is str(bytes) on py2, and str(unicode) on py3. We want unicode.
     if isinstance(code, bytes):
         code = code.decode("utf-8")
-    return code
+    return (code, bool(used_completion))
 
 if __name__ == "__main__":
     code = input_code_with_completion("Enter wormhole code: ",
                                       [], lambda: [], 2)
     print("code is:", code)
```

### Comparing `magic-wormhole-0.9.1/src/wormhole/errors.py` & `magic-wormhole-0.9.2/src/wormhole/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,7 +51,10 @@
     """The programmer did something wrong."""
 
 class WormholeClosedError(InternalError):
     """API calls may not be made after close() is called."""
 
 class TransferError(Exception):
     """Something bad happened and the transfer failed."""
+
+class NoTorError(Exception):
+    """--tor was requested, but 'txtorcon' is not installed."""
```

### Comparing `magic-wormhole-0.9.1/src/wormhole/ipaddrs.py` & `magic-wormhole-0.9.2/src/wormhole/ipaddrs.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/server/cli.py` & `magic-wormhole-0.9.2/src/wormhole/server/cli.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/server/cmd_server.py` & `magic-wormhole-0.9.2/src/wormhole/server/cmd_server.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/server/cmd_usage.py` & `magic-wormhole-0.9.2/src/wormhole/server/cmd_usage.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/server/database.py` & `magic-wormhole-0.9.2/src/wormhole/server/database.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/server/db-schemas/upgrade-to-v3.sql` & `magic-wormhole-0.9.2/src/wormhole/server/db-schemas/upgrade-to-v3.sql`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/server/db-schemas/v2.sql` & `magic-wormhole-0.9.2/src/wormhole/server/db-schemas/v2.sql`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/server/db-schemas/v3.sql` & `magic-wormhole-0.9.2/src/wormhole/server/db-schemas/v3.sql`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/server/rendezvous.py` & `magic-wormhole-0.9.2/src/wormhole/server/rendezvous.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/server/rendezvous_websocket.py` & `magic-wormhole-0.9.2/src/wormhole/server/rendezvous_websocket.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/server/runner.py` & `magic-wormhole-0.9.2/src/wormhole/server/runner.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/server/server.py` & `magic-wormhole-0.9.2/src/wormhole/server/server.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/server/transit_server.py` & `magic-wormhole-0.9.2/src/wormhole/server/transit_server.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/test/common.py` & `magic-wormhole-0.9.2/src/wormhole/test/common.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/test/run_trial.py` & `magic-wormhole-0.9.2/src/wormhole/test/run_trial.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/test/test_args.py` & `magic-wormhole-0.9.2/src/wormhole/test/test_args.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/test/test_database.py` & `magic-wormhole-0.9.2/src/wormhole/test/test_database.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/test/test_hkdf.py` & `magic-wormhole-0.9.2/src/wormhole/test/test_hkdf.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/test/test_scripts.py` & `magic-wormhole-0.9.2/src/wormhole/test/test_scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import print_function, unicode_literals
 import os, sys, re, io, zipfile, six, stat
 from humanize import naturalsize
 import mock
 from twisted.trial import unittest
 from twisted.python import procutils, log
+from twisted.internet import defer, endpoints, reactor
 from twisted.internet.utils import getProcessOutputAndValue
 from twisted.internet.defer import gatherResults, inlineCallbacks
 from .. import __version__
 from .common import ServerBase, config
 from ..cli import cmd_send, cmd_receive
 from ..errors import TransferError, WrongPasswordError, WelcomeError
 
@@ -209,27 +210,42 @@
             log.msg("stderr was %s" % err)
             last = err.strip().split("\n")[-1]
             self.fail("wormhole not runnable: %s" % last)
         ver = out.decode("utf-8") or err
         self.failUnlessEqual(ver.strip(), "magic-wormhole {}".format(__version__))
         self.failUnlessEqual(rc, 0)
 
+class FakeTorManager:
+    # use normal endpoints, but record the fact that we were asked
+    def __init__(self):
+        self.endpoints = []
+    def tor_available(self):
+        return True
+    def start(self):
+        return defer.succeed(None)
+    def get_endpoint_for(self, host, port):
+        self.endpoints.append((host, port))
+        return endpoints.HostnameEndpoint(reactor, host, port)
+
 class PregeneratedCode(ServerBase, ScriptsBase, unittest.TestCase):
     # we need Twisted to run the server, but we run the sender and receiver
     # with deferToThread()
 
     def setUp(self):
         d = self.is_runnable()
         d.addCallback(lambda _: ServerBase.setUp(self))
         return d
 
     @inlineCallbacks
     def _do_test(self, as_subprocess=False,
-                 mode="text", addslash=False, override_filename=False):
-        assert mode in ("text", "file", "directory", "slow-text")
+                 mode="text", addslash=False, override_filename=False,
+                 fake_tor=False):
+        assert mode in ("text", "file", "empty-file", "directory", "slow-text")
+        if fake_tor:
+            assert not as_subprocess
         send_cfg = config("send")
         recv_cfg = config("receive")
         message = "blah blah blah ponies"
 
         for cfg in [send_cfg, recv_cfg]:
             cfg.hide_progress = True
             cfg.relay_url = self.relayurl
@@ -240,18 +256,20 @@
             cfg.stderr = io.StringIO()
 
         send_dir = self.mktemp()
         os.mkdir(send_dir)
         receive_dir = self.mktemp()
         os.mkdir(receive_dir)
 
-        if mode == "text" or mode == "slow-text":
+        if mode in ("text", "slow-text"):
             send_cfg.text = message
 
-        elif mode == "file":
+        elif mode in ("file", "empty-file"):
+            if mode == "empty-file":
+                message = ""
             send_filename = "testfile"
             with open(os.path.join(send_dir, send_filename), "w") as f:
                 f.write(message)
             send_cfg.what = send_filename
             receive_filename = send_filename
 
             recv_cfg.accept_file = True
@@ -337,28 +355,59 @@
             receive_stderr = receive_res[1].decode("utf-8")
             receive_rc = receive_res[2]
             NL = os.linesep
             self.assertEqual((send_rc, receive_rc), (0, 0),
                              (send_res, receive_res))
         else:
             send_cfg.cwd = send_dir
-            send_d = cmd_send.send(send_cfg)
-
             recv_cfg.cwd = receive_dir
-            receive_d = cmd_receive.receive(recv_cfg)
+
+            if fake_tor:
+                send_cfg.tor = True
+                send_cfg.transit_helper = self.transit
+                tx_tm = FakeTorManager()
+                with mock.patch("wormhole.tor_manager.TorManager",
+                                return_value=tx_tm,
+                                ) as mtx_tm:
+                    send_d = cmd_send.send(send_cfg)
+
+                recv_cfg.tor = True
+                recv_cfg.transit_helper = self.transit
+                rx_tm = FakeTorManager()
+                with mock.patch("wormhole.tor_manager.TorManager",
+                                return_value=rx_tm,
+                                ) as mrx_tm:
+                    receive_d = cmd_receive.receive(recv_cfg)
+            else:
+                send_d = cmd_send.send(send_cfg)
+                receive_d = cmd_receive.receive(recv_cfg)
 
             # The sender might fail, leaving the receiver hanging, or vice
             # versa. Make sure we don't wait on one side exclusively
             if mode == "slow-text":
                 with mock.patch.object(cmd_send, "VERIFY_TIMER", 0), \
                       mock.patch.object(cmd_receive, "VERIFY_TIMER", 0):
                     yield gatherResults([send_d, receive_d], True)
             else:
                 yield gatherResults([send_d, receive_d], True)
 
+            if fake_tor:
+                expected_endpoints = [("127.0.0.1", self.relayport)]
+                if mode in ("file", "directory"):
+                    expected_endpoints.append(("127.0.0.1", self.transitport))
+                tx_timing = mtx_tm.call_args[1]["timing"]
+                self.assertEqual(tx_tm.endpoints, expected_endpoints)
+                self.assertEqual(mtx_tm.mock_calls,
+                                 [mock.call(reactor, False, None,
+                                            timing=tx_timing)])
+                rx_timing = mrx_tm.call_args[1]["timing"]
+                self.assertEqual(rx_tm.endpoints, expected_endpoints)
+                self.assertEqual(mrx_tm.mock_calls,
+                                 [mock.call(reactor, False, None,
+                                            timing=rx_timing)])
 
             send_stdout = send_cfg.stdout.getvalue()
             send_stderr = send_cfg.stderr.getvalue()
             receive_stdout = recv_cfg.stdout.getvalue()
             receive_stderr = recv_cfg.stderr.getvalue()
 
             # all output here comes from a StringIO, which uses \n for
@@ -443,19 +492,25 @@
         # check server stats
         self._rendezvous.get_stats()
 
     def test_text(self):
         return self._do_test()
     def test_text_subprocess(self):
         return self._do_test(as_subprocess=True)
+    def test_text_tor(self):
+        return self._do_test(fake_tor=True)
 
     def test_file(self):
         return self._do_test(mode="file")
     def test_file_override(self):
         return self._do_test(mode="file", override_filename=True)
+    def test_file_tor(self):
+        return self._do_test(mode="file", fake_tor=True)
+    def test_empty_file(self):
+        return self._do_test(mode="empty-file")
 
     def test_directory(self):
         return self._do_test(mode="directory")
     def test_directory_addslash(self):
         return self._do_test(mode="directory", addslash=True)
     def test_directory_override(self):
         return self._do_test(mode="directory", override_filename=True)
```

### Comparing `magic-wormhole-0.9.1/src/wormhole/test/test_server.py` & `magic-wormhole-0.9.2/src/wormhole/test/test_server.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/test/test_ssh.py` & `magic-wormhole-0.9.2/src/wormhole/test/test_ssh.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/test/test_transit.py` & `magic-wormhole-0.9.2/src/wormhole/test/test_transit.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/test/test_transit_server.py` & `magic-wormhole-0.9.2/src/wormhole/test/test_transit_server.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/test/test_util.py` & `magic-wormhole-0.9.2/src/wormhole/test/test_util.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/test/test_wormhole.py` & `magic-wormhole-0.9.2/src/wormhole/test/test_wormhole.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import print_function, unicode_literals
-import os, json, re, gc
+import os, json, re, gc, io
 from binascii import hexlify, unhexlify
 import mock
 from twisted.trial import unittest
 from twisted.internet import reactor
 from twisted.internet.defer import Deferred, gatherResults, inlineCallbacks
 from .common import ServerBase
 from .. import wormhole
@@ -101,23 +101,26 @@
         self.assertEqual(mood, "unwelcome")
         # alas WelcomeError instances don't compare against each other
         #self.assertEqual(se.mock_calls, [mock.call(WelcomeError("oops"))])
 
 class InputCode(unittest.TestCase):
     def test_list(self):
         send_command = mock.Mock()
+        stderr = io.StringIO()
         ic = wormhole._InputCode(None, "prompt", 2, send_command,
-                                 DebugTiming())
+                                 DebugTiming(), stderr)
         d = ic._list()
         self.assertNoResult(d)
         self.assertEqual(send_command.mock_calls, [mock.call("list")])
         ic._response_handle_nameplates({"type": "nameplates",
                                         "nameplates": [{"id": "123"}]})
         res = self.successResultOf(d)
         self.assertEqual(res, ["123"])
+        self.assertEqual(stderr.getvalue(), "")
+
 
 class GetCode(unittest.TestCase):
     def test_get(self):
         send_command = mock.Mock()
         gc = wormhole._GetCode(2, send_command, DebugTiming())
         d = gc.go()
         self.assertNoResult(d)
@@ -155,28 +158,29 @@
         sp2 = SPAKE2_Symmetric(wormhole.to_bytes(code),
                                idSymmetric=wormhole.to_bytes(APPID))
         msg2 = sp2.start()
         key = sp2.finish(msg1)
         return key, msg2
 
     def test_create(self):
-        wormhole._Wormhole(APPID, "relay_url", reactor, None, None)
+        wormhole._Wormhole(APPID, "relay_url", reactor, None, None, None)
 
     def test_basic(self):
         # We don't call w._start(), so this doesn't create a WebSocket
         # connection. We provide a mock connection instead. If we wanted to
         # exercise _connect, we'd mock out WSFactory.
         # w._connect = lambda self: None
         # w._event_connected(mock_ws)
         # w._event_ws_opened()
         # w._ws_dispatch_response(payload)
 
         timing = DebugTiming()
         with mock.patch("wormhole.wormhole._WelcomeHandler") as wh_c:
-            w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing)
+            w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing,
+                                   None)
         wh = wh_c.return_value
         self.assertEqual(w._ws_url, "relay_url")
         self.assertTrue(w._flag_need_nameplate)
         self.assertTrue(w._flag_need_to_build_msg1)
         self.assertTrue(w._flag_need_to_send_PAKE)
 
         v = w.verify()
@@ -313,15 +317,15 @@
         w._ws_closed(True, None, None)
         self.assertEqual(self.successResultOf(d), None)
 
     def test_close_wait_0(self):
         # Close before the connection is established. The connection still
         # gets established, but it is then torn down before sending anything.
         timing = DebugTiming()
-        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing)
+        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing, None)
         w._drop_connection = mock.Mock()
 
         d = w.close()
         self.assertNoResult(d)
 
         ws = MockWebSocket()
         w._event_connected(ws)
@@ -331,15 +335,15 @@
 
         w._ws_closed(True, None, None)
         self.successResultOf(d)
 
     def test_close_wait_1(self):
         # close before even claiming the nameplate
         timing = DebugTiming()
-        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing)
+        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing, None)
         w._drop_connection = mock.Mock()
         ws = MockWebSocket()
         w._event_connected(ws)
         w._event_ws_opened(None)
 
         d = w.close()
         self.check_outbound(ws, ["bind"])
@@ -350,15 +354,15 @@
         w._ws_closed(True, None, None)
         self.successResultOf(d)
 
     def test_close_wait_2(self):
         # Close after claiming the nameplate, but before opening the mailbox.
         # The 'claimed' response arrives before we close.
         timing = DebugTiming()
-        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing)
+        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing, None)
         w._drop_connection = mock.Mock()
         ws = MockWebSocket()
         w._event_connected(ws)
         w._event_ws_opened(None)
         CODE = "123-foo-bar"
         w.set_code(CODE)
         self.check_outbound(ws, ["bind", "claim"])
@@ -381,15 +385,15 @@
         w._ws_closed(True, None, None)
         self.successResultOf(d)
 
     def test_close_wait_3(self):
         # close after claiming the nameplate, but before opening the mailbox
         # The 'claimed' response arrives after we start to close.
         timing = DebugTiming()
-        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing)
+        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing, None)
         w._drop_connection = mock.Mock()
         ws = MockWebSocket()
         w._event_connected(ws)
         w._event_ws_opened(None)
         CODE = "123-foo-bar"
         w.set_code(CODE)
         self.check_outbound(ws, ["bind", "claim"])
@@ -406,15 +410,15 @@
 
         w._ws_closed(True, None, None)
         self.successResultOf(d)
 
     def test_close_wait_4(self):
         # close after both claiming the nameplate and opening the mailbox
         timing = DebugTiming()
-        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing)
+        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing, None)
         w._drop_connection = mock.Mock()
         ws = MockWebSocket()
         w._event_connected(ws)
         w._event_ws_opened(None)
         CODE = "123-foo-bar"
         w.set_code(CODE)
         response(w, type="claimed", mailbox="mb456")
@@ -436,15 +440,15 @@
         w._ws_closed(True, None, None)
         self.successResultOf(d)
 
     def test_close_wait_5(self):
         # close after claiming the nameplate, opening the mailbox, then
         # releasing the nameplate
         timing = DebugTiming()
-        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing)
+        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing, None)
         w._drop_connection = mock.Mock()
         ws = MockWebSocket()
         w._event_connected(ws)
         w._event_ws_opened(None)
         CODE = "123-foo-bar"
         w.set_code(CODE)
         response(w, type="claimed", mailbox="mb456")
@@ -477,15 +481,15 @@
     def test_close_errbacks(self):
         # make sure the Deferreds returned by verify() and get() are properly
         # errbacked upon close
         pass
 
     def test_get_code_mock(self):
         timing = DebugTiming()
-        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing)
+        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing, None)
         ws = MockWebSocket() # TODO: mock w._ws_send_command instead
         w._event_connected(ws)
         w._event_ws_opened(None)
         self.check_outbound(ws, ["bind"])
 
         gc_c = mock.Mock()
         gc = gc_c.return_value = mock.Mock()
@@ -496,15 +500,15 @@
 
         gc_d.callback("123-foo-bar")
         code = self.successResultOf(d)
         self.assertEqual(code, "123-foo-bar")
 
     def test_get_code_real(self):
         timing = DebugTiming()
-        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing)
+        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing, None)
         ws = MockWebSocket()
         w._event_connected(ws)
         w._event_ws_opened(None)
         self.check_outbound(ws, ["bind"])
 
         d = w.get_code()
 
@@ -520,15 +524,15 @@
         self.assert_(code.startswith("123-"))
         pieces = code.split("-")
         self.assertEqual(len(pieces), 3) # nameplate plus two words
         self.assert_(re.search(r'^\d+-\w+-\w+$', code), code)
 
     def _test_establish_key_hook(self, established, before):
         timing = DebugTiming()
-        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing)
+        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing, None)
 
         if before:
             d = w.establish_key()
 
         if established is True:
             w._key = b"key"
         elif established is False:
@@ -552,30 +556,30 @@
     def test_establish_key_hook(self):
         for established in (True, False, "error"):
             for before in (True, False):
                 self._test_establish_key_hook(established, before)
 
     def test_establish_key_twice(self):
         timing = DebugTiming()
-        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing)
+        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing, None)
         d = w.establish_key()
         self.assertRaises(InternalError, w.establish_key)
         del d
 
     # make sure verify() can be called both before and after the verifier is
     # computed
 
     def _test_verifier(self, when, order, success):
         assert when in ("early", "middle", "late")
         assert order in ("key-then-version", "version-then-key")
         assert isinstance(success, bool)
         #print(when, order, success)
 
         timing = DebugTiming()
-        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing)
+        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing, None)
         w._drop_connection = mock.Mock()
         w._ws_send_command = mock.Mock()
         w._mailbox_state = wormhole.OPEN
         side2 = "side2"
         d = None
 
         if success:
@@ -630,15 +634,15 @@
     def test_welcome_error(self):
         # A welcome message could arrive at any time, with an [error] key
         # that should make us halt. In practice, though, this gets sent as
         # soon as the connection is established, which limits the possible
         # states in which we might see it.
 
         timing = DebugTiming()
-        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing)
+        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing, None)
         w._drop_connection = mock.Mock()
         ws = MockWebSocket()
         w._event_connected(ws)
         w._event_ws_opened(None)
         self.check_outbound(ws, ["bind"])
 
         d1 = w.get()
@@ -663,15 +667,15 @@
         self.failureResultOf(w.verify(), WelcomeError)
 
     def test_version_error(self):
         # we should only receive the "version" message after we receive the
         # PAKE message, by which point we should know the key. If the
         # confirmation message doesn't decrypt, we signal an error.
         timing = DebugTiming()
-        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing)
+        w = wormhole._Wormhole(APPID, "relay_url", reactor, None, timing, None)
         w._drop_connection = mock.Mock()
         ws = MockWebSocket()
         w._event_connected(ws)
         w._event_ws_opened(None)
         w.set_code("123-foo-bar")
         response(w, type="claimed", mailbox="mb456")
```

### Comparing `magic-wormhole-0.9.1/src/wormhole/test/test_xfer_util.py` & `magic-wormhole-0.9.2/src/wormhole/test/test_xfer_util.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/timing.py` & `magic-wormhole-0.9.2/src/wormhole/timing.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/transit.py` & `magic-wormhole-0.9.2/src/wormhole/transit.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                 priority = float(more_pieces[1])
             except ValueError:
                 print("non-float priority= in TCP hint '%s'" % (hint,),
                       file=stderr)
                 return None
     return DirectTCPV1Hint(hint_host, hint_port, priority)
 
-TIMEOUT=15
+TIMEOUT = 60 # seconds
 
 @implementer(interfaces.IProducer, interfaces.IConsumer)
 class Connection(protocol.Protocol, policies.TimeoutMixin):
     def __init__(self, owner, relay_handshake, start, description):
         self.state = "too-early"
         self.buf = b""
         self.owner = owner
@@ -370,15 +370,16 @@
         """Helper method to glue an instance of e.g. t.p.ftp.FileConsumer to
         us. Inbound records will be written as bytes to the consumer.
 
         Set 'expected' to an integer to automatically disconnect when at
         least that number of bytes have been written. This function will then
         return a Deferred (that fires with the number of bytes actually
         received). If the connection is lost while this Deferred is
-        outstanding, it will errback.
+        outstanding, it will errback. If 'expected' is 0, the Deferred will
+        fire right away.
 
         If 'expected' is None, then this function returns None instead of a
         Deferred, and you must call disconnectConsumer() when you are done."""
 
         if self._consumer:
             raise RuntimeError("A consumer is already attached: %r" %
                                self._consumer)
@@ -398,14 +399,17 @@
         self._consumer = consumer
         self._consumer_bytes_written = 0
         self._consumer_bytes_expected = expected
         d = None
         if expected is not None:
             d = defer.Deferred()
         self._consumer_deferred = d
+        if expected == 0:
+            # write empty record to kick consumer into shutdown
+            self._writeToConsumer(b"")
         # drain any pending records
         while self._consumer and self._inbound_records:
             r = self._inbound_records.popleft()
             self._writeToConsumer(r)
         return d
 
     def _writeToConsumer(self, record):
@@ -424,14 +428,15 @@
         self._consumer_deferred = None
 
     # Helper method to write a known number of bytes to a file. This has no
     # flow control: the filehandle cannot push back. 'progress' is an
     # optional callable which will be called on each write (with the number
     # of bytes written). Returns a Deferred that fires (with the number of
     # bytes written) when the count is reached or the RecordPipe is closed.
+
     def writeToFile(self, f, expected, progress=None, hasher=None):
         fc = FileConsumer(f, progress, hasher)
         return self.connectConsumer(fc, expected)
 
 class OutboundConnectionFactory(protocol.ClientFactory):
     protocol = Connection
 
@@ -807,14 +812,16 @@
             # Check the hint type to see if we can support it (e.g. skip
             # onion hints on a non-Tor client). Do not increase relay_delay
             # unless we have at least one viable hint.
             ep = self._endpoint_from_hint_obj(hint_obj)
             if not ep:
                 continue
             description = "->%s" % describe_hint_obj(hint_obj)
+            if self._tor_manager:
+                description = "tor" + description
             d = self._start_connector(ep, description)
             contenders.append(d)
             relay_delay = self.RELAY_DELAY
 
         # Start trying the relays a few seconds after we start to try the
         # direct hints. The idea is to prefer direct connections, but not be
         # afraid of using a relay when we have direct hints that don't
@@ -832,14 +839,16 @@
 
         for priority in sorted(prioritized_relays, reverse=True):
             for hint_obj in prioritized_relays[priority]:
                 ep = self._endpoint_from_hint_obj(hint_obj)
                 if not ep:
                     continue
                 description = "->relay:%s" % describe_hint_obj(hint_obj)
+                if self._tor_manager:
+                    description = "tor" + description
                 d = task.deferLater(self._reactor, relay_delay,
                                     self._start_connector, ep, description,
                                     is_relay=True)
                 contenders.append(d)
             relay_delay += self.RELAY_DELAY
 
         if not contenders:
```

### Comparing `magic-wormhole-0.9.1/src/wormhole/util.py` & `magic-wormhole-0.9.2/src/wormhole/util.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/wordlist.py` & `magic-wormhole-0.9.2/src/wormhole/wordlist.py`

 * *Files identical despite different names*

### Comparing `magic-wormhole-0.9.1/src/wormhole/wormhole.py` & `magic-wormhole-0.9.2/src/wormhole/wormhole.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,20 +85,22 @@
 
     def _response_handle_allocated(self, msg):
         nid = msg["nameplate"]
         assert isinstance(nid, type("")), type(nid)
         self._allocated_d.callback(nid)
 
 class _InputCode:
-    def __init__(self, reactor, prompt, code_length, send_command, timing):
+    def __init__(self, reactor, prompt, code_length, send_command, timing,
+                 stderr):
         self._reactor = reactor
         self._prompt = prompt
         self._code_length = code_length
         self._send_command = send_command
         self._timing = timing
+        self._stderr = stderr
 
     @inlineCallbacks
     def _list(self):
         self._lister_d = defer.Deferred()
         self._send_command("list")
         nameplates = yield self._lister_d
         self._lister_d = None
@@ -117,20 +119,23 @@
         # latency in the user's indecision and slow typing. If we're lucky
         # the answer will come back before they hit TAB.
 
         initial_nameplate_ids = yield self._list()
         with self._timing.add("input code", waiting="user"):
             t = self._reactor.addSystemEventTrigger("before", "shutdown",
                                                     self._warn_readline)
-            code = yield deferToThread(codes.input_code_with_completion,
-                                       self._prompt,
-                                       initial_nameplate_ids,
-                                       self._list_blocking,
-                                       self._code_length)
+            res = yield deferToThread(codes.input_code_with_completion,
+                                      self._prompt,
+                                      initial_nameplate_ids,
+                                      self._list_blocking,
+                                      self._code_length)
+            (code, used_completion) = res
             self._reactor.removeSystemEventTrigger(t)
+            if not used_completion:
+                self._remind_about_tab()
         returnValue(code)
 
     def _response_handle_nameplates(self, msg):
         nameplates = msg["nameplates"]
         assert isinstance(nameplates, list), type(nameplates)
         nids = []
         for n in nameplates:
@@ -170,14 +175,17 @@
         #   us to fetch the current nameplate_id list.
         #
         # Note that hard-terminating our process with os.kill(os.getpid(),
         # signal.SIGKILL), or SIGTERM, doesn't seem to work: the thread
         # doesn't see the signal, and we must still wait for stdin to make
         # readline finish.
 
+    def _remind_about_tab(self):
+        print(" (note: you can use <Tab> to complete words)", file=self._stderr)
+
 class _WelcomeHandler:
     def __init__(self, url, current_version, signal_error):
         self._ws_url = url
         self._version_warning_displayed = False
         self._current_version = current_version
         self._signal_error = signal_error
 
@@ -207,20 +215,21 @@
 # states for nameplates, mailboxes, and the websocket connection
 (CLOSED, OPENING, OPEN, CLOSING) = ("closed", "opening", "open", "closing")
 
 
 class _Wormhole:
     DEBUG = False
 
-    def __init__(self, appid, relay_url, reactor, tor_manager, timing):
+    def __init__(self, appid, relay_url, reactor, tor_manager, timing, stderr):
         self._appid = appid
         self._ws_url = relay_url
         self._reactor = reactor
         self._tor_manager = tor_manager
         self._timing = timing
+        self._stderr = stderr
 
         self._welcomer = _WelcomeHandler(self._ws_url, __version__,
                                          self._signal_error)
         self._side = bytes_to_hexstr(os.urandom(5))
         self._connection_state = CLOSED
         self._connection_waiters = []
         self._ws_t = None
@@ -456,15 +465,15 @@
     def _API_input_code(self, prompt, code_length):
         if self._code is not None: raise InternalError
         if self._started_input_code: raise InternalError
         self._started_input_code = True
         with self._timing.add("API input_code"):
             yield self._when_connected()
             ic = _InputCode(self._reactor, prompt, code_length,
-                            self._ws_send_command, self._timing)
+                            self._ws_send_command, self._timing, self._stderr)
             self._response_handle_nameplates = ic._response_handle_nameplates
             # we reveal the Deferred we're waiting on, so _signal_error can
             # wake us up if something goes wrong (like a welcome error)
             self._input_code_waiter = ic.go()
             code = yield self._input_code_waiter
             self._input_code_waiter = None
         self._event_learned_code(code)
@@ -923,17 +932,18 @@
         # what needs to happen when _ws_closed() happens unexpectedly
         # * errback all API deferreds
         # * maybe: cause new API calls to fail
         # * obviously can't release nameplate or close mailbox
         # * can't re-close websocket
         # * close(wait=True) callers should fire right away
 
-def wormhole(appid, relay_url, reactor, tor_manager=None, timing=None):
+def wormhole(appid, relay_url, reactor, tor_manager=None, timing=None,
+             stderr=sys.stderr):
     timing = timing or DebugTiming()
-    w = _Wormhole(appid, relay_url, reactor, tor_manager, timing)
+    w = _Wormhole(appid, relay_url, reactor, tor_manager, timing, stderr)
     w._start()
     return w
 
 #def wormhole_from_serialized(data, reactor, timing=None):
 #    timing = timing or DebugTiming()
 #    w = _Wormhole.from_serialized(data, reactor, timing)
 #    return w
```

### Comparing `magic-wormhole-0.9.1/src/wormhole/xfer_util.py` & `magic-wormhole-0.9.2/src/wormhole/xfer_util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import json
 from twisted.internet.defer import inlineCallbacks, returnValue
 
 from .wormhole import wormhole
-
+from .tor_manager import TorManager
+from .errors import NoTorError
 
 @inlineCallbacks
-def receive(reactor, appid, relay_url, code, use_tor=None, on_code=None):
+def receive(reactor, appid, relay_url, code,
+            use_tor=False, launch_tor=False, tor_control_port=None,
+            on_code=None):
     """
     This is a convenience API which returns a Deferred that callbacks
     with a single chunk of data from another wormhole (and then closes
     the wormhole). Under the hood, it's just using an instance
     returned from :func:`wormhole.wormhole`. This is similar to the
     `wormhole receive` command.
 
@@ -20,15 +23,26 @@
     :param unicode code: a pre-existing code to use, or None
 
     :param bool use_tor: True if we should use Tor, False to not use it (None for default)
 
     :param on_code: if not None, this is called when we have a code (even if you passed in one explicitly)
     :type on_code: single-argument callable
     """
-    wh = wormhole(appid, relay_url, reactor, use_tor)
+    tm = None
+    if use_tor:
+        tm = TorManager(reactor, launch_tor, tor_control_port)
+        # For now, block everything until Tor has started. Soon: launch
+        # tor in parallel with everything else, make sure the TorManager
+        # can lazy-provide an endpoint, and overlap the startup process
+        # with the user handing off the wormhole code
+        if not tm.tor_available():
+            raise NoTorError()
+        yield tm.start()
+
+    wh = wormhole(appid, relay_url, reactor, tor_manager=tm)
     if code is None:
         code = yield wh.get_code()
     else:
         wh.set_code(code)
     # we'll call this no matter what, even if you passed in a code --
     # maybe it should be only in the 'if' block above?
     if on_code:
@@ -51,15 +65,17 @@
         )
 
     yield wh.close()
     returnValue(msg)
 
 
 @inlineCallbacks
-def send(reactor, appid, relay_url, data, code, use_tor=None, on_code=None):
+def send(reactor, appid, relay_url, data, code,
+         use_tor=False, launch_tor=False, tor_control_port=None,
+         on_code=None):
     """
     This is a convenience API which returns a Deferred that callbacks
     after a single chunk of data has been sent to another
     wormhole. Under the hood, it's just using an instance returned
     from :func:`wormhole.wormhole`. This is similar to the `wormhole
     send` command.
 
@@ -70,15 +86,25 @@
     :param unicode code: a pre-existing code to use, or None
 
     :param bool use_tor: True if we should use Tor, False to not use it (None for default)
 
     :param on_code: if not None, this is called when we have a code (even if you passed in one explicitly)
     :type on_code: single-argument callable
     """
-    wh = wormhole(appid, relay_url, reactor, use_tor)
+    tm = None
+    if use_tor:
+        tm = TorManager(reactor, launch_tor, tor_control_port)
+        # For now, block everything until Tor has started. Soon: launch
+        # tor in parallel with everything else, make sure the TorManager
+        # can lazy-provide an endpoint, and overlap the startup process
+        # with the user handing off the wormhole code
+        if not tm.tor_available():
+            raise NoTorError()
+        yield tm.start()
+    wh = wormhole(appid, relay_url, reactor, tor_manager=tm)
     if code is None:
         code = yield wh.get_code()
     else:
         wh.set_code(code)
     if on_code:
         on_code(code)
```

### Comparing `magic-wormhole-0.9.1/versioneer.py` & `magic-wormhole-0.9.2/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 
-# Version: 0.17
+# Version: 0.18
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
 * https://github.com/warner/python-versioneer
 * Brian Warner
 * License: Public Domain
-* Compatible With: python2.6, 2.7, 3.2, 3.3, 3.4, 3.5, and pypy
+* Compatible With: python2.6, 2.7, 3.2, 3.3, 3.4, 3.5, 3.6, and pypy
 * [![Latest Version]
 (https://pypip.in/version/versioneer/badge.svg?style=flat)
 ](https://pypi.python.org/pypi/versioneer/)
 * [![Build Status]
 (https://travis-ci.org/warner/python-versioneer.png?branch=master)
 ](https://travis-ci.org/warner/python-versioneer)
 
@@ -147,16 +147,16 @@
 TAG[+DISTANCE.gHEX[.dirty]] , using information from `git describe --tags
 --dirty --always`. For example "0.11+2.g1076c97.dirty" indicates that the
 tree is like the "1076c97" commit but has uncommitted changes (".dirty"), and
 that this commit is two revisions ("+2") beyond the "0.11" tag. For released
 software (exactly equal to a known tag), the identifier will only contain the
 stripped tag, e.g. "0.11".
 
-Other styles are available. See details.md in the Versioneer source tree for
-descriptions.
+Other styles are available. See [details.md](details.md) in the Versioneer
+source tree for descriptions.
 
 ## Debugging
 
 Versioneer tries to avoid fatal errors: if something goes wrong, it will tend
 to return a version of "0+unknown". To investigate the problem, run `setup.py
 version`, which will run the version-lookup code in a verbose mode, and will
 display the full contents of `get_versions()` (including the `error` string,
@@ -360,14 +360,15 @@
     cfg.verbose = get(parser, "verbose")
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
+
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY = {}
 HANDLERS = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Decorator to mark a method as the handler for a particular VCS."""
@@ -411,23 +412,25 @@
         stdout = stdout.decode()
     if p.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, p.returncode
     return stdout, p.returncode
+
+
 LONG_VERSION_PY['git'] = '''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain. Generated by
-# versioneer-0.17 (https://github.com/warner/python-versioneer)
+# versioneer-0.18 (https://github.com/warner/python-versioneer)
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
@@ -1172,16 +1175,17 @@
             root = os.path.dirname(root)  # up a level
 
     if verbose:
         print("Tried directories %s but none started with prefix %s" %
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
+
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.17) from
+# This file was generated by 'versioneer.py' (0.18) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1804,14 +1808,15 @@
         print("You should remove lines like 'versioneer.VCS = ' and")
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
         errors = do_setup()
         errors += scan_setup_py()
         if errors:
             sys.exit(1)
```

