# Comparing `tmp/types-python-xlib-0.33.0.8.tar.gz` & `tmp/types-python-xlib-0.33.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-python-xlib-0.33.0.8.tar", last modified: Fri Feb 24 01:23:24 2023, max compression
+gzip compressed data, was "types-python-xlib-0.33.0.9.tar", last modified: Wed Mar 22 21:13:00 2023, max compression
```

## Comparing `types-python-xlib-0.33.0.8.tar` & `types-python-xlib-0.33.0.9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:23:24.007386 types-python-xlib-0.33.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-02-24 01:23:23.000000 types-python-xlib-0.33.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-24 01:23:23.000000 types-python-xlib-0.33.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-02-24 01:23:24.007386 types-python-xlib-0.33.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:23:24.003386 types-python-xlib-0.33.0.8/Xlib-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-24 01:23:23.000000 types-python-xlib-0.33.0.8/Xlib-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/X.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/XK.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/Xatom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/Xcursorfont.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/Xutil.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/_typing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/display.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/error.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:23:24.003386 types-python-xlib-0.33.0.8/Xlib-stubs/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/composite.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/damage.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/dpms.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/ge.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/nvcontrol.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7379 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/randr.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/record.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/res.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/screensaver.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/security.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/shape.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/xfixes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/xinerama.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/xinput.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/ext/xtest.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:23:24.007386 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/apl.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/arabic.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/cyrillic.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/greek.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/hebrew.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/katakana.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/korean.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/latin1.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/latin2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/latin3.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/latin4.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/miscellany.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/publishing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/special.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/technical.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/thai.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/xf86.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/xk3270.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/xkb.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:23:24.007386 types-python-xlib-0.33.0.8/Xlib-stubs/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/protocol/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/protocol/display.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/protocol/event.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/protocol/request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14811 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/protocol/rq.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/protocol/structs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/rdb.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:23:24.007386 types-python-xlib-0.33.0.8/Xlib-stubs/support/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/support/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/support/connect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/support/lock.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/support/unix_connect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/support/vms_connect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/threaded.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/xauth.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:23:24.007386 types-python-xlib-0.33.0.8/Xlib-stubs/xobject/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/xobject/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/xobject/colormap.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/xobject/cursor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12279 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/xobject/drawable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/xobject/fontable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/xobject/icccm.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-24 01:23:07.000000 types-python-xlib-0.33.0.8/Xlib-stubs/xobject/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 01:23:24.007386 types-python-xlib-0.33.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-02-24 01:23:23.000000 types-python-xlib-0.33.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:23:24.007386 types-python-xlib-0.33.0.8/types_python_xlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-02-24 01:23:23.000000 types-python-xlib-0.33.0.8/types_python_xlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-02-24 01:23:23.000000 types-python-xlib-0.33.0.8/types_python_xlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 01:23:23.000000 types-python-xlib-0.33.0.8/types_python_xlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-24 01:23:23.000000 types-python-xlib-0.33.0.8/types_python_xlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-24 01:23:23.000000 types-python-xlib-0.33.0.8/types_python_xlib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 21:13:00.152178 types-python-xlib-0.33.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-03-22 21:12:58.000000 types-python-xlib-0.33.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-22 21:12:58.000000 types-python-xlib-0.33.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-22 21:13:00.152178 types-python-xlib-0.33.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 21:13:00.144178 types-python-xlib-0.33.0.9/Xlib-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-22 21:12:58.000000 types-python-xlib-0.33.0.9/Xlib-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/X.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/XK.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/Xatom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/Xcursorfont.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/Xutil.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/_typing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/display.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/error.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 21:13:00.144178 types-python-xlib-0.33.0.9/Xlib-stubs/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/composite.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/damage.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/dpms.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/ge.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    53094 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/nvcontrol.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/randr.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/record.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/res.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/screensaver.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/security.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/shape.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/xfixes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/xinerama.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/xinput.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/ext/xtest.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 21:13:00.148178 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/apl.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/arabic.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/cyrillic.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/greek.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/hebrew.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/katakana.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/korean.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/latin1.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/latin2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/latin3.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/latin4.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/miscellany.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/publishing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/special.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/technical.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/thai.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/xf86.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/xk3270.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/xkb.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 21:13:00.148178 types-python-xlib-0.33.0.9/Xlib-stubs/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/protocol/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/protocol/display.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/protocol/event.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/protocol/request.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14590 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/protocol/rq.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/protocol/structs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/rdb.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 21:13:00.148178 types-python-xlib-0.33.0.9/Xlib-stubs/support/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/support/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/support/connect.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/support/lock.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/support/unix_connect.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/support/vms_connect.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/threaded.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/xauth.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 21:13:00.148178 types-python-xlib-0.33.0.9/Xlib-stubs/xobject/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/xobject/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/xobject/colormap.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/xobject/cursor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/xobject/drawable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/xobject/fontable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/xobject/icccm.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-22 21:12:48.000000 types-python-xlib-0.33.0.9/Xlib-stubs/xobject/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 21:13:00.152178 types-python-xlib-0.33.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-03-22 21:12:58.000000 types-python-xlib-0.33.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 21:13:00.152178 types-python-xlib-0.33.0.9/types_python_xlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-22 21:13:00.000000 types-python-xlib-0.33.0.9/types_python_xlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-03-22 21:13:00.000000 types-python-xlib-0.33.0.9/types_python_xlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 21:13:00.000000 types-python-xlib-0.33.0.9/types_python_xlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-22 21:13:00.000000 types-python-xlib-0.33.0.9/types_python_xlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-22 21:13:00.000000 types-python-xlib-0.33.0.9/types_python_xlib.egg-info/top_level.txt
```

### Comparing `types-python-xlib-0.33.0.8/CHANGELOG.md` & `types-python-xlib-0.33.0.9/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.33.0.9 (2023-03-22)
+
+Add defaults for params and constants in python-xlib (#9642)
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 0.33.0.8 (2023-02-24)
 
 Fix some typos in comments (#9802)
 
 ## 0.33.0.7 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-python-xlib-0.33.0.8/PKG-INFO` & `types-python-xlib-0.33.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-xlib
-Version: 0.33.0.8
+Version: 0.33.0.9
 Summary: Typing stubs for python-xlib
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-xlib.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-xlib`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-xlib. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4ca5ee98df5654d0db7f5b24cd2bd3b3fe54f313`.
+This package was generated from typeshed commit `d8e3f928b0e7dbaf3dafdb8fc5e257331532ae4c`.
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/display.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/display.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -30,25 +30,25 @@
     fontable: type[fontable.Fontable]
     font: type[fontable.Font]
     gc: type[fontable.GC]
     colormap: type[colormap.Colormap]
     cursor: type[cursor.Cursor]
 
 class _BaseDisplay(display.Display):
-    def __init__(self, display: str | None = ...) -> None: ...
-    def get_atom(self, atomname: str, only_if_exists: bool = ...) -> int: ...
+    def __init__(self, display: str | None = None) -> None: ...
+    def get_atom(self, atomname: str, only_if_exists: bool = False) -> int: ...
 
 class Display:
     display: _BaseDisplay
     keysym_translations: dict[int, str]
     extensions: list[str]
     class_extension_dicts: dict[str, dict[str, FunctionType]]
     display_extension_methods: dict[str, Callable[..., Any]]
     extension_event: rq.DictWrapper
-    def __init__(self, display: str | None = ...) -> None: ...
+    def __init__(self, display: str | None = None) -> None: ...
     def get_display_name(self) -> str: ...
     def fileno(self) -> int: ...
     def close(self) -> None: ...
     def set_error_handler(self, handler: ErrorHandler[object] | None) -> None: ...
     def flush(self) -> None: ...
     def sync(self) -> None: ...
     def next_event(self) -> rq.Event: ...
@@ -71,92 +71,92 @@
     @overload
     def create_resource_object(self, type: Literal["colormap"], id: int) -> colormap.Colormap: ...
     @overload
     def create_resource_object(self, type: Literal["cursor"], id: int) -> cursor.Cursor: ...
     @overload
     def create_resource_object(self, type: str, id: int) -> resource.Resource: ...
     def __getattr__(self, attr: str) -> MethodType: ...
-    def screen(self, sno: int | None = ...) -> rq.Struct: ...
+    def screen(self, sno: int | None = None) -> rq.Struct: ...
     def screen_count(self) -> int: ...
     def get_default_screen(self) -> int: ...
     def extension_add_method(self, object: str, name: str, function: Callable[..., Any]) -> None: ...
-    def extension_add_event(self, code: int, evt: type, name: str | None = ...) -> None: ...
-    def extension_add_subevent(self, code: int, subcode: int | None, evt: type[rq.Event], name: str | None = ...) -> None: ...
+    def extension_add_event(self, code: int, evt: type, name: str | None = None) -> None: ...
+    def extension_add_subevent(self, code: int, subcode: int | None, evt: type[rq.Event], name: str | None = None) -> None: ...
     def extension_add_error(self, code: int, err: type[error.XError]) -> None: ...
     def keycode_to_keysym(self, keycode: int, index: int) -> int: ...
     def keysym_to_keycode(self, keysym: int) -> int: ...
     def keysym_to_keycodes(self, keysym: int) -> Iterable[tuple[int, int]]: ...
     def refresh_keyboard_mapping(self, evt: rq.Event) -> None: ...
     def lookup_string(self, keysym: int) -> str | None: ...
     def rebind_string(self, keysym: int, newstring: str | None) -> None: ...
-    def intern_atom(self, name: str, only_if_exists: bool = ...) -> int: ...
-    def get_atom(self, atom: str, only_if_exists: bool = ...) -> int: ...
+    def intern_atom(self, name: str, only_if_exists: bool = False) -> int: ...
+    def get_atom(self, atom: str, only_if_exists: bool = False) -> int: ...
     def get_atom_name(self, atom: int) -> str: ...
     def get_selection_owner(self, selection: int) -> int: ...
     def send_event(
         self,
         destination: int,
         event: rq.Event,
-        event_mask: int = ...,
-        propagate: bool = ...,
-        onerror: ErrorHandler[object] | None = ...,
+        event_mask: int = 0,
+        propagate: bool = False,
+        onerror: ErrorHandler[object] | None = None,
     ) -> None: ...
-    def ungrab_pointer(self, time: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def ungrab_pointer(self, time: int, onerror: ErrorHandler[object] | None = None) -> None: ...
     def change_active_pointer_grab(
-        self, event_mask: int, cursor: cursor.Cursor, time: int, onerror: ErrorHandler[object] | None = ...
+        self, event_mask: int, cursor: cursor.Cursor, time: int, onerror: ErrorHandler[object] | None = None
     ) -> None: ...
-    def ungrab_keyboard(self, time: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def allow_events(self, mode: int, time: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def grab_server(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def ungrab_server(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def ungrab_keyboard(self, time: int, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def allow_events(self, mode: int, time: int, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def grab_server(self, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def ungrab_server(self, onerror: ErrorHandler[object] | None = None) -> None: ...
     def warp_pointer(
         self,
         x: int,
         y: int,
-        src_window: int = ...,
-        src_x: int = ...,
-        src_y: int = ...,
-        src_width: int = ...,
-        src_height: int = ...,
-        onerror: ErrorHandler[object] | None = ...,
+        src_window: int = 0,
+        src_x: int = 0,
+        src_y: int = 0,
+        src_width: int = 0,
+        src_height: int = 0,
+        onerror: ErrorHandler[object] | None = None,
     ) -> None: ...
-    def set_input_focus(self, focus: int, revert_to: int, time: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def set_input_focus(self, focus: int, revert_to: int, time: int, onerror: ErrorHandler[object] | None = None) -> None: ...
     def get_input_focus(self) -> request.GetInputFocus: ...
     def query_keymap(self) -> bytes: ...  # TODO: Validate if this is correct
     def open_font(self, name: str) -> _ResourceBaseClass | None: ...
     def list_fonts(self, pattern: Pattern[str] | str, max_names: int) -> list[str]: ...
     def list_fonts_with_info(self, pattern: Pattern[str] | str, max_names: int) -> request.ListFontsWithInfo: ...
-    def set_font_path(self, path: Sequence[str], onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def set_font_path(self, path: Sequence[str], onerror: ErrorHandler[object] | None = None) -> None: ...
     def get_font_path(self) -> list[str]: ...
     def query_extension(self, name: str) -> request.QueryExtension | None: ...
     def list_extensions(self) -> list[str]: ...
     def change_keyboard_mapping(
-        self, first_keycode: int, keysyms: Sequence[Sequence[int]], onerror: ErrorHandler[object] | None = ...
+        self, first_keycode: int, keysyms: Sequence[Sequence[int]], onerror: ErrorHandler[object] | None = None
     ) -> None: ...
     def get_keyboard_mapping(self, first_keycode: int, count: int) -> list[tuple[int, ...]]: ...
-    def change_keyboard_control(self, onerror: ErrorHandler[object] | None = ..., **keys: object) -> None: ...
+    def change_keyboard_control(self, onerror: ErrorHandler[object] | None = None, **keys: object) -> None: ...
     def get_keyboard_control(self) -> request.GetKeyboardControl: ...
-    def bell(self, percent: int = ..., onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def bell(self, percent: int = 0, onerror: ErrorHandler[object] | None = None) -> None: ...
     def change_pointer_control(
-        self, accel: tuple[int, int] | None = ..., threshold: int | None = ..., onerror: ErrorHandler[object] | None = ...
+        self, accel: tuple[int, int] | None = None, threshold: int | None = None, onerror: ErrorHandler[object] | None = None
     ) -> None: ...
     def get_pointer_control(self) -> request.GetPointerControl: ...
     def set_screen_saver(
-        self, timeout: int, interval: int, prefer_blank: int, allow_exposures: int, onerror: ErrorHandler[object] | None = ...
+        self, timeout: int, interval: int, prefer_blank: int, allow_exposures: int, onerror: ErrorHandler[object] | None = None
     ) -> None: ...
     def get_screen_saver(self) -> request.GetScreenSaver: ...
     def change_hosts(
         self,
         mode: int,
         host_family: int,
         host: Sequence[int] | Sequence[bytes],  # TODO: validate
-        onerror: ErrorHandler[object] | None = ...,
+        onerror: ErrorHandler[object] | None = None,
     ) -> None: ...
     def list_hosts(self) -> request.ListHosts: ...
-    def set_access_control(self, mode: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def set_close_down_mode(self, mode: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def force_screen_saver(self, mode: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def set_access_control(self, mode: int, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def set_close_down_mode(self, mode: int, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def force_screen_saver(self, mode: int, onerror: ErrorHandler[object] | None = None) -> None: ...
     def set_pointer_mapping(self, map: Sequence[int]) -> int: ...
     def get_pointer_mapping(self) -> list[int]: ...
     def set_modifier_mapping(self, keycodes: rq._ModifierMappingList8Elements) -> int: ...
     def get_modifier_mapping(self) -> Sequence[Sequence[int]]: ...
-    def no_operation(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def no_operation(self, onerror: ErrorHandler[object] | None = None) -> None: ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/error.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/error.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import SliceableBuffer
-from typing_extensions import Literal
+from typing_extensions import Final, Literal
 
 from Xlib.protocol import display, rq
 
 class DisplayError(Exception):
     display: object
     def __init__(self, display: object) -> None: ...
 
@@ -40,15 +40,15 @@
 class BadColor(XResourceError): ...
 class BadGC(XResourceError): ...
 class BadIDChoice(XResourceError): ...
 class BadName(XError): ...
 class BadLength(XError): ...
 class BadImplementation(XError): ...
 
-xerror_class: dict[int, type[XError]]
+xerror_class: Final[dict[int, type[XError]]]
 
 class CatchError:
     error_types: tuple[type[XError], ...]
     error: XError | None
     request: rq.Request | None
     def __init__(self, *errors: type[XError]) -> None: ...
     def __call__(self, error: XError, request: rq.Request | None) -> Literal[0, 1]: ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/ext/__init__.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/ext/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/ext/composite.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/ext/composite.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from collections.abc import Callable
 from typing import Any
-from typing_extensions import TypeAlias
+from typing_extensions import Final, TypeAlias
 
 from Xlib._typing import ErrorHandler, Unused
 from Xlib.display import Display
 from Xlib.protocol import rq
 from Xlib.xobject import drawable, resource
 
 _Update: TypeAlias = Callable[[rq.DictWrapper | dict[str, Any]], object]
 
-extname: str
-RedirectAutomatic: int
-RedirectManual: int
+extname: Final = "Composite"
+RedirectAutomatic: Final = 0
+RedirectManual: Final = 1
 
 class QueryVersion(rq.ReplyRequest): ...
 
 def query_version(self: Display | resource.Resource) -> QueryVersion: ...
 
 class RedirectWindow(rq.Request): ...
 
-def redirect_window(self: drawable.Window, update: _Update, onerror: ErrorHandler[object] | None = ...) -> None: ...
+def redirect_window(self: drawable.Window, update: _Update, onerror: ErrorHandler[object] | None = None) -> None: ...
 
 class RedirectSubwindows(rq.Request): ...
 
-def redirect_subwindows(self: drawable.Window, update: _Update, onerror: ErrorHandler[object] | None = ...) -> None: ...
+def redirect_subwindows(self: drawable.Window, update: _Update, onerror: ErrorHandler[object] | None = None) -> None: ...
 
 class UnredirectWindow(rq.Request): ...
 
-def unredirect_window(self: drawable.Window, update: _Update, onerror: ErrorHandler[object] | None = ...) -> None: ...
+def unredirect_window(self: drawable.Window, update: _Update, onerror: ErrorHandler[object] | None = None) -> None: ...
 
 class UnredirectSubindows(rq.Request): ...
 
-def unredirect_subwindows(self: drawable.Window, update: _Update, onerror: ErrorHandler[object] | None = ...) -> None: ...
+def unredirect_subwindows(self: drawable.Window, update: _Update, onerror: ErrorHandler[object] | None = None) -> None: ...
 
 class CreateRegionFromBorderClip(rq.Request): ...
 
-def create_region_from_border_clip(self: drawable.Window, onerror: ErrorHandler[object] | None = ...) -> int: ...
+def create_region_from_border_clip(self: drawable.Window, onerror: ErrorHandler[object] | None = None) -> int: ...
 
 class NameWindowPixmap(rq.Request): ...
 
-def name_window_pixmap(self: Display | resource.Resource, onerror: ErrorHandler[object] | None = ...) -> drawable.Pixmap: ...
+def name_window_pixmap(self: Display | resource.Resource, onerror: ErrorHandler[object] | None = None) -> drawable.Pixmap: ...
 
 class GetOverlayWindow(rq.ReplyRequest): ...
 
 def get_overlay_window(self: Display) -> GetOverlayWindow: ...
 def init(disp: Display, info: Unused) -> None: ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/ext/damage.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/ext/damage.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,40 @@
+from typing_extensions import Final, Literal
+
 from Xlib.display import Display
 from Xlib.error import XError
 from Xlib.protocol import request, rq
 from Xlib.xobject import resource
 
-extname: str
-DamageNotifyCode: int
-BadDamageCode: int
-
-class BadDamageError(XError): ...
-
-DamageReportRawRectangles: int
-DamageReportDeltaRectangles: int
-DamageReportBoundingBox: int
-DamageReportNonEmpty: int
-DamageReportLevel: tuple[int, int, int, int]
+extname: Final = "DAMAGE"
+DamageNotifyCode: Final = 0
+BadDamageCode: Final = 0
+DamageReportRawRectangles: Final = 0
+DamageReportDeltaRectangles: Final = 1
+DamageReportBoundingBox: Final = 2
+DamageReportNonEmpty: Final = 3
+DamageReportLevel: Final[tuple[Literal[0], Literal[1], Literal[2], Literal[3]]]
 DAMAGE = rq.Card32
 
+class BadDamageError(XError): ...
 class QueryVersion(rq.ReplyRequest): ...
 
 def query_version(self: Display | resource.Resource) -> QueryVersion: ...
 
 class DamageCreate(rq.Request): ...
 
 def damage_create(self: Display | resource.Resource, level: int) -> int: ...
 
 class DamageDestroy(rq.Request): ...
 
 def damage_destroy(self: Display | resource.Resource, damage: int) -> None: ...
 
 class DamageSubtract(rq.Request): ...
 
-def damage_subtract(self: Display | resource.Resource, damage: int, repair: int = ..., parts: int = ...) -> None: ...
+def damage_subtract(self: Display | resource.Resource, damage: int, repair: int = 0, parts: int = 0) -> None: ...
 
 class DamageAdd(rq.Request): ...
 
 def damage_add(self: Display | resource.Resource, repair: int, parts: int) -> None: ...
 
 class DamageNotify(rq.Event): ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/ext/dpms.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/ext/dpms.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from typing_extensions import Final, Literal
+
 from Xlib._typing import Unused
 from Xlib.display import Display
 from Xlib.protocol import rq
 from Xlib.xobject import resource
 
-extname: str
-DPMSModeOn: int
-DPMSModeStandby: int
-DPMSModeSuspend: int
-DPMSModeOff: int
-DPMSPowerLevel: tuple[int, int, int, int]
+extname: Final = "DPMS"
+DPMSModeOn: Final = 0
+DPMSModeStandby: Final = 1
+DPMSModeSuspend: Final = 2
+DPMSModeOff: Final = 3
+DPMSPowerLevel: Final[tuple[Literal[0], Literal[1], Literal[2], Literal[3]]]
 
 class DPMSGetVersion(rq.ReplyRequest): ...
 
 def get_version(self: Display | resource.Resource) -> DPMSGetVersion: ...
 
 class DPMSCapable(rq.ReplyRequest): ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/ext/randr.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/ext/randr.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 from collections.abc import Sequence
-from typing_extensions import TypeAlias
+from typing_extensions import Final, TypeAlias
 
 from Xlib.display import Display
 from Xlib.protocol import request, rq
 from Xlib.xobject import drawable, resource
 
 _RandRModeInfo13IntSequence: TypeAlias = Sequence[int]
 
-extname: str
-RRScreenChangeNotify: int
-RRNotify: int
-RRNotify_CrtcChange: int
-RRNotify_OutputChange: int
-RRNotify_OutputProperty: int
-RRScreenChangeNotifyMask: int
-RRCrtcChangeNotifyMask: int
-RROutputChangeNotifyMask: int
-RROutputPropertyNotifyMask: int
-SetConfigSuccess: int
-SetConfigInvalidConfigTime: int
-SetConfigInvalidTime: int
-SetConfigFailed: int
-Rotate_0: int
-Rotate_90: int
-Rotate_180: int
-Rotate_270: int
-Reflect_X: int
-Reflect_Y: int
-HSyncPositive: int
-HSyncNegative: int
-VSyncPositive: int
-VSyncNegative: int
-Interlace: int
-DoubleScan: int
-CSync: int
-CSyncPositive: int
-CSyncNegative: int
-HSkewPresent: int
-BCast: int
-PixelMultiplex: int
-DoubleClock: int
-ClockDivideBy2: int
-Connected: int
-Disconnected: int
-UnknownConnection: int
-PROPERTY_RANDR_EDID: str
-PROPERTY_SIGNAL_FORMAT: str
-PROPERTY_SIGNAL_PROPERTIES: str
-PROPERTY_CONNECTOR_TYPE: str
-PROPERTY_CONNECTOR_NUMBER: str
-PROPERTY_COMPATIBILITY_LIST: str
-PROPERTY_CLONE_LIST: str
-SubPixelUnknown: int
-SubPixelHorizontalRGB: int
-SubPixelHorizontalBGR: int
-SubPixelVerticalRGB: int
-SubPixelVerticalBGR: int
-SubPixelNone: int
-BadRROutput: int
-BadRRCrtc: int
-BadRRMode: int
+extname: Final = "RANDR"
+RRScreenChangeNotify: Final = 0
+RRNotify: Final = 1
+RRNotify_CrtcChange: Final = 0
+RRNotify_OutputChange: Final = 1
+RRNotify_OutputProperty: Final = 2
+RRScreenChangeNotifyMask: Final = 0x1
+RRCrtcChangeNotifyMask: Final = 0x2
+RROutputChangeNotifyMask: Final = 0x4
+RROutputPropertyNotifyMask: Final = 0x8
+SetConfigSuccess: Final = 0
+SetConfigInvalidConfigTime: Final = 1
+SetConfigInvalidTime: Final = 2
+SetConfigFailed: Final = 3
+Rotate_0: Final = 1
+Rotate_90: Final = 2
+Rotate_180: Final = 4
+Rotate_270: Final = 8
+Reflect_X: Final = 16
+Reflect_Y: Final = 32
+HSyncPositive: Final = 0x00000001
+HSyncNegative: Final = 0x00000002
+VSyncPositive: Final = 0x00000004
+VSyncNegative: Final = 0x00000008
+Interlace: Final = 0x00000010
+DoubleScan: Final = 0x00000020
+CSync: Final = 0x00000040
+CSyncPositive: Final = 0x00000080
+CSyncNegative: Final = 0x00000100
+HSkewPresent: Final = 0x00000200
+BCast: Final = 0x00000400
+PixelMultiplex: Final = 0x00000800
+DoubleClock: Final = 0x00001000
+ClockDivideBy2: Final = 0x00002000
+Connected: Final = 0
+Disconnected: Final = 1
+UnknownConnection: Final = 2
+PROPERTY_RANDR_EDID: Final = "EDID"
+PROPERTY_SIGNAL_FORMAT: Final = "SignalFormat"
+PROPERTY_SIGNAL_PROPERTIES: Final = "SignalProperties"
+PROPERTY_CONNECTOR_TYPE: Final = "ConnectorType"
+PROPERTY_CONNECTOR_NUMBER: Final = "ConnectorNumber"
+PROPERTY_COMPATIBILITY_LIST: Final = "CompatibilityList"
+PROPERTY_CLONE_LIST: Final = "CloneList"
+SubPixelUnknown: Final = 0
+SubPixelHorizontalRGB: Final = 1
+SubPixelHorizontalBGR: Final = 2
+SubPixelVerticalRGB: Final = 3
+SubPixelVerticalBGR: Final = 4
+SubPixelNone: Final = 5
+BadRROutput: Final = 0
+BadRRCrtc: Final = 1
+BadRRMode: Final = 2
 
 class BadRROutputError(Exception): ...
 class BadRRCrtcError(Exception): ...
 class BadRRModeError(Exception): ...
 
 RandR_ScreenSizes: rq.Struct
 RandR_ModeInfo: rq.Struct
@@ -75,15 +75,15 @@
 
 def query_version(self: Display | resource.Resource) -> QueryVersion: ...
 
 class _1_0SetScreenConfig(rq.ReplyRequest): ...
 class SetScreenConfig(rq.ReplyRequest): ...
 
 def set_screen_config(
-    self: drawable.Drawable, size_id: int, rotation: int, config_timestamp: int, rate: int = ..., timestamp: int = ...
+    self: drawable.Drawable, size_id: int, rotation: int, config_timestamp: int, rate: int = 0, timestamp: int = 0
 ) -> SetScreenConfig: ...
 
 class SelectInput(rq.Request): ...
 
 def select_input(self: drawable.Window, mask: int) -> SelectInput: ...
 
 class GetScreenInfo(rq.ReplyRequest): ...
@@ -96,16 +96,16 @@
 
 class SetScreenSize(rq.Request): ...
 
 def set_screen_size(
     self: drawable.Window,
     width: int,
     height: int,
-    width_in_millimeters: int | None = ...,
-    height_in_millimeters: int | None = ...,
+    width_in_millimeters: int | None = None,
+    height_in_millimeters: int | None = None,
 ) -> SetScreenSize: ...
 
 class GetScreenResources(rq.ReplyRequest): ...
 
 def get_screen_resources(self: drawable.Window) -> GetScreenResources: ...
 
 class GetOutputInfo(rq.ReplyRequest): ...
@@ -139,16 +139,16 @@
 def get_output_property(
     self: Display | resource.Resource,
     output: int,
     property: int,
     type: int,
     long_offset: int,
     long_length: int,
-    delete: bool = ...,
-    pending: bool = ...,
+    delete: bool = False,
+    pending: bool = False,
 ) -> GetOutputProperty: ...
 
 class CreateMode(rq.ReplyRequest): ...
 
 def create_mode(self: drawable.Window, mode: _RandRModeInfo13IntSequence, name: str) -> CreateMode: ...
 
 class DestroyMode(rq.Request): ...
@@ -174,15 +174,15 @@
     crtc: int,
     config_timestamp: int,
     x: int,
     y: int,
     mode: int,
     rotation: int,
     outputs: Sequence[int],
-    timestamp: int = ...,
+    timestamp: int = 0,
 ) -> SetCrtcConfig: ...
 
 class GetCrtcGammaSize(rq.ReplyRequest): ...
 
 def get_crtc_gamma_size(self: Display | resource.Resource, crtc: int) -> GetCrtcGammaSize: ...
 
 class GetCrtcGamma(rq.ReplyRequest): ...
@@ -224,28 +224,28 @@
     track_top: int,
     track_width: int,
     track_height: int,
     border_left: int,
     border_top: int,
     border_width: int,
     border_height: int,
-    timestamp: int = ...,
+    timestamp: int = 0,
 ) -> SetPanning: ...
 
 class SetOutputPrimary(rq.Request): ...
 
 def set_output_primary(self: drawable.Window, output: int) -> SetOutputPrimary: ...
 
 class GetOutputPrimary(rq.ReplyRequest): ...
 
 def get_output_primary(self: drawable.Window) -> GetOutputPrimary: ...
 
 class GetMonitors(rq.ReplyRequest): ...
 
-def get_monitors(self: drawable.Window, is_active: bool = ...) -> GetMonitors: ...
+def get_monitors(self: drawable.Window, is_active: bool = True) -> GetMonitors: ...
 
 class SetMonitor(rq.Request): ...
 
 def set_monitor(
     self: drawable.Window, monitor_info: tuple[int, bool, bool, Sequence[int], int, int, int, int, int]
 ) -> SetMonitor: ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/ext/record.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/ext/record.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from collections.abc import Callable, Sequence, Sized
 from typing import Any, TypeVar
-from typing_extensions import Literal
+from typing_extensions import Final, Literal
 
 from Xlib._typing import Unused
 from Xlib.display import Display
 from Xlib.protocol import display, rq
 from Xlib.xobject import resource
 
 _T = TypeVar("_T")
 _S = TypeVar("_S", bound=Sized)
 
-extname: str
-FromServerTime: int
-FromClientTime: int
-FromClientSequence: int
-CurrentClients: int
-FutureClients: int
-AllClients: int
-FromServer: int
-FromClient: int
-ClientStarted: int
-ClientDied: int
-StartOfData: int
-EndOfData: int
+extname: Final = "RECORD"
+
+FromServerTime: Final = 0x01
+FromClientTime: Final = 0x02
+FromClientSequence: Final = 0x04
+
+CurrentClients: Final = 1
+FutureClients: Final = 2
+AllClients: Final = 3
+
+FromServer: Final = 0
+FromClient: Final = 1
+ClientStarted: Final = 2
+ClientDied: Final = 3
+StartOfData: Final = 4
+EndOfData: Final = 5
 Record_Range8: rq.Struct
 Record_Range16: rq.Struct
 Record_ExtRange: rq.Struct
 Record_Range: rq.Struct
 Record_ClientInfo: rq.Struct
 
 class RawField(rq.ValueField):
@@ -90,15 +93,15 @@
 def get_context(self: Display | resource.Resource, context: int) -> GetContext: ...
 
 class EnableContext(rq.ReplyRequest):
     def __init__(
         self,
         callback: Callable[[rq.DictWrapper | dict[str, Any]], Any],
         display: display.Display,
-        defer: bool = ...,
+        defer: bool = False,
         *args: object | bool,
         **keys: object | bool,
     ) -> None: ...
 
 def enable_context(
     self: Display | resource.Resource, context: int, callback: Callable[[rq.DictWrapper | dict[str, Any]], Any]
 ) -> None: ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/ext/res.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/ext/res.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from collections.abc import Sequence
+from typing_extensions import Final
 
 from Xlib._typing import Unused
 from Xlib.display import Display
 from Xlib.protocol import rq
 from Xlib.xobject import resource
 
-RES_MAJOR_VERSION: int
-RES_MINOR_VERSION: int
-extname: str
-ResQueryVersion: int
-ResQueryClients: int
-ResQueryClientResources: int
-ResQueryClientPixmapBytes: int
-ResQueryClientIds: int
-ResQueryResourceBytes: int
+RES_MAJOR_VERSION: Final = 1
+RES_MINOR_VERSION: Final = 2
+extname: Final = "X-Resource"
+ResQueryVersion: Final = 0
+ResQueryClients: Final = 1
+ResQueryClientResources: Final = 2
+ResQueryClientPixmapBytes: Final = 3
+ResQueryClientIds: Final = 4
+ResQueryResourceBytes: Final = 5
 
 class QueryVersion(rq.ReplyRequest): ...
 
-def query_version(self: Display | resource.Resource, client_major: int = ..., client_minor: int = ...) -> QueryVersion: ...
+def query_version(self: Display | resource.Resource, client_major: int = 1, client_minor: int = 2) -> QueryVersion: ...
 
 Client: rq.Struct
 
 class QueryClients(rq.ReplyRequest): ...
 
 def query_clients(self: Display | resource.Resource) -> QueryClients: ...
 
@@ -36,16 +37,16 @@
 def query_client_pixmap_bytes(self: Display | resource.Resource, client: int) -> QueryClientPixmapBytes: ...
 
 class SizeOf(rq.LengthOf):
     item_size: int
     def __init__(self, name: str | list[str] | tuple[str, ...], size: int, item_size: int) -> None: ...
     def parse_value(self, length: int, display: Unused) -> int: ...  # type: ignore[override]
 
-ClientXIDMask: int
-LocalClientPIDMask: int
+ClientXIDMask: Final = 0x1
+LocalClientPIDMask: Final = 0x2
 ClientIdSpec: rq.Struct
 ClientIdValue: rq.Struct
 
 class QueryClientIds(rq.ReplyRequest): ...
 
 def query_client_ids(self: Display | resource.Resource, specs: Sequence[tuple[int, int]]) -> QueryClientIds: ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/ext/screensaver.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/ext/screensaver.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from typing_extensions import Final
+
 from Xlib._typing import ErrorHandler
 from Xlib.display import Display
 from Xlib.protocol import request, rq
 from Xlib.xobject import drawable
 
-extname: str
-NotifyMask: int
-CycleMask: int
-StateOff: int
-StateOn: int
-StateCycle: int
-KindBlanked: int
-KindInternal: int
-KindExternal: int
+extname: Final = "MIT-SCREEN-SAVER"
+NotifyMask: Final = 1
+CycleMask: Final = 2
+StateOff: Final = 0
+StateOn: Final = 1
+StateCycle: Final = 2
+KindBlanked: Final = 0
+KindInternal: Final = 1
+KindExternal: Final = 2
 
 class QueryVersion(rq.ReplyRequest): ...
 
 def query_version(self: drawable.Drawable) -> QueryVersion: ...
 
 class QueryInfo(rq.ReplyRequest): ...
 
@@ -30,21 +32,21 @@
 def set_attributes(
     self: drawable.Drawable,
     x: int,
     y: int,
     width: int,
     height: int,
     border_width: int,
-    window_class: int = ...,
-    depth: int = ...,
-    visual: int = ...,
-    onerror: ErrorHandler[object] | None = ...,
+    window_class: int = 0,
+    depth: int = 0,
+    visual: int = 0,
+    onerror: ErrorHandler[object] | None = None,
     **keys: object,
 ) -> SetAttributes: ...
 
 class UnsetAttributes(rq.Request): ...
 
-def unset_attributes(self: drawable.Drawable, onerror: ErrorHandler[object] | None = ...) -> UnsetAttributes: ...
+def unset_attributes(self: drawable.Drawable, onerror: ErrorHandler[object] | None = None) -> UnsetAttributes: ...
 
 class Notify(rq.Event): ...
 
 def init(disp: Display, info: request.QueryExtension) -> None: ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/ext/security.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/ext/security.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,33 @@
+from typing_extensions import Final
+
 from Xlib._typing import Unused
 from Xlib.display import Display
 from Xlib.protocol import rq
 from Xlib.xobject import resource
 
-extname: str
-SecurityClientTrusted: int
-SecurityClientUntrusted: int
-SecurityAuthorizationRevokedMask: int
+extname: Final = "SECURITY"
+SecurityClientTrusted: Final = 0
+SecurityClientUntrusted: Final = 1
+SecurityAuthorizationRevokedMask: Final = 1
 AUTHID = rq.Card32
 
 class QueryVersion(rq.ReplyRequest): ...
 
 def query_version(self: Display | resource.Resource) -> QueryVersion: ...
 
 class SecurityGenerateAuthorization(rq.ReplyRequest): ...
 
 def generate_authorization(
     self: Display | resource.Resource,
     auth_proto: str,
-    auth_data: bytes | bytearray = ...,
-    timeout: int | None = ...,
-    trust_level: int | None = ...,
-    group: int | None = ...,
-    event_mask: int | None = ...,
+    auth_data: bytes | bytearray = b"",
+    timeout: int | None = None,
+    trust_level: int | None = None,
+    group: int | None = None,
+    event_mask: int | None = None,
 ) -> SecurityGenerateAuthorization: ...
 
 class SecurityRevokeAuthorization(rq.Request): ...
 
 def revoke_authorization(self: Display | resource.Resource, authid: int) -> SecurityRevokeAuthorization: ...
 def init(disp: Display, info: Unused) -> None: ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/ext/shape.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/ext/shape.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from collections.abc import Sequence
+from typing_extensions import Final
 
 from Xlib.display import Display
 from Xlib.protocol import request, rq
 from Xlib.protocol.structs import _Rectangle4IntSequence
 from Xlib.xobject import drawable, resource
 
-extname: str
+extname: Final = "SHAPE"
 OP = rq.Card8
 
 class SO:
     Set: int
     Union: int
     Intersect: int
     Subtract: int
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/ext/xfixes.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/ext/xfixes.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+from typing_extensions import Final
+
 from Xlib._typing import Unused
 from Xlib.display import Display
 from Xlib.protocol import request, rq
 from Xlib.xobject import drawable, resource
 
-extname: str
-XFixesSelectionNotify: int
-XFixesCursorNotify: int
-XFixesSetSelectionOwnerNotifyMask: int
-XFixesSelectionWindowDestroyNotifyMask: int
-XFixesSelectionClientCloseNotifyMask: int
-XFixesDisplayCursorNotifyMask: int
-XFixesSetSelectionOwnerNotify: int
-XFixesSelectionWindowDestroyNotify: int
-XFixesSelectionClientCloseNotify: int
-XFixesDisplayCursorNotify: int
+extname: Final = "XFIXES"
+XFixesSelectionNotify: Final = 0
+XFixesCursorNotify: Final = 1
+XFixesSetSelectionOwnerNotifyMask: Final = 0x1
+XFixesSelectionWindowDestroyNotifyMask: Final = 0x2
+XFixesSelectionClientCloseNotifyMask: Final = 0x4
+XFixesDisplayCursorNotifyMask: Final = 0x1
+XFixesSetSelectionOwnerNotify: Final = 0
+XFixesSelectionWindowDestroyNotify: Final = 1
+XFixesSelectionClientCloseNotify: Final = 2
+XFixesDisplayCursorNotify: Final = 0
 
 class QueryVersion(rq.ReplyRequest): ...
 
 def query_version(self: Display | resource.Resource) -> QueryVersion: ...
 
 class HideCursor(rq.Request): ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/ext/xinerama.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/ext/xinerama.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from typing_extensions import Final
+
 from Xlib._typing import Unused
 from Xlib.display import Display
 from Xlib.protocol import rq
 from Xlib.xobject import drawable, resource
 
-extname: str
+extname: Final = "XINERAMA"
 
 class QueryVersion(rq.ReplyRequest): ...
 
 def query_version(self: Display | resource.Resource) -> QueryVersion: ...
 
 class GetState(rq.ReplyRequest): ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/ext/xtest.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/ext/xtest.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,28 @@
+from typing_extensions import Final
+
 from Xlib._typing import Unused
 from Xlib.display import Display
 from Xlib.protocol import rq
 from Xlib.xobject import resource
 
-extname: str
-CurrentCursor: int
+extname: Final = "XTEST"
+CurrentCursor: Final = 1
 
 class GetVersion(rq.ReplyRequest): ...
 
 def get_version(self: Display | resource.Resource, major: int, minor: int) -> GetVersion: ...
 
 class CompareCursor(rq.ReplyRequest): ...
 
 def compare_cursor(self: Display | resource.Resource, cursor: int) -> int: ...
 
 class FakeInput(rq.Request): ...
 
 def fake_input(
-    self: Display | resource.Resource,
-    event_type: int,
-    detail: int = ...,
-    time: int = ...,
-    root: int = ...,
-    x: int = ...,
-    y: int = ...,
+    self: Display | resource.Resource, event_type: int, detail: int = 0, time: int = 0, root: int = 0, x: int = 0, y: int = 0
 ) -> None: ...
 
 class GrabControl(rq.Request): ...
 
 def grab_control(self: Display | resource.Resource, impervious: bool) -> None: ...
 def init(disp: Display, info: Unused) -> None: ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/keysymdef/__init__.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/keysymdef/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/protocol/display.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/protocol/display.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 _T = TypeVar("_T")
 
 class bytesview:
     view: memoryview
     @overload
     def __init__(self, data: bytes | bytesview, offset: int, size: int) -> None: ...
     @overload
-    def __init__(self, data: _BufferWithLen, offset: int = ..., size: int | None = ...) -> None: ...
+    def __init__(self, data: _BufferWithLen, offset: int = 0, size: int | None = None) -> None: ...
     @overload
     def __getitem__(self, key: slice) -> bytes: ...
     @overload
     def __getitem__(self, key: int) -> int: ...
     def __len__(self) -> int: ...
 
 class Display:
@@ -55,55 +55,55 @@
     data_sent_bytes: int
     resource_id_lock: lock._DummyLock
     resource_ids: dict[int, None]
     last_resource_id: int
     error_handler: ErrorHandler[object] | None
     big_endian: bool
     info: ConnectionSetupRequest
-    def __init__(self, display: str | None = ...) -> None: ...
+    def __init__(self, display: str | None = None) -> None: ...
     def get_display_name(self) -> str: ...
     def get_default_screen(self) -> int: ...
     def fileno(self) -> int: ...
     def next_event(self) -> rq.Event: ...
     def pending_events(self) -> int: ...
     def flush(self) -> None: ...
     def close(self) -> None: ...
     def set_error_handler(self, handler: ErrorHandler[object] | None) -> None: ...
     def allocate_resource_id(self) -> int: ...
     def free_resource_id(self, rid: int) -> None: ...
     @overload
-    def get_resource_class(self, class_name: Literal["resource"], default: object = ...) -> type[resource.Resource]: ...
+    def get_resource_class(self, class_name: Literal["resource"], default: object = None) -> type[resource.Resource]: ...
     @overload
-    def get_resource_class(self, class_name: Literal["drawable"], default: object = ...) -> type[drawable.Drawable]: ...
+    def get_resource_class(self, class_name: Literal["drawable"], default: object = None) -> type[drawable.Drawable]: ...
     @overload
-    def get_resource_class(self, class_name: Literal["window"], default: object = ...) -> type[drawable.Window]: ...
+    def get_resource_class(self, class_name: Literal["window"], default: object = None) -> type[drawable.Window]: ...
     @overload
-    def get_resource_class(self, class_name: Literal["pixmap"], default: object = ...) -> type[drawable.Pixmap]: ...
+    def get_resource_class(self, class_name: Literal["pixmap"], default: object = None) -> type[drawable.Pixmap]: ...
     @overload
-    def get_resource_class(self, class_name: Literal["fontable"], default: object = ...) -> type[fontable.Fontable]: ...
+    def get_resource_class(self, class_name: Literal["fontable"], default: object = None) -> type[fontable.Fontable]: ...
     @overload
-    def get_resource_class(self, class_name: Literal["font"], default: object = ...) -> type[fontable.Font]: ...
+    def get_resource_class(self, class_name: Literal["font"], default: object = None) -> type[fontable.Font]: ...
     @overload
-    def get_resource_class(self, class_name: Literal["gc"], default: object = ...) -> type[fontable.GC]: ...
+    def get_resource_class(self, class_name: Literal["gc"], default: object = None) -> type[fontable.GC]: ...
     @overload
-    def get_resource_class(self, class_name: Literal["colormap"], default: object = ...) -> type[colormap.Colormap]: ...
+    def get_resource_class(self, class_name: Literal["colormap"], default: object = None) -> type[colormap.Colormap]: ...
     @overload
     def get_resource_class(self, class_name: Literal["cursor"], default: object) -> type[cursor.Cursor]: ...
     @overload
     def get_resource_class(self, class_name: str, default: _T) -> type[_ResourceBaseClass] | _T: ...
     @overload
-    def get_resource_class(self, class_name: str, default: None = ...) -> type[_ResourceBaseClass] | None: ...
+    def get_resource_class(self, class_name: str, default: None = None) -> type[_ResourceBaseClass] | None: ...
     def set_extension_major(self, extname: str, major: int) -> None: ...
     def get_extension_major(self, extname: str) -> int: ...
-    def add_extension_event(self, code: int, evt: type[rq.Event], subcode: int | None = ...) -> None: ...
+    def add_extension_event(self, code: int, evt: type[rq.Event], subcode: int | None = None) -> None: ...
     def add_extension_error(self, code: int, err: type[error.XError]) -> None: ...
     def check_for_error(self) -> None: ...
     def send_request(self, request: rq.Request | rq.ReplyRequest | ConnectionSetupRequest, wait_for_response: bool) -> None: ...
     def close_internal(self, whom: object) -> None: ...
-    def send_and_recv(self, flush: bool = ..., event: bool = ..., request: int | None = ..., recv: bool = ...) -> None: ...
+    def send_and_recv(self, flush: bool = False, event: bool = False, request: int | None = None, recv: bool = False) -> None: ...
     def parse_response(self, request: int) -> bool: ...
     def parse_error_response(self, request: int) -> bool: ...
     def default_error_handler(self, err: object) -> None: ...
     def parse_request_response(self, request: int) -> bool: ...
     def parse_event_response(self, etype: int) -> None: ...
     def get_waiting_request(self, sno: int) -> rq.ReplyRequest | ConnectionSetupRequest | None: ...
     def get_waiting_replyrequest(self) -> rq.ReplyRequest | ConnectionSetupRequest: ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/protocol/event.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/protocol/event.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing_extensions import TypeAlias
+from typing_extensions import Final, TypeAlias
 
 from Xlib.protocol import rq
 
 class AnyEvent(rq.Event): ...
 class KeyButtonPointer(rq.Event): ...
 class KeyPress(KeyButtonPointer): ...
 class KeyRelease(KeyButtonPointer): ...
@@ -73,8 +73,8 @@
     | type[SelectionClear]
     | type[SelectionRequest]
     | type[SelectionNotify]
     | type[ColormapNotify]
     | type[ClientMessage]
     | type[MappingNotify],
 ]
-event_class: _EventClass
+event_class: Final[_EventClass]
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/protocol/request.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/protocol/request.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import NoReturn
+from typing_extensions import Final
 
 from Xlib import display
 from Xlib.protocol import rq
 
 class CreateWindow(rq.Request): ...
 class ChangeWindowAttributes(rq.Request): ...
 class GetWindowAttributes(rq.ReplyRequest): ...
@@ -50,15 +51,15 @@
 class OpenFont(rq.Request): ...
 class CloseFont(rq.Request): ...
 class QueryFont(rq.ReplyRequest): ...
 class QueryTextExtents(rq.ReplyRequest): ...
 class ListFonts(rq.ReplyRequest): ...
 
 class ListFontsWithInfo(rq.ReplyRequest):
-    def __init__(self, display: display.Display, defer: bool = ..., *args: object, **keys: object) -> None: ...
+    def __init__(self, display: display.Display, defer: bool = False, *args: object, **keys: object) -> None: ...
     def __getattr__(self, attr: object) -> NoReturn: ...
     def __getitem__(self, item: str) -> object: ...
     def __len__(self) -> int: ...
 
 class SetFontPath(rq.Request): ...
 class GetFontPath(rq.ReplyRequest): ...
 class CreatePixmap(rq.Request): ...
@@ -126,8 +127,8 @@
 class ForceScreenSaver(rq.Request): ...
 class SetPointerMapping(rq.ReplyRequest): ...
 class GetPointerMapping(rq.ReplyRequest): ...
 class SetModifierMapping(rq.ReplyRequest): ...
 class GetModifierMapping(rq.ReplyRequest): ...
 class NoOperation(rq.Request): ...
 
-major_codes: dict[int, type[rq.Request]]
+major_codes: Final[dict[int, type[rq.Request]]]
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/protocol/rq.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/protocol/rq.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 from _typeshed import ReadableBuffer, SliceableBuffer, SupportsTrunc
 from array import array
 
 # Avoid name collision with List.type
 from builtins import type as Type
 from collections.abc import Callable, Iterable, Sequence
 from typing import Any, SupportsInt, TypeVar, overload, type_check_only
-from typing_extensions import Literal, LiteralString, SupportsIndex, TypeAlias
+from typing_extensions import Final, Literal, LiteralString, SupportsIndex, TypeAlias
 
 from Xlib._typing import ErrorHandler, Unused
-from Xlib.display import _ResourceBaseClass
+from Xlib.display import _BaseDisplay, _ResourceBaseClass
 from Xlib.error import XError
 from Xlib.ext.xinput import ClassInfoClass
 from Xlib.protocol import display
 
 _T = TypeVar("_T")
 _IntNew: TypeAlias = str | ReadableBuffer | SupportsInt | SupportsIndex | SupportsTrunc
 _ModifierMappingList8Elements: TypeAlias = Sequence[Sequence[int]]
 
-# Workaround for pytype crash. Should be Xlib.display._BaseDisplay
-@type_check_only
-class _BaseDisplay(display.Display):
-    def __init__(self, display: str | None = ...) -> None: ...
-    def get_atom(self, atomname: str, only_if_exists: bool = ...) -> int: ...
-
 def decode_string(bs: bytes | bytearray) -> str: ...
 def encode_array(a: array[Any] | memoryview) -> str: ...
 
 class BadDataError(Exception): ...
 
-signed_codes: dict[int, str]
-unsigned_codes: dict[int, str]
-array_unsigned_codes: dict[int, LiteralString]
-struct_to_array_codes: dict[str, LiteralString]
-size: int
+signed_codes: Final[dict[int, str]]
+unsigned_codes: Final[dict[int, str]]
+array_unsigned_codes: Final[dict[int, LiteralString]]
+struct_to_array_codes: Final[dict[str, LiteralString]]
 
 class Field:
     name: str
     default: int | None
     pack_value: Callable[[Any], tuple[Any, int | None, int | None]] | None
     structcode: str | None
     structvalues: int
@@ -86,15 +79,15 @@
 class FormatField(Field):
     structcode: str
     def __init__(self, name: str, size: int) -> None: ...
 
 Format = FormatField
 
 class ValueField(Field):
-    def __init__(self, name: str, default: int | None = ...) -> None: ...
+    def __init__(self, name: str, default: int | None = None) -> None: ...
 
 class Int8(ValueField):
     structcode: str
 
 class Int16(ValueField):
     structcode: str
 
@@ -110,15 +103,15 @@
 class Card32(ValueField):
     structcode: str
 
 class Resource(Card32):
     cast_function: str
     class_name: str
     codes: tuple[int, ...]
-    def __init__(self, name: str, codes: tuple[int, ...] = ..., default: int | None = ...) -> None: ...
+    def __init__(self, name: str, codes: tuple[int, ...] = ..., default: int | None = None) -> None: ...
     @overload  # type: ignore[override]
     def check_value(self, value: Callable[[], _T]) -> _T: ...
     @overload
     def check_value(self, value: _T) -> _T: ...
     def parse_value(self, value: int, display: _BaseDisplay) -> int: ...  # type: ignore[override]  # display: None will error. See: https://github.com/python-xlib/python-xlib/pull/248
 
 class Window(Resource):
@@ -156,86 +149,86 @@
 class Bool(ValueField):
     structcode: str
     def check_value(self, value: object) -> bool: ...  # type: ignore[override]
 
 class Set(ValueField):
     structcode: str
     values: Sequence[object]
-    def __init__(self, name: str, size: int, values: Sequence[object], default: int | None = ...) -> None: ...
+    def __init__(self, name: str, size: int, values: Sequence[object], default: int | None = None) -> None: ...
     def check_value(self, val: _T) -> _T: ...  # type: ignore[override]
 
 class Gravity(Set):
     def __init__(self, name: str) -> None: ...
 
 class FixedBinary(ValueField):
     structcode: str
     def __init__(self, name: str, size: int) -> None: ...
 
 class Binary(ValueField):
     structcode: None
     pad: int
-    def __init__(self, name: str, pad: int = ...) -> None: ...
+    def __init__(self, name: str, pad: int = 1) -> None: ...
     def pack_value(  # type: ignore[override]  # Override Callable
         self, val: bytes | bytearray
     ) -> tuple[bytes | bytearray, int, None]: ...
     @overload  # type: ignore[override]  # Overload for specific values
     def parse_binary_value(self, data: _T, display: Unused, length: None, format: Unused) -> tuple[_T, Literal[b""]]: ...
     @overload
     def parse_binary_value(
         self, data: SliceableBuffer, display: Unused, length: int, format: Unused
     ) -> tuple[SliceableBuffer, SliceableBuffer]: ...
 
 class String8(ValueField):
     structcode: None
     pad: int
-    def __init__(self, name: str, pad: int = ...) -> None: ...
+    def __init__(self, name: str, pad: int = 1) -> None: ...
     def pack_value(self, val: bytes | str) -> tuple[bytes, int, None]: ...  # type: ignore[override]  # Override Callable
     @overload  # type: ignore[override]  # Overload for specific values
     def parse_binary_value(
         self, data: bytes | bytearray, display: Unused, length: None, format: Unused
     ) -> tuple[str, Literal[b""]]: ...
     @overload
     def parse_binary_value(
         self, data: SliceableBuffer, display: Unused, length: int, format: Unused
     ) -> tuple[str, SliceableBuffer]: ...
 
 class String16(ValueField):
     structcode: None
     pad: int
-    def __init__(self, name: str, pad: int = ...) -> None: ...
+    def __init__(self, name: str, pad: int = 1) -> None: ...
     def pack_value(self, val: Sequence[object]) -> tuple[bytes, int, None]: ...  # type: ignore[override]  # Override Callable
     def parse_binary_value(  # type: ignore[override]  # length: None will error. See: https://github.com/python-xlib/python-xlib/pull/248
         self, data: SliceableBuffer, display: Unused, length: int | Literal["odd", "even"], format: Unused
     ) -> tuple[tuple[Any, ...], SliceableBuffer]: ...
 
 class List(ValueField):
     structcode: None
     type: Struct | ScalarObj | ResourceObj | ClassInfoClass | type[ValueField]
     pad: int
     def __init__(
-        self, name: str, type: Struct | ScalarObj | ResourceObj | ClassInfoClass | Type[ValueField], pad: int = ...
+        self, name: str, type: Struct | ScalarObj | ResourceObj | ClassInfoClass | Type[ValueField], pad: int = 1
     ) -> None: ...
     def parse_binary_value(
         self, data: SliceableBuffer, display: display.Display | None, length: SupportsIndex | None, format: Unused
     ) -> tuple[list[DictWrapper | None], SliceableBuffer]: ...
     def pack_value(  # type: ignore[override]  # Override Callable
         self, val: Sequence[object] | dict[str, Any]
     ) -> tuple[bytes, int, None]: ...
 
 class FixedList(List):
     size: int
-    def __init__(self, name: str, size: int, type: Struct | ScalarObj, pad: int = ...) -> None: ...
+    def __init__(self, name: str, size: int, type: Struct | ScalarObj, pad: int = 1) -> None: ...
     def parse_binary_value(
         self, data: SliceableBuffer, display: display.Display | None, length: Unused, format: Unused
     ) -> tuple[list[DictWrapper | None], SliceableBuffer]: ...
 
 class Object(ValueField):
     type: Struct
     structcode: str | None
-    def __init__(self, name: str, type: Struct, default: int | None = ...) -> None: ...
+    def __init__(self, name: str, type: Struct, default: int | None = None) -> None: ...
     def parse_binary_value(
         self, data: SliceableBuffer, display: display.Display | None, length: Unused, format: Unused
     ) -> tuple[DictWrapper, SliceableBuffer]: ...
     def parse_value(self, val: SliceableBuffer, display: display.Display | None) -> DictWrapper: ...  # type: ignore[override]
     def pack_value(  # type: ignore[override]  # Override Callable
         self, val: tuple[object, ...] | dict[str, Any] | DictWrapper
     ) -> bytes: ...
@@ -338,23 +331,23 @@
     def __init__(self, *fields: Field) -> None: ...
     def to_binary(self, *varargs: object, **keys: object) -> bytes: ...
     def pack_value(self, value: tuple[object, ...] | dict[str, Any] | DictWrapper) -> bytes: ...
     @overload
     def parse_value(self, val: SliceableBuffer, display: display.Display | None, rawdict: Literal[True]) -> dict[str, Any]: ...
     @overload
     def parse_value(
-        self, val: SliceableBuffer, display: display.Display | None, rawdict: Literal[False] = ...
+        self, val: SliceableBuffer, display: display.Display | None, rawdict: Literal[False] = False
     ) -> DictWrapper: ...
     @overload
     def parse_binary(
         self, data: SliceableBuffer, display: display.Display | None, rawdict: Literal[True]
     ) -> tuple[dict[str, Any], SliceableBuffer]: ...
     @overload
     def parse_binary(
-        self, data: SliceableBuffer, display: display.Display | None, rawdict: Literal[False] = ...
+        self, data: SliceableBuffer, display: display.Display | None, rawdict: Literal[False] = False
     ) -> tuple[DictWrapper, SliceableBuffer]: ...
     # Structs generate their attributes
     # TODO: Create a specific type-only class for all instances of `Struct`
     @type_check_only
     def __getattr__(self, __name: str) -> Any: ...
 
 class TextElements8(ValueField):
@@ -381,22 +374,22 @@
     def __getitem__(self, key: str) -> object: ...
     def __setitem__(self, key: str, value: object) -> None: ...
     def __delitem__(self, key: str) -> None: ...
     def __setattr__(self, key: str, value: object) -> None: ...
 
 class Request:
     def __init__(
-        self, display: _BaseDisplay, onerror: ErrorHandler[object] | None = ..., *args: object, **keys: object
+        self, display: _BaseDisplay, onerror: ErrorHandler[object] | None = None, *args: object, **keys: object
     ) -> None: ...
 
 class ReplyRequest(GetAttrData):
-    def __init__(self, display: display.Display, defer: int = ..., *args: object, **keys: object) -> None: ...
+    def __init__(self, display: display.Display, defer: int = False, *args: object, **keys: object) -> None: ...
     def reply(self) -> None: ...
 
 class Event(GetAttrData):
     def __init__(
-        self, binarydata: SliceableBuffer | None = ..., display: display.Display | None = ..., **keys: object
+        self, binarydata: SliceableBuffer | None = None, display: display.Display | None = None, **keys: object
     ) -> None: ...
 
 def call_error_handler(
     handler: Callable[[XError, Request | None], _T], error: XError, request: Request | None
 ) -> _T | Literal[0]: ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/protocol/structs.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/protocol/structs.pyi`

 * *Files identical despite different names*

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/rdb.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/rdb.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 from _typeshed import SupportsDunderGT, SupportsDunderLT, SupportsRead
 from collections.abc import Iterable, Mapping, Sequence
 from re import Pattern
 from typing import Any, Protocol, TypeVar, overload
-from typing_extensions import TypeAlias
+from typing_extensions import Final, TypeAlias
 
 from Xlib.display import Display
 from Xlib.support.lock import _DummyLock
 
 _T = TypeVar("_T")
 _T_contra = TypeVar("_T_contra", contravariant=True)
 
 _DB: TypeAlias = dict[str, tuple[_DB, ...]]
 # A recursive type can be a bit annoying due to dict invariance,
 # so this is a slightly less precise version of the _DB alias for parameter annotations
 _DB_Param: TypeAlias = dict[str, Any]
 
 class _SupportsComparisons(SupportsDunderLT[_T_contra], SupportsDunderGT[_T_contra], Protocol[_T_contra]): ...
 
-comment_re: Pattern[str]
-resource_spec_re: Pattern[str]
-value_escape_re: Pattern[str]
-resource_parts_re: Pattern[str]
-NAME_MATCH: int
-CLASS_MATCH: int
-WILD_MATCH: int
-MATCH_SKIP: int
+comment_re: Final[Pattern[str]]
+resource_spec_re: Final[Pattern[str]]
+value_escape_re: Final[Pattern[str]]
+resource_parts_re: Final[Pattern[str]]
+NAME_MATCH: Final = 0
+CLASS_MATCH: Final = 2
+WILD_MATCH: Final = 4
+MATCH_SKIP: Final = 6
 
 class OptionError(Exception): ...
 
 class ResourceDB:
     db: _DB
     lock: _DummyLock
     def __init__(
         self,
-        file: bytes | SupportsRead[str] | None = ...,
-        string: str | None = ...,
-        resources: Iterable[tuple[str, object]] | None = ...,
+        file: bytes | SupportsRead[str] | None = None,
+        string: str | None = None,
+        resources: Iterable[tuple[str, object]] | None = None,
     ) -> None: ...
     def insert_file(self, file: bytes | SupportsRead[str]) -> None: ...
     def insert_string(self, data: str) -> None: ...
     def insert_resources(self, resources: Iterable[tuple[str, object]]) -> None: ...
     def insert(self, resource: str, value: object) -> None: ...
     def __getitem__(self, keys_tuple: tuple[str, str]) -> Any: ...
     @overload
-    def get(self, res: str, cls: str, default: None = ...) -> Any: ...
+    def get(self, res: str, cls: str, default: None = None) -> Any: ...
     @overload
     def get(self, res: str, cls: str, default: _T) -> _T: ...
     def update(self, db: ResourceDB) -> None: ...
     def output(self) -> str: ...
     def getopt(self, name: str, argv: Sequence[str], opts: Mapping[str, Option]) -> Sequence[str]: ...
 
 def bin_insert(list: list[_SupportsComparisons[_T]], element: _SupportsComparisons[_T]) -> None: ...
@@ -90,8 +90,8 @@
     count: int
     def __init__(self, count: int) -> None: ...
 
 def get_display_opts(
     options: Mapping[str, Option], argv: Sequence[str] = ...
 ) -> tuple[Display, str, ResourceDB, Sequence[str]]: ...
 
-stdopts: dict[str, SepArg | NoArg | ResArgClass]
+stdopts: Final[dict[str, SepArg | NoArg | ResArgClass]]
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/support/unix_connect.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/support/unix_connect.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import sys
 from _socket import _Address
 from platform import uname_result
 from re import Pattern
 from socket import socket
-from typing_extensions import Literal, TypeAlias
+from typing_extensions import Final, Literal, TypeAlias
 
 from Xlib._typing import Unused
 
 if sys.platform == "darwin":
-    SUPPORTED_PROTOCOLS: tuple[None, Literal["tcp"], Literal["unix"], Literal["darwin"]]
+    SUPPORTED_PROTOCOLS: Final[tuple[None, Literal["tcp"], Literal["unix"], Literal["darwin"]]]
     _Protocol: TypeAlias = Literal[None, "tcp", "unix", "darwin"]
-    DARWIN_DISPLAY_RE: Pattern[str]
+    DARWIN_DISPLAY_RE: Final[Pattern[str]]
 else:
-    SUPPORTED_PROTOCOLS: tuple[None, Literal["tcp"], Literal["unix"]]
+    SUPPORTED_PROTOCOLS: Final[tuple[None, Literal["tcp"], Literal["unix"]]]
     _Protocol: TypeAlias = Literal[None, "tcp", "unix"]
 uname: uname_result
-DISPLAY_RE: Pattern[str]
+DISPLAY_RE: Final[Pattern[str]]
 
 def get_display(display: str | None) -> tuple[str, str | None, str | None, int, int]: ...
 def get_socket(dname: _Address, protocol: _Protocol, host: _Address | None, dno: int) -> socket: ...
 def new_get_auth(sock: socket, dname: Unused, protocol: _Protocol, host: Unused, dno: int) -> tuple[bytes, bytes]: ...
 def old_get_auth(sock: Unused, dname: _Address, host: Unused, dno: Unused) -> tuple[str | Literal[b""], bytes]: ...
 
 get_auth = new_get_auth
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/xobject/colormap.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/xobject/colormap.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from collections.abc import Sequence
 from re import Pattern
+from typing_extensions import Final
 
 from Xlib._typing import ErrorHandler
 from Xlib.protocol import request, rq
 from Xlib.xobject import resource
 
-rgb_res: list[Pattern[str]]
+rgb_res: Final[list[Pattern[str]]]
 
 class Colormap(resource.Resource):
     __colormap__ = resource.Resource.__resource__
-    def free(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def free(self, onerror: ErrorHandler[object] | None = None) -> None: ...
     def copy_colormap_and_free(self, scr_cmap: int) -> Colormap: ...
-    def install_colormap(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def uninstall_colormap(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def install_colormap(self, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def uninstall_colormap(self, onerror: ErrorHandler[object] | None = None) -> None: ...
     def alloc_color(self, red: int, green: int, blue: int) -> request.AllocColor: ...
     def alloc_named_color(self, name: str) -> request.AllocColor | request.AllocNamedColor | None: ...
     def alloc_color_cells(self, contiguous: bool, colors: int, planes: int) -> request.AllocColorCells: ...
     def alloc_color_planes(self, contiguous: bool, colors: int, red: int, green: int, blue: int) -> request.AllocColorPlanes: ...
-    def free_colors(self, pixels: Sequence[int], plane_mask: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def store_colors(self, items: dict[str, int], onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def store_named_color(self, name: str, pixel: int, flags: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def free_colors(self, pixels: Sequence[int], plane_mask: int, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def store_colors(self, items: dict[str, int], onerror: ErrorHandler[object] | None = None) -> None: ...
+    def store_named_color(self, name: str, pixel: int, flags: int, onerror: ErrorHandler[object] | None = None) -> None: ...
     def query_colors(self, pixels: Sequence[int]) -> rq.Struct: ...
     def lookup_color(self, name: str) -> request.LookupColor: ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/xobject/drawable.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/xobject/drawable.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -18,246 +18,248 @@
         src_drawable: int,
         src_x: int,
         src_y: int,
         width: int,
         height: int,
         dst_x: int,
         dst_y: int,
-        onerror: ErrorHandler[object] | None = ...,
+        onerror: ErrorHandler[object] | None = None,
     ) -> None: ...
     def copy_plane(
         self,
         gc: int,
         src_drawable: int,
         src_x: int,
         src_y: int,
         width: int,
         height: int,
         dst_x: int,
         dst_y: int,
         bit_plane: int,
-        onerror: ErrorHandler[object] | None = ...,
+        onerror: ErrorHandler[object] | None = None,
     ) -> None: ...
     def poly_point(
-        self, gc: int, coord_mode: int, points: Sequence[tuple[int, int]], onerror: ErrorHandler[object] | None = ...
+        self, gc: int, coord_mode: int, points: Sequence[tuple[int, int]], onerror: ErrorHandler[object] | None = None
     ) -> None: ...
-    def point(self, gc: int, x: int, y: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def point(self, gc: int, x: int, y: int, onerror: ErrorHandler[object] | None = None) -> None: ...
     def poly_line(
-        self, gc: int, coord_mode: int, points: Sequence[tuple[int, int]], onerror: ErrorHandler[object] | None = ...
+        self, gc: int, coord_mode: int, points: Sequence[tuple[int, int]], onerror: ErrorHandler[object] | None = None
     ) -> None: ...
-    def line(self, gc: int, x1: int, y1: int, x2: int, y2: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def line(self, gc: int, x1: int, y1: int, x2: int, y2: int, onerror: ErrorHandler[object] | None = None) -> None: ...
     def poly_segment(
-        self, gc: int, segments: Sequence[_Segment4IntSequence], onerror: ErrorHandler[object] | None = ...
+        self, gc: int, segments: Sequence[_Segment4IntSequence], onerror: ErrorHandler[object] | None = None
     ) -> None: ...
     def poly_rectangle(
-        self, gc: int, rectangles: Sequence[_Rectangle4IntSequence], onerror: ErrorHandler[object] | None = ...
+        self, gc: int, rectangles: Sequence[_Rectangle4IntSequence], onerror: ErrorHandler[object] | None = None
     ) -> None: ...
-    def rectangle(self, gc: int, x: int, y: int, width: int, height: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def poly_arc(self, gc: int, arcs: Sequence[_Arc6IntSequence], onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def rectangle(
+        self, gc: int, x: int, y: int, width: int, height: int, onerror: ErrorHandler[object] | None = None
+    ) -> None: ...
+    def poly_arc(self, gc: int, arcs: Sequence[_Arc6IntSequence], onerror: ErrorHandler[object] | None = None) -> None: ...
     def arc(
         self,
         gc: int,
         x: int,
         y: int,
         width: int,
         height: int,
         angle1: int,
         angle2: int,
-        onerror: ErrorHandler[object] | None = ...,
+        onerror: ErrorHandler[object] | None = None,
     ) -> None: ...
     def fill_poly(
-        self, gc: int, shape: int, coord_mode: int, points: Sequence[tuple[int, int]], onerror: ErrorHandler[object] | None = ...
+        self, gc: int, shape: int, coord_mode: int, points: Sequence[tuple[int, int]], onerror: ErrorHandler[object] | None = None
     ) -> None: ...
     def poly_fill_rectangle(
-        self, gc: int, rectangles: Sequence[_Rectangle4IntSequence], onerror: ErrorHandler[object] | None = ...
+        self, gc: int, rectangles: Sequence[_Rectangle4IntSequence], onerror: ErrorHandler[object] | None = None
     ) -> None: ...
     def fill_rectangle(
-        self, gc: int, x: int, y: int, width: int, height: int, onerror: ErrorHandler[object] | None = ...
+        self, gc: int, x: int, y: int, width: int, height: int, onerror: ErrorHandler[object] | None = None
     ) -> None: ...
-    def poly_fill_arc(self, gc: int, arcs: Sequence[_Arc6IntSequence], onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def poly_fill_arc(self, gc: int, arcs: Sequence[_Arc6IntSequence], onerror: ErrorHandler[object] | None = None) -> None: ...
     def fill_arc(
         self,
         gc: int,
         x: int,
         y: int,
         width: int,
         height: int,
         angle1: int,
         angle2: int,
-        onerror: ErrorHandler[object] | None = ...,
+        onerror: ErrorHandler[object] | None = None,
     ) -> None: ...
     def put_image(
         self,
         gc: int,
         x: int,
         y: int,
         width: int,
         height: int,
         format: int,
         depth: int,
         left_pad: int,
         data: bytes | bytearray,
-        onerror: ErrorHandler[object] | None = ...,
+        onerror: ErrorHandler[object] | None = None,
     ) -> None: ...
-    def put_pil_image(self, gc: int, x: int, y: int, image: Image.Image, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def put_pil_image(self, gc: int, x: int, y: int, image: Image.Image, onerror: ErrorHandler[object] | None = None) -> None: ...
     def get_image(self, x: int, y: int, width: int, height: int, format: int, plane_mask: int) -> request.GetImage: ...
     def draw_text(
-        self, gc: int, x: int, y: int, text: dict[str, str | int], onerror: ErrorHandler[object] | None = ...
+        self, gc: int, x: int, y: int, text: dict[str, str | int], onerror: ErrorHandler[object] | None = None
     ) -> None: ...
     def poly_text(
-        self, gc: int, x: int, y: int, items: Sequence[dict[str, str | int]], onerror: ErrorHandler[object] | None = ...
+        self, gc: int, x: int, y: int, items: Sequence[dict[str, str | int]], onerror: ErrorHandler[object] | None = None
     ) -> None: ...
     def poly_text_16(
-        self, gc: int, x: int, y: int, items: Sequence[dict[str, str | int]], onerror: ErrorHandler[object] | None = ...
+        self, gc: int, x: int, y: int, items: Sequence[dict[str, str | int]], onerror: ErrorHandler[object] | None = None
     ) -> None: ...
-    def image_text(self, gc: int, x: int, y: int, string: str, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def image_text_16(self, gc: int, x: int, y: int, string: str, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def image_text(self, gc: int, x: int, y: int, string: str, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def image_text_16(self, gc: int, x: int, y: int, string: str, onerror: ErrorHandler[object] | None = None) -> None: ...
     def query_best_size(self, item_class: int, width: int, height: int) -> request.QueryBestSize: ...
 
 class Window(Drawable):
     __window__ = resource.Resource.__resource__
     def create_window(
         self,
         x: int,
         y: int,
         width: int,
         height: int,
         border_width: int,
         depth: int,
-        window_class: int = ...,
-        visual: int = ...,
-        onerror: ErrorHandler[object] | None = ...,
+        window_class: int = 0,
+        visual: int = 0,
+        onerror: ErrorHandler[object] | None = None,
         **keys: object,
     ) -> Window: ...
-    def change_attributes(self, onerror: ErrorHandler[object] | None = ..., **keys: object) -> None: ...
+    def change_attributes(self, onerror: ErrorHandler[object] | None = None, **keys: object) -> None: ...
     def get_attributes(self) -> request.GetWindowAttributes: ...
-    def destroy(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def destroy_sub_windows(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def change_save_set(self, mode: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def reparent(self, parent: int, x: int, y: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def map(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def map_sub_windows(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def unmap(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def unmap_sub_windows(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def configure(self, onerror: ErrorHandler[object] | None = ..., **keys: object) -> None: ...
-    def circulate(self, direction: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def raise_window(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def destroy(self, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def destroy_sub_windows(self, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def change_save_set(self, mode: int, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def reparent(self, parent: int, x: int, y: int, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def map(self, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def map_sub_windows(self, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def unmap(self, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def unmap_sub_windows(self, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def configure(self, onerror: ErrorHandler[object] | None = None, **keys: object) -> None: ...
+    def circulate(self, direction: int, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def raise_window(self, onerror: ErrorHandler[object] | None = None) -> None: ...
     def query_tree(self) -> request.QueryTree: ...
     def change_property(
         self,
         property: int,
         property_type: int,
         format: int,
         data: Sequence[float] | Sequence[str],
-        mode: int = ...,
-        onerror: ErrorHandler[object] | None = ...,
+        mode: int = 0,
+        onerror: ErrorHandler[object] | None = None,
     ) -> None: ...
     def change_text_property(
-        self, property: int, property_type: int, data: bytes | str, mode: int = ..., onerror: ErrorHandler[object] | None = ...
+        self, property: int, property_type: int, data: bytes | str, mode: int = 0, onerror: ErrorHandler[object] | None = None
     ) -> None: ...
-    def delete_property(self, property: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def delete_property(self, property: int, onerror: ErrorHandler[object] | None = None) -> None: ...
     def get_property(
-        self, property: int, property_type: int, offset: int, length: int, delete: bool = ...
+        self, property: int, property_type: int, offset: int, length: int, delete: bool = False
     ) -> request.GetProperty | None: ...
-    def get_full_property(self, property: int, property_type: int, sizehint: int = ...) -> request.GetProperty | None: ...
-    def get_full_text_property(self, property: int, property_type: int = ..., sizehint: int = ...) -> str | None: ...
+    def get_full_property(self, property: int, property_type: int, sizehint: int = 10) -> request.GetProperty | None: ...
+    def get_full_text_property(self, property: int, property_type: int = 0, sizehint: int = 10) -> str | None: ...
     def list_properties(self) -> list[int]: ...
-    def set_selection_owner(self, selection: int, time: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def set_selection_owner(self, selection: int, time: int, onerror: ErrorHandler[object] | None = None) -> None: ...
     def convert_selection(
-        self, selection: int, target: int, property: int, time: int, onerror: ErrorHandler[object] | None = ...
+        self, selection: int, target: int, property: int, time: int, onerror: ErrorHandler[object] | None = None
     ) -> None: ...
     def send_event(
-        self, event: rq.Event, event_mask: int = ..., propagate: bool = ..., onerror: ErrorHandler[object] | None = ...
+        self, event: rq.Event, event_mask: int = 0, propagate: bool = False, onerror: ErrorHandler[object] | None = None
     ) -> None: ...
     def grab_pointer(
         self, owner_events: bool, event_mask: int, pointer_mode: int, keyboard_mode: int, confine_to: int, cursor: int, time: int
     ) -> int: ...
     def grab_button(
         self,
         button: int,
         modifiers: int,
         owner_events: bool,
         event_mask: int,
         pointer_mode: int,
         keyboard_mode: int,
         confine_to: int,
         cursor: int,
-        onerror: ErrorHandler[object] | None = ...,
+        onerror: ErrorHandler[object] | None = None,
     ) -> None: ...
-    def ungrab_button(self, button: int, modifiers: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def ungrab_button(self, button: int, modifiers: int, onerror: ErrorHandler[object] | None = None) -> None: ...
     def grab_keyboard(self, owner_events: bool, pointer_mode: int, keyboard_mode: int, time: int) -> int: ...
     def grab_key(
         self,
         key: int,
         modifiers: int,
         owner_events: bool,
         pointer_mode: int,
         keyboard_mode: int,
-        onerror: ErrorHandler[object] | None = ...,
+        onerror: ErrorHandler[object] | None = None,
     ) -> None: ...
-    def ungrab_key(self, key: int, modifiers: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def ungrab_key(self, key: int, modifiers: int, onerror: ErrorHandler[object] | None = None) -> None: ...
     def query_pointer(self) -> request.QueryPointer: ...
     def get_motion_events(self, start: int, stop: int) -> rq.Struct: ...
     def translate_coords(self, src_window: int, src_x: int, src_y: int) -> request.TranslateCoords: ...
     def warp_pointer(
         self,
         x: int,
         y: int,
-        src_window: int = ...,
-        src_x: int = ...,
-        src_y: int = ...,
-        src_width: int = ...,
-        src_height: int = ...,
-        onerror: ErrorHandler[object] | None = ...,
+        src_window: int = 0,
+        src_x: int = 0,
+        src_y: int = 0,
+        src_width: int = 0,
+        src_height: int = 0,
+        onerror: ErrorHandler[object] | None = None,
     ) -> None: ...
-    def set_input_focus(self, revert_to: int, time: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def set_input_focus(self, revert_to: int, time: int, onerror: ErrorHandler[object] | None = None) -> None: ...
     def clear_area(
         self,
-        x: int = ...,
-        y: int = ...,
-        width: int = ...,
-        height: int = ...,
-        exposures: bool = ...,
-        onerror: ErrorHandler[object] | None = ...,
+        x: int = 0,
+        y: int = 0,
+        width: int = 0,
+        height: int = 0,
+        exposures: bool = False,
+        onerror: ErrorHandler[object] | None = None,
     ) -> None: ...
     def create_colormap(self, visual: int, alloc: int) -> colormap.Colormap: ...
     def list_installed_colormaps(self) -> list[colormap.Colormap]: ...
-    def rotate_properties(self, properties: Sequence[int], delta: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def set_wm_name(self, name: bytes | str, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def rotate_properties(self, properties: Sequence[int], delta: int, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def set_wm_name(self, name: bytes | str, onerror: ErrorHandler[object] | None = None) -> None: ...
     def get_wm_name(self) -> str | None: ...
-    def set_wm_icon_name(self, name: bytes | str, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def set_wm_icon_name(self, name: bytes | str, onerror: ErrorHandler[object] | None = None) -> None: ...
     def get_wm_icon_name(self) -> str | None: ...
-    def set_wm_class(self, inst: str, cls: str, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def set_wm_class(self, inst: str, cls: str, onerror: ErrorHandler[object] | None = None) -> None: ...
     def get_wm_class(self) -> tuple[str, str] | None: ...
-    def set_wm_transient_for(self, window: Window, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def set_wm_transient_for(self, window: Window, onerror: ErrorHandler[object] | None = None) -> None: ...
     def get_wm_transient_for(self) -> Window | None: ...
-    def set_wm_protocols(self, protocols: Iterable[int], onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def set_wm_protocols(self, protocols: Iterable[int], onerror: ErrorHandler[object] | None = None) -> None: ...
     def get_wm_protocols(self) -> list[int]: ...
-    def set_wm_colormap_windows(self, windows: Iterable[Window], onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def set_wm_colormap_windows(self, windows: Iterable[Window], onerror: ErrorHandler[object] | None = None) -> None: ...
     def get_wm_colormap_windows(self) -> Iterable[Window]: ...
-    def set_wm_client_machine(self, name: bytes | str, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def set_wm_client_machine(self, name: bytes | str, onerror: ErrorHandler[object] | None = None) -> None: ...
     def get_wm_client_machine(self) -> str | None: ...
     def set_wm_normal_hints(
-        self, hints: rq.DictWrapper | dict[str, Any] = ..., onerror: ErrorHandler[object] | None = ..., **keys: object
+        self, hints: rq.DictWrapper | dict[str, Any] = ..., onerror: ErrorHandler[object] | None = None, **keys: object
     ) -> None: ...
     def get_wm_normal_hints(self) -> rq.DictWrapper | None: ...
     def set_wm_hints(
-        self, hints: rq.DictWrapper | dict[str, Any] = ..., onerror: ErrorHandler[object] | None = ..., **keys: object
+        self, hints: rq.DictWrapper | dict[str, Any] = ..., onerror: ErrorHandler[object] | None = None, **keys: object
     ) -> None: ...
     def get_wm_hints(self) -> rq.DictWrapper | None: ...
     def set_wm_state(
-        self, hints: rq.DictWrapper | dict[str, Any] = ..., onerror: ErrorHandler[object] | None = ..., **keys: object
+        self, hints: rq.DictWrapper | dict[str, Any] = ..., onerror: ErrorHandler[object] | None = None, **keys: object
     ) -> None: ...
     def get_wm_state(self) -> rq.DictWrapper | None: ...
     def set_wm_icon_size(
-        self, hints: rq.DictWrapper | dict[str, Any] = ..., onerror: ErrorHandler[object] | None = ..., **keys: object
+        self, hints: rq.DictWrapper | dict[str, Any] = ..., onerror: ErrorHandler[object] | None = None, **keys: object
     ) -> None: ...
     def get_wm_icon_size(self) -> rq.DictWrapper | None: ...
 
 class Pixmap(Drawable):
     __pixmap__ = resource.Resource.__resource__
-    def free(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def free(self, onerror: ErrorHandler[object] | None = None) -> None: ...
     def create_cursor(
         self, mask: int, foreground: _RGB3IntIterable, background: _RGB3IntIterable, x: int, y: int
     ) -> cursor.Cursor: ...
 
 def roundup(value: int, unit: int) -> int: ...
```

### Comparing `types-python-xlib-0.33.0.8/Xlib-stubs/xobject/fontable.pyi` & `types-python-xlib-0.33.0.9/Xlib-stubs/xobject/fontable.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 class Fontable(resource.Resource):
     __fontable__ = resource.Resource.__resource__
     def query(self) -> request.QueryFont: ...
     def query_text_extents(self, string: str) -> request.QueryTextExtents: ...
 
 class GC(Fontable):
     __gc__ = resource.Resource.__resource__
-    def change(self, onerror: ErrorHandler[object] | None = ..., **keys: object) -> None: ...
-    def copy(self, src_gc: int, mask: int, onerror: ErrorHandler[object] | None = ...) -> None: ...
-    def set_dashes(self, offset: int, dashes: Sequence[int], onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def change(self, onerror: ErrorHandler[object] | None = None, **keys: object) -> None: ...
+    def copy(self, src_gc: int, mask: int, onerror: ErrorHandler[object] | None = None) -> None: ...
+    def set_dashes(self, offset: int, dashes: Sequence[int], onerror: ErrorHandler[object] | None = None) -> None: ...
     def set_clip_rectangles(
         self,
         x_origin: int,
         y_origin: int,
         rectangles: Sequence[dict[str, int]],
         ordering: int,
-        onerror: ErrorHandler[object] | None = ...,
+        onerror: ErrorHandler[object] | None = None,
     ) -> None: ...
-    def free(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def free(self, onerror: ErrorHandler[object] | None = None) -> None: ...
 
 class Font(Fontable):
     __font__ = resource.Resource.__resource__
-    def close(self, onerror: ErrorHandler[object] | None = ...) -> None: ...
+    def close(self, onerror: ErrorHandler[object] | None = None) -> None: ...
     def create_glyph_cursor(
         self, mask: Font, source_char: int, mask_char: int, foreground: _RGB3IntIterable, background: _RGB3IntIterable
     ) -> cursor.Cursor: ...
```

### Comparing `types-python-xlib-0.33.0.8/setup.py` & `types-python-xlib-0.33.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-xlib`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-xlib. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4ca5ee98df5654d0db7f5b24cd2bd3b3fe54f313`.
+This package was generated from typeshed commit `d8e3f928b0e7dbaf3dafdb8fc5e257331532ae4c`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.33.0.8",
+      version="0.33.0.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-xlib.md",
```

### Comparing `types-python-xlib-0.33.0.8/types_python_xlib.egg-info/PKG-INFO` & `types-python-xlib-0.33.0.9/types_python_xlib.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-xlib
-Version: 0.33.0.8
+Version: 0.33.0.9
 Summary: Typing stubs for python-xlib
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-xlib.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-xlib`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-xlib. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4ca5ee98df5654d0db7f5b24cd2bd3b3fe54f313`.
+This package was generated from typeshed commit `d8e3f928b0e7dbaf3dafdb8fc5e257331532ae4c`.
```

### Comparing `types-python-xlib-0.33.0.8/types_python_xlib.egg-info/SOURCES.txt` & `types-python-xlib-0.33.0.9/types_python_xlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

