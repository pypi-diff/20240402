# Comparing `tmp/auto-editor-24.7.1.tar.gz` & `tmp/auto-editor-24.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-editor-24.7.1.tar", last modified: Fri Feb 16 00:54:59 2024, max compression
+gzip compressed data, was "auto-editor-24.9.1.tar", last modified: Thu Feb 29 19:19:54 2024, max compression
```

## Comparing `auto-editor-24.7.1.tar` & `auto-editor-24.9.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:59.887195 auto-editor-24.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-02-16 00:54:43.000000 auto-editor-24.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-02-16 00:54:59.887195 auto-editor-24.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-02-16 00:54:43.000000 auto-editor-24.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:59.875195 auto-editor-24.7.1/ae-ffmpeg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:59.879195 auto-editor-24.7.1/ae-ffmpeg/ae_ffmpeg/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-16 00:54:44.000000 auto-editor-24.7.1/ae-ffmpeg/ae_ffmpeg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:44.000000 auto-editor-24.7.1/ae-ffmpeg/ae_ffmpeg/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-02-16 00:54:44.000000 auto-editor-24.7.1/ae-ffmpeg/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:59.879195 auto-editor-24.7.1/auto_editor/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9827 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14489 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/ffwrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:59.883195 auto-editor-24.7.1/auto_editor/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/formats/fcp11.py
--rw-r--r--   0 runner    (1001) docker     (127)    17692 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/formats/fcp7.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/formats/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/formats/shotcut.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/formats/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8150 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:59.883195 auto-editor-24.7.1/auto_editor/lang/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/lang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/lang/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/lang/libmath.py
--rw-r--r--   0 runner    (1001) docker     (127)    56368 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/lang/palet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:59.883195 auto-editor-24.7.1/auto_editor/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/lib/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/lib/data_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/lib/err.py
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/make_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/preview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:59.883195 auto-editor-24.7.1/auto_editor/render/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/render/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/render/subtitle.py
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/render/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:59.883195 auto-editor-24.7.1/auto_editor/subcommands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/subcommands/desc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/subcommands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/subcommands/levels.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/subcommands/palet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/subcommands/repl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/subcommands/subdump.py
--rw-r--r--   0 runner    (1001) docker     (127)    24729 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/subcommands/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:59.887195 auto-editor-24.7.1/auto_editor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/utils/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/utils/chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/utils/cmdkw.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/utils/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/utils/func.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/validate_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     9902 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/vanparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-02-16 00:54:44.000000 auto-editor-24.7.1/auto_editor/wavfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 00:54:59.887195 auto-editor-24.7.1/auto_editor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-02-16 00:54:59.000000 auto-editor-24.7.1/auto_editor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-16 00:54:59.000000 auto-editor-24.7.1/auto_editor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 00:54:59.000000 auto-editor-24.7.1/auto_editor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-16 00:54:59.000000 auto-editor-24.7.1/auto_editor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-16 00:54:59.000000 auto-editor-24.7.1/auto_editor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-16 00:54:59.000000 auto-editor-24.7.1/auto_editor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-02-16 00:54:44.000000 auto-editor-24.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 00:54:59.887195 auto-editor-24.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:54.644699 auto-editor-24.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-02-29 19:19:38.000000 auto-editor-24.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-02-29 19:19:54.644699 auto-editor-24.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-02-29 19:19:38.000000 auto-editor-24.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:54.632699 auto-editor-24.9.1/ae-ffmpeg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:54.632699 auto-editor-24.9.1/ae-ffmpeg/ae_ffmpeg/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-29 19:19:38.000000 auto-editor-24.9.1/ae-ffmpeg/ae_ffmpeg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:38.000000 auto-editor-24.9.1/ae-ffmpeg/ae_ffmpeg/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-02-29 19:19:38.000000 auto-editor-24.9.1/ae-ffmpeg/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:54.636700 auto-editor-24.9.1/auto_editor/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9827 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8667 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/ffwrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:54.636700 auto-editor-24.9.1/auto_editor/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/formats/fcp11.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17757 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/formats/fcp7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/formats/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/formats/shotcut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/formats/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:54.640699 auto-editor-24.9.1/auto_editor/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/lang/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/lang/libmath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59027 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/lang/palet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:54.640699 auto-editor-24.9.1/auto_editor/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/lib/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/lib/data_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/lib/err.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/make_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/preview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:54.640699 auto-editor-24.9.1/auto_editor/render/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/render/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/render/subtitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/render/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:54.640699 auto-editor-24.9.1/auto_editor/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/subcommands/desc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/subcommands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/subcommands/levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/subcommands/palet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/subcommands/repl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/subcommands/subdump.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24823 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/subcommands/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:54.644699 auto-editor-24.9.1/auto_editor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/utils/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/utils/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/utils/cmdkw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/utils/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/utils/func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/validate_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9902 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/vanparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-02-29 19:19:38.000000 auto-editor-24.9.1/auto_editor/wavfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 19:19:54.644699 auto-editor-24.9.1/auto_editor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2024-02-29 19:19:54.000000 auto-editor-24.9.1/auto_editor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-29 19:19:54.000000 auto-editor-24.9.1/auto_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 19:19:54.000000 auto-editor-24.9.1/auto_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-29 19:19:54.000000 auto-editor-24.9.1/auto_editor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-29 19:19:54.000000 auto-editor-24.9.1/auto_editor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-29 19:19:54.000000 auto-editor-24.9.1/auto_editor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-02-29 19:19:38.000000 auto-editor-24.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 19:19:54.644699 auto-editor-24.9.1/setup.cfg
```

### Comparing `auto-editor-24.7.1/LICENSE` & `auto-editor-24.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/PKG-INFO` & `auto-editor-24.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-editor
-Version: 24.7.1
+Version: 24.9.1
 Summary: Auto-Editor: Effort free video editing!
 Author-email: WyattBlue <wyattblue@auto-editor.com>
 License: Unlicense
 Project-URL: Bug Tracker, https://github.com/WyattBlue/auto-editor/issues
 Project-URL: Source Code, https://github.com/WyattBlue/auto-editor
 Project-URL: homepage, https://auto-editor.com
 Keywords: video,audio,media,editor,editing,processing,nonlinear,automatic,silence-detect,silence-removal,silence-speedup,motion-detection
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auto-editor Version: 24.7.1 Summary: Auto-Editor:
+Metadata-Version: 2.1 Name: auto-editor Version: 24.9.1 Summary: Auto-Editor:
 Effort free video editing! Author-email: WyattBlue
 auto-editor.com> License: Unlicense Project-URL: Bug Tracker, https://
 github.com/WyattBlue/auto-editor/issues Project-URL: Source Code, https://
 github.com/WyattBlue/auto-editor Project-URL: homepage, https://auto-editor.com
 Keywords:
 video,audio,media,editor,editing,processing,nonlinear,automatic,silence-
 detect,silence-removal,silence-speedup,motion-detection Requires-Python: >=3.10
```

### Comparing `auto-editor-24.7.1/README.md` & `auto-editor-24.9.1/README.md`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/ae-ffmpeg/setup.py` & `auto-editor-24.9.1/ae-ffmpeg/setup.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/__main__.py` & `auto-editor-24.9.1/auto_editor/__main__.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/analyze.py` & `auto-editor-24.9.1/auto_editor/analyze.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,32 +17,28 @@
     is_threshold,
     is_void,
     orc,
 )
 from auto_editor.lib.data_structs import Sym
 from auto_editor.render.subtitle import SubtitleParser
 from auto_editor.utils.cmdkw import (
-    ParserError,
     Required,
-    parse_with_palet,
     pAttr,
     pAttrs,
 )
-from auto_editor.utils.func import boolop
 from auto_editor.wavfile import read
 
 if TYPE_CHECKING:
     from fractions import Fraction
     from typing import Any
 
     from av.filter import FilterContext
     from numpy.typing import NDArray
 
     from auto_editor.ffwrapper import FileInfo
-    from auto_editor.lib.data_structs import Env
     from auto_editor.output import Ensure
     from auto_editor.utils.bar import Bar
     from auto_editor.utils.log import Log
 
 
 audio_builder = pAttrs(
     "audio",
@@ -408,85 +404,7 @@
                 )
                 threshold_list[index] = np.count_nonzero(diff) / total_pixels
 
             prev_frame = current_frame
 
         self.bar.end()
         return self.cache("motion", mobj, threshold_list[:index])
-
-
-def edit_method(val: str, filesetup: FileSetup, env: Env) -> NDArray[np.bool_]:
-    assert isinstance(filesetup, FileSetup)
-    src = filesetup.src
-    tb = filesetup.tb
-    ensure = filesetup.ensure
-    strict = filesetup.strict
-    bar = filesetup.bar
-    temp = filesetup.temp
-    log = filesetup.log
-
-    if ":" in val:
-        method, attrs = val.split(":", 1)
-    else:
-        method, attrs = val, ""
-
-    levels = Levels(ensure, src, tb, bar, temp, log)
-
-    if method == "none":
-        return levels.none()
-    if method == "all/e":
-        return levels.all()
-
-    try:
-        obj = parse_with_palet(attrs, builder_map[method], env)
-    except ParserError as e:
-        log.error(e)
-
-    try:
-        if method == "audio":
-            s = obj["stream"]
-            if s == "all" or s == Sym("all"):
-                total_list: NDArray[np.bool_] | None = None
-                for s in range(len(src.audios)):
-                    audio_list = to_threshold(levels.audio(s), obj["threshold"])
-                    if total_list is None:
-                        total_list = audio_list
-                    else:
-                        total_list = boolop(total_list, audio_list, np.logical_or)
-
-                if total_list is None:
-                    if strict:
-                        log.error("Input has no audio streams.")
-                    stream_data = levels.all()
-                else:
-                    stream_data = total_list
-            else:
-                assert isinstance(s, int)
-                stream_data = to_threshold(levels.audio(s), obj["threshold"])
-
-            assert isinstance(obj["minclip"], int)
-            assert isinstance(obj["mincut"], int)
-
-            mut_remove_small(stream_data, obj["minclip"], replace=1, with_=0)
-            mut_remove_small(stream_data, obj["mincut"], replace=0, with_=1)
-
-            return stream_data
-
-        if method == "motion":
-            return to_threshold(
-                levels.motion(obj["stream"], obj["blur"], obj["width"]),
-                obj["threshold"],
-            )
-
-        if method == "subtitle":
-            return levels.subtitle(
-                obj["pattern"],
-                obj["stream"],
-                obj["ignore_case"],
-                obj["max_count"],
-            )
-    except LevelError as e:
-        if strict:
-            log.error(e)
-
-        return levels.all()
-    raise ValueError("Unreachable")
```

### Comparing `auto-editor-24.7.1/auto_editor/edit.py` & `auto-editor-24.9.1/auto_editor/edit.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/ffwrapper.py` & `auto-editor-24.9.1/auto_editor/ffwrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,18 +235,21 @@
                 ]
             )
             _sar, c_range, c_space, c_primary, c_transfer = _raw.strip().split("\n")
         except Exception:
             log.debug("Unexpected ffprobe shape")
 
         if v.sample_aspect_ratio is None:
-            try:
-                sar = Fraction(_sar.replace(":", "/"))
-            except Exception:
+            if _sar is None:
                 sar = Fraction(1)
+            else:
+                try:
+                    sar = Fraction(_sar.replace(":", "/"))
+                except Exception:
+                    sar = Fraction(1)
         else:
             sar = v.sample_aspect_ratio
 
         videos += (
             VideoStream(
                 v.width,
                 v.height,
```

### Comparing `auto-editor-24.7.1/auto_editor/formats/fcp11.py` & `auto-editor-24.9.1/auto_editor/formats/fcp11.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/formats/fcp7.py` & `auto-editor-24.9.1/auto_editor/formats/fcp7.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,15 +359,14 @@
 
         vschar = ET.SubElement(videodef, "samplecharacteristics")
         rate = ET.SubElement(vschar, "rate")
         ET.SubElement(rate, "timebase").text = f"{tb}"
         ET.SubElement(rate, "ntsc").text = ntsc
         ET.SubElement(vschar, "width").text = f"{tl.res[0]}"
         ET.SubElement(vschar, "height").text = f"{tl.res[1]}"
-        ET.SubElement(vschar, "anamorphic").text = "FALSE"
         ET.SubElement(vschar, "pixelaspectratio").text = "square"
 
     for aud in src.audios:
         audiodef = ET.SubElement(mediadef, "audio")
         aschar = ET.SubElement(audiodef, "samplecharacteristics")
         ET.SubElement(aschar, "depth").text = DEPTH
         ET.SubElement(aschar, "samplerate").text = f"{tl.sr}"
@@ -385,71 +384,72 @@
 
     for src in set(tl.sources):
         the_id = f"file-{len(src_to_id)+1}"
         src_to_url[src] = f"{src.path.resolve()}"
         src_to_id[src] = the_id
 
     xmeml = ET.Element("xmeml", version="5")
-    sequence = ET.SubElement(xmeml, "sequence")
+    sequence = ET.SubElement(xmeml, "sequence", explodedTracks="true")
     ET.SubElement(sequence, "name").text = name
     ET.SubElement(sequence, "duration").text = f"{int(tl.out_len())}"
     rate = ET.SubElement(sequence, "rate")
     ET.SubElement(rate, "timebase").text = f"{timebase}"
     ET.SubElement(rate, "ntsc").text = ntsc
     media = ET.SubElement(sequence, "media")
     video = ET.SubElement(media, "video")
     vformat = ET.SubElement(video, "format")
     vschar = ET.SubElement(vformat, "samplecharacteristics")
 
-    rate = ET.SubElement(vschar, "rate")
-    ET.SubElement(rate, "timebase").text = f"{timebase}"
-    ET.SubElement(rate, "ntsc").text = ntsc
     ET.SubElement(vschar, "width").text = f"{width}"
     ET.SubElement(vschar, "height").text = f"{height}"
     ET.SubElement(vschar, "pixelaspectratio").text = "square"
 
+    rate = ET.SubElement(vschar, "rate")
+    ET.SubElement(rate, "timebase").text = f"{timebase}"
+    ET.SubElement(rate, "ntsc").text = ntsc
+
     if len(tl.v) > 0 and len(tl.v[0]) > 0:
         track = ET.SubElement(video, "track")
 
         for j, clip in enumerate(tl.v[0]):
             assert isinstance(clip, TlVideo)
 
             _start = f"{clip.start}"
             _end = f"{clip.start + clip.dur}"
             _in = f"{int(clip.offset / clip.speed)}"
             _out = f"{int(clip.offset / clip.speed) + clip.dur}"
 
             clipitem = ET.SubElement(track, "clipitem", id=f"clipitem-{j+1}")
             ET.SubElement(clipitem, "name").text = src.path.stem
+            ET.SubElement(clipitem, "enabled").text = "TRUE"
             ET.SubElement(clipitem, "start").text = _start
             ET.SubElement(clipitem, "end").text = _end
             ET.SubElement(clipitem, "in").text = _in
             ET.SubElement(clipitem, "out").text = _out
 
             _id = src_to_id[clip.src]
             filedef = ET.SubElement(clipitem, "file", id=_id)
 
             pathurl = src_to_url[clip.src]
             if pathurl not in file_defs:
                 media_def(filedef, pathurl, clip.src, tl, timebase, ntsc)
                 file_defs.add(pathurl)
 
+            ET.SubElement(clipitem, "compositemode").text = "normal"
             if clip.speed != 1:
                 clipitem.append(speedup(clip.speed * 100))
 
             for i in range(len(src.audios) * 2 + 1):  # `2` because stereo.
                 link = ET.SubElement(clipitem, "link")
                 ET.SubElement(
                     link, "linkclipref"
                 ).text = f"clipitem-{(i*(len(tl.v[0])))+j+1}"
                 ET.SubElement(link, "mediatype").text = "video" if i == 0 else "audio"
                 ET.SubElement(link, "trackindex").text = str(max(i, 1))
                 ET.SubElement(link, "clipindex").text = str(j + 1)
-                if i > 0:
-                    ET.SubElement(link, "groupindex").text = "1"
 
     # Audio definitions and clips
     audio = ET.SubElement(media, "audio")
     ET.SubElement(audio, "numOutputChannels").text = "2"
     aformat = ET.SubElement(audio, "format")
     aschar = ET.SubElement(aformat, "samplecharacteristics")
     ET.SubElement(aschar, "depth").text = DEPTH
@@ -485,32 +485,33 @@
                 clipitem = ET.SubElement(
                     track,
                     "clipitem",
                     id=f"clipitem-{clip_item_num}",
                     premiereChannelType="stereo",
                 )
                 ET.SubElement(clipitem, "name").text = src.path.stem
+                ET.SubElement(clipitem, "enabled").text = "TRUE"
                 ET.SubElement(clipitem, "start").text = _start
                 ET.SubElement(clipitem, "end").text = _end
                 ET.SubElement(clipitem, "in").text = _in
                 ET.SubElement(clipitem, "out").text = _out
 
                 pathurl = src_to_url[aclip.src]
                 filedef = ET.SubElement(clipitem, "file", id=src_to_id[aclip.src])
                 if pathurl not in file_defs:
                     media_def(filedef, pathurl, aclip.src, tl, timebase, ntsc)
                     file_defs.add(pathurl)
 
                 sourcetrack = ET.SubElement(clipitem, "sourcetrack")
                 ET.SubElement(sourcetrack, "mediatype").text = "audio"
-                ET.SubElement(sourcetrack, "trackindex").text = f"{t + 1}"
+                ET.SubElement(sourcetrack, "trackindex").text = f"{t}"
                 labels = ET.SubElement(clipitem, "labels")
                 ET.SubElement(labels, "label2").text = "Iris"
 
                 if aclip.speed != 1:
                     clipitem.append(speedup(aclip.speed * 100))
 
             audio.append(track)
 
     tree = ET.ElementTree(xmeml)
-    ET.indent(tree, space="\t", level=0)
+    ET.indent(tree, space="  ", level=0)
     tree.write(output, xml_declaration=True, encoding="utf-8")
```

### Comparing `auto-editor-24.7.1/auto_editor/formats/json.py` & `auto-editor-24.9.1/auto_editor/formats/json.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/formats/shotcut.py` & `auto-editor-24.9.1/auto_editor/formats/shotcut.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/formats/utils.py` & `auto-editor-24.9.1/auto_editor/formats/utils.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/help.py` & `auto-editor-24.9.1/auto_editor/help.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,24 +21,27 @@
 
 --set-range-for-speed 2.5,400,800
 
 will set the speed from 400 ticks to 800 ticks to 2.5x
 If timebase is 30, 400 ticks to 800 means 13.33 to 26.66 seconds
 """.strip(),
         "--edit-based-on": """
-Evalutes a palet expression that returns a bool-array?. The array is then used for
+Evaluates a palet expression that returns a bool-array?. The array is then used for
 editing.
 
 Editing Methods:
  - audio  ; Audio silence/loudness detection
     - threshold threshold? : 4%
-    - stream (or/c nat? 'all "all") : 0
+    - stream (or/c nat? 'all) : 'all
     - mincut nat? : 6
     - minclip nat? : 3
 
+ ; mincut is more significant, there it has a larger default value.
+ ; minclip gets applied first, then mincut
+
  - motion  ; Motion detection specialized for noisy real-life videos
     - threshold threshold? : 2%
     - stream nat? : 0
     - blur nat? : 9
     - width nat1? : 400
 
  - subtitle  ; Detect when subtitle matches pattern as a RegEx string.
@@ -147,18 +150,14 @@
 `--audio-bitrate` sets the target bitrate for the audio encoder.
 The value accepts a natural number and the units: ``, `k`, `K`, and `M`.
 The special value `unset` may also be used, and means: Don't pass any value to ffmpeg, let it choose a default bitrate.
 """.strip(),
         "--video-bitrate": """
 `--video-bitrate` sets the target bitrate for the video encoder. It accepts the same format as `--audio-bitrate` and the special `unset` value is allowed.
 """.strip(),
-        "--silent-threshold": """
-Silent threshold is a percentage where 0% represents absolute silence and 100% represents the highest volume in the media file.
-Setting the threshold to `0%` will cut only out areas where area is absolutely silence.
-""".strip(),
         "--margin": """
 Default value: 0.2s,0.2s
 
 `--margin` takes either one number of two numbers with a `,` in-between.
 The numbers may be written in the 'time' format. Here is a quick recap:
 
   frames / timebase : `` (no units)
```

### Comparing `auto-editor-24.7.1/auto_editor/lang/json.py` & `auto-editor-24.9.1/auto_editor/lang/json.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/lang/libmath.py` & `auto-editor-24.9.1/auto_editor/lang/libmath.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/lang/palet.py` & `auto-editor-24.9.1/auto_editor/lang/palet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Palet is a light-weight scripting languge. It handles `--edit` and the `repl`.
 The syntax is inspired by the Racket Programming language.
 """
 
-
 from __future__ import annotations
 
 from cmath import sqrt as complex_sqrt
 from dataclasses import dataclass
 from difflib import get_close_matches
 from fractions import Fraction
 from functools import reduce
@@ -15,15 +14,20 @@
 from operator import add, ge, gt, is_, le, lt, mod, mul
 from time import sleep
 from typing import TYPE_CHECKING
 
 import numpy as np
 from numpy import logical_and, logical_not, logical_or, logical_xor
 
-from auto_editor.analyze import edit_method, mut_remove_large, mut_remove_small
+from auto_editor.analyze import (
+    LevelError,
+    mut_remove_large,
+    mut_remove_small,
+    to_threshold,
+)
 from auto_editor.lib.contracts import *
 from auto_editor.lib.data_structs import *
 from auto_editor.lib.err import MyError
 from auto_editor.utils.func import boolop, mut_margin
 
 if TYPE_CHECKING:
     from collections.abc import Callable
@@ -44,17 +48,16 @@
 ###############################################################################
 #                                                                             #
 #  LEXER                                                                      #
 #                                                                             #
 ###############################################################################
 
 LPAREN, RPAREN, LBRAC, RBRAC, LCUR, RCUR, EOF = "(", ")", "[", "]", "{", "}", "EOF"
-VAL, QUOTE, SEC, DB, DOT, VLIT = "VAL", "QUOTE", "SEC", "DB", "DOT", "VLIT"
+VAL, QUOTE, SEC, DB, DOT, VLIT, M = "VAL", "QUOTE", "SEC", "DB", "DOT", "VLIT", "M"
 SEC_UNITS = ("s", "sec", "secs", "second", "seconds")
-METHODS = ("audio:", "motion:", "subtitle:")
 brac_pairs = {LPAREN: RPAREN, LBRAC: RBRAC, LCUR: RCUR}
 
 str_escape = {
     "a": "\a",
     "b": "\b",
     "t": "\t",
     "n": "\n",
@@ -312,15 +315,14 @@
                     self.allow_lang_prag = False
                     continue
                 else:
                     return self.hash_literal()
 
             result = ""
             has_illegal = False
-            is_method = False
 
             def normal() -> bool:
                 return (
                     self.char is not None
                     and self.char not in '.()[]{}"; \t\n\r\x0b\x0c'
                 )
 
@@ -329,30 +331,32 @@
                 if self.char == '"':
                     self.advance()
                     result = f'{result}"{self.string()}"'
                     return handle_strings()
                 else:
                     return self.char_is_norm()
 
+            is_method = False
             while normal():
-                result += self.char
-                if (result + ":") in METHODS:
+                if self.char == ":":
+                    name = result
+                    result = ""
                     is_method = True
                     normal = handle_strings
+                else:
+                    result += self.char
 
                 if self.char in "'`|\\":
                     has_illegal = True
                 self.advance()
 
             if is_method:
-                return Token(VAL, Method(result))
+                from auto_editor.utils.cmdkw import parse_method
 
-            for method in METHODS:
-                if result == method[:-1]:
-                    return Token(VAL, Method(result))
+                return Token(M, parse_method(name, result, env))
 
             if self.char == ".":  # handle `object.method` syntax
                 self.advance()
                 return Token(DOT, (Sym(result), self.get_next_token()))
 
             if has_illegal:
                 self.error(f"Symbol has illegal character(s): {result}")
@@ -365,24 +369,14 @@
 ###############################################################################
 #                                                                             #
 #  PARSER                                                                     #
 #                                                                             #
 ###############################################################################
 
 
-@dataclass(slots=True)
-class Method:
-    val: str
-
-    def __str__(self) -> str:
-        return f"#<method:{self.val}>"
-
-    __repr__ = __str__
-
-
 class Parser:
     def __init__(self, lexer: Lexer):
         self.lexer = lexer
         self.current_token = self.lexer.get_next_token()
 
     def eat(self) -> None:
         self.current_token = self.lexer.get_next_token()
@@ -409,14 +403,24 @@
             self.eat()
             return (Sym("round"), (Sym("*"), token.value, Sym("timebase")))
 
         if token.type == DB:
             self.eat()
             return (Sym("pow"), 10, (Sym("/"), token.value, 20))
 
+        if token.type == M:
+            self.eat()
+            name, args, kwargs = token.value
+            _result = [Sym(name)] + args
+            for key, val in kwargs.items():
+                _result.append(Keyword(key))
+                _result.append(val)
+
+            return tuple(_result)
+
         if token.type == DOT:
             self.eat()
             if type(token.value[1].value) is not Sym:
                 raise MyError(". macro: attribute call needs to be an identifier")
 
             return (Sym("@r"), token.value[0], token.value[1].value)
 
@@ -502,15 +506,15 @@
     try:
         port = open(name, "w", encoding="utf-8")
     except Exception:
         return False
     return OutputPort(name, port, port.write, False)
 
 
-def raise_(msg: str) -> None:
+def raise_(msg: str | Exception) -> NoReturn:
     raise MyError(msg)
 
 
 def is_equal(a: object, b: object) -> bool:
     if isinstance(a, np.ndarray) and isinstance(b, np.ndarray):
         return np.array_equal(a, b)
     return type(a) == type(b) and a == b
@@ -804,55 +808,38 @@
         for item in self.body[0:-1]:
             my_eval(inner_env, item)
 
         return my_eval(inner_env, self.body[-1])
 
 
 @dataclass(slots=True)
-class KeywordProc:
+class KeywordUserProc:
     env: Env
     name: str
     parms: list[str]
     kw_parms: list[str]
     body: Node
     arity: tuple[int, None]
     contracts: list[Any] | None = None
 
-    def __call__(self, *args: Any) -> Any:
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
         env = {}
+        all_parms = self.parms + self.kw_parms
+        for i, arg in enumerate(args):
+            if i >= len(all_parms):
+                raise MyError("Too many arguments")
+            env[all_parms[i]] = arg
 
-        for i, parm in enumerate(self.parms):
-            if type(args[i]) is Keyword:
-                raise MyError(f"Invalid keyword `{args[i]}`")
-            env[parm] = args[i]
-
-        remain_args = args[len(self.parms) :]
-
-        allow_pos = True
-        pos_index = 0
-        key = ""
-        for arg in remain_args:
-            if type(arg) is Keyword:
-                if key:
-                    raise MyError("Expected value for keyword but got another keyword")
-                key = arg.val
-                allow_pos = False
-            elif key:
-                env[key] = arg
-                key = ""
+        for key, val in kwargs.items():
+            if key in env:
+                raise MyError(
+                    f"Keyword: {key} already fulfilled by positional argument."
+                )
             else:
-                if not allow_pos:
-                    raise MyError("Positional argument not allowed here")
-                if pos_index >= len(self.kw_parms):
-                    base = f"`{self.name}` has an arity mismatch. Expected"
-                    upper = len(self.parms) + len(self.kw_parms)
-                    raise MyError(f"{base} at most {upper}")
-
-                env[self.kw_parms[pos_index]] = arg
-                pos_index += 1
+                env[key] = val
 
         inner_env = Env(env, self.env)
 
         for item in self.body[0:-1]:
             my_eval(inner_env, item)
 
         return my_eval(inner_env, self.body[-1])
@@ -949,15 +936,15 @@
                     kparms.append(item.val)
                 elif type(item) is Sym:
                     parms.append(item.val)
                 else:
                     raise MyError(f"{node[0]}: must be an identifier")
 
         if kw_only:
-            env[n] = KeywordProc(env, n, parms, kparms, body, (len(parms), None))
+            env[n] = KeywordUserProc(env, n, parms, kparms, body, (len(parms), None))
         else:
             env[n] = UserProc(env, n, parms, (), body)
         return None
 
     elif type(node[1]) is not Sym:
         raise MyError(f"{node[0]}: must be an identifier")
 
@@ -1478,32 +1465,102 @@
 def edit_all() -> np.ndarray:
     if "@levels" not in env:
         raise MyError("Can't use `all/e` if there's no input media")
 
     return env["@levels"].all()
 
 
+def edit_audio(
+    threshold: float = 0.04,
+    stream: object = Sym("all"),
+    mincut: int = 6,
+    minclip: int = 3,
+) -> np.ndarray:
+    if "@levels" not in env or "@filesetup" not in env:
+        raise MyError("Can't use `audio` if there's no input media")
+
+    levels = env["@levels"]
+    src = env["@filesetup"].src
+    strict = env["@filesetup"].strict
+
+    stream_data: NDArray[np.bool_] | None = None
+    if stream == Sym("all"):
+        stream_range = range(0, len(src.audios))
+    else:
+        assert isinstance(stream, int)
+        stream_range = range(stream, stream + 1)
+
+    try:
+        for s in stream_range:
+            audio_list = to_threshold(levels.audio(s), threshold)
+            if stream_data is None:
+                stream_data = audio_list
+            else:
+                stream_data = boolop(stream_data, audio_list, np.logical_or)
+    except LevelError as e:
+        raise_(e) if strict else levels.all()
+
+    if stream_data is not None:
+        mut_remove_small(stream_data, minclip, replace=1, with_=0)
+        mut_remove_small(stream_data, mincut, replace=0, with_=1)
+
+        return stream_data
+
+    stream = 0 if stream == Sym("all") else stream
+    return raise_(f"audio stream '{stream}' does not exist") if strict else levels.all()
+
+
+def edit_motion(
+    threshold: float = 0.02,
+    stream: int = 0,
+    blur: int = 9,
+    width: int = 400,
+) -> np.ndarray:
+    if "@levels" not in env:
+        raise MyError("Can't use `motion` if there's no input media")
+
+    levels = env["@levels"]
+    strict = env["@filesetup"].strict
+    try:
+        return to_threshold(levels.motion(stream, blur, width), threshold)
+    except LevelError as e:
+        return raise_(e) if strict else levels.all()
+
+
+def edit_subtitle(pattern, stream=0, **kwargs):
+    if "@levels" not in env:
+        raise MyError("Can't use `subtitle` if there's no input media")
+
+    levels = env["@levels"]
+    strict = env["@filesetup"].strict
+    if "ignore-case" not in kwargs:
+        kwargs["ignore-case"] = False
+    if "max-count" not in kwargs:
+        kwargs["max-count"] = None
+    ignore_case = kwargs["ignore-case"]
+    max_count = kwargs["max-count"]
+    try:
+        return levels.subtitle(pattern, stream, ignore_case, max_count)
+    except LevelError as e:
+        return raise_(e) if strict else levels.all()
+
+
 def my_eval(env: Env, node: object) -> Any:
     if type(node) is Sym:
         val = env.get(node.val)
         if type(val) is NotFound:
             if mat := get_close_matches(node.val, env.data):
                 raise MyError(
                     f"variable `{node.val}` not found. Did you mean: {mat[0]}"
                 )
             raise MyError(
                 f"variable `{node.val}` not found. Did you mean a string literal."
             )
         return val
 
-    if isinstance(node, Method):
-        if "@filesetup" not in env:
-            raise MyError("Can't use edit methods if there's no input files")
-        return edit_method(node.val, env["@filesetup"], env)
-
     if type(node) is list:
         return [my_eval(env, item) for item in node]
 
     if type(node) is tuple:
         if not node:
             raise MyError("Illegal () expression")
 
@@ -1527,29 +1584,55 @@
             raise MyError(
                 f"Tried to run: {print_str(oper)} with args: {print_str(node[1:])}"
             )
 
         if type(oper) is Syntax:
             return oper(env, node)
 
-        return oper(*(my_eval(env, c) for c in node[1:]))
+        i = 1
+        args: list[Any] = []
+        kwargs: dict[str, Any] = {}
+        while i < len(node):
+            result = my_eval(env, node[i])
+            if type(result) is Keyword:
+                i += 1
+                if i >= len(node):
+                    raise MyError("Keyword need argument")
+                kwargs[result.val] = my_eval(env, node[i])
+            else:
+                args.append(result)
+            i += 1
+
+        return oper(*args, **kwargs)
 
     return node
 
 
 # fmt: off
 env = Env({})
 env.update({
     # constants
     "true": True,
     "false": False,
     "all": Sym("all"),
     # edit procedures
     "none": Proc("none", edit_none, (0, 0)),
     "all/e": Proc("all/e", edit_all, (0, 0)),
+    "audio": Proc("audio", edit_audio, (0, 4),
+        is_threshold, orc(is_nat, Sym("all")), is_nat,
+        {"threshold": 0, "stream": 1, "minclip": 2, "mincut": 2}
+    ),
+    "motion": Proc("motion", edit_motion, (0, 4),
+        is_threshold, is_nat, is_nat1,
+        {"threshold": 0, "stream": 1, "blur": 1, "width": 2}
+    ),
+    "subtitle": Proc("subtitle", edit_subtitle, (1, 4),
+        is_str, is_nat, is_bool, orc(is_nat, is_void),
+        {"pattern": 0, "stream": 1, "ignore-case": 2, "max-count": 3}
+    ),
     # syntax
     "lambda": Syntax(syn_lambda),
     "λ": Syntax(syn_lambda),
     "define": Syntax(syn_define),
     "define/c": Syntax(syn_definec),
     "set!": Syntax(syn_set),
     "incf": Syntax(syn_incf),
```

### Comparing `auto-editor-24.7.1/auto_editor/lib/contracts.py` & `auto-editor-24.9.1/auto_editor/lib/contracts.py`

 * *Files 23% similar despite different names*

```diff
@@ -43,24 +43,24 @@
         return val is False
     if type(c) in (int, float, Fraction, complex, str, Sym):
         return val == c
     raise MyError(f"Invalid contract, got: {print_str(c)}")
 
 
 def check_args(
-    o: str,
+    name: str,
     values: list | tuple,
     arity: tuple[int, int | None],
     cont: tuple[Any, ...],
 ) -> None:
     lower, upper = arity
     amount = len(values)
 
     assert not (upper is not None and lower > upper)
-    base = f"`{o}` has an arity mismatch. Expected "
+    base = f"`{name}` has an arity mismatch. Expected "
 
     if lower == upper and len(values) != lower:
         raise MyError(f"{base}{lower}, got {amount}")
     if upper is None and amount < lower:
         raise MyError(f"{base}at least {lower}, got {amount}")
     if upper is not None and (amount > upper or amount < lower):
         raise MyError(f"{base}between {lower} and {upper}, got {amount}")
@@ -68,31 +68,72 @@
     if not cont:
         return
 
     for i, val in enumerate(values):
         check = cont[-1] if i >= len(cont) else cont[i]
         if not check_contract(check, val):
             exp = f"{check}" if callable(check) else print_str(check)
-            raise MyError(f"`{o}` expected a {exp}, got {print_str(val)}")
+            raise MyError(f"`{name}` expected {exp}, but got {print_str(val)}")
 
 
 class Proc:
-    __slots__ = ("name", "proc", "arity", "contracts")
+    __slots__ = ("name", "proc", "arity", "contracts", "kw_contracts")
 
     def __init__(
         self, n: str, p: Callable, a: tuple[int, int | None] = (1, None), *c: Any
     ):
         self.name = n
         self.proc = p
         self.arity = a
-        self.contracts: tuple[Any, ...] = c
 
-    def __call__(self, *args: Any) -> Any:
-        check_args(self.name, args, self.arity, self.contracts)
-        return self.proc(*args)
+        if c and type(c[-1]) is dict:
+            self.kw_contracts: dict[str, int] | None = c[-1]
+            self.contracts: tuple[Any, ...] = c[:-1]
+        else:
+            self.kw_contracts = None
+            self.contracts = c
+
+    def __call__(self, *args: Any, **kwargs: Any):
+        lower, upper = self.arity
+        amount = len(args)
+        cont = self.contracts
+        kws = self.kw_contracts
+
+        assert not (upper is not None and lower > upper)
+        base = f"`{self.name}` has an arity mismatch. Expected "
+
+        if lower == upper and len(args) != lower:
+            raise MyError(f"{base}{lower}, got {amount}")
+        if upper is None and amount < lower:
+            raise MyError(f"{base}at least {lower}, got {amount}")
+        if upper is not None and (amount > upper or amount < lower):
+            raise MyError(f"{base}between {lower} and {upper}, got {amount}")
+
+        if not cont:
+            return self.proc(*args)
+
+        if kws is not None:
+            for key, val in kwargs.items():
+                check = cont[-1] if kws[key] >= len(cont) else cont[kws[key]]
+                if not check_contract(check, val):
+                    exp = f"{check}" if callable(check) else print_str(check)
+                    raise MyError(
+                        f"`{self.name} #:{key}` expected {exp}, but got {print_str(val)}"
+                    )
+
+        elif len(kwargs) > 0:
+            raise MyError("Keyword arguments are not allowed here")
+
+        for i, val in enumerate(args):
+            check = cont[-1] if i >= len(cont) else cont[i]
+            if not check_contract(check, val):
+                exp = f"{check}" if callable(check) else print_str(check)
+                raise MyError(f"`{self.name}` expected {exp}, but got {print_str(val)}")
+
+        return self.proc(*args, **kwargs)
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         n = "inf" if self.arity[1] is None else f"{self.arity[1]}"
 
@@ -133,21 +174,27 @@
 is_threshold = Contract(
     "threshold?",
     lambda v: type(v) in (int, float) and v >= 0 and v <= 1,  # type: ignore
 )
 is_proc = Contract("procedure?", lambda v: isinstance(v, Proc | Contract))
 
 
+def contract_printer(cs) -> str:
+    return " ".join(
+        c.name if isinstance(c, Proc | Contract) else print_str(c) for c in cs
+    )
+
+
 def andc(*cs: object) -> Proc:
-    name = "(and/c " + " ".join(f"{c}" for c in cs) + ")"
+    name = f"(and/c {contract_printer(cs)})"
     return Proc(name, lambda v: all(check_contract(c, v) for c in cs), (1, 1), any_p)
 
 
 def orc(*cs: object) -> Proc:
-    name = "(or/c " + " ".join(f"{c}" for c in cs) + ")"
+    name = f"(or/c {contract_printer(cs)})"
     return Proc(name, lambda v: any(check_contract(c, v) for c in cs), (1, 1), any_p)
 
 
 def notc(c: object) -> Proc:
     return Proc("flat-not/c", lambda v: not check_contract(c, v), (1, 1), any_p)
```

### Comparing `auto-editor-24.7.1/auto_editor/lib/data_structs.py` & `auto-editor-24.9.1/auto_editor/lib/data_structs.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         return NotFound()
 
 
 class Sym:
     __slots__ = ("val", "hash")
 
     def __init__(self, val: str):
+        assert isinstance(val, str)
         self.val = val
         self.hash = hash(val)
 
     def __str__(self) -> str:
         return self.val
 
     __repr__ = __str__
```

### Comparing `auto-editor-24.7.1/auto_editor/make_layers.py` & `auto-editor-24.9.1/auto_editor/make_layers.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/output.py` & `auto-editor-24.9.1/auto_editor/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
             + _ffset("-color_trc", src.videos[0].color_transfer)
         )
 
     if args.extras is not None:
         cmd.extend(args.extras.split(" "))
     cmd.extend(["-strict", "-2"])  # Allow experimental codecs.
 
-    if not args.sn:
+    if s_tracks > 0:
         cmd.extend(["-map", "0:t?"])  # Add input attachments to output.
 
     # This was causing a crash for 'example.mp4 multi-track.mov'
     # cmd.extend(["-map", "0:d?"])
 
     cmd.append(output_path)
     ffmpeg.run_check_errors(cmd, log, path=output_path)
```

### Comparing `auto-editor-24.7.1/auto_editor/preview.py` & `auto-editor-24.9.1/auto_editor/preview.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/render/audio.py` & `auto-editor-24.9.1/auto_editor/render/audio.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/render/subtitle.py` & `auto-editor-24.9.1/auto_editor/render/subtitle.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/render/video.py` & `auto-editor-24.9.1/auto_editor/render/video.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 
 def make_image_cache(tl: v3) -> dict[tuple[FileInfo, int], np.ndarray]:
     img_cache = {}
     for clip in tl.v:
         for obj in clip:
             if isinstance(obj, TlImage) and obj.src not in img_cache:
                 with av.open(obj.src.path) as cn:
+                    assert isinstance(cn, av.InputContainer)
                     my_stream = cn.streams.video[0]
                     for frame in cn.decode(my_stream):
                         if obj.width != 0:
                             graph = av.filter.Graph()
                             link_nodes(
                                 graph.add_buffer(template=my_stream),
                                 graph.add("scale", f"{obj.width}:-1"),
@@ -164,36 +165,47 @@
     log.debug(f"Tous: {tous}")
     log.debug(f"Clips: {tl.v}")
 
     target_pix_fmt = target_pix_fmt if target_pix_fmt in allowed_pix_fmt else "yuv420p"
     log.debug(f"Target pix_fmt: {target_pix_fmt}")
 
     apply_video_later = True
-
-    if args.scale != 1:
-        apply_video_later = False
-    elif args.video_codec in encoders:
+    if args.video_codec in encoders:
         apply_video_later = set(encoders[args.video_codec]).isdisjoint(allowed_pix_fmt)
 
     log.debug(f"apply video quality settings now: {not apply_video_later}")
 
-    width, height = tl.res
+    if args.scale == 1.0:
+        target_width, target_height = tl.res
+        scale_graph = None
+    else:
+        target_width = max(round(tl.res[0] * args.scale), 2)
+        target_height = max(round(tl.res[1] * args.scale), 2)
+        scale_graph = av.filter.Graph()
+        link_nodes(
+            scale_graph.add(
+                "buffer", video_size="1x1", time_base="1/1", pix_fmt=target_pix_fmt
+            ),
+            scale_graph.add("scale", f"{target_width}:{target_height}"),
+            scale_graph.add("buffersink"),
+        )
+
     spedup = os.path.join(temp, "spedup0.mp4")
 
     cmd = [
         "-hide_banner",
         "-y",
         "-f",
         "rawvideo",
         "-c:v",
         "rawvideo",
         "-pix_fmt",
         target_pix_fmt,
         "-s",
-        f"{width}*{height}",
+        f"{target_width}*{target_height}",
         "-framerate",
         f"{tl.tb}",
         "-i",
         "-",
         "-pix_fmt",
         target_pix_fmt,
     ]
@@ -220,15 +232,15 @@
     seek = 10
     seek_frame = None
     frames_saved = 0
 
     bar.start(tl.end, "Creating new video")
 
     bg = color(args.background)
-    null_frame = make_solid(width, height, target_pix_fmt, bg)
+    null_frame = make_solid(target_width, target_height, target_pix_fmt, bg)
     frame_index = -1
     try:
         for index in range(tl.end):
             obj_list: list[VideoFrame | TlRect | TlImage] = []
             for layer in tl.v:
                 for lobj in layer:
                     if isinstance(lobj, TlVideo):
@@ -278,15 +290,16 @@
                                 f"Skipped {frame_index - seek_frame} frame indexes"
                             )
                             frames_saved += frame_index - seek_frame
                             seek_frame = None
                         if frame.key_frame:
                             log.debug(f"Keyframe {frame_index} {frame.pts}")
 
-                    if frame.width != width or frame.height != height:
+                    if (frame.width, frame.height) != tl.res:
+                        width, height = tl.res
                         graph = av.filter.Graph()
                         link_nodes(
                             graph.add_buffer(template=my_stream),
                             graph.add(
                                 "scale",
                                 f"{width}:{height}:force_original_aspect_ratio=decrease:eval=frame",
                             ),
@@ -341,14 +354,18 @@
                     # Blend the overlay image with the ROI based on the opacity
                     roi = (1 - obj.opacity) * roi + obj.opacity * clipped_overlay
                     array[y_start:y_end, x_start:x_end] = roi
                     array = np.clip(array, 0, 255).astype(np.uint8)
 
                     frame = av.VideoFrame.from_ndarray(array, format="rgb24")
 
+            if scale_graph is not None and frame.width != target_width:
+                scale_graph.push(frame)
+                frame = scale_graph.pull()
+
             if frame.format.name != target_pix_fmt:
                 frame = frame.reformat(format=target_pix_fmt)
                 bar.tick(index)
             elif index % 3 == 0:
                 bar.tick(index)
 
             process2.stdin.write(frame.to_ndarray().tobytes())
@@ -359,23 +376,8 @@
     except (OSError, BrokenPipeError):
         bar.end()
         ffmpeg.run_check_errors(cmd, log, True)
         log.error("FFmpeg Error!")
 
     log.debug(f"Total frames saved seeking: {frames_saved}")
 
-    if args.scale != 1:
-        sped_input = os.path.join(temp, "spedup0.mp4")
-        spedup = os.path.join(temp, "scale0.mp4")
-        scale_filter = f"scale=iw*{args.scale}:ih*{args.scale}"
-
-        cmd = ["-i", sped_input, "-vf", scale_filter, spedup]
-
-        check_errors = ffmpeg.pipe(cmd)
-        if "Error" in check_errors or "failed" in check_errors:
-            if "-allow_sw 1" in check_errors:
-                cmd.insert(-1, "-allow_sw")
-                cmd.insert(-1, "1")
-            # Run again to show errors even if it might not work.
-            ffmpeg.run(cmd)
-
     return spedup, apply_video_later
```

### Comparing `auto-editor-24.7.1/auto_editor/subcommands/desc.py` & `auto-editor-24.9.1/auto_editor/subcommands/desc.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/subcommands/info.py` & `auto-editor-24.9.1/auto_editor/subcommands/info.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/subcommands/levels.py` & `auto-editor-24.9.1/auto_editor/subcommands/levels.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/subcommands/palet.py` & `auto-editor-24.9.1/auto_editor/subcommands/palet.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/subcommands/repl.py` & `auto-editor-24.9.1/auto_editor/subcommands/repl.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/subcommands/subdump.py` & `auto-editor-24.9.1/auto_editor/subcommands/subdump.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/subcommands/test.py` & `auto-editor-24.9.1/auto_editor/subcommands/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,24 +128,27 @@
     total_time = 0.0
 
     passed = 0
     total = len(tests)
     for index, test in enumerate(tests, start=1):
         name = test.__name__
         start = perf_counter()
+        outputs = None
 
         try:
             outputs = test()
             dur = perf_counter() - start
             total_time += dur
         except KeyboardInterrupt:
             print("Testing Interrupted by User.")
             clean_all()
             sys.exit(1)
         except Exception as e:
+            dur = perf_counter() - start
+            total_time += dur
             print(f"{name:<24} ({index}/{total})  {round(dur, 2):<4} secs  [FAILED]")
             if args.no_fail_fast:
                 print(f"\n{e}")
             else:
                 print("")
                 clean_all()
                 raise e
@@ -680,16 +683,16 @@
             ('(define s "hello")s.title', "Hello"),
             ("(define v #(2 0 3 -4 -2 5 1 4)) v.sort", [-4, -2, 0, 1, 2, 3, 4, 5]),
             ("(define v #(2 0 3 -4 -2 5 1 4)) v.sort! v", [-4, -2, 0, 1, 2, 3, 4, 5]),
             ('#(#("sym" "symbol?") "bool?")', [["sym", "symbol?"], "bool?"]),
         )
 
     def palet_scripts():
-        run.raw(["palet", "resources/scripts/maxcut.pal"])
         run.raw(["palet", "resources/scripts/scope.pal"])
+        run.raw(["palet", "resources/scripts/maxcut.pal"])
         run.raw(["palet", "resources/scripts/case.pal"])
         run.raw(["palet", "resources/scripts/testmath.pal"])
 
     tests = []
 
     if args.category in ("palet", "all"):
         tests.extend([palet_python_bridge, palet_scripts])
```

### Comparing `auto-editor-24.7.1/auto_editor/timeline.py` & `auto-editor-24.9.1/auto_editor/timeline.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/utils/bar.py` & `auto-editor-24.9.1/auto_editor/utils/bar.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/utils/container.py` & `auto-editor-24.9.1/auto_editor/utils/container.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/utils/encoder.py` & `auto-editor-24.9.1/auto_editor/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/utils/func.py` & `auto-editor-24.9.1/auto_editor/utils/func.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/utils/log.py` & `auto-editor-24.9.1/auto_editor/utils/log.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/utils/types.py` & `auto-editor-24.9.1/auto_editor/utils/types.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/validate_input.py` & `auto-editor-24.9.1/auto_editor/validate_input.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/vanparse.py` & `auto-editor-24.9.1/auto_editor/vanparse.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor/wavfile.py` & `auto-editor-24.9.1/auto_editor/wavfile.py`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/auto_editor.egg-info/PKG-INFO` & `auto-editor-24.9.1/auto_editor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-editor
-Version: 24.7.1
+Version: 24.9.1
 Summary: Auto-Editor: Effort free video editing!
 Author-email: WyattBlue <wyattblue@auto-editor.com>
 License: Unlicense
 Project-URL: Bug Tracker, https://github.com/WyattBlue/auto-editor/issues
 Project-URL: Source Code, https://github.com/WyattBlue/auto-editor
 Project-URL: homepage, https://auto-editor.com
 Keywords: video,audio,media,editor,editing,processing,nonlinear,automatic,silence-detect,silence-removal,silence-speedup,motion-detection
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auto-editor Version: 24.7.1 Summary: Auto-Editor:
+Metadata-Version: 2.1 Name: auto-editor Version: 24.9.1 Summary: Auto-Editor:
 Effort free video editing! Author-email: WyattBlue
 auto-editor.com> License: Unlicense Project-URL: Bug Tracker, https://
 github.com/WyattBlue/auto-editor/issues Project-URL: Source Code, https://
 github.com/WyattBlue/auto-editor Project-URL: homepage, https://auto-editor.com
 Keywords:
 video,audio,media,editor,editing,processing,nonlinear,automatic,silence-
 detect,silence-removal,silence-speedup,motion-detection Requires-Python: >=3.10
```

### Comparing `auto-editor-24.7.1/auto_editor.egg-info/SOURCES.txt` & `auto-editor-24.9.1/auto_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-editor-24.7.1/pyproject.toml` & `auto-editor-24.9.1/pyproject.toml`

 * *Files identical despite different names*

