# Comparing `tmp/bundlewrap-4.8.2.tar.gz` & `tmp/bundlewrap-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bundlewrap-4.8.2.tar", last modified: Thu May 27 09:20:54 2021, max compression
+gzip compressed data, was "bundlewrap-4.9.0.tar", last modified: Mon Jun 28 10:04:41 2021, max compression
```

## Comparing `bundlewrap-4.8.2.tar` & `bundlewrap-4.9.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-05-27 09:20:54.677183 bundlewrap-4.8.2/
--rw-r--r--   0 trehn     (1000) trehn     (1000)      354 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/AUTHORS
--rw-r--r--   0 trehn     (1000) trehn     (1000)    26650 2021-05-27 09:19:11.000000 bundlewrap-4.8.2/CHANGELOG.md
--rw-r--r--   0 trehn     (1000) trehn     (1000)    35147 2018-07-08 15:30:23.000000 bundlewrap-4.8.2/LICENSE
--rw-r--r--   0 trehn     (1000) trehn     (1000)       47 2018-07-08 15:30:23.000000 bundlewrap-4.8.2/MANIFEST.in
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1439 2021-05-27 09:20:54.677183 bundlewrap-4.8.2/PKG-INFO
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1349 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/README.md
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-05-27 09:20:54.670517 bundlewrap-4.8.2/bundlewrap/
--rw-r--r--   0 trehn     (1000) trehn     (1000)       73 2021-05-27 08:57:00.000000 bundlewrap-4.8.2/bundlewrap/__init__.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     6549 2021-03-24 21:26:22.000000 bundlewrap-4.8.2/bundlewrap/bundle.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-05-27 09:20:54.673850 bundlewrap-4.8.2/bundlewrap/cmdline/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     4865 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/cmdline/__init__.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     4708 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/cmdline/apply.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      824 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/cmdline/debug.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    13411 2021-05-12 15:14:20.000000 bundlewrap-4.8.2/bundlewrap/cmdline/diff.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      953 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/cmdline/groups.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2852 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/cmdline/hash.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     5688 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/cmdline/items.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     7013 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/cmdline/lock.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     6481 2021-05-06 19:05:08.000000 bundlewrap-4.8.2/bundlewrap/cmdline/metadata.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2972 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/cmdline/nodes.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    31748 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/cmdline/parser.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1137 2021-03-24 21:26:22.000000 bundlewrap-4.8.2/bundlewrap/cmdline/plot.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      172 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/cmdline/repo.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     5262 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/cmdline/run.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1396 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/cmdline/stats.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    12152 2021-05-12 12:26:37.000000 bundlewrap-4.8.2/bundlewrap/cmdline/test.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     4452 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/cmdline/verify.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1269 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/cmdline/zen.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     6315 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/concurrency.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    21229 2021-05-12 14:51:28.000000 bundlewrap-4.8.2/bundlewrap/deps.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2437 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/exceptions.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    10682 2021-05-01 15:52:32.000000 bundlewrap-4.8.2/bundlewrap/group.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3752 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/itemqueue.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-05-27 09:20:54.677183 bundlewrap-4.8.2/bundlewrap/items/
--rw-r--r--   0 trehn     (1000) trehn     (1000)    31069 2021-05-12 22:20:17.000000 bundlewrap-4.8.2/bundlewrap/items/__init__.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     9791 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/items/actions.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    10417 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/items/directories.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    18827 2021-05-12 14:19:32.000000 bundlewrap-4.8.2/bundlewrap/items/files.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    11361 2021-05-27 08:56:31.000000 bundlewrap-4.8.2/bundlewrap/items/git_deploy.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3797 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/items/groups.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    15489 2021-05-12 12:23:29.000000 bundlewrap-4.8.2/bundlewrap/items/kubernetes.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2308 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/items/pkg.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      865 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/items/pkg_apk.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2381 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/items/pkg_apt.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      988 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/items/pkg_dnf.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2769 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/items/pkg_freebsd.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     4357 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/items/pkg_openbsd.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      881 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/items/pkg_opkg.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1620 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/items/pkg_pacman.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3892 2021-05-27 09:10:40.000000 bundlewrap-4.8.2/bundlewrap/items/pkg_pip.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      825 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/items/pkg_snap.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)      988 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/items/pkg_yum.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1979 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/items/pkg_zypper.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3323 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/items/postgres_dbs.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3918 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/items/postgres_roles.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     4915 2021-05-01 15:52:32.000000 bundlewrap-4.8.2/bundlewrap/items/routeros.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3381 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/items/svc_openbsd.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3360 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/items/svc_openrc.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     4488 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/items/svc_systemd.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2447 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/items/svc_systemv.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2965 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/items/svc_upstart.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     6528 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/items/symlinks.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    12778 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/items/users.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     9245 2021-03-24 21:26:22.000000 bundlewrap-4.8.2/bundlewrap/lock.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    12322 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/metadata.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    18756 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/metagen.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    35888 2021-05-12 22:12:04.000000 bundlewrap-4.8.2/bundlewrap/node.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    10284 2021-05-06 19:06:14.000000 bundlewrap-4.8.2/bundlewrap/operations.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    17708 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/repo.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    11747 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/secrets.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-05-27 09:20:54.677183 bundlewrap-4.8.2/bundlewrap/utils/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     9009 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/utils/__init__.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3076 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/utils/cmdline.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    14961 2021-05-19 16:46:59.000000 bundlewrap-4.8.2/bundlewrap/utils/dicts.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3823 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/utils/metastack.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     8394 2021-03-25 12:56:36.000000 bundlewrap-4.8.2/bundlewrap/utils/plot.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     3331 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/utils/remote.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1813 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/utils/scm.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     6493 2020-10-21 12:43:05.000000 bundlewrap-4.8.2/bundlewrap/utils/table.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2034 2021-03-24 21:26:22.000000 bundlewrap-4.8.2/bundlewrap/utils/testing.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)     6703 2021-05-12 10:51:55.000000 bundlewrap-4.8.2/bundlewrap/utils/text.py
--rw-r--r--   0 trehn     (1000) trehn     (1000)    14061 2021-05-18 08:15:44.000000 bundlewrap-4.8.2/bundlewrap/utils/ui.py
-drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-05-27 09:20:54.670517 bundlewrap-4.8.2/bundlewrap.egg-info/
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1439 2021-05-27 09:20:54.000000 bundlewrap-4.8.2/bundlewrap.egg-info/PKG-INFO
--rw-r--r--   0 trehn     (1000) trehn     (1000)     2272 2021-05-27 09:20:54.000000 bundlewrap-4.8.2/bundlewrap.egg-info/SOURCES.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)        1 2021-05-27 09:20:54.000000 bundlewrap-4.8.2/bundlewrap.egg-info/dependency_links.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)       48 2021-05-27 09:20:54.000000 bundlewrap-4.8.2/bundlewrap.egg-info/entry_points.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)        1 2018-06-27 18:37:37.000000 bundlewrap-4.8.2/bundlewrap.egg-info/not-zip-safe
--rw-r--r--   0 trehn     (1000) trehn     (1000)       73 2021-05-27 09:20:54.000000 bundlewrap-4.8.2/bundlewrap.egg-info/requires.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)       11 2021-05-27 09:20:54.000000 bundlewrap-4.8.2/bundlewrap.egg-info/top_level.txt
--rw-r--r--   0 trehn     (1000) trehn     (1000)      173 2021-05-27 09:20:54.677183 bundlewrap-4.8.2/setup.cfg
--rw-r--r--   0 trehn     (1000) trehn     (1000)     1902 2021-05-27 08:56:50.000000 bundlewrap-4.8.2/setup.py
+drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-06-28 10:04:41.159026 bundlewrap-4.9.0/
+-rw-r--r--   0 trehn     (1000) trehn     (1000)      354 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/AUTHORS
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    26907 2021-06-28 10:03:08.000000 bundlewrap-4.9.0/CHANGELOG.md
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    35147 2018-07-08 15:30:23.000000 bundlewrap-4.9.0/LICENSE
+-rw-r--r--   0 trehn     (1000) trehn     (1000)       47 2018-07-08 15:30:23.000000 bundlewrap-4.9.0/MANIFEST.in
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     1464 2021-06-28 10:04:41.159026 bundlewrap-4.9.0/PKG-INFO
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     1349 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/README.md
+drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-06-28 10:04:41.155693 bundlewrap-4.9.0/bundlewrap/
+-rw-r--r--   0 trehn     (1000) trehn     (1000)       73 2021-06-28 10:03:27.000000 bundlewrap-4.9.0/bundlewrap/__init__.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     6549 2021-03-24 21:26:22.000000 bundlewrap-4.9.0/bundlewrap/bundle.py
+drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-06-28 10:04:41.155693 bundlewrap-4.9.0/bundlewrap/cmdline/
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     4865 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/cmdline/__init__.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     4708 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/cmdline/apply.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)      824 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/cmdline/debug.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    13411 2021-05-12 15:14:20.000000 bundlewrap-4.9.0/bundlewrap/cmdline/diff.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)      953 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/cmdline/groups.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     2852 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/cmdline/hash.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     5688 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/cmdline/items.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     7013 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/cmdline/lock.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     6481 2021-05-06 19:05:08.000000 bundlewrap-4.9.0/bundlewrap/cmdline/metadata.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     2972 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/cmdline/nodes.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    31748 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/cmdline/parser.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     1137 2021-03-24 21:26:22.000000 bundlewrap-4.9.0/bundlewrap/cmdline/plot.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)      172 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/cmdline/repo.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     5262 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/cmdline/run.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     1396 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/cmdline/stats.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    12152 2021-05-12 12:26:37.000000 bundlewrap-4.9.0/bundlewrap/cmdline/test.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     4452 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/cmdline/verify.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     1269 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/cmdline/zen.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     6315 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/concurrency.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    21252 2021-05-31 16:59:30.000000 bundlewrap-4.9.0/bundlewrap/deps.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     2437 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/exceptions.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    10690 2021-05-31 16:59:30.000000 bundlewrap-4.9.0/bundlewrap/group.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     3752 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/itemqueue.py
+drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-06-28 10:04:41.159026 bundlewrap-4.9.0/bundlewrap/items/
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    31069 2021-05-31 16:59:30.000000 bundlewrap-4.9.0/bundlewrap/items/__init__.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     9791 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/items/actions.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    10417 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/items/directories.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    18827 2021-05-12 14:19:32.000000 bundlewrap-4.9.0/bundlewrap/items/files.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    11642 2021-06-28 09:57:34.000000 bundlewrap-4.9.0/bundlewrap/items/git_deploy.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     4081 2021-06-28 09:48:32.000000 bundlewrap-4.9.0/bundlewrap/items/groups.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    15489 2021-05-12 12:23:29.000000 bundlewrap-4.9.0/bundlewrap/items/kubernetes.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     2308 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/items/pkg.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)      865 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/items/pkg_apk.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     2381 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/items/pkg_apt.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)      988 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/items/pkg_dnf.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     2769 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/items/pkg_freebsd.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     4357 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/items/pkg_openbsd.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)      881 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/items/pkg_opkg.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     1620 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/items/pkg_pacman.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     3892 2021-05-27 09:10:40.000000 bundlewrap-4.9.0/bundlewrap/items/pkg_pip.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)      825 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/items/pkg_snap.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)      988 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/items/pkg_yum.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     1979 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/items/pkg_zypper.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     3253 2021-05-31 16:59:30.000000 bundlewrap-4.9.0/bundlewrap/items/postgres_dbs.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     3845 2021-05-31 16:59:30.000000 bundlewrap-4.9.0/bundlewrap/items/postgres_roles.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     4915 2021-05-01 15:52:32.000000 bundlewrap-4.9.0/bundlewrap/items/routeros.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     3381 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/items/svc_openbsd.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     3360 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/items/svc_openrc.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     4488 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/items/svc_systemd.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     2447 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/items/svc_systemv.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     2965 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/items/svc_upstart.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     6528 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/items/symlinks.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    13060 2021-06-28 09:48:32.000000 bundlewrap-4.9.0/bundlewrap/items/users.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     9245 2021-03-24 21:26:22.000000 bundlewrap-4.9.0/bundlewrap/lock.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    12322 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/metadata.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    18756 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/metagen.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    35921 2021-05-31 16:59:30.000000 bundlewrap-4.9.0/bundlewrap/node.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    10377 2021-05-31 16:59:30.000000 bundlewrap-4.9.0/bundlewrap/operations.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    17708 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/repo.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    12397 2021-05-31 16:59:30.000000 bundlewrap-4.9.0/bundlewrap/secrets.py
+drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-06-28 10:04:41.159026 bundlewrap-4.9.0/bundlewrap/utils/
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     9009 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/utils/__init__.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     3076 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/utils/cmdline.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    14961 2021-05-19 16:46:59.000000 bundlewrap-4.9.0/bundlewrap/utils/dicts.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     3823 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/utils/metastack.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     8394 2021-03-25 12:56:36.000000 bundlewrap-4.9.0/bundlewrap/utils/plot.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     3331 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/utils/remote.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     1813 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/utils/scm.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     6493 2020-10-21 12:43:05.000000 bundlewrap-4.9.0/bundlewrap/utils/table.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     2034 2021-03-24 21:26:22.000000 bundlewrap-4.9.0/bundlewrap/utils/testing.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     6703 2021-05-12 10:51:55.000000 bundlewrap-4.9.0/bundlewrap/utils/text.py
+-rw-r--r--   0 trehn     (1000) trehn     (1000)    14061 2021-05-18 08:15:44.000000 bundlewrap-4.9.0/bundlewrap/utils/ui.py
+drwxr-xr-x   0 trehn     (1000) trehn     (1000)        0 2021-06-28 10:04:41.155693 bundlewrap-4.9.0/bundlewrap.egg-info/
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     1464 2021-06-28 10:04:41.000000 bundlewrap-4.9.0/bundlewrap.egg-info/PKG-INFO
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     2272 2021-06-28 10:04:41.000000 bundlewrap-4.9.0/bundlewrap.egg-info/SOURCES.txt
+-rw-r--r--   0 trehn     (1000) trehn     (1000)        1 2021-06-28 10:04:41.000000 bundlewrap-4.9.0/bundlewrap.egg-info/dependency_links.txt
+-rw-r--r--   0 trehn     (1000) trehn     (1000)       48 2021-06-28 10:04:41.000000 bundlewrap-4.9.0/bundlewrap.egg-info/entry_points.txt
+-rw-r--r--   0 trehn     (1000) trehn     (1000)        1 2018-06-27 18:37:37.000000 bundlewrap-4.9.0/bundlewrap.egg-info/not-zip-safe
+-rw-r--r--   0 trehn     (1000) trehn     (1000)       73 2021-06-28 10:04:41.000000 bundlewrap-4.9.0/bundlewrap.egg-info/requires.txt
+-rw-r--r--   0 trehn     (1000) trehn     (1000)       11 2021-06-28 10:04:41.000000 bundlewrap-4.9.0/bundlewrap.egg-info/top_level.txt
+-rw-r--r--   0 trehn     (1000) trehn     (1000)      173 2021-06-28 10:04:41.159026 bundlewrap-4.9.0/setup.cfg
+-rw-r--r--   0 trehn     (1000) trehn     (1000)     1902 2021-06-28 10:03:33.000000 bundlewrap-4.9.0/setup.py
```

### Comparing `bundlewrap-4.8.2/CHANGELOG.md` & `bundlewrap-4.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+# 4.9.0
+
+2021-06-28
+
+* added `repo.vault.cmd()`
+* postgres items can now be used with `doas` instead of `sudo`
+* improved error reporting of `git_deploy`
+* fixed dependencies being skipped when using `bw apply -o`
+* fixed user and group management on BSD
+
+
 # 4.8.2
 
 2021-05-27
 
 * fixed clobbered env vars for `git_deploy`
 * fixed `pkg_pip` failing with underscores in package names
```

### Comparing `bundlewrap-4.8.2/LICENSE` & `bundlewrap-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/PKG-INFO` & `bundlewrap-4.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: bundlewrap
-Version: 4.8.2
+Version: 4.9.0
 Summary: Config management with Python
 Home-page: http://bundlewrap.org
 Author: Torsten Rehn
 Author-email: torsten@rehn.email
 License: GPLv3
-Description: By allowing for easy and low-overhead config management, BundleWrap fills the gap between complex deployments using Chef or Puppet and old school system administration over SSH.
-        While most other config management systems rely on a client-server architecture, BundleWrap works off a repository cloned to your local machine. It then automates the process of SSHing into your servers and making sure everything is configured the way it's supposed to be. You won't have to install anything on managed servers.
 Keywords: configuration,config,management
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -19,7 +17,13 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
+License-File: LICENSE
+License-File: AUTHORS
+
+By allowing for easy and low-overhead config management, BundleWrap fills the gap between complex deployments using Chef or Puppet and old school system administration over SSH.
+While most other config management systems rely on a client-server architecture, BundleWrap works off a repository cloned to your local machine. It then automates the process of SSHing into your servers and making sure everything is configured the way it's supposed to be. You won't have to install anything on managed servers.
+
```

### Comparing `bundlewrap-4.8.2/README.md` & `bundlewrap-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/bundle.py` & `bundlewrap-4.9.0/bundlewrap/bundle.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/__init__.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/__init__.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/apply.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/apply.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/debug.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/debug.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/diff.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/diff.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/groups.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/groups.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/hash.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/hash.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/items.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/items.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/lock.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/lock.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/metadata.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/metadata.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/nodes.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/nodes.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/parser.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/parser.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/plot.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/plot.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/run.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/run.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/stats.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/stats.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/test.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/test.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/verify.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/verify.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/cmdline/zen.py` & `bundlewrap-4.9.0/bundlewrap/cmdline/zen.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/concurrency.py` & `bundlewrap-4.9.0/bundlewrap/concurrency.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/deps.py` & `bundlewrap-4.9.0/bundlewrap/deps.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     """
     Recursively retrieves and returns a list of all inherited
     dependencies of the given item.
 
     This can handle loops, but will ignore them.
     """
     item._flattened_deps = {item.id for item in item._deps}
-    item._flattened_deps_needs = {item.id for item in item._deps_needs}
+    item._flattened_deps_needs = {item.id for item in item._deps_needs | item._deps_needed_by}
 
     for dep_item in item._deps:
         # Don't recurse if we have already resolved nested
         # dependencies for this item. Also serves as a guard
         # against infinite recursion when there are loops.
         if not hasattr(dep_item, '_flattened_deps'):
             _flatten_deps_for_item(dep_item, items)
```

### Comparing `bundlewrap-4.8.2/bundlewrap/exceptions.py` & `bundlewrap-4.9.0/bundlewrap/exceptions.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/group.py` & `bundlewrap-4.9.0/bundlewrap/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     TUPLE_OF_INTS,
 )
 from .utils.text import mark_for_translation as _, toml_clean, validate_name
 
 
 GROUP_ATTR_DEFAULTS = {
     'cmd_wrapper_inner': "export LANG=C; {}",
-    'cmd_wrapper_outer': "sudo sh -c {}",
+    'cmd_wrapper_outer': "sudo -u {1} sh -c {0}",
     'lock_dir': "/var/lib/bundlewrap",
     'dummy': False,
     'kubectl_context': None,
     'locking_node': None,
     'os': 'linux',
     # Setting os_version to 0 by default will probably yield less
     # surprises than setting it to max_int. Users will probably
```

### Comparing `bundlewrap-4.8.2/bundlewrap/itemqueue.py` & `bundlewrap-4.9.0/bundlewrap/itemqueue.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/__init__.py` & `bundlewrap-4.9.0/bundlewrap/items/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,15 +680,15 @@
         for tag in self.tags:
             if "tag:{}".format(tag) in components:
                 return True
         return False
 
     def covered_by_autoonly_selector(self, autoonly_selector, check_deps=True):
         """
-        True if this item should be NOT skipped based on the given selector
+        True if this item should NOT be skipped based on the given selector
         (e.g. ("tag:foo", "bundle:bar")).
         """
         if not autoonly_selector:
             return True
         components = [c.strip() for c in autoonly_selector]
         if (
             self.id in components or
```

### Comparing `bundlewrap-4.8.2/bundlewrap/items/actions.py` & `bundlewrap-4.9.0/bundlewrap/items/actions.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/directories.py` & `bundlewrap-4.9.0/bundlewrap/items/directories.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/files.py` & `bundlewrap-4.9.0/bundlewrap/items/files.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/git_deploy.py` & `bundlewrap-4.9.0/bundlewrap/items/git_deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,17 +226,24 @@
         result.return_code = git_process.returncode
         self._command_results.append({
             'command': " ".join(cmdline),
             'result': result,
         })
 
         if result.return_code != 0:
-            raise RuntimeError(_("`git {command}` failed in {dir}").format(
+            raise RuntimeError(_(
+                "`git {command}` failed in {dir} for {item} from bundle {bundle}:\n"
+                "{stdout}\n{stderr}"
+            ).format(
                 command=" ".join(cmdline[1:]),
                 dir=repo_dir,
+                item=self.id,
+                bundle=self.bundle.name,
+                stdout=result.stdout.decode('utf-8'),
+                stderr=result.stderr.decode('utf-8'),
             ))
         return stdout.decode('utf-8').strip()
 
     def clone_to_dir(self, remote_url, rev):
         """
         Clones the given URL to a temporary directory, using a shallow clone
         if the given revision is definitely not a commit hash. Clones to
```

### Comparing `bundlewrap-4.8.2/bundlewrap/items/groups.py` & `bundlewrap-4.9.0/bundlewrap/items/groups.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,18 +55,25 @@
         else:
             command = ""
 
         if status.must_be_deleted:
             command += f"groupdel {self.name}"
         else:
             command += "groupadd " if status.must_be_created else "groupmod "
-            command += f"{self.name} "
 
             if self.attributes['gid'] is not None:
-                command += "-g {}".format(self.attributes['gid'])
+                command += "-g {} ".format(self.attributes['gid'])
+
+            if self.node.os == 'freebsd':
+                # FreeBSD expects <name> to be the first argument to
+                # `pw groupadd/mod`, however we can also pass it using -n
+                # instead. Then it is positionally independent.
+                command += "-n "
+
+            command += f"{self.name}"
         self.run(command, may_fail=True)
 
     def sdict(self):
         # verify content of /etc/group
         grep_result = self.run(
             "grep -e '^{}:' /etc/group".format(self.name),
             may_fail=True,
```

### Comparing `bundlewrap-4.8.2/bundlewrap/items/kubernetes.py` & `bundlewrap-4.9.0/bundlewrap/items/kubernetes.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/pkg.py` & `bundlewrap-4.9.0/bundlewrap/items/pkg.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/pkg_apk.py` & `bundlewrap-4.9.0/bundlewrap/items/pkg_apk.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/pkg_apt.py` & `bundlewrap-4.9.0/bundlewrap/items/pkg_apt.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/pkg_dnf.py` & `bundlewrap-4.9.0/bundlewrap/items/pkg_dnf.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/pkg_freebsd.py` & `bundlewrap-4.9.0/bundlewrap/items/pkg_freebsd.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/pkg_openbsd.py` & `bundlewrap-4.9.0/bundlewrap/items/pkg_openbsd.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/pkg_opkg.py` & `bundlewrap-4.9.0/bundlewrap/items/pkg_opkg.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/pkg_pacman.py` & `bundlewrap-4.9.0/bundlewrap/items/pkg_pacman.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/pkg_pip.py` & `bundlewrap-4.9.0/bundlewrap/items/pkg_pip.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/pkg_snap.py` & `bundlewrap-4.9.0/bundlewrap/items/pkg_snap.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/pkg_yum.py` & `bundlewrap-4.9.0/bundlewrap/items/pkg_yum.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/pkg_zypper.py` & `bundlewrap-4.9.0/bundlewrap/items/pkg_zypper.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/postgres_dbs.py` & `bundlewrap-4.9.0/bundlewrap/items/postgres_dbs.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from bundlewrap.exceptions import BundleError
 from bundlewrap.items import Item
 from bundlewrap.utils.text import force_text, mark_for_translation as _
 
 
 def create_db(node, name, owner, when_creating):
     template = None
-    cmd = "sudo -u postgres createdb -wO {} ".format(owner)
+    cmd = "createdb -wO {} ".format(owner)
 
     if when_creating.get('collation') is not None:
         cmd += "--lc-collate={} ".format(when_creating['collation'])
         template = "template0"
 
     if when_creating.get('ctype') is not None:
         cmd += "--lc-ctype={} ".format(when_creating['ctype'])
@@ -22,40 +22,35 @@
         template = "template0"
 
     if template is not None:
         cmd += "--template={} ".format(template)
 
     cmd += name
 
-    return node.run(cmd)
+    return node.run(cmd, user="postgres")
 
 
 def drop_db(node, name):
-    return node.run("sudo -u postgres dropdb -w {}".format(quote(name)))
+    return node.run("dropdb -w {}".format(quote(name)), user="postgres")
 
 
 def get_databases(node):
-    output = node.run("echo '\\l' | sudo -u postgres psql -Anqt -F '|' | grep '|'").stdout
+    output = node.run("psql -Anqt -F '|' -c '\\l' | grep '|'", user="postgres").stdout
     result = {}
     for line in force_text(output).strip().split("\n"):
         db, owner = line.strip().split("|", 2)[:2]
         result[db] = {
             'owner': owner,
         }
     return result
 
 
 def set_owner(node, name, owner):
-    return node.run(
-        "echo 'ALTER DATABASE \"{name}\" OWNER TO \"{owner}\"' | "
-        "sudo -u postgres psql -nqw".format(
-            name=name,
-            owner=owner,
-        ),
-    )
+    sql = f"ALTER DATABASE \\\"{name}\\\" OWNER TO \\\"{owner}\\\""
+    return node.run(f"psql -nqw -c \"{sql}\"", user="postgres")
 
 
 class PostgresDB(Item):
     """
     A postgres database.
     """
     BUNDLE_ATTRIBUTE_NAME = "postgres_dbs"
```

### Comparing `bundlewrap-4.8.2/bundlewrap/items/postgres_roles.py` & `bundlewrap-4.9.0/bundlewrap/items/postgres_roles.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,34 +9,31 @@
     "rolcanlogin": 'can_login',
     "rolsuper": 'superuser',
     "rolpassword": 'password_hash',
 }
 
 
 def delete_role(node, role):
-    node.run("sudo -u postgres dropuser -w {}".format(role))
+    node.run("dropuser -w {}".format(role), user="postgres")
 
 
 def fix_role(node, role, attrs, create=False):
     password = " PASSWORD '{}'".format(attrs['password_hash'])
-    node.run(
-        "echo \"{operation} ROLE \\\"{role}\\\" WITH LOGIN {superuser}SUPERUSER{password}\" "
-        "| sudo -u postgres psql -nqw".format(
-            operation="CREATE" if create else "ALTER",
-            password="" if attrs['password_hash'] is None else password,
-            role=role,
-            superuser="" if attrs['superuser'] is True else "NO",
-        )
+    sql = "{operation} ROLE \\\"{role}\\\" WITH LOGIN {superuser}SUPERUSER{password}".format(
+        operation="CREATE" if create else "ALTER",
+        password="" if attrs['password_hash'] is None else password,
+        role=role,
+        superuser="" if attrs['superuser'] is True else "NO",
     )
+    node.run(f"psql -nqw -c \"{sql}\"", user="postgres")
 
 
 def get_role(node, role):
-    result = node.run("echo \"SELECT rolcanlogin, rolsuper, rolpassword from pg_authid "
-                      "WHERE rolname='{}'\" "
-                      "| sudo -u postgres psql -Anqwx -F '|'".format(role))
+    sql = f"SELECT rolcanlogin, rolsuper, rolpassword from pg_authid WHERE rolname='{role}'"
+    result = node.run(f"psql -Anqwx -F '|' -c \"{sql}\"", user="postgres")
 
     role_attrs = {}
     for line in force_text(result.stdout).strip().split("\n"):
         try:
             key, value = line.split("|")
         except ValueError:
             pass
```

### Comparing `bundlewrap-4.8.2/bundlewrap/items/routeros.py` & `bundlewrap-4.9.0/bundlewrap/items/routeros.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/svc_openbsd.py` & `bundlewrap-4.9.0/bundlewrap/items/svc_openbsd.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/svc_openrc.py` & `bundlewrap-4.9.0/bundlewrap/items/svc_openrc.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/svc_systemd.py` & `bundlewrap-4.9.0/bundlewrap/items/svc_systemd.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/svc_systemv.py` & `bundlewrap-4.9.0/bundlewrap/items/svc_systemv.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/svc_upstart.py` & `bundlewrap-4.9.0/bundlewrap/items/svc_upstart.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/symlinks.py` & `bundlewrap-4.9.0/bundlewrap/items/symlinks.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/items/users.py` & `bundlewrap-4.9.0/bundlewrap/items/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,14 @@
             command = ""
 
         if status.must_be_deleted:
             command += "userdel {}"
             self.run(command.format(self.name), may_fail=True)
         else:
             command += "useradd " if status.must_be_created else "usermod "
-            command += f"{self.name} "
 
             stdin = None
             for attr, option in sorted(_ATTRIBUTE_OPTIONS.items()):
                 if (attr in status.keys_to_fix or status.must_be_created) and \
                         self.attributes[attr] is not None:
                     if attr == 'groups':
                         value = ",".join(self.attributes[attr])
@@ -157,14 +156,22 @@
                         # Using -H <n> we pass the password hash using file descriptor <n> instead.
                         option = '-H'
                         value = '0'  # FD 0 = stdin
                         stdin = self.attributes[attr].encode()
                     else:
                         value = str(self.attributes[attr])
                     command += "{} {} ".format(option, quote(value))
+
+            if self.node.os == 'freebsd':
+                # FreeBSD expects <name> to be the first argument to
+                # `pw useradd/mod`, however we can also pass it using -n
+                # instead. Then it is positionally independent.
+                command += "-n "
+
+            command += f"{self.name}"
             self.run(command, data_stdin=stdin, may_fail=True)
 
     def display_on_create(self, cdict):
         for attr_name, attr_display_name in _ATTRIBUTE_NAMES.items():
             if attr_name == attr_display_name:
                 # Don't change anything; the `del` below would
                 # always remove the key entirely!
```

### Comparing `bundlewrap-4.8.2/bundlewrap/lock.py` & `bundlewrap-4.9.0/bundlewrap/lock.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/metadata.py` & `bundlewrap-4.9.0/bundlewrap/metadata.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/metagen.py` & `bundlewrap-4.9.0/bundlewrap/metagen.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/node.py` & `bundlewrap-4.9.0/bundlewrap/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -797,15 +797,15 @@
     @property
     def partial_metadata(self):
         """
         Deprecated, remove in 5.0.0
         """
         return self.metadata
 
-    def run(self, command, data_stdin=None, may_fail=False, log_output=False):
+    def run(self, command, data_stdin=None, may_fail=False, log_output=False, user="root"):
         assert self.os in self.OS_FAMILY_UNIX
 
         if log_output:
             def log_function(msg):
                 io.stdout("{x} {node}  {msg}".format(
                     node=bold(self.name),
                     msg=force_text(msg).rstrip("\n"),
@@ -840,14 +840,15 @@
             add_host_keys=self._add_host_keys,
             data_stdin=data_stdin,
             ignore_failure=may_fail,
             log_function=log_function,
             username=self.username,
             wrapper_inner=self.cmd_wrapper_inner,
             wrapper_outer=self.cmd_wrapper_outer,
+            user=user,
         )
 
     @cached_property
     def toml(self):
         if not self.file_path or not self.file_path.endswith(".toml"):
             raise ValueError(_("node {} not in TOML format").format(self.name))
         return toml_parse(get_file_contents(self.file_path))
@@ -886,29 +887,29 @@
             wrapper_outer=self.cmd_wrapper_outer,
         )
 
     def verify(
         self,
         autoskip_selector=(),
         autoonly_selector=(),
-        show_all=False, 
-        show_diff=True, 
+        show_all=False,
+        show_diff=True,
         workers=4,
     ):
         result = []
         start = datetime.now()
 
         if not self.items:
             io.stdout(_("{x} {node}  has no items").format(node=bold(self.name), x=yellow("!")))
         else:
             result = verify_items(
                 self,
                 autoskip_selector=autoskip_selector,
                 autoonly_selector=autoonly_selector,
-                show_all=show_all, 
+                show_all=show_all,
                 show_diff=show_diff,
                 workers=workers,
             )
 
         return {
             'good': result.count(True),
             'bad': result.count(False),
```

### Comparing `bundlewrap-4.8.2/bundlewrap/operations.py` & `bundlewrap-4.9.0/bundlewrap/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,32 +201,35 @@
         127,  # command not found
         255,  # SSH error
     ),
     log_function=None,
     username=None,  # SSH auth
     wrapper_inner="{}",
     wrapper_outer="{}",
+    user="root",  # remote user running the command
 ):
     """
     Runs a command on a remote system.
     """
+    shell_command = wrapper_outer.format(quote(wrapper_inner.format(command)), user)
+
     ssh_command = [
         "ssh",
         "-o", "BatchMode=yes",
         "-o", "KbdInteractiveAuthentication=no",
         "-o", "PasswordAuthentication=no",
         "-o", "StrictHostKeyChecking=no" if add_host_keys else "StrictHostKeyChecking=yes",
     ]
     if username:
         ssh_command += ["-l", str(username)]
     extra_args = environ.get("BW_SSH_ARGS", "").strip()
     if extra_args:
         ssh_command.extend(split(extra_args))
     ssh_command.append(hostname)
-    ssh_command.append(wrapper_outer.format(quote(wrapper_inner.format(command))))
+    ssh_command.append(shell_command)
 
     result = run_local(
         ssh_command,
         data_stdin=data_stdin,
         log_function=log_function,
     )
```

### Comparing `bundlewrap-4.8.2/bundlewrap/repo.py` & `bundlewrap-4.9.0/bundlewrap/repo.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/secrets.py` & `bundlewrap-4.9.0/bundlewrap/secrets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from base64 import b64encode, urlsafe_b64decode
 from configparser import ConfigParser
 import hashlib
 import hmac
 from os import environ
 from os.path import join
 from string import ascii_letters, punctuation, digits
+from subprocess import PIPE, run
 
 from cryptography.fernet import Fernet
 
 from .exceptions import FaultUnavailable
 from .utils import Fault, get_file_contents
-from .utils.text import mark_for_translation as _
+from .utils.text import force_text, mark_for_translation as _
 from .utils.ui import io
 
 
 HUMAN_CHARS_START = list("bcdfghjklmnprstvwxz")
 HUMAN_CHARS_VOWELS = list("aeiou") + ["ai", "ao", "au", "ea", "ee", "ei",
                                       "eu", "ia", "ie", "oo", "ou"]
 HUMAN_CHARS_CONS = HUMAN_CHARS_START + ["bb", "bl", "cc", "ch", "ck", "dd", "dr",
@@ -244,14 +245,35 @@
             io.debug(_("unable to read {}").format(secrets_file))
             return {}
         result = {}
         for section in config.sections():
             result[section] = config.get(section, 'key').encode('utf-8')
         return result
 
+    @staticmethod
+    def cmd(cmdline, as_text=True, strip=True):
+        def callback():
+            output = run(
+                cmdline,
+                check=True,
+                shell=True,
+                stdout=PIPE,  # replace with capture_output=True
+                              # when dropping support for Python 3.6
+            ).stdout
+            if as_text:
+                output = force_text(output)
+            if strip:
+                output = output.strip()
+            return output
+
+        return Fault(
+            'bw secrets cmd ' + cmdline,
+            callback,
+        )
+
     def decrypt(self, cryptotext, key=None):
         return Fault(
             'bw secrets decrypt',
             self._decrypt,
             cryptotext=cryptotext,
             key=key,
         )
```

### Comparing `bundlewrap-4.8.2/bundlewrap/utils/__init__.py` & `bundlewrap-4.9.0/bundlewrap/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/utils/cmdline.py` & `bundlewrap-4.9.0/bundlewrap/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/utils/dicts.py` & `bundlewrap-4.9.0/bundlewrap/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/utils/metastack.py` & `bundlewrap-4.9.0/bundlewrap/utils/metastack.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/utils/plot.py` & `bundlewrap-4.9.0/bundlewrap/utils/plot.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/utils/remote.py` & `bundlewrap-4.9.0/bundlewrap/utils/remote.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/utils/scm.py` & `bundlewrap-4.9.0/bundlewrap/utils/scm.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/utils/table.py` & `bundlewrap-4.9.0/bundlewrap/utils/table.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/utils/testing.py` & `bundlewrap-4.9.0/bundlewrap/utils/testing.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/utils/text.py` & `bundlewrap-4.9.0/bundlewrap/utils/text.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap/utils/ui.py` & `bundlewrap-4.9.0/bundlewrap/utils/ui.py`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/bundlewrap.egg-info/PKG-INFO` & `bundlewrap-4.9.0/bundlewrap.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: bundlewrap
-Version: 4.8.2
+Version: 4.9.0
 Summary: Config management with Python
 Home-page: http://bundlewrap.org
 Author: Torsten Rehn
 Author-email: torsten@rehn.email
 License: GPLv3
-Description: By allowing for easy and low-overhead config management, BundleWrap fills the gap between complex deployments using Chef or Puppet and old school system administration over SSH.
-        While most other config management systems rely on a client-server architecture, BundleWrap works off a repository cloned to your local machine. It then automates the process of SSHing into your servers and making sure everything is configured the way it's supposed to be. You won't have to install anything on managed servers.
 Keywords: configuration,config,management
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -19,7 +17,13 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
+License-File: LICENSE
+License-File: AUTHORS
+
+By allowing for easy and low-overhead config management, BundleWrap fills the gap between complex deployments using Chef or Puppet and old school system administration over SSH.
+While most other config management systems rely on a client-server architecture, BundleWrap works off a repository cloned to your local machine. It then automates the process of SSHing into your servers and making sure everything is configured the way it's supposed to be. You won't have to install anything on managed servers.
+
```

### Comparing `bundlewrap-4.8.2/bundlewrap.egg-info/SOURCES.txt` & `bundlewrap-4.9.0/bundlewrap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bundlewrap-4.8.2/setup.py` & `bundlewrap-4.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 
 setup(
     name="bundlewrap",
-    version="4.8.2",
+    version="4.9.0",
     description="Config management with Python",
     long_description=(
         "By allowing for easy and low-overhead config management, BundleWrap fills the gap between complex deployments using Chef or Puppet and old school system administration over SSH.\n"
         "While most other config management systems rely on a client-server architecture, BundleWrap works off a repository cloned to your local machine. It then automates the process of SSHing into your servers and making sure everything is configured the way it's supposed to be. You won't have to install anything on managed servers."
     ),
     author="Torsten Rehn",
     author_email="torsten@rehn.email",
```

