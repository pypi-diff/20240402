# Comparing `tmp/foss-flame-0.19.8.tar.gz` & `tmp/foss-flame-0.19.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foss-flame-0.19.8.tar", last modified: Thu Feb  1 13:27:20 2024, max compression
+gzip compressed data, was "foss-flame-0.19.9.tar", last modified: Fri Feb  2 15:20:07 2024, max compression
```

## Comparing `foss-flame-0.19.8.tar` & `foss-flame-0.19.9.tar`

### file list

```diff
@@ -1,233 +1,233 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:27:20.480334 foss-flame-0.19.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:27:20.444335 foss-flame-0.19.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-01 13:27:09.000000 foss-flame-0.19.8/LICENSES/BSD-2-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17023 2024-02-01 13:27:09.000000 foss-flame-0.19.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34674 2024-02-01 13:27:09.000000 foss-flame-0.19.8/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-01 13:27:09.000000 foss-flame-0.19.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-02-01 13:27:20.480334 foss-flame-0.19.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-02-01 13:27:09.000000 foss-flame-0.19.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:27:20.448335 foss-flame-0.19.8/flame/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8700 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-01 13:27:20.000000 foss-flame-0.19.8/flame/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    13977 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    24314 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/license_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:27:20.448335 foss-flame-0.19.8/flame/var/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/license_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:27:20.476334 foss-flame-0.19.8/flame/var/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/0BSD.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/0BSD.json
--rw-r--r--   0 runner    (1001) docker     (127)    34639 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/AGPL-3.0-only.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/AGPL-3.0-only.json
--rw-r--r--   0 runner    (1001) docker     (127)    35156 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/AGPL-3.0-or-later.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/AGPL-3.0-or-later.json
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Apache-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Apache-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Apache-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Apache-1.1.json
--rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Apache-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Artistic-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Artistic-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Artistic-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Artistic-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/BSD-2-Clause.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/BSD-2-Clause.json
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/BSD-3-Clause.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/BSD-3-Clause.json
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/BSD-4-Clause-UC.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/BSD-4-Clause-UC.json
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/BSD-4-Clause.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/BSD-4-Clause.json
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/BSL-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/BSL-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Beerware.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Beerware.json
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/BlueOak-1.0.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/BlueOak-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    19466 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CC-BY-3.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CC-BY-3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CC-BY-4.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CC-BY-4.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CC-BY-SA-2.5.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CC-BY-SA-2.5.json
--rw-r--r--   0 runner    (1001) docker     (127)    22239 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CC-BY-SA-3.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CC-BY-SA-3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    20131 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CC-BY-SA-4.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CC-BY-SA-4.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CC0-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CC0-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    16768 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CDDL-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CDDL-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    17212 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CDDL-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/CDDL-1.1.json
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Classpath-exception-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Classpath-exception-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/EPL-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/EPL-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    14148 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/EPL-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/EPL-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/EUPL-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/EUPL-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    13133 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/EUPL-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/EUPL-1.1.json
--rw-r--r--   0 runner    (1001) docker     (127)    12796 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/EUPL-1.2.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/EUPL-1.2.json
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/FTL.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/FTL.json
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/GCC-exception-3.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/GCC-exception-3.1.json
--rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/GPL-1.0-only.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/GPL-1.0-only.json
--rw-r--r--   0 runner    (1001) docker     (127)    13277 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/GPL-1.0-or-later.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/GPL-1.0-or-later.json
--rw-r--r--   0 runner    (1001) docker     (127)    18149 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/GPL-2.0-only.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/GPL-2.0-only.json
--rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/GPL-2.0-or-later.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/GPL-2.0-or-later.json
--rw-r--r--   0 runner    (1001) docker     (127)    35269 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/GPL-3.0-only.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/GPL-3.0-only.json
--rw-r--r--   0 runner    (1001) docker     (127)    35762 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/GPL-3.0-or-later.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/GPL-3.0-or-later.json
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/HPND.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/HPND.json
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/ICU.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/ICU.json
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/IJG.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/IJG.json
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/ISC.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/ISC.json
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/JSON.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/JSON.json
--rw-r--r--   0 runner    (1001) docker     (127)    25372 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LGPL-2.0-only.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LGPL-2.0-only.json
--rw-r--r--   0 runner    (1001) docker     (127)    26075 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LGPL-2.0-or-later.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LGPL-2.0-or-later.json
--rw-r--r--   0 runner    (1001) docker     (127)    26613 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LGPL-2.1-only.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LGPL-2.1-only.json
--rw-r--r--   0 runner    (1001) docker     (127)    27235 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LGPL-2.1-or-later.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LGPL-2.1-or-later.json
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LGPL-3.0-only.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LGPL-3.0-only.json
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LGPL-3.0-or-later.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LGPL-3.0-or-later.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Latex2e.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Latex2e.json
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Libpng.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Libpng.json
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LicenseRef-scancode-docbook.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LicenseRef-scancode-docbook.json
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LicenseRef-scancode-iso-8879.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LicenseRef-scancode-iso-8879.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LicenseRef-scancode-public-domain.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LicenseRef-scancode-public-domain.json
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LicenseRef-scancode-wtfpl-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LicenseRef-scancode-wtfpl-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LicenseRef-scancode-zpl-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/LicenseRef-scancode-zpl-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MIT-0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MIT-0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MIT-advertising.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MIT-advertising.json
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MIT-open-group.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MIT-open-group.json
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MIT.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MIT.json
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MITNFA.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MITNFA.json
--rw-r--r--   0 runner    (1001) docker     (127)    17912 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MPL-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MPL-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    23255 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MPL-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MPL-1.1.json
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MPL-2.0-no-copyleft-exception.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MPL-2.0-no-copyleft-exception.json
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MPL-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/MPL-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/NCSA.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/NCSA.json
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/NTP.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/NTP.json
--rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/ODC-By-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/ODC-By-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/OFL-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/OFL-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/OFL-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/OFL-1.1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/OML.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/OML.json
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/OpenSSL.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/OpenSSL.json
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Plexus.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Plexus.json
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/PostgreSQL.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/PostgreSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Python-2.0.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Python-2.0.1.json
--rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Python-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Python-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/RSA-MD.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/RSA-MD.json
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/SAX-PD.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/SAX-PD.json
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/SGI-B-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/SGI-B-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    30608 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/SSPL-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/SSPL-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/SWL.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/SWL.json
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Sendmail.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Sendmail.json
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/TCL.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/TCL.json
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/TU-Berlin-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/TU-Berlin-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/TU-Berlin-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/TU-Berlin-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Unlicense.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Unlicense.json
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Vim.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Vim.json
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/W3C.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/W3C.json
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/WTFPL.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/WTFPL.json
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/X11-distribute-modifications-variant.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/X11-distribute-modifications-variant.json
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/X11.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/X11.json
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/ZPL-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/ZPL-1.1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/ZPL-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/ZPL-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/ZPL-2.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/ZPL-2.1.json
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Zlib.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/Zlib.json
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/ambiguities.json
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/blessing.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/blessing.json
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/bzip2-1.0.6.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/bzip2-1.0.6.json
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/compounds.json
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/curl.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/curl.json
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/duals.json
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/libpng-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/libpng-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/libtiff.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/libtiff.json
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/x11-keith-packard.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/licenses/x11-keith-packard.json
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-01 13:27:09.000000 foss-flame-0.19.8/flame/var/operators.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:27:20.480334 foss-flame-0.19.8/foss_flame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-02-01 13:27:20.000000 foss-flame-0.19.8/foss_flame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-02-01 13:27:20.000000 foss-flame-0.19.8/foss_flame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 13:27:20.000000 foss-flame-0.19.8/foss_flame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-01 13:27:20.000000 foss-flame-0.19.8/foss_flame.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-01 13:27:20.000000 foss-flame-0.19.8/foss_flame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-01 13:27:20.000000 foss-flame-0.19.8/foss_flame.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-01 13:27:09.000000 foss-flame-0.19.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-01 13:27:09.000000 foss-flame-0.19.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-02-01 13:27:20.480334 foss-flame-0.19.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-01 13:27:09.000000 foss-flame-0.19.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:20:07.302974 foss-flame-0.19.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:20:07.270974 foss-flame-0.19.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-02 15:19:54.000000 foss-flame-0.19.9/LICENSES/BSD-2-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17023 2024-02-02 15:19:54.000000 foss-flame-0.19.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34674 2024-02-02 15:19:54.000000 foss-flame-0.19.9/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-02 15:19:54.000000 foss-flame-0.19.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-02-02 15:20:07.302974 foss-flame-0.19.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-02-02 15:19:54.000000 foss-flame-0.19.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:20:07.270974 foss-flame-0.19.9/flame/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8700 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-02-02 15:20:07.000000 foss-flame-0.19.9/flame/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14047 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24541 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/license_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:20:07.270974 foss-flame-0.19.9/flame/var/
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/ambiguities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/compounds.json
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/duals.json
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/license_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:20:07.302974 foss-flame-0.19.9/flame/var/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/0BSD.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/0BSD.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34639 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-only.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-only.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35156 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-or-later.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-or-later.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Apache-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Apache-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Apache-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Apache-1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Apache-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Artistic-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Artistic-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Artistic-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Artistic-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-2-Clause.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-2-Clause.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-3-Clause.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-3-Clause.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-4-Clause-UC.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-4-Clause-UC.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-4-Clause.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-4-Clause.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Beerware.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Beerware.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BlueOak-1.0.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BlueOak-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19466 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-3.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-4.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-4.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-2.5.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-2.5.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22239 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-3.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20131 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-4.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-4.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC0-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC0-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16768 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CDDL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CDDL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17212 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CDDL-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CDDL-1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Classpath-exception-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Classpath-exception-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EPL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EPL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14148 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EPL-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EPL-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EUPL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EUPL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13133 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EUPL-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EUPL-1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12796 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EUPL-1.2.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EUPL-1.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/FTL.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/FTL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GCC-exception-3.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GCC-exception-3.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-1.0-only.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-1.0-only.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13277 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-1.0-or-later.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-1.0-or-later.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18149 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-2.0-only.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-2.0-only.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-2.0-or-later.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-2.0-or-later.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35269 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-3.0-only.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-3.0-only.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35762 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-3.0-or-later.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-3.0-or-later.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/HPND.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/HPND.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ICU.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ICU.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/IJG.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/IJG.json
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ISC.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ISC.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/JSON.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/JSON.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25372 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.0-only.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.0-only.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26075 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.0-or-later.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.0-or-later.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26613 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-only.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-only.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27235 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-or-later.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-or-later.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-only.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-only.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-or-later.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-or-later.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Latex2e.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Latex2e.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Libpng.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Libpng.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-docbook.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-docbook.json
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-iso-8879.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-iso-8879.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-public-domain.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-public-domain.json
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-wtfpl-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-wtfpl-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-zpl-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-zpl-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT-0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT-0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT-advertising.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT-advertising.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT-open-group.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT-open-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MITNFA.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MITNFA.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17912 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23255 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-2.0-no-copyleft-exception.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-2.0-no-copyleft-exception.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/NCSA.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/NCSA.json
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/NTP.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/NTP.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ODC-By-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ODC-By-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OFL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OFL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OFL-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OFL-1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OML.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OML.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OpenSSL.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OpenSSL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Plexus.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Plexus.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/PostgreSQL.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/PostgreSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Python-2.0.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Python-2.0.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Python-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Python-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/RSA-MD.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/RSA-MD.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SAX-PD.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SAX-PD.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SGI-B-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SGI-B-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30608 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SSPL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SSPL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SWL.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SWL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Sendmail.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Sendmail.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/TCL.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/TCL.json
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/TU-Berlin-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/TU-Berlin-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/TU-Berlin-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/TU-Berlin-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Unlicense.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Unlicense.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Vim.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Vim.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/W3C.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/W3C.json
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/WTFPL.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/WTFPL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/X11-distribute-modifications-variant.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/X11-distribute-modifications-variant.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/X11.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/X11.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ZPL-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ZPL-1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ZPL-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ZPL-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ZPL-2.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ZPL-2.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Zlib.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Zlib.json
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/blessing.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/blessing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/bzip2-1.0.6.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/bzip2-1.0.6.json
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/curl.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/curl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/libpng-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/libpng-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/libtiff.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/libtiff.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/x11-keith-packard.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/x11-keith-packard.json
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/operators.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:20:07.302974 foss-flame-0.19.9/foss_flame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-02-02 15:20:07.000000 foss-flame-0.19.9/foss_flame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-02-02 15:20:07.000000 foss-flame-0.19.9/foss_flame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 15:20:07.000000 foss-flame-0.19.9/foss_flame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-02 15:20:07.000000 foss-flame-0.19.9/foss_flame.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-02 15:20:07.000000 foss-flame-0.19.9/foss_flame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-02 15:20:07.000000 foss-flame-0.19.9/foss_flame.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-02 15:19:54.000000 foss-flame-0.19.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-02 15:19:54.000000 foss-flame-0.19.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-02-02 15:20:07.302974 foss-flame-0.19.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-02 15:19:54.000000 foss-flame-0.19.9/setup.py
```

### Comparing `foss-flame-0.19.8/LICENSES/BSD-2-Clause.txt` & `foss-flame-0.19.9/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/LICENSES/CC-BY-4.0.txt` & `foss-flame-0.19.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/LICENSES/GPL-3.0-or-later.txt` & `foss-flame-0.19.9/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/PKG-INFO` & `foss-flame-0.19.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foss-flame
-Version: 0.19.8
+Version: 0.19.9
 Summary: FOSS License Additional Metadata
 Home-page: https://github.com/hesa/license-db
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `foss-flame-0.19.8/README.md` & `foss-flame-0.19.9/README.md`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/__main__.py` & `foss-flame-0.19.9/flame/__main__.py`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/config.py` & `foss-flame-0.19.9/flame/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import json
 import logging
 import os
 import flame.exception
 
-SW_VERSION = '0.19.8'
+SW_VERSION = '0.19.9'
 
 PYTHON_DIR = os.path.dirname(os.path.realpath(__file__))
 VAR_DIR = os.path.join(PYTHON_DIR, 'var')
 LICENSE_DIR = os.path.join(VAR_DIR, 'licenses')
 
 LICENSE_SCHEMA_FILE = os.path.join(VAR_DIR, 'license_schema.json')
 LICENSE_OPERATORS_FILE = os.path.join(VAR_DIR, 'operators.json')
+LICENSE_COMPUNDS_FILE = os.path.join(VAR_DIR, 'compounds.json')
+LICENSE_AMBIG_FILE = os.path.join(VAR_DIR, 'ambiguities.json')
+LICENSE_DUALS_FILE = os.path.join(VAR_DIR, 'duals.json')
 
 DESCRIPTION = """
 NAME
   flame (FOSS License Additional Metadata) is a python API and
   command line tool
 
 DESCRIPTION
```

### Comparing `foss-flame-0.19.8/flame/format.py` & `foss-flame-0.19.9/flame/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,18 +54,19 @@
         :raise FlameException: if compat is not valid
         :return: formatted string
         :rtype: str
 
         :Example:
 
         >>> from flame.license_db import FossLicenses
+        >>> from flame.format import OutputFormatterFactory
         >>> fl = FossLicenses()
         >>> compat = fl.expression_compatibility_as('x11-keith-packard')
         >>> formatter = OutputFormatterFactory.formatter("TEXT")
-        >>> formatted = formatter.format_compatibilities(compat)
+        >>> formatted, warnings = formatter.format_compatibilities(compat)
         >>> print(formatted)
         HPND
         """
         return None, None
 
     def format_compat_list(self, all_compats, verbose=False):
         """
```

### Comparing `foss-flame-0.19.8/flame/license_db.py` & `foss-flame-0.19.9/flame/license_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import collections
 import glob
 import json
 import logging
-import os
 import re
 from pathlib import Path
 import license_expression
 from enum import Enum
 
-from flame.config import LICENSE_DIR, LICENSE_OPERATORS_FILE, LICENSE_SCHEMA_FILE, read_config
+from flame.config import LICENSE_DIR, LICENSE_SCHEMA_FILE, read_config
+from flame.config import LICENSE_OPERATORS_FILE, LICENSE_COMPUNDS_FILE, LICENSE_AMBIG_FILE, LICENSE_DUALS_FILE
+
 from flame.exception import FlameException
 from jsonschema import validate
 
 import osadl_matrix
 
 json_schema = None
 
@@ -73,14 +74,15 @@
         config_from_file.update((k, v) for k, v in config.items() if v is not None)
         config = config_from_file
 
         check = config.get('check', False)
         logging_level = self.__str_to_loggin_info(config)
         logging.basicConfig(level=logging_level)
 
+        self.config = config
         self.license_dir = config.get('license-dir', LICENSE_DIR)
         self.additional_license_dir = config.get('additional-license-dir', [])
         self.__init_license_db(check)
         self.supported_licenses = None
         self.compat_cache = {}
         self.license_cache = {}
 
@@ -131,63 +133,78 @@
         license_dirs = [self.license_dir]
         self.ambiguities = {'ambiguities': [], 'aliases': {}}
 
         if self.additional_license_dir:
             license_dirs.append(self.additional_license_dir)
         for license_dir in license_dirs:
             for license_file in glob.glob(f'{license_dir}/*.json'):
-                logging.debug(f' * {license_file}')
-                if os.path.basename(license_file) == 'ambiguities.json':
-                    logging.debug(f' * ambiguities file: {license_file}')
-                    data = self.__read_json(f'{license_dir}/ambiguities.json')
-                    data['aliases'] = {}
-
-                    for k, v in data['ambiguities'].items():
-                        # for quicker lookups, add 'aliases' which is the reverse of
-                        # the aliases per license I.e a quicker lookup table when
-                        # identifying ambiguous licenses
-                        for alias in v['aliases']:
-                            data['aliases'][alias] = k
-                        data['aliases'][k] = k
-                    self.ambiguities = data
-
-                elif os.path.basename(license_file) == 'compounds.json':
-                    # some compound licenses are incorrectly stated as
-                    # one, e.g. "GPL-2.0-with-classpath-exception" which
-                    # should be "GPL-2.0-only WITH
-                    # Classpath-exception-2.0". This file provides
-                    # translations for such
-                    data = self.__read_json(license_file)
-                    for compound in data[COMPOUNDS_TAG]:
-                        licenses[compound['spdxid']] = compound
-                        for alias in compound[FLAME_ALIASES_TAG]:
-                            if alias in aliases:
-                                raise FlameException(f'Alias "{alias}" -> {compound["spdxid"]} already defined as "{aliases[alias]}".')
-
-                            aliases[alias] = compound['spdxid']
-                elif os.path.basename(license_file) == 'duals.json':
-                    # Read license with built-in dual feature, e.g
-                    # "GPL-2.0-or-later" which can be seen as a dual
-                    # license "GPL-2.0-only OR GPL-3.0-only"
-                    data = self.__read_json(license_file)
-                    for dual in data[DUAL_LICENSES_TAG]:
-                        duals[dual['spdxid']] = dual
-                else:
-                    data = self.__read_license_file(license_file, check)
-                    licenses[data['spdxid']] = data
-                    for alias in data[FLAME_ALIASES_TAG]:
-                        if alias in aliases:
-                            raise FlameException(f'Alias "{alias}" -> {data["spdxid"]} already defined as "{aliases[alias]}".')
+                if "duals" in license_file:
+                    continue
+                if "compounds" in license_file:
+                    continue
+                if "ambig" in license_file:
+                    continue
+                logging.debug(f'license_file: {license_file}')
+                data = self.__read_license_file(license_file, check)
+                licenses[data['spdxid']] = data
+                for alias in data[FLAME_ALIASES_TAG]:
+                    if alias in aliases:
+                        raise FlameException(f'Alias "{alias}" -> {data["spdxid"]} already defined as "{aliases[alias]}".')
 
-                        aliases[alias] = data['spdxid']
+                    aliases[alias] = data['spdxid']
                 if SCANCODE_KEY_TAG in data:
                     scancode_keys[data[SCANCODE_KEY_TAG]] = data['spdxid']
                 if COMPATIBILITY_AS_TAG in data:
                     compats[data['spdxid']] = data[COMPATIBILITY_AS_TAG]
 
+        # Ambiguous licenses
+        ambig_file = self.config.get('ambiguity_file', LICENSE_AMBIG_FILE)
+        logging.debug(f' * ambiguities file: {ambig_file}')
+        data = self.__read_json(ambig_file)
+        data['aliases'] = {}
+
+        for k, v in data['ambiguities'].items():
+            # for quicker lookups, add 'aliases' which is the reverse of
+            # the aliases per license I.e a quicker lookup table when
+            # identifying ambiguous licenses
+            for alias in v['aliases']:
+                data['aliases'][alias] = k
+            data['aliases'][k] = k
+        self.ambiguities = data
+
+        # Compound licenses
+        # some compound licenses are incorrectly stated as
+        # one, e.g. "GPL-2.0-with-classpath-exception" which
+        # should be "GPL-2.0-only WITH
+        # Classpath-exception-2.0". This file provides
+        # translations for such
+        compounds_file = self.config.get('compunds_file', LICENSE_COMPUNDS_FILE)
+        data = self.__read_json(compounds_file)
+        for compound in data[COMPOUNDS_TAG]:
+            licenses[compound['spdxid']] = compound
+            for alias in compound[FLAME_ALIASES_TAG]:
+                if alias in aliases:
+                    raise FlameException(f'Alias "{alias}" -> {compound["spdxid"]} already defined as "{aliases[alias]}".')
+
+                aliases[alias] = compound['spdxid']
+
+        # Dual licenses
+        # Read license with built-in dual feature, e.g
+        # "GPL-2.0-or-later" which can be seen as a dual
+        # license "GPL-2.0-only OR GPL-3.0-only"
+        duals_file = self.config.get('duals_file', LICENSE_DUALS_FILE)
+        data = self.__read_json(duals_file)
+        for dual in data[DUAL_LICENSES_TAG]:
+            duals[dual['spdxid']] = dual
+
+        logging.debug(f'compounds_file: {compounds_file}')
+        logging.debug(f'ambig_file: {ambig_file}')
+        logging.debug(f'duals_file: {duals_file}')
+        logging.debug(f'config: {self.config}')
+
         self.license_expression = license_expression.get_spdx_licensing()
         self.license_db[DUALS_TAG] = duals
         self.license_db[AMBIG_TAG] = self.ambiguities
         self.license_db[LICENSES_TAG] = licenses
         self.license_db[COMPATS_TAG] = compats
         self.license_db[FLAME_ALIASES_TAG] = aliases
         self.license_db[SCANCODE_KEYS_TAG] = scancode_keys
```

### Comparing `foss-flame-0.19.8/flame/var/license_schema.json` & `foss-flame-0.19.9/flame/var/license_schema.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/0BSD.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/0BSD.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/AGPL-3.0-only.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-only.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/AGPL-3.0-only.json` & `foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-only.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/AGPL-3.0-or-later.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-or-later.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/AGPL-3.0-or-later.json` & `foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-or-later.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Apache-1.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/Apache-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Apache-1.0.json` & `foss-flame-0.19.9/flame/var/licenses/Apache-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Apache-1.1.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/Apache-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Apache-1.1.json` & `foss-flame-0.19.9/flame/var/licenses/Apache-1.1.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Apache-2.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/Apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Apache-2.0.json` & `foss-flame-0.19.9/flame/var/licenses/Apache-2.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Artistic-1.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/Artistic-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Artistic-1.0.json` & `foss-flame-0.19.9/flame/var/licenses/Artistic-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Artistic-2.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/Artistic-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Artistic-2.0.json` & `foss-flame-0.19.9/flame/var/licenses/Artistic-2.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/BSD-2-Clause.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/BSD-2-Clause.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/BSD-2-Clause.json` & `foss-flame-0.19.9/flame/var/licenses/BSD-2-Clause.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/BSD-3-Clause.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/BSD-3-Clause.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/BSD-3-Clause.json` & `foss-flame-0.19.9/flame/var/licenses/BSD-3-Clause.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/BSD-4-Clause-UC.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/BSD-4-Clause-UC.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/BSD-4-Clause.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/BSD-4-Clause.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/BSD-4-Clause.json` & `foss-flame-0.19.9/flame/var/licenses/BSD-4-Clause.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/BSL-1.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/BSL-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/BSL-1.0.json` & `foss-flame-0.19.9/flame/var/licenses/BSL-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/BlueOak-1.0.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/BlueOak-1.0.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CC-BY-3.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/CC-BY-3.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CC-BY-3.0.json` & `foss-flame-0.19.9/flame/var/licenses/CC-BY-3.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CC-BY-4.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/CC-BY-4.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CC-BY-4.0.json` & `foss-flame-0.19.9/flame/var/licenses/CC-BY-4.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CC-BY-SA-2.5.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-2.5.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CC-BY-SA-2.5.json` & `foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-2.5.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CC-BY-SA-3.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-3.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CC-BY-SA-3.0.json` & `foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-3.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CC-BY-SA-4.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-4.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CC-BY-SA-4.0.json` & `foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-4.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CC0-1.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/CC0-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CC0-1.0.json` & `foss-flame-0.19.9/flame/var/licenses/CC0-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CDDL-1.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/CDDL-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CDDL-1.0.json` & `foss-flame-0.19.9/flame/var/licenses/CDDL-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CDDL-1.1.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/CDDL-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/CDDL-1.1.json` & `foss-flame-0.19.9/flame/var/licenses/CDDL-1.1.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Classpath-exception-2.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/Classpath-exception-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/EPL-1.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/EPL-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/EPL-1.0.json` & `foss-flame-0.19.9/flame/var/licenses/EPL-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/EPL-2.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/EPL-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/EPL-2.0.json` & `foss-flame-0.19.9/flame/var/licenses/EPL-2.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/EUPL-1.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/EUPL-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/EUPL-1.0.json` & `foss-flame-0.19.9/flame/var/licenses/EUPL-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/EUPL-1.1.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/EUPL-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/EUPL-1.1.json` & `foss-flame-0.19.9/flame/var/licenses/EUPL-1.1.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/EUPL-1.2.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/EUPL-1.2.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/EUPL-1.2.json` & `foss-flame-0.19.9/flame/var/licenses/EUPL-1.2.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/FTL.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/FTL.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/FTL.json` & `foss-flame-0.19.9/flame/var/licenses/FTL.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/GCC-exception-3.1.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/GCC-exception-3.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/GPL-1.0-only.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/GPL-1.0-only.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/GPL-1.0-only.json` & `foss-flame-0.19.9/flame/var/licenses/GPL-1.0-only.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/GPL-1.0-or-later.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/GPL-1.0-or-later.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/GPL-1.0-or-later.json` & `foss-flame-0.19.9/flame/var/licenses/GPL-1.0-or-later.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/GPL-2.0-only.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/GPL-2.0-only.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/GPL-2.0-only.json` & `foss-flame-0.19.9/flame/var/licenses/GPL-2.0-only.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/GPL-2.0-or-later.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/GPL-2.0-or-later.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/GPL-2.0-or-later.json` & `foss-flame-0.19.9/flame/var/licenses/GPL-2.0-or-later.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/GPL-3.0-only.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/GPL-3.0-only.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/GPL-3.0-only.json` & `foss-flame-0.19.9/flame/var/licenses/GPL-3.0-only.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/GPL-3.0-or-later.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/GPL-3.0-or-later.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/GPL-3.0-or-later.json` & `foss-flame-0.19.9/flame/var/licenses/GPL-3.0-or-later.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/HPND.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/HPND.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/HPND.json` & `foss-flame-0.19.9/flame/var/licenses/HPND.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/ICU.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/ICU.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/IJG.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/IJG.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/ISC.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/ISC.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/JSON.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/JSON.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/LGPL-2.0-only.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/LGPL-2.0-only.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/LGPL-2.0-or-later.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/LGPL-2.0-or-later.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/LGPL-2.0-or-later.json` & `foss-flame-0.19.9/flame/var/licenses/LGPL-2.0-or-later.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/LGPL-2.1-only.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-only.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/LGPL-2.1-only.json` & `foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-only.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/LGPL-2.1-or-later.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-or-later.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/LGPL-2.1-or-later.json` & `foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-or-later.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/LGPL-3.0-only.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-only.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/LGPL-3.0-only.json` & `foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-only.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/LGPL-3.0-or-later.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-or-later.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/LGPL-3.0-or-later.json` & `foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-or-later.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Latex2e.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/Latex2e.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Libpng.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/Libpng.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/LicenseRef-scancode-docbook.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-docbook.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/LicenseRef-scancode-zpl-1.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-zpl-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/MIT-0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/MIT-0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/MIT-advertising.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/MIT-advertising.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/MIT-advertising.json` & `foss-flame-0.19.9/flame/var/licenses/MIT-advertising.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/MIT-open-group.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/MIT-open-group.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/MIT.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/MIT.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/MIT.json` & `foss-flame-0.19.9/flame/var/licenses/MIT.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/MITNFA.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/MITNFA.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/MPL-1.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/MPL-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/MPL-1.0.json` & `foss-flame-0.19.9/flame/var/licenses/MPL-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/MPL-1.1.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/MPL-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/MPL-1.1.json` & `foss-flame-0.19.9/flame/var/licenses/MPL-1.1.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/MPL-2.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/MPL-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/MPL-2.0.json` & `foss-flame-0.19.9/flame/var/licenses/MPL-2.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/NCSA.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/NCSA.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/NCSA.json` & `foss-flame-0.19.9/flame/var/licenses/NCSA.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/NTP.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/NTP.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/ODC-By-1.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/ODC-By-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/ODC-By-1.0.json` & `foss-flame-0.19.9/flame/var/licenses/ODC-By-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/OFL-1.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/OFL-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/OFL-1.1.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/OFL-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/OFL-1.1.json` & `foss-flame-0.19.9/flame/var/licenses/OFL-1.1.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/OML.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/OML.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/OpenSSL.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/OpenSSL.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Plexus.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/Plexus.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/PostgreSQL.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/PostgreSQL.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Python-2.0.1.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/Python-2.0.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Python-2.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/Python-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Python-2.0.json` & `foss-flame-0.19.9/flame/var/licenses/Python-2.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/RSA-MD.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/RSA-MD.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/SAX-PD.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/SAX-PD.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/SAX-PD.json` & `foss-flame-0.19.9/flame/var/licenses/SAX-PD.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/SGI-B-2.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/SGI-B-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/SGI-B-2.0.json` & `foss-flame-0.19.9/flame/var/licenses/SGI-B-2.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/SSPL-1.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/SSPL-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/SSPL-1.0.json` & `foss-flame-0.19.9/flame/var/licenses/SSPL-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/SWL.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/SWL.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/SWL.json` & `foss-flame-0.19.9/flame/var/licenses/SWL.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Sendmail.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/Sendmail.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/TCL.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/TCL.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/TU-Berlin-1.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/TU-Berlin-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/TU-Berlin-1.0.json` & `foss-flame-0.19.9/flame/var/licenses/TU-Berlin-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/TU-Berlin-2.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/TU-Berlin-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/TU-Berlin-2.0.json` & `foss-flame-0.19.9/flame/var/licenses/TU-Berlin-2.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Unlicense.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/Unlicense.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Vim.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/Vim.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/W3C.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/W3C.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/W3C.json` & `foss-flame-0.19.9/flame/var/licenses/W3C.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/WTFPL.json` & `foss-flame-0.19.9/flame/var/licenses/WTFPL.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/X11-distribute-modifications-variant.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/X11-distribute-modifications-variant.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/X11.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/X11.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/ZPL-1.1.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/ZPL-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/ZPL-2.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/ZPL-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/ZPL-2.1.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/ZPL-2.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Zlib.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/Zlib.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/Zlib.json` & `foss-flame-0.19.9/flame/var/licenses/Zlib.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/ambiguities.json` & `foss-flame-0.19.9/flame/var/ambiguities.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/bzip2-1.0.6.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/bzip2-1.0.6.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/compounds.json` & `foss-flame-0.19.9/flame/var/compounds.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/curl.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/curl.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/duals.json` & `foss-flame-0.19.9/flame/var/duals.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/libpng-2.0.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/libpng-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/libtiff.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/libtiff.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/x11-keith-packard.LICENSE` & `foss-flame-0.19.9/flame/var/licenses/x11-keith-packard.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/flame/var/licenses/x11-keith-packard.json` & `foss-flame-0.19.9/flame/var/licenses/x11-keith-packard.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/foss_flame.egg-info/PKG-INFO` & `foss-flame-0.19.9/foss_flame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foss-flame
-Version: 0.19.8
+Version: 0.19.9
 Summary: FOSS License Additional Metadata
 Home-page: https://github.com/hesa/license-db
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `foss-flame-0.19.8/foss_flame.egg-info/SOURCES.txt` & `foss-flame-0.19.9/foss_flame.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 LICENSES/GPL-3.0-or-later.txt
 flame/__init__.py
 flame/__main__.py
 flame/config.py
 flame/exception.py
 flame/format.py
 flame/license_db.py
+flame/var/ambiguities.json
+flame/var/compounds.json
+flame/var/duals.json
 flame/var/license_schema.json
 flame/var/operators.json
 flame/var/licenses/0BSD.LICENSE
 flame/var/licenses/0BSD.json
 flame/var/licenses/AGPL-3.0-only.LICENSE
 flame/var/licenses/AGPL-3.0-only.json
 flame/var/licenses/AGPL-3.0-or-later.LICENSE
@@ -199,23 +202,20 @@
 flame/var/licenses/ZPL-1.1.json
 flame/var/licenses/ZPL-2.0.LICENSE
 flame/var/licenses/ZPL-2.0.json
 flame/var/licenses/ZPL-2.1.LICENSE
 flame/var/licenses/ZPL-2.1.json
 flame/var/licenses/Zlib.LICENSE
 flame/var/licenses/Zlib.json
-flame/var/licenses/ambiguities.json
 flame/var/licenses/blessing.LICENSE
 flame/var/licenses/blessing.json
 flame/var/licenses/bzip2-1.0.6.LICENSE
 flame/var/licenses/bzip2-1.0.6.json
-flame/var/licenses/compounds.json
 flame/var/licenses/curl.LICENSE
 flame/var/licenses/curl.json
-flame/var/licenses/duals.json
 flame/var/licenses/libpng-2.0.LICENSE
 flame/var/licenses/libpng-2.0.json
 flame/var/licenses/libtiff.LICENSE
 flame/var/licenses/libtiff.json
 flame/var/licenses/x11-keith-packard.LICENSE
 flame/var/licenses/x11-keith-packard.json
 foss_flame.egg-info/PKG-INFO
```

### Comparing `foss-flame-0.19.8/setup.cfg` & `foss-flame-0.19.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.8/setup.py` & `foss-flame-0.19.9/setup.py`

 * *Files identical despite different names*

