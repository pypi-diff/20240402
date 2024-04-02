# Comparing `tmp/neon-skill-speak-2.0.1a1.tar.gz` & `tmp/neon-skill-speak-2.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-speak-2.0.1a1.tar", last modified: Mon Feb  5 23:13:21 2024, max compression
+gzip compressed data, was "neon-skill-speak-2.0.1a2.tar", last modified: Tue Apr  2 19:49:57 2024, max compression
```

## Comparing `neon-skill-speak-2.0.1a1.tar` & `neon-skill-speak-2.0.1a2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.643104 neon-skill-speak-2.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-02-05 23:13:21.643104 neon-skill-speak-2.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.635105 neon-skill-speak-2.0.1a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/ca-es/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/cs-cz/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/da-dk/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/da-dk/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/de-de/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/el-gr/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/el-gr/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/en-us/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/es-es/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/es-lm/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/es-lm/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/eu-eu/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/eu-eu/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/fa-ir/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/fa-ir/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/fr-fr/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/ga-ie/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/ga-ie/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/gl-es/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/gl-es/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/hu-hu/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/hu-hu/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/it-it/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/kab-dz/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/kab-dz/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/nl-nl/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/pl-pl/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/pt-br/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/ro-ro/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/ru-ru/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/sv-se/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.639104 neon-skill-speak-2.0.1a1/locale/tr-tr/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/locale/tr-tr/speak.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:13:21.643104 neon-skill-speak-2.0.1a1/neon_skill_speak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-02-05 23:13:21.000000 neon-skill-speak-2.0.1a1/neon_skill_speak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-05 23:13:21.000000 neon-skill-speak-2.0.1a1/neon_skill_speak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 23:13:21.000000 neon-skill-speak-2.0.1a1/neon_skill_speak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-05 23:13:21.000000 neon-skill-speak-2.0.1a1/neon_skill_speak.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-05 23:13:21.000000 neon-skill-speak-2.0.1a1/neon_skill_speak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-05 23:13:21.000000 neon-skill-speak-2.0.1a1/neon_skill_speak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 23:13:21.643104 neon-skill-speak-2.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/skill.json
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-05 23:13:17.000000 neon-skill-speak-2.0.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.724221 neon-skill-speak-2.0.1a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.724221 neon-skill-speak-2.0.1a2/locale/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/ca-es/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.724221 neon-skill-speak-2.0.1a2/locale/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/cs-cz/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.724221 neon-skill-speak-2.0.1a2/locale/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/da-dk/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.724221 neon-skill-speak-2.0.1a2/locale/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/de-de/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.724221 neon-skill-speak-2.0.1a2/locale/el-gr/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/el-gr/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.724221 neon-skill-speak-2.0.1a2/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/en-us/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.724221 neon-skill-speak-2.0.1a2/locale/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/es-es/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/es-lm/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/es-lm/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/eu-eu/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/eu-eu/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/fa-ir/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/fa-ir/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/fr-fr/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/ga-ie/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/ga-ie/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/gl-es/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/hu-hu/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/hu-hu/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/it-it/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/kab-dz/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/kab-dz/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/nl-nl/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/pl-pl/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/pt-br/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/ro-ro/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/ru-ru/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/sv-se/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/locale/tr-tr/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/locale/tr-tr/speak.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/neon_skill_speak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-02 19:49:57.000000 neon-skill-speak-2.0.1a2/neon_skill_speak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-02 19:49:57.000000 neon-skill-speak-2.0.1a2/neon_skill_speak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:49:57.000000 neon-skill-speak-2.0.1a2/neon_skill_speak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-02 19:49:57.000000 neon-skill-speak-2.0.1a2/neon_skill_speak.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 19:49:57.000000 neon-skill-speak-2.0.1a2/neon_skill_speak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 19:49:57.000000 neon-skill-speak-2.0.1a2/neon_skill_speak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:49:57.728221 neon-skill-speak-2.0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/skill.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-02 19:49:53.000000 neon-skill-speak-2.0.1a2/version.py
```

### Comparing `neon-skill-speak-2.0.1a1/LICENSE` & `neon-skill-speak-2.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-speak-2.0.1a1/LICENSE.md` & `neon-skill-speak-2.0.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-speak-2.0.1a1/PKG-INFO` & `neon-skill-speak-2.0.1a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-speak
-Version: 2.0.1a1
+Version: 2.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-speak
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `neon-skill-speak-2.0.1a1/README.md` & `neon-skill-speak-2.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-speak-2.0.1a1/__init__.py` & `neon-skill-speak-2.0.1a2/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-speak-2.0.1a1/neon_skill_speak.egg-info/PKG-INFO` & `neon-skill-speak-2.0.1a2/neon_skill_speak.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-speak
-Version: 2.0.1a1
+Version: 2.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-speak
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `neon-skill-speak-2.0.1a1/neon_skill_speak.egg-info/SOURCES.txt` & `neon-skill-speak-2.0.1a2/neon_skill_speak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-speak-2.0.1a1/setup.py` & `neon-skill-speak-2.0.1a2/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-speak-2.0.1a1/skill.json` & `neon-skill-speak-2.0.1a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-speak-2.0.1a1/version.py` & `neon-skill-speak-2.0.1a2/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.0.1a1"
+__version__ = "2.0.1a2"
```

