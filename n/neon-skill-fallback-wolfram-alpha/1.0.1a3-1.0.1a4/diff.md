# Comparing `tmp/neon-skill-fallback_wolfram_alpha-1.0.1a3.tar.gz` & `tmp/neon-skill-fallback_wolfram_alpha-1.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-fallback_wolfram_alpha-1.0.1a3.tar", last modified: Tue Mar 26 17:30:23 2024, max compression
+gzip compressed data, was "neon-skill-fallback_wolfram_alpha-1.0.1a4.tar", last modified: Tue Apr  2 19:16:56 2024, max compression
```

## Comparing `neon-skill-fallback_wolfram_alpha-1.0.1a3.tar` & `neon-skill-fallback_wolfram_alpha-1.0.1a4.tar`

### file list

```diff
@@ -1,225 +1,225 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.204139 neon-skill-fallback_wolfram_alpha-1.0.1a3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-26 17:30:23.204139 neon-skill-fallback_wolfram_alpha-1.0.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10179 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.176139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.180139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ca-es/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ca-es/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ca-es/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ca-es/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ca-es/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.180139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/cs-cz/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/cs-cz/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/cs-cz/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/cs-cz/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/cs-cz/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.180139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/da-dk/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/da-dk/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/da-dk/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/da-dk/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/da-dk/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/da-dk/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.184139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/de-de/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/de-de/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/de-de/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/de-de/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/de-de/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.184139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/el-gr/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/el-gr/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/el-gr/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/el-gr/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/el-gr/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/el-gr/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.184139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/en-us/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/en-us/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/en-us/no.email.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/en-us/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/en-us/no.response.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/en-us/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/en-us/response.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/en-us/sent.email.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/en-us/wait.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.184139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/es-es/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/es-es/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/es-es/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/es-es/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/es-es/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.184139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/es-lm/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/es-lm/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/es-lm/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/es-lm/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/es-lm/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/es-lm/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.188139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/fr-fr/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/fr-fr/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/fr-fr/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/fr-fr/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/fr-fr/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.188139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/gl-es/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/gl-es/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/gl-es/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/gl-es/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/gl-es/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/gl-es/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.188139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/it-it/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/it-it/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/it-it/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/it-it/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/it-it/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.188139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/kab-dz/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/kab-dz/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/kab-dz/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/kab-dz/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/kab-dz/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/kab-dz/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.188139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/nl-nl/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/nl-nl/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/nl-nl/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/nl-nl/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/nl-nl/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.192139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/pl-pl/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/pl-pl/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/pl-pl/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/pl-pl/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/pl-pl/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.192139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/pt-br/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/pt-br/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/pt-br/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/pt-br/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/pt-br/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.192139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ro-ro/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ro-ro/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ro-ro/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ro-ro/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ro-ro/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.192139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ru-ru/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ru-ru/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ru-ru/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ru-ru/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/ru-ru/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.192139 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/sv-se/email.body.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/sv-se/email.subject.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/sv-se/no.info.to.send.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/sv-se/not.understood.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/dialog/sv-se/sent.email.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/neon_skill_fallback_wolfram_alpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-26 17:30:23.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/neon_skill_fallback_wolfram_alpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-03-26 17:30:23.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/neon_skill_fallback_wolfram_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 17:30:23.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/neon_skill_fallback_wolfram_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-26 17:30:23.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/neon_skill_fallback_wolfram_alpha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-26 17:30:23.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/neon_skill_fallback_wolfram_alpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-26 17:30:23.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/neon_skill_fallback_wolfram_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.176139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/ca-es/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/cs-cz/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/da-dk/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/da-dk/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/de-de/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/el-gr/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/el-gr/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/en-us/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/es-es/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/es-lm/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/es-lm/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/fr-fr/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/gl-es/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/gl-es/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/it-it/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/kab-dz/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/kab-dz/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/nl-nl/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/pl-dz/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/pl-dz/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/pl-pl/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/pt-br/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/ro-ro/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/ru-ru/list.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/regex/sv-se/list.rx
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 17:30:23.204139 neon-skill-fallback_wolfram_alpha-1.0.1a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/skill.json
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.180139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/ca-es/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/ca-es/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/cs-cz/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/cs-cz/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.196139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/da-dk/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/da-dk/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/da-dk/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.200139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/de-de/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/de-de/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.200139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/el-gr/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/el-gr/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/el-gr/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.200139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/en-us/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/en-us/Request.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/en-us/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.200139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/es-es/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/es-es/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.200139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/es-lm/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/es-lm/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/es-lm/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.200139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/fr-fr/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/fr-fr/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.200139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/gl-es/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/gl-es/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/gl-es/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.200139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/it-it/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/it-it/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.200139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/kab-dz/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/kab-dz/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/kab-dz/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.200139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/nl-nl/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/nl-nl/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.200139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/pl-pl/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/pl-pl/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.200139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/pt-br/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/pt-br/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.200139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/ro-ro/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/ro-ro/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.204139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/ru-ru/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/ru-ru/Source.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 17:30:23.204139 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/sv-se/Give.voc
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-26 17:30:05.000000 neon-skill-fallback_wolfram_alpha-1.0.1a3/vocab/sv-se/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.188007 neon-skill-fallback_wolfram_alpha-1.0.1a4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-02 19:16:56.188007 neon-skill-fallback_wolfram_alpha-1.0.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10179 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.160008 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.168007 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ca-es/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ca-es/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ca-es/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ca-es/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ca-es/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.168007 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/cs-cz/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/cs-cz/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/cs-cz/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/cs-cz/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/cs-cz/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.168007 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/da-dk/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/da-dk/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/da-dk/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/da-dk/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/da-dk/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.168007 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/de-de/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/de-de/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/de-de/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/de-de/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/de-de/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.168007 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/el-gr/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/el-gr/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/el-gr/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/el-gr/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/el-gr/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/el-gr/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.172007 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/en-us/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/en-us/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/en-us/no.email.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/en-us/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/en-us/no.response.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/en-us/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/en-us/response.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/en-us/sent.email.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/en-us/wait.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.172007 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/es-es/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/es-es/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/es-es/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/es-es/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/es-es/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.172007 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/es-lm/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/es-lm/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/es-lm/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/es-lm/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/es-lm/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/es-lm/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.172007 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/fr-fr/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/fr-fr/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/fr-fr/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/fr-fr/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/fr-fr/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.172007 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/gl-es/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/gl-es/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/gl-es/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/gl-es/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/gl-es/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.176008 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/it-it/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/it-it/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/it-it/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/it-it/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/it-it/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.176008 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/kab-dz/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/kab-dz/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/kab-dz/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/kab-dz/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/kab-dz/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/kab-dz/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.176008 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/nl-nl/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/nl-nl/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/nl-nl/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/nl-nl/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/nl-nl/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.176008 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/pl-pl/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/pl-pl/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/pl-pl/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/pl-pl/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/pl-pl/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.176008 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/pt-br/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/pt-br/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/pt-br/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/pt-br/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/pt-br/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.176008 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ro-ro/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ro-ro/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ro-ro/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ro-ro/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ro-ro/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ru-ru/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ru-ru/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ru-ru/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ru-ru/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/ru-ru/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/sv-se/email.body.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/sv-se/email.subject.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/sv-se/no.info.to.send.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/sv-se/not.understood.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/dialog/sv-se/sent.email.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/neon_skill_fallback_wolfram_alpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-02 19:16:56.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/neon_skill_fallback_wolfram_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-04-02 19:16:56.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/neon_skill_fallback_wolfram_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:16:56.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/neon_skill_fallback_wolfram_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 19:16:56.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/neon_skill_fallback_wolfram_alpha.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-02 19:16:56.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/neon_skill_fallback_wolfram_alpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 19:16:56.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/neon_skill_fallback_wolfram_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.164008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/ca-es/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/cs-cz/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/da-dk/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/de-de/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/el-gr/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/el-gr/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/en-us/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/es-es/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/es-lm/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/es-lm/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/fr-fr/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/gl-es/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/it-it/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/kab-dz/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/kab-dz/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/nl-nl/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/pl-dz/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/pl-dz/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/pl-pl/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.180008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/pt-br/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/ro-ro/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/ru-ru/list.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/regex/sv-se/list.rx
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:16:56.188007 neon-skill-fallback_wolfram_alpha-1.0.1a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/skill.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.164008 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/ca-es/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/ca-es/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/cs-cz/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/cs-cz/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/da-dk/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/da-dk/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/de-de/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/de-de/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/el-gr/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/el-gr/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/el-gr/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/en-us/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/en-us/Request.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/en-us/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/es-es/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/es-es/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/es-lm/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/es-lm/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/es-lm/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/fr-fr/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/fr-fr/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/gl-es/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/gl-es/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/it-it/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/it-it/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/kab-dz/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/kab-dz/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/kab-dz/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.184008 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/nl-nl/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/nl-nl/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.188007 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/pl-pl/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/pl-pl/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.188007 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/pt-br/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/pt-br/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.188007 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/ro-ro/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/ro-ro/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.188007 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/ru-ru/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/ru-ru/Source.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:56.188007 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/sv-se/Give.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 19:16:40.000000 neon-skill-fallback_wolfram_alpha-1.0.1a4/vocab/sv-se/Source.voc
```

### Comparing `neon-skill-fallback_wolfram_alpha-1.0.1a3/LICENSE` & `neon-skill-fallback_wolfram_alpha-1.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_wolfram_alpha-1.0.1a3/LICENSE.md` & `neon-skill-fallback_wolfram_alpha-1.0.1a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_wolfram_alpha-1.0.1a3/PKG-INFO` & `neon-skill-fallback_wolfram_alpha-1.0.1a4/neon_skill_fallback_wolfram_alpha.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: neon-skill-fallback_wolfram_alpha
-Version: 1.0.1a3
+Name: neon-skill-fallback-wolfram-alpha
+Version: 1.0.1a4
 Home-page: https://github.com/NeonGeckoCom/skill-fallback_wolfram_alpha
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
@@ -13,20 +13,22 @@
 
 ## Summary
 
 General knowledge fallback handler based on [Wolfram Alpha](https://wolframalpha.com) services
 
 ## Description
 
-Answers general knowledge, math, and definition questions by using Wolfram Alpha Api services. If the user is interested in knowing where the information for the spoken answer came from, Neon can send the most recent source of the spoken details to user’s email.
-Responses are cached and saved for later use.
-
-Use of this skill requires use of third-party APIs. If you do not have access to Neon API servers, you may access the
-Wolfram|Alpha API directly by providing a key in `~/wolfram.txt`. You can generate a Wolfram|Alpha key
-[here](https://developer.wolframalpha.com/portal/myapps/).
+Answers general knowledge, math, and definition questions by using Wolfram Alpha
+API services. If the user is interested in knowing where the information for the
+spoken answer came from, Neon can send the most recent source of the spoken 
+details to user’s email.
+
+Use of this skill requires use of third-party APIs. This skill will use Neon AI
+servers by default, but you can deploy your own instance of 
+[Diana](https://github.com/NeonGeckoCom/neon-diana-utils).
 
 ## Examples
 
 Ask Neon any questions starting with `What`, `Why`, or `How`
 - What is 2 + 2?
 - Who won best picture in 2006?
 - How far away is the moon?
```

### Comparing `neon-skill-fallback_wolfram_alpha-1.0.1a3/README.md` & `neon-skill-fallback_wolfram_alpha-1.0.1a4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 
 ## Summary
 
 General knowledge fallback handler based on [Wolfram Alpha](https://wolframalpha.com) services
 
 ## Description
 
-Answers general knowledge, math, and definition questions by using Wolfram Alpha Api services. If the user is interested in knowing where the information for the spoken answer came from, Neon can send the most recent source of the spoken details to user’s email.
-Responses are cached and saved for later use.
-
-Use of this skill requires use of third-party APIs. If you do not have access to Neon API servers, you may access the
-Wolfram|Alpha API directly by providing a key in `~/wolfram.txt`. You can generate a Wolfram|Alpha key
-[here](https://developer.wolframalpha.com/portal/myapps/).
+Answers general knowledge, math, and definition questions by using Wolfram Alpha
+API services. If the user is interested in knowing where the information for the
+spoken answer came from, Neon can send the most recent source of the spoken 
+details to user’s email.
+
+Use of this skill requires use of third-party APIs. This skill will use Neon AI
+servers by default, but you can deploy your own instance of 
+[Diana](https://github.com/NeonGeckoCom/neon-diana-utils).
 
 ## Examples
 
 Ask Neon any questions starting with `What`, `Why`, or `How`
 - What is 2 + 2?
 - Who won best picture in 2006?
 - How far away is the moon?
```

### Comparing `neon-skill-fallback_wolfram_alpha-1.0.1a3/__init__.py` & `neon-skill-fallback_wolfram_alpha-1.0.1a4/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_wolfram_alpha-1.0.1a3/neon_skill_fallback_wolfram_alpha.egg-info/PKG-INFO` & `neon-skill-fallback_wolfram_alpha-1.0.1a4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: neon-skill-fallback-wolfram-alpha
-Version: 1.0.1a3
+Name: neon-skill-fallback_wolfram_alpha
+Version: 1.0.1a4
 Home-page: https://github.com/NeonGeckoCom/skill-fallback_wolfram_alpha
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
@@ -13,20 +13,22 @@
 
 ## Summary
 
 General knowledge fallback handler based on [Wolfram Alpha](https://wolframalpha.com) services
 
 ## Description
 
-Answers general knowledge, math, and definition questions by using Wolfram Alpha Api services. If the user is interested in knowing where the information for the spoken answer came from, Neon can send the most recent source of the spoken details to user’s email.
-Responses are cached and saved for later use.
-
-Use of this skill requires use of third-party APIs. If you do not have access to Neon API servers, you may access the
-Wolfram|Alpha API directly by providing a key in `~/wolfram.txt`. You can generate a Wolfram|Alpha key
-[here](https://developer.wolframalpha.com/portal/myapps/).
+Answers general knowledge, math, and definition questions by using Wolfram Alpha
+API services. If the user is interested in knowing where the information for the
+spoken answer came from, Neon can send the most recent source of the spoken 
+details to user’s email.
+
+Use of this skill requires use of third-party APIs. This skill will use Neon AI
+servers by default, but you can deploy your own instance of 
+[Diana](https://github.com/NeonGeckoCom/neon-diana-utils).
 
 ## Examples
 
 Ask Neon any questions starting with `What`, `Why`, or `How`
 - What is 2 + 2?
 - Who won best picture in 2006?
 - How far away is the moon?
```

### Comparing `neon-skill-fallback_wolfram_alpha-1.0.1a3/neon_skill_fallback_wolfram_alpha.egg-info/SOURCES.txt` & `neon-skill-fallback_wolfram_alpha-1.0.1a4/neon_skill_fallback_wolfram_alpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_wolfram_alpha-1.0.1a3/setup.py` & `neon-skill-fallback_wolfram_alpha-1.0.1a4/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-fallback_wolfram_alpha-1.0.1a3/skill.json` & `neon-skill-fallback_wolfram_alpha-1.0.1a4/skill.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'description'": "'Answers general knowledge, math, and definition questions by using Wolfram "*

 * *                  'Alpha API services. If the user is interested in knowing where the information '*

 * *                  'for the spoken answer came from, Neon can send the most recent source of the '*

 * *                  'spoken details to user’s email. Use of this skill requires use of third-party '*

 * *                  'APIs. This skill will use Neon AI servers by default, but you can deploy your '*

 * *                  " […]*

```diff
@@ -4,15 +4,15 @@
     "categories": [],
     "category": "",
     "credits": [
         "Mycroft AI",
         "NeonDaniel",
         "reginaneon"
     ],
-    "description": "Answers general knowledge, math, and definition questions by using Wolfram Alpha Api services. If the user is interested in knowing where the information for the spoken answer came from, Neon can send the most recent source of the spoken details to user\u2019s email. Responses are cached and saved for later use. Use of this skill requires use of third-party APIs. If you do not have access to Neon API servers, you may access the Wolfram|Alpha API directly by providing a key in `~/wolfram.txt`. You can generate a Wolfram|Alpha key [here](https://developer.wolframalpha.com/portal/myapps/).",
+    "description": "Answers general knowledge, math, and definition questions by using Wolfram Alpha API services. If the user is interested in knowing where the information for the spoken answer came from, Neon can send the most recent source of the spoken details to user\u2019s email. Use of this skill requires use of third-party APIs. This skill will use Neon AI servers by default, but you can deploy your own instance of [Diana](https://github.com/NeonGeckoCom/neon-diana-utils).",
     "desktopFile": false,
     "examples": [
         "What is 2 + 2?",
         "Who won best picture in 2006?",
         "How far away is the moon?",
         "Send me the source for that."
     ],
```

### Comparing `neon-skill-fallback_wolfram_alpha-1.0.1a3/version.py` & `neon-skill-fallback_wolfram_alpha-1.0.1a4/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a3"
+__version__ = "1.0.1a4"
```

